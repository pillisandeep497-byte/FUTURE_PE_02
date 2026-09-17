# AI UGC Ad System — Prompt Framework for Short-Form Video Ads

**A reusable prompt system that turns one product brief into a full UGC ad content pack: hooks, scripts, CTAs, captions, platform cutdowns, creator briefs, and an ad-compliance QA pass.**

Built for **Future Interns — Prompt Engineering Task 2 (2026)**.
**Author:** Pilli Sandeep · **Contact:** WhatsApp +91 91002 12761

---

## Why this exists

Polished brand ads get scrolled past. UGC-style ads work because they look like a friend's phone video and sound like an honest opinion. Brands, D2C founders and agencies now buy this content by the script — but most people writing "UGC scripts with AI" produce generic ad copy with a fake-casual voice. It reads like a script. It doesn't read like a person.

This system fixes that with three things:

1. **A hook library with a scoring rubric** — the first 2 seconds decide the ad, so hooks get generated in volume and scored before anything else is written.
2. **UGC authenticity constraints** — banned phrases, "say it out loud" tests, permission to be negative, and a rule against ad-speak.
3. **An ad-compliance gate** — because real UGC ads run as paid media, and unsubstantiated claims get accounts banned.

---

## The client run

**Glow Studio by Sanjana** — hair & bridal studio, MVP Colony, Visakhapatnam
*(Same client as Task 1, so the two projects read as one agency relationship: website copy + paid ad content.)*

**Problem the ads solve:** the studio has 4 chairs, a 7-day waiting list problem in wedding season, and no video content. It cannot afford a production agency. But it has something better — 300 brides, repeat clients, and an owner who says honest things on camera ("if your hair can't take keratin, we'll say no").

**The ad system built for them:** 24 hooks, 6 shootable scripts (20–35s), 3 CTAs each, 12 captions, 6 platform cutdowns, and a shot-by-shot creator brief that a stylist can film on a phone between clients.

> ⚠️ **Integrity note:** Glow Studio is a **representative demonstration business**, not a verified client. Prices, client counts and testimonials are marked `*(verify)*`. Before running this for a paying brand: replace the brief with real facts, and confirm every claim is substantiated — UGC ads run as paid media and are subject to Meta/Google ad policies. See `prompts/05-ugc-authenticity-qa.md`.

📄 Brief: [`client-runs/01-glow-studio-vizag/product-brief.md`](client-runs/01-glow-studio-vizag/product-brief.md)

---

## What the system produces

| Output | What's inside |
|---|---|
| **Hooks** | 24 hooks across 10 archetypes, each scored on a 5-point rubric (scroll-stop, clarity, honesty, native-to-platform, no ad-speak) |
| **Scripts** | 6 full scripts using 6 different frameworks: PAS, BAB, Storytime/POV, Objection-crusher, Review-reaction, Founder-POV |
| **Shot + creator brief** | For each script: timestamped beats, shot list, b-roll, on-screen text, audio direction, who films it, what to shoot on a phone |
| **CTAs & captions** | 3 CTA variants per script, 12 captions, hashtag sets, pinned-comment strategy |
| **Platform cutdowns** | Reels 30s / 15s / 7s, YouTube Shorts, Meta ad primary text + headline, TikTok-style pacing notes |
| **QA & compliance** | 30-point scorecard: authenticity + ad-policy risk + claim substantiation + accessibility |

---

## The prompt logic (how the system works)

Every prompt in this repo follows the same eight-part skeleton:

```
ROLE → BRAND DNA → TASK → HARD CONSTRAINTS → BANNED LIST
→ OUTPUT FORMAT → QUALITY BAR → SELF-CHECK
```

**Seven decisions that make the output usable rather than generic:**

| Decision | Why it matters |
|---|---|
| **Hooks are generated first, separately, and scored** | 80% of a UGC ad's performance is the first 2 seconds. Writing hooks as a volume exercise (with a scoring rubric) beats writing one clever line. |
| **A framework library, not one template** | Six frameworks stop the sixth script sounding like the first. Each script is labelled with its framework so you can A/B test structure, not just wording. |
| **The "say it out loud" test** | Every line must be something a real customer would actually say. Scripts get flagged where they fail. |
| **Permission to be negative** | Real UGC names a downside ("it's not the cheapest in MVP Colony"). The prompt requires at least one honest limitation per script — it raises trust and lowers ad-fatigue. |
| **Banned ad-speak list** | "Game-changer", "must-have", "transform your life", "link in bio" alone as a CTA — all banned. This is what separates UGC from an ad. |
| **A compliance gate** | Health/beauty claims, before/after rules, "results may vary", paid-partnership disclosure (#ad), and music licensing notes. Most AI UGC systems ignore this. It's the difference between content that can be published and content that gets an account restricted. |
| **Platform-specific constraints are hard rules** | Hook window (1.5s Reels vs 3s Meta feed), caption burn-in, aspect ratio, safe zones, and text limits are enforced per platform, not left to the model's judgement. |

**Reusability:** the brand intake brief (prompt 00) is the only thing that changes between clients. See [`client-runs/adaptability-proof.md`](client-runs/adaptability-proof.md) — the same system run on a D2C skincare brand, a cafe, a gym, a SaaS tool and a dental clinic, each with genuinely different hooks and voice.

---

## Tools used

| Tool | Role |
|---|---|
| **Claude** | Primary script + hook generation (best at holding the "ban list" and the authenticity voice) |
| **ChatGPT** | Framework variation, objection-mapping, and the QA/compliance scan |
| **Gemini** | Platform cutdowns, caption/hashtag research, hook A/B matrix |
| **CapCut** | Editing the shot list into a finished ad (burned-in captions, 3-beat cut rhythm, trending audio) |
| **Runway / Pika** *(optional)* | B-roll generation where the business can't shoot (product close-ups, textures) |
| **Canva / Instagram** | Publishing the mockup for the mandatory social sharing step |

---

## Repo structure

```
.
├── prompts/                                   ← THE SYSTEM
│   ├── 00-brand-product-intake.md             ← 14-question brief + variable map
│   ├── 01-hook-generator.md                   ← 10 archetypes + scoring rubric
│   ├── 02-ugc-script-generator.md             ← 6 frameworks + beat-level output
│   ├── 03-platform-adapter.md                 ← Reels / Shorts / Meta / TikTok rules
│   ├── 04-cta-caption-comments.md             ← CTAs, captions, pinned comments
│   ├── 05-ugc-authenticity-qa.md              ← 30-point authenticity + ad-policy scorecard
│   └── 06-creator-brief-and-shotlist.md       ← brief a phone-shooter, not a film crew
│
├── client-runs/
│   ├── 01-glow-studio-vizag/
│   │   ├── product-brief.md                   ← filled intake
│   │   ├── hooks.md                           ← 24 hooks, scored
│   │   ├── scripts.md                         ← 6 shootable scripts
│   │   ├── ctas-captions.md                   ← CTAs, captions, hashtags, comments
│   │   ├── platform-variants.md               ← 30s/15s/7s, Shorts, Meta ad copy
│   │   ├── creator-shot-brief.md              ← what to film, on what, in what order
│   │   ├── qa-scorecard.md                    ← scored + compliance flags
│   │   ├── prompt-log.md                      ← which prompt made what
│   │   └── content-pack.md                    ← ⭐ the deliverable you hand the client
│   └── adaptability-proof.md                  ← 1 system, 5 brands, 5 voices
│
├── preview/index.html                         ← visual content pack (screenshot for IG/LinkedIn)
├── docs/
│   ├── submission-checklist.md
│   ├── instagram-post.md                      ← MANDATORY social sharing copy
│   ├── linkedin-post.md
│   ├── client-outreach-and-rate-card.md       ← how to sell this (₹ per script)
│   └── tools-and-workflow.md
├── PLAN.md                                    ← execution plan + time budget
├── LICENSE · .gitignore
```

---

## How to reuse for another brand (about 90 minutes)

1. **Intake** (`prompts/00`) — 14 questions with the founder. Fill `product-brief.md`.
2. **Hooks** (`prompts/01`) — generate 20+, score them, keep the top 6.
3. **Scripts** (`prompts/02`) — one script per framework, minimum 6.
4. **Platform cutdowns** (`prompts/03`) — 30s → 15s → 7s, plus Meta ad copy.
5. **CTAs + captions** (`prompts/04`).
6. **Creator brief** (`prompts/06`) — hand this to whoever films.
7. **QA** (`prompts/05`) — fix every High-severity flag, then publish.

**Human pass before delivery:** read every script out loud. If a line sounds like an ad, cut it. Add one detail only a real customer would know.

---

## Results

| Metric | Result |
|---|---|
| Hooks written & scored | 24 (top 6 promoted into scripts) |
| Full scripts | 6, using 6 different frameworks |
| Platform variants | 6 (Reels 30/15/7, Shorts, Meta ad, TikTok pacing) |
| CTAs | 18 (3 per script) + 12 captions |
| Ad-policy flags caught by QA | See `qa-scorecard.md` — 5 claims softened, 3 disclosures added |
| Banned ad-speak in final pack | 0 (11 removed during QA) |
| Brands the system has been proven on | 6 (salon, D2C skincare, cafe, gym, SaaS, dental clinic) |

---

## Limitations (honest version)

- **Scripts are not videos.** This system produces the script, hooks, shot list and edit beats. Filming and editing still need a phone and 40 minutes in CapCut.
- **Claims must be substantiated by the brand.** Where the brief has no proof, scripts carry a `[NEEDS PROOF]` flag instead of an invented benefit. In beauty and health categories this isn't optional — it's the difference between a running ad and a rejected one.
- **Hook performance is empirical.** The rubric predicts, it doesn't guarantee. Always shoot 2–3 hook variants of the same script and let the platform decide.
- **AI-generated UGC faces have disclosure requirements** on Meta in some markets, and audiences increasingly spot them. Real customer footage outperforms synthetic faces for local businesses — this system is built for real footage, with AI used for scripts and cutdowns.

---

## License

MIT. Prompt system by **Pilli Sandeep** for the Future Interns Prompt Engineering Internship, 2026.
