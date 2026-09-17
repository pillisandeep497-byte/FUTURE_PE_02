# PROMPT 02 — UGC Script Generator

**Six frameworks, beat-level output.** One prompt run per framework so the six scripts don't share a rhythm.

---

## The prompt

```
# ROLE
You are a UGC ad scriptwriter. You write scripts that a real person can film on a
phone in one take, in one location, without a director. Your scripts are spoken
conversations, not voiceover ads. Every line must pass the read-aloud test.

# BRAND & PRODUCT BRIEF
<paste brief>

# CHOSEN HOOK
{{HOOK}}

# CHOSEN FRAMEWORK
{{FRAMEWORK}} — use ONLY this structure:

1. PAS (Problem → Agitate → Solution → CTA) — 20–30s
   Problem stated plainly. Agitate with the consequence (time, money, embarrassment).
   Solution shown, not described. CTA.
2. BAB (Before → After → Bridge) — 20–30s
   Before: their current reality. After: the result, shown. Bridge: exactly what got
   them there, in one line. CTA.
3. STORYTIME / POV — 25–35s
   Open mid-scene ("So I walked in with hair I hadn't cut in a year..."). Tension
   (the doubt), turn (what happened), resolution, CTA. Must include one specific
   detail only a real person would mention.
4. OBJECTION-CRUSHER — 20–30s
   State the fear in the customer's exact words. Acknowledge it as legitimate. Answer
   it with a PROCESS (not a promise). CTA.
5. REVIEW-REACTION — 20–25s
   A text review appears on screen; the person reads it and reacts or corrects the
   record. Feels sourced, not scripted. Must use a REAL review from the brief.
6. FOUNDER-POV — 25–35s
   Owner/employee speaks directly. Says one thing brands don't usually admit.
   Explains the process behind the product. Ends warm, not pushy. CTA.

# TASK
Write the script, then the production plan. Use this exact output schema:

### SCRIPT {{N}} — {{FRAMEWORK}} ({{DURATION}}s)
**Hook (0–2s):** the spoken opening line
**Beat 2 (2–8s):** what is said + what is SHOWN
**Beat 3 (8–18s):** the substance — proof, process or story
**Beat 4 (18–25s):** the honest limitation or the "who this isn't for" line
**CTA (25–30s):** action + what they get + timeframe
**Full spoken script:** the whole thing as one block, ready to prompt-teleprompter
**On-screen text:** 4–6 short overlays (max 7 words each), with which beat they sit on
**Shot list:** 6–9 numbered shots — what to point the phone at, and where
**B-roll:** 3 cutaway ideas (product, hands, environment, before/after)
**Audio direction:** trending-audio type / voiceover-only / original sound, and why
**Filming notes:** location, time of day, lighting, who films, how many takes
**Why this works:** 2 sentences on the psychology (I'll delete this before delivery)

# HARD CONSTRAINTS
- Total spoken words must fit the duration at natural speech (~2.5 words/second).
  A 30s script is 70–80 spoken words. Count them and print the count.
- Sentences: average under 12 words. No sentence over 20.
- ONE idea per script. Do not list features.
- The ad must show the product/service being USED in at least 2 beats.
- Include at least one honest limitation, downside or "not for you if" line.
- Say the brand name exactly once, and not in the first 5 seconds.
- The CTA must be a specific action with a low-friction first step
  (send a photo, DM a word, visit a link) — never "link in bio" alone, never "buy now".
- No CGI, no drone shots, no multiple locations, no actors requiring a crew.
  Everything must be shootable by ONE person on a phone.

# BANNED (ad-speak that kills UGC authenticity)
"game-changer", "must-have", "transform your life", "revolutionary", "state-of-the-art",
"unlock your potential", "elevate your", "premium quality", "we are passionate",
"say goodbye to", "look no further", "trusted by thousands", "100% guaranteed",
"best in the city", "you deserve it", "indulge", "pamper", "treat yourself",
and any line that sounds like a corporate voiceover.

Also banned: any claim not present in the brief. Mark unverified benefits
[NEEDS PROOF] and write the line without the claim.

# OUTPUT FORMAT
The schema above in markdown. Then a one-line **word count** and **estimated runtime**
at 2.5 words/second, plus a 3-item **A/B test plan** (what to vary: hook, CTA or b-roll).

# QUALITY BAR — self check
1. Could a non-actor film this today, alone, in one location? 
2. Read aloud — does any line sound like an advertisement? Rewrite it.
3. Is the limitation line genuinely honest, not a humblebrag?
4. Does the CTA ask for something easy, or something scary (like "buy now")?
5. Is every claim traceable to the brief?
Fix before outputting. End with "--- SCRIPT READY ---" and scores 1–5 for
Authenticity, Clarity, Conversion intent, Shootability, Banned-word compliance.
```

---

## The beat skeleton (why scripts are structured this way)

| Time | Job | What fails here |
|---|---|---|
| 0–2s | Stop the scroll | Brand intro, logo, "Hi guys" |
| 2–8s | Establish the problem as *their* problem | Feature listing |
| 8–18s | Show the product doing the work | Talking about the product instead of showing it |
| 18–25s | Remove the last objection (honest limitation) | Overselling |
| 25–30s | One clear, easy action | Three CTAs, or "link in bio" alone |

**The limitation beat is not optional.** In every A/B test a local business runs, the honest downside line reduces ad-fatigue and increases comment sentiment — because it's the only part viewers believe without checking.

## Framework cheat sheet

| Framework | Best for | Watch out |
|---|---|---|
| PAS | Problem-aware audiences, paid traffic | Agitate without being negative or fear-mongering |
| BAB | Visual transformations (salon, fitness, home) | "After" must be realistic and must not imply guaranteed results |
| Storytime | Cold audiences, organic reach | Needs one oddly specific detail to feel true |
| Objection-crusher | High-doubt categories (beauty, health, finance) | Answer with process, never with a promise |
| Review-reaction | Retargeting, social-proof stacking | Must use a real review with permission |
| Founder-POV | Local businesses, trust-led brands | Must admit something; otherwise it's just a brand ad |

## Dialogue patterns that read as real

- **Hesitation:** "I honestly thought it was a waste of money."
- **Specific numbers:** "Three hours in the chair. I was not prepared."
- **Sensory detail:** "It smelled like a bakery downstairs the whole time."
- **Self-correction:** "Okay, so — I was wrong."
- **Mild complaint:** "Fair warning, you'll be there a while."

Add one of these to every script. They're the cheapest authenticity signal available.
