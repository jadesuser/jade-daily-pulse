# Jade Daily Pulse

A daily 1-page memo on what the world is saying about your brand. Runs in **Claude Cowork**. Delivered to a markdown file every morning at 7am (and optionally to your inbox via the Gmail connector).

Built for beauty, CPG, and fashion brand executives by [Jade](https://thejade.shop).

---

## What the memo gives you

Every morning, four sections plus a competitor footer:

1. **The dominant narrative** — the single loudest thing being said about you right now, with two real quoted sources.
2. **Three tensions** — places where two true things about your brand pull against each other.
3. **Where the world disagrees with your messaging** — the gap between how you talk about yourself and what consumers actually say.
4. **One early signal** — the thing happening at the edge nobody on your team is tracking yet.
5. **Competitor pulse** — 3–5 lines on what your named competitors did in the last 24 hours.

Total length: fits on one phone screen. ~400 words.

---

## What the agent looks at

Every run, the agent searches a prioritized list of sources for signal on your brand, your category, and your named competitors:

1. **Reddit** — where unvarnished consumer sentiment lives
2. **TikTok and Instagram chatter** — creator content and comment-section themes
3. **Press and trade** — Glossy, Beauty Independent, Business of Fashion, WWD, Modern Retail, Food Dive (CPG)
4. **Substack and niche newsletters** — the opinionated takes
5. **X / Twitter** — real-time discourse
6. **Competitor parallel scan** — repeats steps 1–3 for each competitor in your profile

All of this runs through Cowork's built-in web search and fetch — no extra setup, no API keys, works out of the box.

**Want deeper sourcing?** If you want the agent wired directly into Reddit's API, a dedicated scraper for Substacks you trust, or your own social listening feeds, that's part of the 1:1 follow-up. Ask whoever ran your workshop.

---

## Get started

**→ Read [SETUP.md](SETUP.md) for the 8-step install. Takes about 15 minutes.**

Quick orientation:

```
jade-daily-pulse/
├── SKILL.md                    # the universal product — Cowork reads this on every run
├── brand-profile.md            # YOUR config — edit this
├── brand-profile.example.md    # filled example (thejade.shop)
├── SETUP.md                    # 8-step participant install guide
├── README.md                   # this file
└── memos/                      # daily memos save here
```

The **skill** is shared by everyone. The **brand-profile.md** is yours. Change the profile, change tomorrow's memo — the skill reads it on every run.

---

## Requirements

- Claude Desktop with **Cowork** enabled
- Paid Claude plan: Pro, Max, Team, or Enterprise
- macOS or Windows (Cowork is not on Linux)

Don't have Cowork yet? Grab Claude Desktop at [claude.com/download](https://claude.com/download).

---

## Want the deeper version?

The Daily Pulse is the **inward lens** — what the world is saying about *you*.

There is also an outward lens — the **Daily Intelligence Brief** — that watches your category and competitive landscape. Five sections, tuned to your taste in a private 1:1 hour. If you came in through a Jade workshop, ask the facilitator how to book.

---

*Built by [Jade](https://thejade.shop). Jade builds AI agents that do operational work for consumer brands.*
