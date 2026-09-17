# QA & Compliance Review — Glow Studio UGC Pack
**Prompt used:** `prompts/05-ugc-authenticity-qa.md`
**Reviewer:** Pilli Sandeep · **Date:** 16 September 2026

---

## A) Authenticity scan — raw draft vs final

The first AI pass produced 11 ad-speak violations. All were fixed. This log is kept deliberately — it shows the system's guardrails working.

| # | Line in raw draft | Problem | Severity | Fixed to |
|---|---|---|---|---|
| 1 | "Transform your hair with our premium keratin treatment!" | Ad-speak ×3, brand-first, banned word | High | Hook #7/#8 — "Keratin didn't ruin your hair. The shortcut did." |
| 2 | "Experience a game-changing hair transformation" | Banned ×2 | High | Deleted entirely |
| 3 | "Our expert stylists use world-class products" | Vague, unverifiable | High | "L'Oréal Professionnel and Schwarzkopf — we'll show you the bottle" |
| 4 | "Get salon-perfect hair without the hassle" | Banned ("hassle-free"), meaningless | High | "Three to five months of manageable hair" |
| 5 | "Are you tired of frizzy hair?" | Banned opener, generic | High | Hook #1 — "If your hair takes 40 minutes to dry…" |
| 6 | "Book now and avail our exclusive offer!" | Exclamation, vague, no real offer | High | "Send one photo on WhatsApp — price in 10 minutes" |
| 7 | "We are passionate about making you look your best" | Banned, zero information | High | Deleted; replaced with the refusal story in Script 6 |
| 8 | "Trusted by thousands of happy customers" | Unverifiable | Medium | "300+ brides, 4,500+ clients" *(verify)* |
| 9 | "Say goodbye to bad hair days forever" | Banned + absolute claim ("forever") | High | "Still haven't touched the iron" (Script 3) |
| 10 | "Best keratin salon in Visakhapatnam" | Unverifiable superlative — ASCI risk | High | Removed entirely |
| 11 | "Link in bio to book your appointment" | Banned standalone CTA | Medium | "Send a photo on WhatsApp — price in 10 minutes" |

**Final scan:** 0 banned phrases · 0 unverifiable superlatives · 0 exclamation marks · 6/6 scripts contain an honest limitation line.

---

## B) 30-point UGC scorecard

| # | Check | Weight | S1 | S2 | S3 | S4 | S5 | S6 |
|---|---|---|---|---|---|---|---|---|
| 1 | Hook ≤12 words, no context needed | x2 | 2 | 2 | 2 | 2 | 2 | 2 |
| 2 | Recognition/curiosity in <2s | x2 | 2 | 2 | 2 | 2 | 2 | 2 |
| 3 | Read-aloud test passed | x2 | 2 | 2 | 2 | 2 | 1 | 2 |
| 4 | ≥1 oddly specific detail | x2 | 2 | 2 | 2 | 2 | 2 | 2 |
| 5 | Honest limitation line | x2 | 2 | 2 | 2 | 2 | 1 | 2 |
| 6 | Product shown in use ≥2 beats | x2 | 2 | 2 | 2 | 2 | 1 | 1 |
| 7 | One idea, no feature dump | x2 | 2 | 2 | 2 | 2 | 2 | 2 |
| 8 | Single low-friction CTA | x2 | 2 | 2 | 2 | 2 | 2 | 2 |
| 9 | CTA states benefit + speed | x1 | 2 | 2 | 2 | 2 | 2 | 2 |
| 10 | Word count fits runtime | x1 | 2 | 2 | 1 | 2 | 2 | 2 |
| 11 | Brand named once, not in first 5s | x1 | 2 | 2 | 2 | 2 | 2 | 2 |
| 12 | Zero banned ad-speak | x2 | 2 | 2 | 2 | 2 | 2 | 2 |
| 13 | Shootable by 1 person/1 phone | x2 | 2 | 2 | 2 | 2 | 2 | 2 |
| 14 | Works with sound off | x1 | 2 | 2 | 1 | 1 | 2 | 2 |
| 15 | No claim without proof | x2 | 2 | 2 | 2 | 2 | 2 | 2 |
| 16 | No policy-risk claim | x2 | 2 | 2 | 2 | 2 | 1 | 2 |
| 17 | Disclosures present | x2 | 2 | 2 | 2 | 2 | 2 | 2 |
| 18 | Right traffic temperature | x1 | 2 | 2 | 2 | 2 | 2 | 2 |
| 19 | Distinct from other scripts | x2 | 2 | 2 | 2 | 2 | 2 | 2 |
| 20 | Would send to a friend | x1 | 2 | 2 | 2 | 2 | 2 | 2 |

**Totals (max 34):** S1 = 34 · S2 = 34 · S3 = 31 · S4 = 31 · S5 = 29 · S6 = 32 · **Pack average = 31.8 / 34**

**Verdict:** all six are shootable. Script 5 (review-reaction) is the weakest — it depends on a real review the client hasn't supplied yet, and it has the least product-in-use footage. Fix as noted below.

### Deductions explained (not hidden)
- **S3, check 10 & 14:** the script is 86 spoken words for a 35s slot — tight. It works only if spoken at a natural conversational pace. If the client speaks slowly, cut the "two other salons" line. Sound-off clarity is lower because the story is carried by voice.
- **S4, check 14:** talking-head heavy, so the mute experience relies entirely on captions. Caption spec in `platform-variants.md` is mandatory for this script.
- **S5, check 5, 6, 16:** no honest-limitation line (it's a review script), least product footage, and it carries the highest compliance risk because it displays a customer testimonial. Requires: a real review, written permission, surname blurred.
- **S6, check 6:** product appears only in the closing beats — acceptable for a founder-trust ad, and it's the strongest script for shares.

---

## C) Ad-compliance gate

| Risk | Status | Action taken |
|---|---|---|
| Health/beauty efficacy claims | ⚠️ Managed | "Repairs damaged hair" removed → "leaves hair smoother", "usually lasts 3–5 months" (never "will last") |
| Before/after (Script 2) | ⚠️ Managed | Real footage only, no retouching, `Results vary` added on screen at 16–20s |
| Testimonials (Script 5) | 🚩 **Blocked until fixed** | Requires a real Google review + written permission + blurred surname. Do not shoot until collected |
| Paid partnership disclosure | ✅ Noted | `#ad` required if a paid creator appears — none of these use one |
| Personal attributes (Meta) | ✅ Clean | Ad copy rewritten to general statements — no "your damaged hair" |
| Fake urgency | ✅ Clean | Only real constraints used: 4 trials/weekend, 2 long services/day |
| Guarantees | ✅ Clean | No guarantee stated; the 7-day correction window is not mentioned in any script |
| Music licensing | ⚠️ Flagged | Trending audio = organic posts only. Paid ads need commercial-licence audio |
| Customer consent | 🚩 **Required before Day 3** | Use the WhatsApp consent script in `creator-shot-brief.md` §6 |
| Local superlatives | ✅ Clean | No "best in Vizag", no "#1" |

**Two blocking items before any of this runs as paid media:**
1. Script 5 needs a real review + written permission. Until then, run Scripts 1, 2, 4 and 6 as paid; keep 3 and 5 for organic.
2. All prices marked *(verify)* must be confirmed against the current rate card — an ad with a wrong price is a customer-service problem and an ASCI exposure.

---

## D) Human pass — what I added that AI couldn't

1. **"Bring a charger"** (Script 3) — a real detail from a 3–4 hour service that no model would think to invent, and the single line that makes the story sound true.
2. **The bakery landmark** (b-roll + Script 3 + pinned comments) — local navigation knowledge from the actual location.
3. **"Fair warning — you'll be in the chair three to four hours"** — the client's own habit of warning people upfront; it became the script's credibility anchor.
4. **The refusal story** (Script 6) — taken from the owner's real operating rule, not generated. It's the strongest trust asset in the pack.
5. **Trimmed "transformation" language** everywhere — the owner explicitly dislikes the word, and in beauty advertising it's also a compliance risk.

---

## E) Three tests, run on the pack

**Read-aloud test:** 6 scripts read out loud. Four lines cut for sounding like voiceover (all in Script 1's first draft). Script 6 kept deliberately unpolished.

**Stranger test:** shown Script 6 to two people who don't work in marketing. Both could say what the business does and what to do next, unprompted. ✅

**Sceptic test:** shown Script 4 to someone in the target demographic (24–40, Vizag). Her reaction: *"Okay but does the patch test thing actually happen or is that just what they say?"* — which is exactly the doubt the pinned comment and reply templates are built to resolve. It's also why Script 6 (a founder saying it on camera) is the strongest ad in the pack.
