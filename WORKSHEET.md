# Jade Workshop Worksheet
**Daily Pulse for your brand · 60 minutes**

This is your worksheet for the workshop. Keep it open in another tab. By the end of the hour, you'll walk out with a working AI agent that delivers a daily 1-page brand memo to your computer every morning.

---

## Part 1 · The mental model

> Think of this as briefing a new executive assistant. When a great EA starts on Monday, you don't hand them a job description. You hand them who you are, who your customers are, who you watch, and what matters to you. Then every morning they bring you what you'd otherwise miss.

That's what we're building today. The EA is an AI agent. It works while you sleep.

---

## Part 2 · The building blocks of Claude Cowork

There are four things in Cowork you'll touch today. Once you know what these are, the rest is just typing.

### 1. Projects

**What it is:** A persistent workspace inside Cowork. Each Project has its own files, instructions, memory, and chat history.

**Why it matters:** Today you'll create one Project called *Jade Daily Pulse*. That Project will contain your brand profile and become the home for every memo the agent produces.

**How to make one:** Sidebar → **+ New Project** → **Create from folder** → pick the `jade-daily-pulse` folder you downloaded.

---

### 2. Skills

**What it is:** A reusable set of instructions — written in plain English in a file called `SKILL.md` — that tells Claude how to do a specific job. Skills are shareable. We wrote one called *Jade Daily Pulse* that everyone in the room will install.

**Why it matters:** A Skill is the "product." A Skill plus your specific brand profile is your personal version of that product. Same Skill, different profile, completely different memo.

**How you use one today:** You don't write the Skill — we wrote it for you. You just need to make sure Cowork knows to use it. That's what you'll do in the *Project instructions* step.

> **The pattern to remember:** *Skill = universal. Config = yours.* Same Skill for every executive in this room; their `brand-profile.md` is what makes their memo different from yours.

---

### 3. Scheduled tasks

**What it is:** A way to tell Cowork to run a prompt automatically at a specific cadence — hourly, daily, weekly, weekdays, or manually.

**Why it matters:** A tool you have to remember to run isn't an agent — it's a tool. The schedule is what turns the Jade Daily Pulse from "a thing you could run" into "a memo that just appears every morning." This is the step that matters most today.

**How to make one:** In your Project chat, type `/schedule` and fill in the form. Frequency = Daily, Time = 7:00 AM, Prompt = `Run the Jade Daily Pulse.`

**The one catch:** Scheduled tasks only fire while your laptop is awake and Claude Desktop is open. If your laptop is closed at 7am, the task auto-runs the next time you open the app. Practically: leave your laptop awake overnight, or accept that the memo lands when you open Claude with your coffee.

---

### 4. Connectors

**What it is:** Pre-built integrations with services you already use — Gmail, Google Drive, Docusign, FactSet, and more. Connectors let Cowork take real actions in those services (read your email, save a file to Drive, etc.) when you give it permission.

**Why it matters:** Today's optional step is connecting Gmail so your daily memo lands in your inbox at 7am, not just inside Cowork. You don't need this to make the workshop work — but it's the difference between "I check Claude every morning" and "my memo is in my inbox before my first meeting."

**How to set one up:** Claude Desktop → **Settings → Connectors** → find Gmail → **Connect** → sign in.

---

## Part 3 · Quick reference

You'll use these during the workshop and after.

| What you want to do | How to do it |
|---|---|
| Make a new Project | Sidebar → **+ New Project** → Create from folder |
| Edit a Project's brief | Open the Project → **Project instructions** field |
| Run the agent on demand | Type `Run the Jade Daily Pulse.` in the Project chat |
| Schedule the agent | Type `/schedule` in the Project chat |
| See / edit / pause your scheduled tasks | Sidebar → **Scheduled** |
| Connect Gmail (or any service) | **Settings → Connectors** in Claude Desktop |
| Change what the memo focuses on | Edit `brand-profile.md` in your Project folder |
| Switch from daily to weekly | Edit your scheduled task's frequency |

---

## Part 4 · Your turn — brand profile

These are the fields you'll fill in inside `brand-profile.md`. Use this worksheet to draft your answers first; copy them into the file once you're happy.

> Short answers. Sentences, not paragraphs. Be specific.

**Brand**
*Your brand name.*

> ____________________________________________________________

**Positioning** *(2 sentences)*
*What you sell, who it's for, what's genuinely different. Don't write "premium" or "innovative" — those words mean nothing to the agent. Be concrete.*

> ____________________________________________________________
> ____________________________________________________________
> ____________________________________________________________

**ICP — your actual customer** *(1 sentence)*
*Demographics + psychographics. Who really buys you. Age, geography, what else they buy.*

> ____________________________________________________________
> ____________________________________________________________

**Competitors** *(2 to 4 brands)*
*Brands you actually watch. Not "the entire category" — name names.*

> ____________________________________________________________

**Topics to flag** *(2 to 4 topics)*
*Ingredients, narratives, controversies, or trends you specifically want surfaced if they come up.*

> ____________________________________________________________
> ____________________________________________________________

**Sources you trust** *(optional)*
*Subreddits, outlets, creators, Substacks you want weighted higher. Leave blank if no preferences.*

> ____________________________________________________________

**Cadence**
*Daily or weekly?*

> ____________________________________________________________

**Delivery time**
*Default is 7:00 AM your local time. Want different?*

> ____________________________________________________________

**Timezone**
*Like `America/New_York`, `America/Los_Angeles`, etc.*

> ____________________________________________________________

---

## Part 5 · What's on your memo every morning

Once you've finished the workshop, every morning at 7am (laptop willing) you'll see a memo with four sections plus a competitor footer:

1. **The dominant narrative** — the loudest single thing being said about your brand, with two real quoted sources. Not a roundup — *the* narrative.

2. **Three tensions** — places where two true things about your brand pull against each other. Tensions are different from splits ("some love it / some hate it" is a split, not a tension). The agent looks for the genuinely interesting friction.

3. **Where the world disagrees with your messaging** — the gap between how you talk about yourself and what consumers actually say. This is the section CMOs forward to their team.

4. **One early signal** — the thing happening at the edge of your category that nobody on your team is tracking yet. Could be a creator gaining traction, a sub-narrative forming in comments, a quiet competitor move, a new use case.

**Plus competitor pulse:** 3 to 5 lines on what your named competitors did in the last 24 hours.

---

## Part 6 · After the workshop

A few things worth knowing as you start using the agent day-to-day.

**Editing your profile.** Open `brand-profile.md` and change anything. The agent reads it on every run, so the next morning's memo reflects your edits. Most useful edits over time: adding a topic to *topics to flag* when something new starts mattering, or swapping out a competitor.

**Quiet days.** Some mornings your brand simply won't have much chatter. The agent will say so plainly rather than invent. That's a feature: when the memo has content, you can trust it; when it says "quiet day on this front," that's signal too.

**Switching to weekly.** If daily is too much, edit your scheduled task's *frequency* to Weekly and pick a day (Monday morning is the usual pick). Or run two — a daily quick pulse, a weekly deeper memo. Cowork lets you have multiple scheduled tasks per Project.

**Want deeper sourcing?** The agent uses Cowork's built-in web search across Reddit, press, social, Substacks, and X. If you want it wired directly into Reddit's API, a custom scraper for Substacks you trust, or your own social listening feed — that's the 1:1 follow-up.

---

## Part 7 · Want the deeper version?

The Daily Pulse is the **inward lens** — what the world is saying about *you*.

The 1:1 follow-up builds the **outward lens** — what's happening in your *category and competitive landscape*. A 5-section daily intelligence brief, tuned to your taste over a private hour:

- **Overnight in your world** — competitor drops, exec moves, funding, M&A, retail expansions
- **Your brand in the wild** — press, creator content, retailer mentions, social spikes
- **What dropped, what sold out** — new launches in your category, hero SKU sell-outs
- **Cultural pulse** — what's gaining velocity in your category and why it matters
- **One you'd otherwise miss** — the delight slot, the thing that makes the brief feel curated

The 1:1 is free. Ask your workshop facilitator how to book.

---

*Built with [Jade](https://jade.build) — daily intel agents for consumer brands.*
