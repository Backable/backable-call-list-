# Backable Call Sheet — Setup Guide
Two steps. Takes about 10 minutes total. Free.

---

## STEP 1 — Put the app online (Netlify)

1. Go to **netlify.com** and click "Sign up" — use your Google or GitHub account
2. Once logged in, you'll see a dashboard. Look for a box that says **"Deploy manually"** or drag and drop
3. Drag the entire **backable-deploy** folder onto that box
4. Netlify gives you a URL instantly — something like `https://amazing-name-123.netlify.app`
5. Share that URL with your team member — that's all they need

> Want a cleaner URL? In Netlify go to Site Settings → General → Change site name
> You can make it something like `backable-calls.netlify.app`

---

## STEP 2 — Set up shared sync (JSONBin)

This is what makes "mark as called" sync between both callers in real time.

1. Go to **jsonbin.io** and click "Sign Up Free"
2. Once logged in, click your profile icon (top right) → **API Keys**
3. Click **"+ Create API Key"** — name it "Backable"
4. Copy the key that appears (starts with `$2b$10$...`)

Now open your Netlify app URL and:
1. Click **⚙️ Setup** (top right of the app)
2. Paste your API key into the first field
3. Leave "Bin ID" blank — it creates one automatically on first save
4. Click **Save & connect**

**Share the same API key with your second caller.** They do the same setup steps on their browser. Once both are connected, "mark as called" syncs between them in real time.

> The Bin ID is created the first time someone uploads an Excel file. After that, copy it from the Setup field and give it to the second caller too — paste it into their "Bin ID" field so they connect to the same data.

---

## DAILY USE

**Each morning:**
1. Open the app URL
2. Enter your name
3. Upload today's Excel file (one person does this — it syncs to the other automatically)
4. Work down the call list — click "Mark as called" after each one
5. Hit ↻ Refresh any time to see what your colleague has marked

**Excel columns needed:**
- First Name
- Last Name
- Phone
- Email
- Signup Date
- Everything Complete? (Yes/No)
- Profile Setup Complete? (Yes/No)
- Dream Analyser Complete? (Yes/No)

---

## CALL TYPES

| Badge | Meaning |
|-------|---------|
| ⚡ Reactivate call | Signed up before Feb 2026 — re-engage |
| 💰 Buy now call | 14+ days since signup — convert to paid |
| 🔔 Prompt — Everything | 3+ days, hasn't completed Everything |
| 🔔 Prompt — next steps | Completed Everything, missing Profile Setup or Dream Analyser |

---

## IF SOMETHING GOES WRONG

**"Sync error" showing** — check your API key is correct in ⚙️ Setup

**Second caller not seeing updates** — make sure they have the same API key AND Bin ID in their Setup panel

**Excel not loading** — check column names match exactly (case doesn't matter, but the words do)

**Works offline too** — if there's no internet, the app saves locally to that browser. It'll push to the cloud next time there's a connection.

---

Questions? Forward to whoever built this.
