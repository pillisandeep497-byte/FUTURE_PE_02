# Upload guide — the no-drag method (folder structure safe)

Your unzipped folder looks like this:

```
ai-ugc-ad-studio/
├── README.md  PLAN.md  LICENSE  .gitignore      ← 4 files at root
├── prompts/            7 files   ← THE MOST IMPORTANT FOLDER
├── client-runs/
│   ├── adaptability-proof.md
│   └── 01-glow-studio-vizag/   9 files
├── docs/               5 files
└── preview/            1 file (index.html)
```

---

## Step 0 — Create the repo

GitHub → **+** → **New repository** → name: `ai-ugc-ad-generator` → **Public** →
do **NOT** tick "Add a README file" → **Create repository**.

## Step 1 — Root files (4 files)

**Add file ▾ → Upload files → choose your files** → select `README.md`, `PLAN.md`,
`LICENSE`, `.gitignore` → **Commit changes**.

*(`.gitignore` is hidden: Windows → View → Show → Hidden items; macOS → Cmd+Shift+.)*
If you can't find it, skip it and create it later with **Create new file**.

## Step 2 — Create the `prompts/` folder FIRST

1. **Add file ▾ → Create new file**
2. In the file name box type exactly: `prompts/README.md`  *(the slash creates the folder)*
3. Content:
   ```
   # Prompts

   The structured UGC ad prompt system. Read in order:
   00 brand brief → 01 hooks → 02 scripts → 03 platform → 04 CTA/caption → 05 QA → 06 shot brief
   ```
4. **Commit changes**

## Step 3 — Put the 7 prompt files inside it

1. Click into the **`prompts`** folder (breadcrumb shows `ai-ugc-ad-generator / prompts`)
2. **Add file ▾ → Upload files → choose your files**
3. Open your unzipped `prompts` folder → select **all 7 files** → Open → **Commit changes**

✅ You should now see 7 files + README.md inside `prompts/`.

## Step 4 — `client-runs/01-glow-studio-vizag/`

1. **Create new file** → name: `client-runs/01-glow-studio-vizag/README.md`
   Content: `# Client run 01 — Glow Studio by Sanjana, MVP Colony, Visakhapatnam` → Commit
2. Click into that folder → **Upload files → choose your files** →
   select all **9 files** from your unzipped `client-runs/01-glow-studio-vizag` folder → Commit

## Step 5 — `client-runs/adaptability-proof.md`

Go back to the **`client-runs`** folder → **Upload files → choose your files** →
select **only** `adaptability-proof.md` → Commit.

## Step 6 — `docs/` (5 files)

1. Create new file: `docs/README.md` with content `# Docs — checklist, Instagram, LinkedIn, outreach, tools` → Commit
2. Click into `docs` → Upload the 5 files from your unzipped `docs` folder → Commit

## Step 7 — `preview/` (1 file)

1. Create new file: `preview/README.md` with content `# Preview — open index.html to see the content pack as a page` → Commit
2. Click into `preview` → Upload `index.html` → Commit

---

## Final check — repo home should show 8 items

```
client-runs/    docs/    preview/    prompts/
.gitignore   LICENSE   PLAN.md   README.md
```

Open `README.md` — it must render **formatted** (headings, bold, tables), not as plain text.

---

## The 10-second anti-flatten check

After dropping files on GitHub's upload page, look at the file list:

- ✅ `prompts/01-hook-generator.md` → folder preserved
- ❌ `01-hook-generator.md` → **flattened. Click Cancel and redo step 3.**

---

## Bulletproof alternative: GitHub Desktop

1. Install **GitHub Desktop** → sign in → **File → Clone repository** → pick `ai-ugc-ad-generator`
2. Open the cloned folder and delete everything inside it
3. **Copy the contents** of your unzipped folder into it (4 folders + 4 files)
4. GitHub Desktop → summary: `Add UGC ad system` → **Commit to main** → **Push origin**

Folders are guaranteed correct, and every future edit is two clicks.
