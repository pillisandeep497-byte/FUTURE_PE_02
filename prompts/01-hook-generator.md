# PROMPT 01 — Hook Generator (the highest-leverage prompt in the system)

**The rule behind the system:** a UGC ad is won or lost in the first 1.5–3 seconds. Hooks deserve their own dedicated prompt, their own volume target, and their own scoring rubric — never a single clever line tacked onto a script.

---

## The prompt

```
# ROLE
You are a UGC creative strategist who has written hooks for hundreds of short-form
ads. You know that the hook's only job is to stop the scroll by making the viewer
feel "that's me" or "wait, what?" in under two seconds. You do not write ad copy.
You write the first sentence a real person would say.

# BRAND & PRODUCT BRIEF
<paste brief>

# TASK
Generate 24 hooks for {{HERO_OFFER}} across the 10 archetypes below.
Distribute them: 3 for the top 4 archetypes, 2 for the remaining 6.

THE 10 ARCHETYPES
1. PROBLEM CALL-OUT — name the pain as they experience it
   e.g. "If your hair takes 40 minutes to dry, this is for you."
2. CONFESSION / SECRET — admit something slightly embarrassing
   e.g. "I spent ₹12,000 on keratin before I found this place."
3. CONTRARIAN / MYTH-BUST — say the opposite of what they expect
   e.g. "Stop asking for keratin. Here's why."
4. POV / STORYTIME — drop them mid-scene
   e.g. "POV: it's 6 AM and your hair already looks like a mess."
5. OBJECTION-AS-HOOK — open with their exact doubt
   e.g. "Will keratin ruin my hair? I asked."
6. SOCIAL PROOF / REVIEW — lead with someone else's words
   e.g. "My friend said don't go here unless you have 4 hours. She was right."
7. LOCAL IDENTITY — use the area, landmark or shared frustration of the place
   e.g. "Vizag humidity vs my hair: round one."
8. BEFORE/AFTER TEASE — promise visible change without claiming a miracle
   e.g. "Same hair. Three hours apart."
9. FOUNDER / INSIDER — an employee or owner says the thing brands hide
   e.g. "Hi, I'm Sanjana. Here's why I turn down ₹6,000 bookings."
10. URGENCY / DEADLINE (only if {{URGENCY}} is real)
   e.g. "November brides: this is your last month for a trial."

# HARD CONSTRAINTS
- Max 12 words per hook. Most should be 5–9 words.
- Hook must be speakable. Read-aloud test: no line may sound like a caption or a slogan.
- No hook may start with the brand name. Nobody stops scrolling for a brand.
- Each hook must work WITHOUT context — assume the viewer has never heard of the brand.
- At least 4 hooks must contain a specific number, place, price or timeframe.
- At least 3 hooks must name a downside or limitation (honesty stops the scroll).
- Write in the language set in the brief. If it's a mixed language, keep the hook in
  English and put colloquial phrasing in the second line only.
- No hook may be rephrased from another hook — each must use a different psychological
  trigger.

# BANNED
"Are you tired of...", "Introducing...", "Say goodbye to...", "The secret nobody tells
you", "You won't believe...", "This one trick", "Game-changer", "Must-have",
"Attention!", "Do you want to...", "It's time to...", "Unlock", "Elevate",
and any hook starting with "We" or "Our".

# OUTPUT FORMAT
A table, sorted by archetype:
| # | Archetype | Hook (≤12 words) | Trigger | Best platform | Delivery note |

Then a second section: **TOP 6 — PROMOTED TO SCRIPTS**
Pick 6 hooks from different archetypes and say, for each, which script framework it
suits best (PAS / BAB / Storytime / Objection-crusher / Review-reaction / Founder-POV).

# QUALITY BAR — self-check before answering
1. Would a real customer say this line, exactly, out loud? 
2. Does each hook create either recognition ("that's me") or curiosity ("what?")?
3. Is any hook interchangeable with a competitor's ad? Delete and rewrite.
4. Does any hook over-promise a result the brief can't substantiate? Soften it.
5. Are all 24 hooks genuinely distinct in psychological trigger?

End with a scoring table — for every hook, rate 1–5 on:
**Scroll-stop | Clarity | Honesty | Platform-native | Free of ad-speak** (max 25).
Flag any hook scoring under 18 and rewrite it once.
Finish with "--- HOOKS READY ---" and the average score.
```

---

## The hook scoring rubric (use this to filter, not the model's opinion)

| Criterion | 1 (weak) | 3 (okay) | 5 (strong) |
|---|---|---|---|
| **Scroll-stop** | generic statement | mildly interesting | creates a "wait, what?" gap |
| **Clarity** | needs context | understandable | instant, no second read |
| **Honesty** | over-promises | neutral | admits a downside or a real number |
| **Platform-native** | sounds like a TV ad | acceptable | sounds like a DM from a friend |
| **No ad-speak** | "transforms your life" | mild marketing | zero marketing vocabulary |

**Cut everything under 18/25.** Six great hooks beat 24 average ones — but generate 24 so the six are actually great.

## Hook patterns worth stealing (with why they work)

| Pattern | Example | Why it works |
|---|---|---|
| Specific confession | "I spent ₹12,000 before I found this place." | Numbers + vulnerability = credibility |
| Cost of the problem | "40 minutes of ironing every morning. Every morning." | Repetition mimics lived frustration |
| Anti-sell | "Don't come here for a quick fix." | Inverts expectation; reads as honesty, not advertising |
| Named place | "Vizag humidity has entered the chat." | Local audience recognises itself instantly |
| Insider admission | "I turn down bookings. Here's why." | Curious + trustworthy at once |
| Mid-scene POV | "POV: it's 6 AM and your hair is already a problem." | Drops viewer into a story, no setup needed |

## The four-test filter before a hook goes into production

1. **Say it out loud.** Awkward in speech = cut.
2. **Cover the brand name.** Does it still work? If it only works because it's an ad, cut it.
3. **Ask "so what?"** If the viewer's honest response is "so what?", it's a fact, not a hook.
4. **Ask "would their competitor say the same?"** If yes, it's category copy, not a hook.
