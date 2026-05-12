# Jade Daily Pulse — Setup

Eight steps. About 15 minutes start to finish. By the end you'll have a daily 1-page memo on your brand landing every morning at 7am.

Prerequisite: Claude Desktop installed with Cowork enabled (Pro, Max, Team, or Enterprise plan). If you don't have it yet, grab it at [claude.com/download](https://claude.com/download).

---

## Step 1 · Confirm Cowork is on

Open Claude Desktop. In the sidebar you should see **Cowork**. If you don't, go to Settings → Cowork and enable it.

**How you know it worked:** the sidebar shows Cowork, with options for Tasks, Projects, and Scheduled.

---

## Step 2 · Download the Jade Daily Pulse folder

Go to [github.com/jadesuser/jade-daily-pulse](https://github.com/jadesuser/jade-daily-pulse) and click **Code → Download ZIP**.

Unzip it. Move the folder to a stable location on your machine — `~/Documents/jade-daily-pulse/` works well. (Don't put it inside Downloads; macOS cleans Downloads on a schedule.)

**How you know it worked:** the folder is at e.g. `~/Documents/jade-daily-pulse/` and contains `SKILL.md`, `brand-profile.md`, `brand-profile.example.md`, `SETUP.md`, `README.md`, and an empty `memos/` subfolder.

---

## Step 3 · Create a Cowork Project and connect the folder

In Cowork, click **+ New Project**. Name it **Jade Daily Pulse**.

Inside the new project, click **Connect folder** (or "Add folder" — wording varies). Browse to your `jade-daily-pulse/` folder and connect it. Grant Cowork read and write permission when prompted.

**How you know it worked:** Cowork shows the folder contents in the project sidebar. You can see `SKILL.md`, `brand-profile.md`, etc.

---

## Step 4 · Set the project instructions

In the project, open the **Project instructions** field. Paste:

> Follow the instructions in `SKILL.md` in this project's connected folder. When the user asks to run the Jade Daily Pulse, or when invoked on a schedule, execute that skill — read `brand-profile.md`, gather signals, and write the memo to `memos/{today}.md`.

Save the instructions.

**How you know it worked:** the project instructions show your saved text.

---

## Step 5 · Fill in your brand profile

Open `brand-profile.md` from the connected folder (either inside Cowork's file view or in your normal text editor — both work, since Cowork sees the file system live).

Replace every `<...>` placeholder. Sentences, not paragraphs. The companion file `brand-profile.example.md` shows the shape using thejade.shop.

| Field | What to write |
|---|---|
| **brand** | Your brand name. |
| **positioning** | Two sentences. What you sell, who it's for, what makes you different. No "premium," no "innovative." |
| **ICP** | Who actually buys you, one sentence. Demographic + psychographic. |
| **competitors** | 2–4 named brands you actually watch. |
| **topics to flag** | 2–4 topics, narratives, or controversies you want surfaced. |
| **sources you trust** | Optional. Subreddits, outlets, creators, Substacks. |
| **cadence** | `daily` or `weekly`. |
| **delivery time** | Default `07:00`. |
| **timezone** | e.g., `America/New_York`. |

Save the file.

---

## Step 6 · Preview the pulse once

This is a one-time preview so you can see what the agent does before you set it loose on a schedule. In your project's chat, type:

> Run the Jade Daily Pulse.

Cowork reads your brand profile, searches the web (Reddit, press, social, competitors), and writes a memo. Takes 60–120 seconds.

**How you know it worked:** Cowork prints the memo in chat and saves a new file at `memos/<today>.md` inside your connected folder.

This is the same memo you'll receive every morning once you schedule it in Step 8.

---

## Step 7 · Read it (two minutes)

The memo has four sections plus a competitor footer:

1. **The dominant narrative** — single loudest thing being said about you, with two real quoted sources.
2. **Three tensions** — two-things-both-true pulling against each other.
3. **Where the world disagrees with your messaging** — gap between your positioning and what consumers say.
4. **One early signal** — the thing nobody on your team is tracking yet.

If a section feels generic, the fix is usually in your `positioning` or `topics to flag`. Edit `brand-profile.md` and re-run.

---

## Step 8 · Schedule it — this is the part that matters

The preview in Step 6 was a one-off. **This step is the actual product** — the scheduled task is what makes the Jade Daily Pulse a daily artifact instead of a tool you have to remember to run.

In your project's chat, type:

> /schedule

Cowork walks you through a scheduled-task modal. Fill in:
- **Task name:** Jade Daily Pulse
- **Prompt:** `Run the Jade Daily Pulse.`
- **Frequency:** Daily
- **Time:** 07:00 (your local time)
- **Folder/Project:** Jade Daily Pulse (the project you just created)

Save the scheduled task.

**The one constraint to know about:** Cowork scheduled tasks only fire while your laptop is awake and Claude Desktop is open. If your laptop is closed at 7am, the task auto-runs the next time you open the app — and Cowork tells you it caught up. **Practically:** either leave your laptop awake overnight, or accept that the memo lands whenever you next open Claude. Both are fine.

**How you'll know it worked:** tomorrow morning, you'll see a new file at `memos/<tomorrow's-date>.md` that you didn't create. That's the proof loop closed.

To see, edit, or pause your scheduled task later: sidebar → **Scheduled**.

---

## Step 9 · (Optional) Have it land in your inbox

Skip this step if you're happy reading the memo inside Cowork.

**One-time Gmail connection (~60 seconds):**

1. In Claude Desktop, go to Settings → **Connectors**.
2. Find **Gmail** in the list. Click Connect, sign in with your Google account, grant permission.
3. Confirm by asking in any Cowork chat: `What's the subject of my most recent email?` — if Cowork can answer, you're connected.

**Tell your scheduled task to email you:**

Edit the scheduled task. Change the prompt to:

> Run the Jade Daily Pulse. After saving the memo, email it to <your-email@example.com> with subject "Your Jade Daily Pulse — {today's date}".

That's it. The memo now lands in your inbox every morning before your first meeting (whenever the scheduled task next fires).

---

## You're done

The scheduled task in Step 8 is the product. Tomorrow morning at 7am — as long as your laptop is awake and Cowork is open — a fresh memo will be waiting for you on:
- what consumers are actually saying about you,
- where their words diverge from yours,
- and the one signal you'd otherwise miss.

You don't have to run anything manually again. The skill reads `brand-profile.md` on every scheduled run, so any time you want to change what gets surfaced, edit the profile — the next morning's memo reflects it.

---

## Want the deeper version?

The Daily Pulse is the **inward** lens — what the world is saying about *you*.

The 1:1 follow-up builds the **outward** lens — what's happening in your *category and competitive landscape*. A five-section daily intelligence brief tuned to your taste over a private hour. Book a session with whoever ran your workshop.
