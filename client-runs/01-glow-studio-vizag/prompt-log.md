# Prompt Log — which prompt produced what

| # | Prompt | Output | Model | Notes |
|---|---|---|---|---|
| 1 | `prompts/00-brand-product-intake.md` | `product-brief.md` | Claude | 14 questions, then the brief template. Prices left flagged. |
| 2 | `prompts/01-hook-generator.md` | `hooks.md` | Claude; cross-checked on ChatGPT | 24 hooks across 10 archetypes + scoring rubric. 4 hooks were cut and rewritten. |
| 3 | `prompts/02-ugc-script-generator.md` | `scripts.md` | Claude | Run 6 times, once per framework, so the rhythms differ. |
| 4 | `prompts/03-platform-adapter.md` | `platform-variants.md` | Gemini | 30/15/7s cutdowns, Shorts, Meta ad copy. Character counts verified manually. |
| 5 | `prompts/04-cta-caption-comments.md` | `ctas-captions.md` | Claude | 18 CTAs, 12 captions, hashtag sets, pinned comments, DM replies. |
| 6 | `prompts/06-creator-brief-and-shotlist.md` | `creator-shot-brief.md` | ChatGPT | Shot list, shoot schedule, consent script, edit handoff. |
| 7 | `prompts/05-ugc-authenticity-qa.md` | `qa-scorecard.md` | ChatGPT + manual | Found 11 ad-speak violations; compliance gate flagged 2 blockers. |
| 8 | — | `content-pack.md` | Manual assembly | Client-facing version: rationale notes and internal flags consolidated. |

---

## Model comparison (from actually running all three)

| Aspect | Claude | ChatGPT | Gemini |
|---|---|---|---|
| Holding the banned-phrase list | **Strongest** — self-corrects mid-generation | Good, needs one re-prompt | Reintroduces clichés in CTAs |
| UGC authenticity (sounds like a person) | **Best** — natural micro-complaints and hesitations | Good | Tends to write ad-voiceover prose |
| Beat-level output with timestamps | **Best** | Very good | Good |
| Platform rules & character counting | Good (verify counts manually) | Good | **Best for cutdowns + caption work** |
| Compliance awareness | Good — flags claims when told to | **Best at the QA/policy scan** | Weakest |
| Caption/hashtag ideation | Good | Good | **Best** |
| Best role in this project | Hooks + scripts | QA + compliance + creator brief | Platform cutdowns + captions |

**Workflow used:** Claude for hooks and scripts → Gemini for platform variants and captions → ChatGPT for the compliance/authenticity scan. Same brief pasted into each so all three worked from identical facts.

---

## What I changed by hand (the honest 20%)

1. **Cut 11 ad-speak lines** the raw drafts contained — logged in `qa-scorecard.md`.
2. **Added "bring a charger" and the bakery landmark** — real local detail only a site visit produces.
3. **Rewrote every CTA.** The raw output still leaned on "book now" and "link in bio".
4. **Removed "transformation" language** — a word the owner dislikes and a compliance liability in beauty ads.
5. **Softened three efficacy claims** ("repairs damaged hair" → "leaves hair smoother").
6. **Replaced 4 hooks** that failed the "would a friend say this" test.
7. **Added the refusal story** (Script 6) from the owner's actual operating rule.
8. **Cut 6 exclamation marks** across the pack (down from 6 to 0).
9. **Rebalanced Script 1** after the read-aloud test — the first draft had four sentences that sounded like a voiceover.

---

## Reproducing this for another brand

1. `prompts/00` → new brief (20–30 min with the founder)
2. `prompts/01` → 24 hooks, score them, promote 6
3. `prompts/02` → 6 runs, one per framework
4. `prompts/03` → platform cutdowns
5. `prompts/04` → CTAs, captions, comments
6. `prompts/06` → shot brief for whoever films
7. `prompts/05` → scan, fix High flags, check the compliance gate

**Time:** ~2.5 hours once the system exists. That's what makes it sellable per script.
