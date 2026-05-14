# Jade Daily Pulse — Setup

Seven short steps. About 15 minutes. By the end, a 1-page brand memo will land on your computer every morning at 7am.

**Before you start:** Make sure Claude Desktop is installed and you're on a paid plan (Pro, Max, Team, or Enterprise). Cowork only works on paid plans. If you don't have Claude Desktop yet, grab it at [claude.com/download](https://claude.com/download).

---

## Step 1 · Open Cowork

Open the Claude app. In the left sidebar, find and click **Cowork**.

**You'll know it worked when** the sidebar shows options like **Tasks**, **Projects**, and **Scheduled**.

---

## Step 2 · Download the Jade Daily Pulse folder

Go to [github.com/jadesuser/jade-daily-pulse](https://github.com/jadesuser/jade-daily-pulse). Click the green **Code** button, then **Download ZIP**.

Find the downloaded ZIP, unzip it, and move the resulting folder into your **Documents** folder. (Don't leave it in Downloads — your computer cleans Downloads automatically.)

**You'll know it worked when** there's a folder called `jade-daily-pulse` inside your Documents.

---

## Step 3 · Make a Cowork project from that folder

In Cowork's sidebar, click **Projects**, then click **+ New Project**.

When Cowork asks how you want to create the project, choose **Create from folder**. Browse to the `jade-daily-pulse` folder you just placed in Documents and select it.

If Cowork asks for permission to read and write inside this folder, click **Allow**.

**You'll know it worked when** a new project called **jade-daily-pulse** appears in your sidebar, and you can see files inside it (`SKILL.md`, `brand-profile.md`, and a few others). Don't open any of them yet.

---

## Step 4 · Tell Claude how to behave in this project

Inside your new project, find the **Project instructions** field (usually a text box near the top). Copy and paste this:

> Follow the instructions in `SKILL.md` in this project's folder. When I ask you to run the Jade Daily Pulse — or when this is triggered on a schedule — read `brand-profile.md`, gather signals from the web, and save the memo as today's date inside the `memos/` folder.

Click **Save**.

**You'll know it worked when** the project instructions show your saved text.

---

## Step 5 · Fill in your brand info

In the project file list, click **`brand-profile.md`** to open it.

You'll see fields — *brand*, *positioning*, *ICP*, *competitors*, and a few others — each with a placeholder in pointy brackets like `<...>`. Replace every placeholder with your own answer. Short sentences, not paragraphs.

If you get stuck on what to write, open **`brand-profile.example.md`**. It shows the same fields filled in for a real brand (thejade.shop) you can use as a reference.

Save the file when you're done.

**A few prompts that help:**
- **Positioning:** avoid words like "premium" or "innovative." Be specific. What do you actually sell, to whom, and what is genuinely different?
- **Competitors:** 2 to 4 brands you actually watch.
- **Cadence:** type `daily` or `weekly`.
- **Timezone:** use your local zone, like `America/New_York`.

---

## Step 6 · Try it once

This is a one-time test so you can see the agent in action — *the real product is the scheduled task in Step 7*, but it's worth watching it work in front of you first.

In your project's chat box, type:

> Run the Jade Daily Pulse.

…and hit enter.

Claude goes off and searches the web for 60–120 seconds (Reddit, press, social, competitors). When it's done, you'll see the memo in chat **and** a new file appear in your project's `memos` folder named with today's date.

Read the memo. It has four sections plus a competitor footer:

1. **The dominant narrative** — the loudest thing being said about you right now, with two real quoted sources.
2. **Three tensions** — places where two true things about your brand pull against each other.
3. **Where the world disagrees with your messaging** — the gap between how you talk about yourself and what consumers actually say.
4. **One early signal** — the thing nobody on your team is tracking yet.

Plus a **Competitor pulse** footer with 3–5 lines on what your competitors did in the last 24 hours.

If anything reads generic, the fix is usually in your *positioning* or *topics to flag*. Edit `brand-profile.md`, save, and try this step again.

---

## Step 7 · Schedule it — this is the part that matters

This is the actual product. The scheduled task is what turns the Jade Daily Pulse from a tool-you-have-to-remember-to-run into a daily artifact that just shows up.

In your project's chat box, type:

> /schedule

…and hit enter. Claude opens a scheduling form. Fill it in:

- **Task name:** Jade Daily Pulse
- **Prompt:** `Run the Jade Daily Pulse.`
- **Frequency:** Daily
- **Time:** 7:00 AM (your local time)
- **Folder/Project:** jade-daily-pulse

Click **Save**.

**One thing to know about scheduled tasks in Cowork:** they only fire while your computer is awake and the Claude app is open. If your laptop is closed at 7am, the task auto-runs the next time you open Claude, and Claude tells you it caught up.

In practice, this means: either leave your laptop awake overnight, or accept that your morning memo lands whenever you next open Claude with your coffee. Both are fine — but if you don't know about this, you'll think it's broken Saturday morning.

**You'll know it worked when** — tomorrow morning — a new file appears in your project's `memos` folder named with tomorrow's date. A file you didn't create. That's your proof.

---

## Optional · Have the memo land in your inbox

Skip this if you're happy reading the memo inside Claude.

**Connect Gmail (one-time, about 60 seconds):**

1. In Claude Desktop, go to **Settings → Connectors**.
2. Find **Gmail** in the list. Click **Connect** and sign in with your Google account.
3. Test it: in any Claude chat, ask *"What's the subject of my most recent email?"* If Claude can answer, you're connected.

**Then have your scheduled task email you:**

Go to **Cowork → Scheduled**. Click your **Jade Daily Pulse** task. Edit the **Prompt** to:

> Run the Jade Daily Pulse. After saving the memo, email it to me at <your-email@example.com> with the subject "Your Jade Daily Pulse — [today's date]".

Save. From tomorrow morning on, the memo also lands in your inbox.

---

## You're done

You don't have to run anything yourself anymore. Every morning, a fresh memo will be waiting for you on:

- what consumers are actually saying about you,
- where their words diverge from yours,
- and the one signal you'd otherwise miss.

To change what gets surfaced later, open `brand-profile.md` and edit it. The agent reads it on every run, so the next morning's memo will reflect your changes.

---

## Want the deeper version?

The Daily Pulse is the **inward lens** — what the world is saying about *you*.

The 1:1 follow-up builds the **outward lens** — what's happening in your *category and competitive landscape*. A five-section daily intelligence brief, tuned to your taste in a private hour. Ask whoever ran your workshop how to book it.
