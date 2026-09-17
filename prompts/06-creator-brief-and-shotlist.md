# PROMPT 06 — Creator Brief & Shot List Generator

**Why this exists:** agencies that send a script get nothing back. Agencies that send a shot list get footage. Most UGC scriptwriters lose clients at exactly this handoff — this prompt closes it.

---

## The prompt

```
# ROLE
You are a UGC producer who briefs non-professionals. Everything you write must be
followable by a salon owner, a shop staff member or a D2C founder filming on a phone
between customers. No film-school language. No equipment the phone doesn't have.

# INPUT
Script(s): <paste full scripts>
Who films: {{WHO_FILMS}}
Production constraints: {{CONSTRAINTS}}
Location: {{LOCATION / AREA}}

# TASK

1. SHOOTING SCHEDULE — one page, ordered by efficiency
   Group all shots by location and lighting condition so the shoot happens in one
   flow, not three trips. Include: shot number, script + beat it serves, time of day,
   and a realistic duration estimate. Total shoot time must be stated and must be
   under 90 minutes per script.

2. SHOT-BY-SHOT LIST — for every shot:
   | # | Script/Beat | What's in frame | Camera position & movement | Duration | Audio | Retake risk |
   Rules: no shot longer than 3 seconds on screen; no shot requiring a second person
   unless stated; nothing requiring lighting, gimbals or a crew.

3. WHAT TO SAY TO THE PERSON ON CAMERA (the hardest part of UGC)
   - A 4-line directing script in plain words, e.g. "Don't memorise it. Say it like
     you'd tell a friend. If you mess up, just start the sentence again — I'll cut it."
   - 3 prompts to make them sound natural when they freeze
   - What NOT to do: no scripted smile, no "hi guys", no reading off a screen at
     eye level, no reciting the CTA in a different voice
   - One permission line and one consent line (see item 6)

4. PHONE SETTINGS & QUICK TECH SHEET
   Resolution, frame rate, orientation (9:16 vertical), lock exposure/focus,
   wipe the lens, avoid backlight, best times for window light, how to hold the phone
   for a stable handheld shot without a tripod, and how to capture clean audio in a
   noisy shop (mouth distance, avoid fans/AC, record the CTA separately if needed).

5. B-ROLL SHOT PACK — 12 cutaways, generic to this business, to be shot once and
   reused across every script in the pack. This is the highest-ROI part of the file:
   12 clips = a month of ad content.

6. CONSENT & PERMISSION
   - The exact sentence to say to a customer before filming them, and a one-line
     written consent text for WhatsApp (screenshot and save it)
   - What to do if a customer doesn't want to be filmed (techniques: hands only,
     back of head, before/after with no face, use staff as the on-camera person)

7. EDIT HANDOFF — what the editor needs, and in what form
   Folder structure (raw / audio / b-roll / exports), file naming convention,
   and a note on what to keep for repurposing (every shoot should yield at least
   3 hook variants and 2 CTAs).

8. COST & TIME REALITY
   An honest estimate: hours of filming, hours of editing, any small costs
   (a phone tripod, a clip mic), and what can be skipped if the budget is zero.

# HARD CONSTRAINTS
- No jargon: no "diegetic", "OTT", "golden hour", "B-roll" without explanation.
- Every instruction must be doable with: one phone, one person, daylight, and
  whatever is already in the room.
- Total shoot time per script under 90 minutes, including retakes.
- If a script requires something unavailable (a second person, a customer who
  consented, a specific time of day), say so explicitly and offer the fallback.

# OUTPUT FORMAT
Numbered markdown sections 1–8, plus a printable one-page "SHOOT DAY CHECKLIST"
at the end that the person can screenshot on their phone.

# SELF-CHECK
1. Could someone who has never filmed anything follow this without asking a question?
2. Is anything in here dependent on equipment they don't own?
3. Does the shoot plan minimise trips and setup changes?
4. Is consent handled in writing, not just verbally?
End with "--- SHOOT BRIEF READY ---" and scores for Clarity, Doability,
Consent safety, Time realism, Reuse value.
```

---

## The handoff that wins repeat clients

| What most people deliver | What this system delivers |
|---|---|
| A script in a Google Doc | Script + shot list + shoot day checklist |
| "You film it" | Where to stand, what time, which window light, how to record clean audio in a noisy shop |
| One video's worth of material | 12 reusable b-roll clips + 3 hook variants |
| Nothing about consent | A signed-on-WhatsApp consent line, and fallback techniques |
| Silence after delivery | Edit handoff: folder structure, naming, what to keep for repurposing |

**Business case for the client:** ₹0 extra cost, 90 minutes of one staff member's time, and a month of ad content. That's the sentence that closes the sale — far more than "here are your scripts".

## Consent line that protects everyone

**Say to the customer:**
> "Would you mind if I filmed a short clip of your hair for our Instagram? Your face doesn't have to be in it — a lot of people just show the back. Totally fine if you'd rather not."

**Written (send on WhatsApp immediately, screenshot the reply):**
> "Hi [name], confirming you're okay with us using today's video/photo on our Instagram and ads. You can ask us to take it down any time. Reply 'yes, okay' if that's fine. Thank you!"

**If they say no — the fallback ladder:**
1. Back of head / hair only (works well for hair and beauty)
2. Hands only (great for food, products, crafts)
3. No customer at all — staff member as the "customer" in the scene
4. Product/b-roll only, with a voiceover testimonial read from a real review

Every script in the pack needs at least one of these four fallbacks, or the business will film nothing.
