# Call Transcript — Nordkredit

**Date:** March 2026 · **Duration:** ~18 minutes · **Call type:** First discovery call, following outbound
**Rep:** Anna Kowalski (Sundial Analytics) · **Prospect:** Lena Virtanen, Head of Credit Risk, Nordkredit (regional lender, Nordics, ~€600M annual origination)

*Context: Lena responded to an outbound email referencing her recent hire and Nordkredit's tooling migration (see [`personalized-outbound`](../personalized-outbound/example.md)).*

---

**Anna:** Lena, thanks for making time — I know you're three weeks into the role, so I appreciate it. I'll keep this loose: I'd rather understand what you're actually dealing with than run you through slides. Sound okay?

**Lena:** That works. Honestly your email was the first one this month that didn't try to sell me something before asking a question, so — here we are.

**Anna:** Ha, good. So, high level — what pulled you into this migration? Was it something you inherited, or something you decided once you got in the seat?

**Lena:** Bit of both. My predecessor had already flagged that our valuation tooling was a black box — literally, it gives you a number and a confidence percentage and that's it. We had an internal audit finding last year, nothing catastrophic, but the examiner's note was basically "you couldn't explain how three of these numbers were derived if asked." That report was sitting on my desk my first day.

**Anna:** That's about as clean a mandate as it gets. When you say "couldn't explain" — walk me through what happens today when someone does ask.

**Lena:** Our current tool — we use Estemate, have for years — gives a confidence score and a short methodology PDF that's the same for every valuation. It doesn't tell you which comparables were used for *this specific property*, or how they were weighted. So if an examiner or an internal risk committee asks "why this number," the honest answer is "the model said so," which is not an answer anyone wants to give twice.

**Anna:** Okay, that's useful, and it's exactly the gap we built around. Every valuation we produce comes with the actual comparables used and their weighting — not a generic doc, the specific inputs for that specific output. Would it help if I showed that live, on one of your own past valuations, rather than a canned demo?

**Lena:** Yes, actually — that would matter a lot more than slides. Can you genuinely do that with a real property, or does it need to be one that's already in your system somehow?

**Anna:** We'd need the property details and whatever comparables your team already used, but yes — we can run it live and you can see the actual audit trail it produces, not a mocked-up one.

**Lena:** Okay. I'll be honest, we also looked at ValuAI a few months back, before I started. I've heard from a colleague at another bank that ValuAI's sales team said something almost identical to what you just said.

**Anna:** That's a fair thing to bring up, and I'd rather you ask it directly than wonder. What did your colleague say happened?

**Lena:** She said when they pushed ValuAI in a follow-up technical call — not the first demo, the second one — the "audit trail" turned out to be a confidence breakdown by category, not actual named comparables. It looked good in the first meeting and then didn't hold up when their data team asked for specifics.

**Anna:** That matches what we've heard elsewhere too, for what it's worth — though I'd rather you verify it yourself than take our word for it, since obviously we have a horse in this race. What I'd suggest: when you evaluate us, do exactly what your colleague did with ValuAI — push past the first demo, ask us for a comparable-level breakdown on a property your own team picks, not one we prepare. If we can't produce it, that tells you something. If we can, that also tells you something.

**Lena:** That's a reasonable way to structure it. Okay — separately, timeline. We have a board audit scheduled for Q3. I don't want to be mid-migration when that happens — that would be worse than not migrating at all.

**Anna:** Understood, and that's a real constraint, not a soft one. What's the actual date, if you know it?

**Lena:** Second week of September, tentatively.

**Anna:** Okay. Typical implementation for a bank your size is a few weeks, not months, assuming we're not waiting on your side for data access approvals — that's usually the longest pole. If we started in, say, June, you'd have real runway before September, with buffer. I don't want to promise a date I can't back up, so let me confirm exact weeks with our implementation team rather than guess on this call.

**Lena:** Appreciate you not just saying "sure, no problem." One more thing — pricing. Your website says "custom," which usually means "we'll figure out how much you can pay."

**Anna:** Fair reaction, and no, that's not what it means here — it's usage-based per valuation call, and it scales with your volume, so I can actually give you a real range today rather than making you sit through two more calls to get a number. Given roughly what you described — €600M origination — you're likely in [a specific tier], which I can follow up with in writing so you have it in front of you rather than half-remembering a number from a call.

**Lena:** That's more than I expected to get today, honestly. Okay — what's the actual next step?

**Anna:** I'd suggest a technical validation call — bring whoever on your team would actually push on the audit trail, and we run it live against a real property your side selects. No slides. If that goes well, we can talk implementation timeline against your September date specifically.

**Lena:** That works. Let me check with our data lead on availability — I'll follow up this week.

**Anna:** Sounds good. I'll send the pricing tier detail in writing today so you have something concrete either way.

**Lena:** Appreciate it. Talk soon.

---

## Internal notes (rep-logged, not read aloud on the call)

- Strong, specific buying signal: real audit-finding trigger, dated board deadline (Q3, tentatively second week of September).
- ValuAI explicitly in play, but via secondhand account, not confirmed head-to-head yet — worth revisiting if it resurfaces with more specifics.
- Estemate is the incumbent being displaced — confirms `competitive-landscape.md`'s Estemate entry (dated, generic methodology doc, no comparable-level detail).
- Next step: technical validation call with Nordkredit's data lead, live audit trail on a real property they select.
- Action: send pricing tier confirmation in writing today (open commitment made on the call — must follow through).
