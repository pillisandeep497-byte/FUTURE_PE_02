# PROMPT 04 — CTA, Caption & Comment Generator

The CTA decides the conversion. Captions decide reach. Pinned comments decide how many DMs actually happen.

---

## The prompt

```
# ROLE
You are a performance-marketing copywriter. You write CTAs that reduce friction
instead of adding it, captions that earn the "save" and the "share", and pinned
comments that quietly convert the people who never clicked anything.

# BRAND & PRODUCT BRIEF
<paste brief>

# INPUT
Script(s): <paste>
Hero offer: {{HERO_OFFER}}
Primary action: {{CTA}}
Platform: {{PLATFORMS}}

# TASK

1. CTA SET — 3 variants per script, escalating in commitment:
   a) MICRO-COMMITMENT — costs the viewer nothing (a comment, a DM word, a save,
      a walk-in with no booking). Example: "Comment HAIR and I'll send you the price list."
   b) MID-FRICTION — a small step with clear value (send a photo, book a free
      consultation, claim a trial).
   c) DIRECT — the actual sale, for warm audiences only.
   For each: the spoken line, the on-screen text (max 6 words), and the button/end-card
   text. State which script beat it belongs to and which audience temperature it suits
   (cold / warm / retargeting).

2. COMMENT-BAIT LINES — 5 lines designed to generate genuine comments (not engagement
   bait): a question with an easy answer, a mild controversial opinion, a local
   call-out ("Vizag people, does this happen to you too?"), a "which one" choice,
   and a "tell me if I'm wrong" line.

3. CAPTIONS — 12 total, structured:
   - 3 SHORT (under 8 words, for Reels where the video carries it)
   - 4 STORY (1–2 sentences, first person, risk/objection-aware)
   - 3 OFFER (feature + proof + action)
   - 2 LOCAL (area/landmark based)
   Rules: first line must work as a standalone hook (it's all that shows before
   "more"). No emoji spam — max 2 emoji per caption and only if the brand voice allows.
   No hashtags inside the sentence.

4. HASHTAG SETS — 3 sets, mixed intent, 8–12 tags each:
   - LOCAL set (area + city + category)
   - NICHE set (specific to the product/service, not generic)
   - BROAD set (category-level, high volume)
   Flag any tag with under 10k posts (too small to add reach) and any banned
   or spam-flagged pattern.

5. PINNED-COMMENT STRATEGY — for each script, one pinned comment that:
   states the price or the process (whatever the viewer's real first question is),
   and invites a low-friction next step. Plus 3 reply templates for the most likely
   DMs (price question, availability question, "is it worth it" question).

6. CTA PLACEMENT MAP — a table: Script | Platform | Spoken CTA beat | On-screen CTA |
   End card | Pinned comment. This is the checklist the editor uses.

# HARD CONSTRAINTS
- Every CTA = verb + specific object + benefit + (where relevant) timeframe.
  Bad: "Book now". Good: "Send one photo on WhatsApp — price in 10 minutes."
- Max 1 CTA per video variant. Multiple asks kill conversions.
- Never ask for more than one action in a single CTA.
- No false scarcity. If the brief says there's no real deadline, don't invent one —
  use a slot-based or walk-in CTA instead.
- Keep language at the brief's setting (English / Hinglish / Telugu-English).
  Colloquial phrasing goes in captions and comments, never in the hero line.
- No ALL-CAPS words, no more than 2 exclamation marks across the entire document.

# BANNED CTAs
"Click here", "Learn more", "Get in touch", "Contact us today", "Don't miss out"
(unless a real deadline exists), "Act fast", "Limited time only" (same),
"Hurry", "Book now!!", "DM for details" (too vague — say what they'll get),
"Buy now", "Shop now" as a standalone, "Link in bio" alone.

# OUTPUT FORMAT
Numbered sections 1–6 in markdown, publish-ready, with counts printed for every
character-limited element.

# SELF-CHECK
1. Could a viewer complete the micro-CTA without leaving the app? (If not, it isn't micro.)
2. Does each caption's first line work alone?
3. Are all hashtags relevant (no #viral #fyp spam)?
4. Is any urgency claim unverifiable? Flag it.
5. Is any CTA asking for more than one thing?
End with "--- CTA & CAPTIONS READY ---" and scores for Friction, Clarity,
Conversion intent, Platform-fit, Honesty.
```

---

## CTA friction ladder (the concept behind the prompt)

| Level | Ask | When to use | Example |
|---|---|---|---|
| 0 | Comment a word / save the video | Cold traffic, no trust yet | "Comment PRICE and I'll send the rate card." |
| 1 | DM or WhatsApp a photo | Slightly warm, curiosity high | "Send a hair photo — you'll get a price in 10 minutes." |
| 2 | Walk in / free consultation | Local, low-commitment | "Walk in any weekday 11–4. No booking needed." |
| 3 | Book and pay a token / trial | Warm, has intent | "Book the ₹0 consultation for Saturday." |
| 4 | Buy / full booking | Retargeting only | "Book your wedding date — 4 trials left this month." |

**Rule:** cold audiences almost never take level 3–4 CTAs. Match the CTA to the temperature of the traffic, and the same video will convert better on both cold and retargeting.

## Caption anatomy that works for local + D2C

```
Line 1  → standalone hook (this is all that shows before "more")
Line 2  → the objection or the honest caveat
Line 3  → proof (number, brand, review, place)
Line 4  → the action, with the specific thing they get
Line 5  → 8–12 hashtags (local + niche + broad)
```

## Pinned comment: the most underused conversion slot

People read comments before they click anything. A pinned comment that answers "how much?" and "where are you?" converts the silent majority who never DM.

**Template:**
> 💬 "Price, since everyone asks: [service] starts at ₹[X] and goes up to ₹[Y] depending on [variable]. Exact price confirmed in writing before we start. Send a photo on WhatsApp to get your range — [link/number]. No appointment needed to ask."

That single comment removes the two biggest frictions (price and access) for every viewer who scrolls the comments instead of messaging.
