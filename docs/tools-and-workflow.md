# Tools & Workflow for UGC Ad Production

---

## 1. The AI models — what each is actually best at

| Tool | Best role here | Notes from real use |
|---|---|---|
| **Claude** | Hooks and scripts | Best at holding the banned-phrase list without being re-prompted. Produces natural hesitations and micro-complaints ("fair warning, you'll be there a while") that read as real speech. |
| **ChatGPT** | QA/compliance scan + creator briefs | Best at structured critique: it will genuinely flag a line as "sounds like an ad" and explain why. Strong at turning a script into a shootable shot list. |
| **Gemini** | Platform cutdowns, captions, hashtags | Best at 30/15/7s restructuring and caption/hashtag research. Weaker at authenticity — needs the banned list enforced twice. |

**Cross-model method:** identical brand brief pasted into all three. Any fact appearing in an output but not in the brief gets deleted — that's the guard against invented prices, reviews and results.

---

## 2. Video tools

### CapCut (free) — the workhorse
- **Auto-captions:** generate, then manually set 3–5 words per line. Never trust the default line breaks.
- **Text template:** save one style (position above the bottom 20%, 2 lines max) and reuse across every video — brand consistency without effort.
- **Audio:** trending sounds → use for organic posts only. For paid ads, use CapCut's commercial-licence audio library or your own voiceover.
- **Export preset:** 1080×1920, 30fps, H.264, high bitrate. Save it.
- **Speed trick:** edit the 30s version first, then duplicate the project and delete beats for the 15s and 7s cuts. Never rebuild from scratch.

### Runway / Pika (optional, paid credits)
- Use for **b-roll that can't be shot**: product macro textures, environment shots, abstract transitions.
- ⚠️ Do not generate **fake customers or faces** for a local business ad. Audiences are good at spotting it now, and Meta has disclosure requirements for synthetic media in some markets. Real footage of a real salon outperforms synthetic video every time.
- Legitimate uses: texture close-ups (water, foam, fabric), background plates, motion transitions between real shots.

### For local businesses: the phone is the tool
The brief-a-stylist approach in `prompts/06` beats any AI video tool for this category. 40 minutes of real footage will outperform a month of generated clips — authenticity is the product.

---

## 3. The workflow, end to end

```
1. INTAKE       prompts/00 → 14 questions with the founder → brief
                          (reviews + Instagram stalking first, so you ask better questions)

2. HOOKS        prompts/01 → 24 hooks → score /25 → promote 6
                          (read them aloud — this filters half of them)

3. SCRIPTS      prompts/02 → 6 runs, one per framework
                          (never generate 6 scripts in one run — they'll share a rhythm)

4. PLATFORM     prompts/03 → 30/15/7s, Shorts, Meta ad copy
                          (verify all character counts manually)

5. CTA/CAPTION  prompts/04 → CTAs on the friction ladder, captions, pinned comments

6. SHOOT BRIEF  prompts/06 → shot list, phone settings, consent script, edit handoff

7. QA           prompts/05 → authenticity scan + 30-point scorecard + compliance gate
                          (fix every High; check the ad-policy table)

8. PACKAGE      content-pack.md (client deck) + preview/index.html (visual) + repo

9. SHIP         GitHub push → Instagram post (tag @future_interns) → LinkedIn → client pitch
```

**Time per client once the system exists:** ~2.5 hours for the full pack. That's what makes ₹5,000 per pack viable.

---

## 4. The three lines that do the most work

1. **"Read every line out loud. If it sounds like an advertisement, it is one."**
2. **"Include one honest limitation per script. That line is what makes the other 90% believable."**
3. **"Never invent proof. Write `[NEEDS PROOF]` instead — unsubstantiated claims get ad accounts restricted, not just rejected."**

---

## 5. Cost & access

| Item | Cost |
|---|---|
| ChatGPT / Claude / Gemini free tiers | ₹0 — sufficient for this task |
| CapCut | ₹0 (free tier) |
| Phone tripod + clip mic (optional) | ₹500–₹1,300 total |
| Meta ads test budget (optional, to validate a hook) | ₹300–₹500 for 5 days |
| Runway/Pika (optional) | Paid credits — not needed for local businesses |

**Total to produce and publish a UGC content pack: under ₹1,500.** That number belongs in your pitch — it's why a local business says yes.

---

## 6. Common failure modes (and the fix)

| Failure | Symptom | Fix |
|---|---|---|
| Ad-speak creeps back | "Transform your hair today!" | Re-run the banned-list scan; it always catches 3–5 lines |
| All six scripts sound identical | Same rhythm in every open | One prompt run per framework — never batch |
| Hooks are clever but unusable | No visual partner for the line | Every hook must have an obvious first frame; if not, cut it |
| Script is unfilmable | Needs two people, a second location, or good acting | Everything must be shootable by one person, one phone, one room |
| Nothing gets filmed | Client has a script and no plan | Send the shot list + phone settings + shoot-day checklist |
| Compliance problem after publishing | "Guaranteed", before/after with no disclaimer, fake review | Run the Part C gate before delivery, every time |
| No consent, client unhappy | Footage used without permission | WhatsApp consent script, screenshot the reply, keep it |
