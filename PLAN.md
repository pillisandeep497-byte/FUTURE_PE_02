# Execution Plan — Future Interns, Prompt Engineering Task 2 (2026)
## "AI Content Marketing using UGC Ads"

**Intern:** Pilli Sandeep
**Chosen business:** Glow Studio by Sanjana — Hair & Bridal Studio, MVP Colony, Visakhapatnam
**Total time budget:** ~9 hours across 5 sessions

---

## 0. What's actually being graded

| Task requirement | Where it lives | Proof |
|---|---|---|
| Authentic UGC tone, not salesy | `prompts/05-ugc-authenticity-qa.md` + `qa-scorecard.md` | Banned ad-speak list, "say it out loud" test, 3 negative/honest lines per script |
| **Multiple hooks for one product** | `hooks.md` | 24 hooks across 10 archetypes, each scored on a 5-point rubric |
| Clear conversion intent | `scripts.md` + `ctas-captions.md` | Every script ends in a named action; 18 CTA variants |
| Platform-specific content | `platform-variants.md` | Reels 30/15/7s, Shorts, Meta ad copy, TikTok pacing |
| Reusable prompt structure | `prompts/00`–`06` | Variable-driven, 6 brand types proven in `adaptability-proof.md` |
| UGC Ad Content Pack | `content-pack.md` | The single file you'd send a brand founder |
| Public GitHub repo + docs | `README.md`, this file, `docs/` | Requirement-by-requirement map in `docs/submission-checklist.md` |
| **Mandatory Instagram post** | `docs/instagram-post.md` | Ready-to-post captions + carousel plan, tag **@future_interns** |

**The differentiator:** most submissions are "I asked ChatGPT for a UGC script". Yours is a *production system* — hook library with a scoring rubric, six frameworks, platform cutdowns, a compliance gate, and a shot brief a stylist can shoot between clients. That's what an agency sells.

---

## 1. The five sessions

### Session 1 — Brand + product intake (60 min)
Pick a product you can actually get footage of. Ranked by how easy they are to sell and shoot:

1. **Local business** (salon, cafe, gym, clinic) — easiest footage access, easiest to pitch in person, real customers available
2. **D2C product you own or can get a sample of** — most ad budget, most competition, highest per-script rates
3. **Creator brand / course** — you can be the UGC creator yourself
4. **SaaS** — highest pay per script, hardest to make look native

Then run `prompts/00-brand-product-intake.md` with the founder (or fill it yourself from their site, reviews and Instagram if you can't get a meeting). **Reviews are gold** — real customer complaints and compliments are where the best hooks come from.

### Session 2 — Hook engineering (90 min)
This is the session that decides whether the ads work.

1. Run `prompts/01` → get 20–30 hooks.
2. Score each on the rubric (scroll-stop, clarity, honesty, native-to-platform, no ad-speak).
3. Promote the top 6 into scripts. Keep the rest — they become A/B variants and short-form captions.
4. **Read every hook out loud.** If you'd feel awkward saying it to a friend, it's an ad, not a hook.

### Session 3 — Script writing (2 hr)
1. `prompts/02` → 6 scripts, one per framework: PAS, BAB, Storytime/POV, Objection-crusher, Review-reaction, Founder-POV.
2. Each script comes back beat-by-beat with timestamps, shot list, b-roll, on-screen text and audio direction — not just dialogue.
3. `prompts/06` → the creator/shot brief. **This is what you hand over** — most people send a script and the business films nothing. Send a shot list and they film it the same day.
4. Cut everything that isn't shootable on a phone by one person.

### Session 4 — Platform adaptation + captions (90 min)
1. `prompts/03` → 30s → 15s → 7s cutdowns, Shorts, Meta ad primary text + headline.
2. `prompts/04` → CTAs (3 per script), 12 captions, pinned-comment strategy.
3. Note the hard platform rules: Reels hook window ~1.5s, Shorts ~3s, Meta feed ~3s; 9:16 for Reels/Shorts/TikTok; burned-in captions everywhere (85% watch on mute).

### Session 5 — QA, packaging, shipping (2 hr)
1. `prompts/05` → authenticity + ad-compliance scorecard. Fix every High flag.
2. Assemble `content-pack.md` — the client-facing deck (no rationale notes).
3. Build `preview/index.html` and screenshot it.
4. Push to GitHub (`ai-ugc-ad-generator`), post on **Instagram** (mandatory — tag `@future_interns`), post on LinkedIn, then pitch the business.

---

## 2. Deliverables checklist

```
✅ UGC Ad Content Pack   → client-runs/01-.../content-pack.md
   ├── 24 hooks (scored)
   ├── 6 scripts (beat-level, shootable)
   ├── 18 CTAs + 12 captions
   └── 6 platform variants
✅ Structured prompts     → prompts/00 … 06
✅ Generated outputs      → client-runs/01-glow-studio-vizag/
✅ Documentation          → README.md + docs/
✅ Instagram post         → docs/instagram-post.md (tag @future_interns)
✅ LinkedIn post          → docs/linkedin-post.md
```

---

## 3. Exact GitHub commands

```bash
cd ~/ai-ugc-ad-studio
git init
git add .
git commit -m "feat: AI UGC ad prompt system + content pack (Glow Studio, Vizag)"
git branch -M main
git remote add origin https://github.com/pillisandeep497-byte/ai-ugc-ad-generator.git
git push -u origin main
```

Repo settings: **Description** — `Reusable prompt system that generates UGC-style short-form video ad content: hooks, scripts, CTAs, platform cutdowns and ad-compliance QA. Future Interns Prompt Engineering Task 2.`
**Topics:** `ugc-ads`, `prompt-engineering`, `ai-marketing`, `short-form-video`, `instagram-reels`, `future-interns`

---

## 4. Selling this (the Learn & Earn part)

| Package | What you deliver | Suggested price |
|---|---|---|
| **Starter** | 5 hooks + 1 script + caption | ₹1,500 |
| **Standard** | 10 hooks + 3 scripts + CTAs + captions + shot brief | ₹5,000 |
| **Campaign** | 15 hooks + 5 scripts + 3 platform cutdowns + Meta ad copy + 1 revision round | ₹12,000 |
| **Retainer** | 4 scripts + 8 hooks + captions monthly | ₹8,000/month |

Agencies in India pay roughly ₹2,000–₹6,000 **per UGC script**, and D2C brands buying "creator-style" content often pay ₹5,000–₹15,000 for a script + shot brief. Your advantage: you deliver in a day with a documented system. Full pitch scripts in `docs/client-outreach-and-rate-card.md`.

---

## 5. Do-not-skip

1. **Read every script out loud.** If it sounds like an ad, it is one, and it will underperform.
2. **Keep the negative line.** "It's not the cheapest in MVP Colony" is the most persuasive sentence in the pack.
3. **Never invent proof.** `[NEEDS PROOF]` flags exist for a reason — unsubstantiated claims = rejected ads and restricted ad accounts.
4. **Add the disclosure.** Paid creator content needs `#ad`; check Meta's rules before running anything as paid media.
5. **Post to Instagram.** It's mandatory for this task and it's how you get inbound client DMs.
6. **Shoot one of the scripts yourself.** A 25-second phone video of your own product or a willing local shop turns a "content pack" into a portfolio.
