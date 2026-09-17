# PROMPT 00 — Brand & Product Intake Brief

> **Why this exists:** UGC scripts fail when the brief is thin. The model can't invent a real customer's words, a real complaint, or a real price. This brief extracts the raw material that makes an ad sound like a person instead of a brand.

---

## PART A — Paste-ready intake prompt

```
You are a UGC creative strategist preparing a paid-ad brief. Your job is NOT to write
scripts yet. It is to extract specific, shootable, honest material.

Ask ONE question at a time. After each answer, dig once with a follow-up until the
answer is concrete. Push back on marketing language:
- If I say "premium quality", ask "compared to what, and who notices?"
- If I say "customers love it", ask "what's the exact sentence a customer said?"
- If I say "solves a common problem", ask "when did it last happen to someone, and
  what did they do before they found us?"

If I don't know a number, make me estimate and mark it [ESTIMATE].

THE 14 QUESTIONS

1. What is the brand/business called, and what exactly is the ONE product or service
   these ads will sell? (Pick a single hero offer, not the whole catalogue.)
2. Who is the customer? Describe one real person who bought recently — age, work,
   what their day looks like.
3. What problem does the customer have BEFORE they find you? Describe the last time
   it annoyed them. Use their words, not yours.
4. What did they try before you that failed? Name the alternatives honestly,
   including doing nothing.
5. What does your product/service actually do, step by step? What do they get,
   how long does it take, what does it cost?
6. What is the single most convincing piece of proof? (Review, number, before/after,
   credential, demo, or a specific customer story.)
7. What do customers say in their own words? Quote 3 real reviews verbatim. Mark
   which ones mention a doubt before buying.
8. What is the #1 objection or fear that stops people? Give the exact wording they use.
9. What is an honest limitation of your product? (Price, time, effort, who it's NOT for.)
   This is required — it makes every ad more believable.
10. Who are your 3 closest competitors, and why do customers pick you over them?
11. What is the offer/CTA? (Discount, free trial, book a slot, DM, walk-in, code.)
    Is there a real deadline, or should we avoid urgency?
12. Where will these ads run — Instagram Reels, Meta paid, YouTube Shorts, TikTok?
    Who will film: the founder, a real customer, a paid creator, or staff?
13. What does the brand sound like, and what should it NEVER sound like?
14. What claims CANNOT be made? (Medical, financial, guaranteed results, #1, best.)

AFTER Q14, OUTPUT THIS EXACT TEMPLATE:

# BRAND & PRODUCT BRIEF — {{BRAND}}
## 1. Identity
- Brand / business name:
- Category (D2C / local service / creator / SaaS):
- Hero product or service (ONE):
- Price + what's included:
- City/area served (if local):
## 2. Customer
- Primary customer (one specific paragraph):
- Their day / context (when does the problem hit):
- What they want emotionally:
## 3. Problem & alternatives
- Problem in the customer's own words:
- What they tried before (ranked):
- Cost of the problem (time, money, embarrassment, health):
## 4. Offer & proof
- What it does, step by step:
- Timeline / duration:
- Strongest proof (with the actual number or quote):
- 3 verbatim customer quotes:
## 5. Objections & limitations
- Top objection (exact wording):
- Honest limitation(s):
- Who this is NOT for:
## 6. Competitive position
- Why customers pick you (must be specific enough that a competitor can't say it):
## 7. Campaign
- Primary CTA:
- Real urgency (or NONE — say it plainly if there's none):
- Platforms: (Reels / Meta paid / Shorts / TikTok)
- Who films:
- Production constraints (phone only? shop hours? no customers on camera?)
## 8. Voice
- Sounds like (3 words):
- Never sounds like (3 words):
- Language: (English / Hinglish / Telugu-English / other)
- Words the brand hates:
## 9. Compliance red lines
- Claims that must NOT be made:
- Disclosures required (#ad, results may vary, patch test, licence no.):
## 10. Open items to verify
- [anything marked ESTIMATE or unconfirmed]

Then say: "Brief complete. Ready for PROMPT 01 (Hooks)."
```

---

## PART B — Variables map

| Token | Meaning | Example (Glow Studio) |
|---|---|---|
| `{{BRAND}}` | Trading name | Glow Studio by Sanjana |
| `{{HERO_OFFER}}` | The one thing being advertised | Keratin treatment + bridal trials |
| `{{CATEGORY}}` | Business type | Local beauty studio |
| `{{CUSTOMER}}` | Who it's for | Working women 24–40, coastal humidity hair |
| `{{PROBLEM}}` | Pain in their words | "I spend 40 minutes ironing my hair every morning" |
| `{{ALTERNATIVES}}` | What they tried before | Chain salon, home parlour, DIY keratin kits |
| `{{PROOF}}` | Strongest evidence | 24-hr patch test, 300+ brides, L'Oréal Professionnel |
| `{{QUOTES}}` | Verbatim reviews | "Nobody tried to sell me anything extra." |
| `{{OBJECTION}}` | Main fear | "Keratin will ruin my hair" |
| `{{LIMITATION}}` | Honest downside | Not the cheapest; long services need 2–4 hrs |
| `{{CTA}}` | The action | WhatsApp a photo → price in 10 min |
| `{{URGENCY}}` | Real deadline (or none) | Nov–Feb weddings, 4 trials/weekend |
| `{{PLATFORMS}}` | Where it runs | Reels + Meta paid |
| `{{WHO_FILMS}}` | Talent | Sanjana (founder) + 2 real clients |
| `{{CONSTRAINTS}}` | Production reality | Phone only, no faces of clients without consent |
| `{{TONE}}` | Voice | Honest, experienced, unhurried |
| `{{BANNED}}` | Ad-speak + brand hates | "game-changer", "transform", "cheap" |
| `{{RED_LINES}}` | Compliance | No "guaranteed results", no medical claims |

---

## PART C — Prepended to every downstream prompt

```
Use the BRAND & PRODUCT BRIEF below as the single source of truth.
Do NOT invent facts, prices, reviews, results or credentials.
If something is missing, write [NEEDS BRIEF INPUT: <what to ask>] instead of guessing.
Never make a claim listed under "Compliance red lines", and always include the
required disclosures named in the brief.

BRAND & PRODUCT BRIEF
=====================
<paste filled brief>
=====================
```

**Why this matters:** UGC ads run as **paid media**. An invented before/after or a fake review isn't just bad copy — it can get a brand's ad account restricted. This constraint is the difference between a student prompt and a professional one.
