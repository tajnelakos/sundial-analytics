# Deliverability Checklist

A persona-specific sequence is wasted if it lands in spam — this checklist is generic to any sequence run out of this folder, not tied to one persona or campaign. Run it before the first send of a new sequence, and re-check the authentication items if the sending domain or ESP ever changes.

## Before the first send

- [ ] **SPF record** published for the sending domain, covering every service actually allowed to send as that domain (ESP, CRM, any transactional mailer) — an SPF record that's too narrow silently fails sends from a legitimate but unlisted source.
- [ ] **DKIM** configured and signing outbound mail — verify with a test send, not just by confirming the DNS record exists; a published record with signing not actually enabled looks correct and fails silently.
- [ ] **DMARC** published, starting at `p=none` (monitor-only) if this is a new domain or subdomain, moving to `p=quarantine` once a few weeks of reports show no legitimate mail failing alignment.
- [ ] **Dedicated sending subdomain** for marketing sequences (e.g. `send.sundialanalytics.com`), separate from the primary corporate domain — isolates sequence sending reputation from transactional and corporate mail reputation.
- [ ] **Warm-up schedule** for a new sending domain or subdomain — start at a small daily volume and ramp over 2-3 weeks rather than sending a full segment on day one; a cold domain sending high volume immediately is a strong spam signal to receiving mailbox providers regardless of content.

## Before each new sequence or segment

- [ ] **List hygiene** — remove hard bounces immediately, and suppress addresses that haven't opened anything in the last 2 sequences before adding them to a new one; a list with accumulated stale addresses drags reputation down for the whole send.
- [ ] **Segment size sanity check** — confirm the list was built from the actual trigger condition (e.g. "downloaded this specific whitepaper") and not accidentally the full contact database; an oversized, low-intent segment depresses open rate in a way that reads as a deliverability problem even when the real cause is targeting.
- [ ] **Subject line spam-trigger scan** — avoid ALL CAPS, excessive punctuation ("!!!"), and words that skew spam-filter scoring regardless of legitimate use (`free`, `guarantee`, `act now`). Neither A/B variant in [`campaign-metrics.csv`](./campaign-metrics.csv) uses any of these — keep future variants to the same standard.
- [ ] **Working, one-click unsubscribe link** in every email, and confirm it actually removes the contact rather than just recording the click — required under CAN-SPAM and GDPR, and a broken unsubscribe flow itself generates spam complaints from people who resort to marking the mail as spam instead.
- [ ] **Physical mailing address** in the footer (CAN-SPAM requirement for commercial email to US recipients).
- [ ] **Plaintext fallback / good text-to-image ratio** — an email that's a single large image with little real text scores worse with most spam filters and fails for recipients with images disabled by default.

## During the send

- [ ] **Bounce rate under 2%.** Above that, pause the sequence and audit the list rather than continuing to send — sustained high bounce rate is one of the fastest ways to damage sending-domain reputation.
- [ ] **Spam complaint rate under 0.1%.** Gmail and other major providers throttle or block senders that exceed this, independent of open/click performance looking otherwise healthy.
- [ ] **Monitor for a mid-sequence deliverability cliff** — if open rate drops sharply partway through a sequence (sharper than the normal decay pattern in [`campaign-performance-analysis.html`](./campaign-performance-analysis.html)), check inbox placement before assuming the content itself stopped working; a placement problem and a content problem look identical in aggregate open-rate data alone.

## Reference

- [`campaign-metrics.csv`](./campaign-metrics.csv) — this repo's own tracked send data, for comparing a live campaign's bounce/unsubscribe rates against a known baseline.
- CAN-SPAM Act requirements apply to any commercial email to US recipients regardless of where Sundial Analytics is headquartered; GDPR applies to any EU recipient regardless of sender location. Neither is optional based on segment size.
