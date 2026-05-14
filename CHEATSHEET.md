# Jade Workshop — Take-Home Cheatsheet

Everything worth remembering from today's workshop, in one page. Keep this open the first week. After that you probably won't need it.

---

## The vocabulary (what these words mean)

**Chat** — A back-and-forth conversation. You ask Claude something, it answers. It does what you ask, when you ask. Closes when you close it.

**Agent** — A chat that *runs on its own*. You set it up once, give it instructions, put it on a schedule. It works while you sleep. The Jade Daily Pulse you built today is an agent.

**Project** — A workspace inside Cowork with its own files, instructions, and chat history. Different projects can do completely different jobs. The *Jade Daily Pulse* project does one job (your daily memo). You'll likely have more projects over time.

**Skill** — A reusable set of instructions written in plain English that teaches Claude how to do a specific job. We wrote one called *Jade Daily Pulse* for you. Skills can be shared across projects, across teammates, and across the team's whole Cowork. *You can also create your own — see "Make your own skill" below.*

**Connector** — A pre-built integration with services you already use (Gmail, Drive, Docusign, etc.) that lets Claude take actions in those services with your permission.

**Scheduled task** — A prompt that runs automatically on a cadence (daily, weekly, etc.). This is the thing that makes an agent feel like an agent rather than a tool.

---

## What you built today

A daily agent that reads your brand profile, searches the web each morning, and writes you a 1-page memo with:

1. **The dominant narrative** — the loudest single thing being said about you, with 2 quoted sources.
2. **Three tensions** — places where two true things about your brand pull against each other.
3. **Where the world disagrees with your messaging** — the gap between how you talk about yourself and what consumers actually say.
4. **One early signal** — the thing nobody on your team is tracking yet.
5. **Competitor pulse** — 3–5 lines on what your competitors did in the last 24 hours.

You can read it inside Cowork, or have it emailed to your inbox if you connected Gmail.

---

## Which Claude model should you use?

Claude Cowork lets you pick which model handles your prompts (look for the **model selector** at the top of your project or chat). You can ignore this most of the time, but knowing the menu helps. As of May 2026:

| Model | When it's the right pick |
|---|---|
| **Claude Opus 4.7** | The deepest thinker, currently the strongest model. Best for real reasoning — strategic decisions, weighing tradeoffs, nuanced writing, deep research. Slower and pricier per run. **The recommended default for your Jade Daily Pulse**, since the agent's whole job is finding tensions and signals. |
| **Claude Opus 4.6** | The previous Opus. Still excellent reasoning. Available in "Fast mode" with faster output. Use when you want Opus-level depth but want it sooner. |
| **Claude Sonnet 4.6** | The balanced middle. Fast enough for live conversation, smart enough for almost everything that isn't deep analysis. Good default for drafting, formatting, summarizing, light reasoning. |
| **Claude Haiku 4.5** | The lightweight, high-speed model. Built for volume — classification, simple extractions, short replies. Cheapest per run. Not the right choice for nuanced thinking. |

**Practical rule of thumb:**
- *Building something or making a real decision?* Opus 4.7.
- *Quick drafting, formatting, "rewrite this for me"?* Sonnet 4.6.
- *High-volume / simple lookups?* Haiku 4.5.

---

## Five things to remember

1. **Skill = universal. Profile = yours.** The same Skill runs for everyone in this room. What makes your memo *yours* is the `brand-profile.md` you wrote. Edit the profile any time — the next morning's memo reflects your changes.

2. **The schedule is the product.** Running the agent on demand is just a tool. The scheduled task is what makes it an *agent*. If you didn't schedule it today, schedule it before you close Claude — type `/schedule` in your project chat.

3. **The laptop-awake catch.** Cowork scheduled tasks only fire while your laptop is awake and Claude Desktop is open. If your laptop is closed at 7am, the task runs the next time you open Claude — and Claude tells you it caught up. Plan accordingly.

4. **The agent won't pad.** Some mornings your brand will be quiet — small inventory cycle, off-news days. The agent will say so plainly rather than invent content. When it has content, you can trust it. "Quiet day on this front" is also signal.

5. **You can make your own skills.** After walking through any repeatable task with Claude — drafting a weekly review, summarizing your inbox, prepping for a recurring meeting — say "turn this into a skill." Claude will package the workflow into a Skill you can reuse forever and share with your team.

---

## Things you'll do most often

| To do this | How |
|---|---|
| Read this morning's memo | Open the `memos` folder in your project |
| Change what gets surfaced | Tell Claude in chat (e.g., *"add Vrai to my competitors"*) — or edit `brand-profile.md` directly |
| Run the agent now (don't wait for tomorrow) | Type `Run the Jade Daily Pulse.` in your project chat |
| Change the schedule (time, frequency) | Sidebar → **Scheduled** → click your task |
| Pause the agent (vacation, etc.) | Sidebar → **Scheduled** → pause toggle |
| Connect or disconnect Gmail | **Settings → Connectors → Gmail** |
| Make your own Skill from a workflow | Walk through the workflow with Claude, then type `Turn this into a skill.` |

---

## When the memo feels off

The first few days are calibration days. If a section reads generic or misses what you'd want, the fix is almost always in your brand profile. The fastest way to adjust it: just tell Claude in your project chat what to change. Examples:

- *"Tighten my positioning — we're not 'premium,' we're [actual specific description]."*
- *"Add 'retailer expansion at Sephora' to my topics to flag."*
- *"Swap Glossier out of my competitors, swap Tower 28 in."*

Claude updates `brand-profile.md` directly and tells you what it changed. Then run `Run the Jade Daily Pulse.` to see the new memo immediately — you don't have to wait for tomorrow's scheduled run.

If you'd rather edit the file by hand, you still can — open `brand-profile.md` and change it directly.

---

## Want more

**Switch to weekly.** Edit your scheduled task's frequency. Monday morning is the usual choice.

**Run two agents.** Daily quick pulse + weekly deeper memo. Cowork lets you have multiple scheduled tasks per project.

**Wire in your own sources.** The Daily Pulse uses Cowork's built-in web search. For deeper integration (Reddit API, niche scrapers, your own social listening) — that's the 1:1 follow-up.

---

*Built with [Jade](https://jade.build) — daily intel agents for consumer brands.*
