# PROMPT 05 — UGC Authenticity & Ad-Compliance QA

Two gates in one: does it sound like a real person, and can it legally run as paid media?

---

## PART A — Authenticity scan (paste your scripts, run this)

```
You are a ruthless UGC editor. Your job is to find every line that sounds like an
advertisement rather than a person.

FLAG every instance of:
game-changer, must-have, revolutionary, transform, transformation, unlock, elevate,
indulge, pamper, treat yourself, say goodbye to, look no further, trusted by thousands,
premium quality, state-of-the-art, world-class, best-in-class, we are passionate,
dedicated to excellence, seamlessly, hassle-free, your journey, in today's world,
one-stop solution, 100% guaranteed, scientifically proven (unless a citation exists),
and any sentence using "we" where a real customer would say "I".

ALSO FLAG these structural tells:
1. Any hook that starts with the brand name — nobody stops for a brand.
2. Any sentence longer than 20 words — unspoken language.
3. Feature lists dressed as dialogue (three benefits in a row).
4. Adjective triads ("smooth, shiny and healthy").
5. Claims with no number, name, place or source behind them.
6. Zero downsides mentioned — an ad with no downside reads as an ad.
7. A CTA that asks for a purchase from a cold audience.
8. Anything you could imagine in a corporate voiceover. That's the worst kind.

OUTPUT: a table | Script | Line | Problem | Severity (High/Med/Low) | Rewritten line
Then output the corrected scripts in full.

Also answer, for the whole pack:
- Which single line in each script is the most believable? (That's the line to keep.)
- Which script would a viewer most likely call "just an ad"? Why?
```

---

## PART B — The 30-point UGC scorecard

Score every script. Under 24 = don't shoot it.

| # | Check | Weight | Score 0–2 |
|---|---|---|---|
| 1 | Hook lands in ≤12 words and needs no context | x2 | |
| 2 | Hook creates recognition or curiosity in under 2 seconds | x2 | |
| 3 | Spoken language passes the read-aloud test | x2 | |
| 4 | Contains ≥1 oddly specific detail (number, time, place, price) | x2 | |
| 5 | Includes one honest limitation or "not for you if" line | x2 | |
| 6 | Product/service is SHOWN being used in ≥2 beats | x2 | |
| 7 | One idea per script, no feature dumping | x2 | |
| 8 | CTA is a single action with a low-friction first step | x2 | |
| 9 | CTA states what the viewer gets and how fast | x1 | |
| 10 | Word count fits the runtime (2.5 words/sec) | x1 | |
| 11 | Brand name appears once and not in the first 5 seconds | x1 | |
| 12 | Zero banned ad-speak | x2 | |
| 13 | Shootable by one person, one location, one phone | x2 | |
| 14 | Would still make sense with the sound off (captions + visuals) | x1 | |
| 15 | No claim without proof from the brief | x2 | |
| 16 | No policy-risk claim (see Part C) | x2 | |
| 17 | Required disclosures present (#ad, results vary, etc.) | x2 | |
| 18 | Written for the right traffic temperature (cold/warm/retargeting) | x1 | |
| 19 | Distinct from the other scripts in the pack (no repeated rhythm) | x2 | |
| 20 | Would you send this to a friend without embarrassment? | x1 | |

**Max 34.** 30+ → shoot it. 24–29 → fix specifics. Below 24 → the brief is thin; go back to PROMPT 00.

---

## PART C — Ad-compliance gate (do not skip this)

| Risk | Rule | Where it bites |
|---|---|---|
| **Health / beauty efficacy claims** | No claims of curing, treating or preventing a condition. "Repairs damaged hair" is a claim; "leaves hair smoother for 3–5 months" is an experience. | Meta ad rejection, ASCI complaints in India |
| **Before / after** | Allowed as creative, but must not imply a guaranteed or typical result. Add "results vary". No retouching that misrepresents the outcome. | Meta policy, consumer law |
| **Testimonials** | Must be real, used with permission, and must not include a claim that would be restricted in an ad. Keep proof of the original message. | FTC / ASCI, and it's a legal risk for the brand |
| **Paid partnership disclosure** | If a creator is paid or gifted, the content needs `#ad` or the platform's paid-partnership tag, visible and not buried in hashtags. | Platform enforcement; brands get penalised too |
| **Personal attributes (Meta)** | Never imply you know the viewer's condition ("your damaged hair", "your debt"). Reframe to the general case. | Instant rejection, repeat strikes restrict the account |
| **Fake urgency / scarcity** | Only real deadlines. "Only 2 left" must be true. | Policy + consumer law |
| **Guarantees** | Only state guarantees the brand actually honours, with the conditions and window. | Consumer protection |
| **Music** | Trending audio is often licensed only for organic use, not paid ads. For paid, use commercial-licence audio or the platform's ad library. | Takedowns and account issues |
| **Consent** | Any customer on camera needs written consent, especially for before/after. For minors, guardian consent. | Legal + reputational |
| **Local claims** | "Best in [city]" and "#1" are unverifiable superlatives — cut them. | ASCI guidelines, ad rejection |

**Print this as a final checklist before delivery:**
- [ ] Every claim traceable to the brief or a real review
- [ ] `#ad` added wherever a creator was paid or gifted
- [ ] "Results vary" added where before/after or outcome language appears
- [ ] No personal-attribute language in paid ad copy
- [ ] Real deadlines only
- [ ] Commercial-licence audio flagged for paid use
- [ ] Written consent for any customer appearing on camera
- [ ] No unverifiable superlatives

---

## PART D — Human pass (do this manually, 15 minutes)

- [ ] **Read every script out loud.** Cut every line you stumble on.
- [ ] **Add one detail only a local person would know** — the bakery downstairs, the 4 pm rush, the Tuesday walk-in gap.
- [ ] **Vary the rhythm.** If two scripts open with the same energy, rewrite one hook.
- [ ] **Check the numbers.** Prices, durations, counts — everything must match the brief.
- [ ] **Delete every "Why this works" note** before sending to the client (keep them in the repo version).
- [ ] **Film one.** A single 25-second phone take turns this from a document into proof of work.
