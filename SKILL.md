---
name: jade-daily-pulse
description: Generate the Jade Daily Pulse — a 1-page morning memo on what the world is saying about a brand. Use when the user asks for their brand pulse, daily sentiment memo, "what are people saying about us today," or when invoked on a schedule. Reads brand-profile.md from the connected project folder and writes the memo to memos/YYYY-MM-DD.md inside the same folder.
---

# Jade Daily Pulse

You are generating today's **Jade Daily Pulse** — a one-page morning memo for a brand executive. They will read it on their phone, with coffee, before their first meeting. It must be worth opening.

This instruction file lives inside the user's Cowork project folder. Read sibling files (`brand-profile.md`) from this same folder and write memo output to the `memos/` subfolder.

## Inputs

1. Read `brand-profile.md` from this project folder. It contains: brand name, positioning, ICP, top competitors, topics to flag, cadence. If the file is missing or unfilled (still has `<...>` placeholders), stop and tell the user to fill it in.
2. Use today's date as the memo date. Use the user's local timezone.

## What to gather

Use WebSearch and WebFetch. Cast wide, then filter hard. Aim for **last 24–48 hours** for daily cadence, **last 7 days** for weekly cadence (check `cadence:` in the profile).

Sources to prioritize, in this order:
1. **Reddit** — search `site:reddit.com "<brand name>"`. Reddit is where unvarnished sentiment lives.
2. **TikTok/Instagram chatter** — search `"<brand>" tiktok` and `"<brand>" "instagram"`. Look for creator content and comment-section themes.
3. **Press & trade** — Glossy, Beauty Independent, Business of Fashion, WWD, Modern Retail, Retail Brew, Food Dive (for CPG).
4. **Substack / niche newsletters** — search `"<brand>" substack` for opinionated takes.
5. **X / Twitter** — search `"<brand>" site:twitter.com OR site:x.com`.
6. **Competitor parallel scan** — repeat a lighter version of #1–#3 for each named competitor to find sentiment differentials.

Pull **real quotes with attribution**. A quote without a source is unusable. If you can't find a source URL, drop the quote.

## What to produce

Write the memo to `memos/{YYYY-MM-DD}.md` inside this project folder. Use this exact structure:

```markdown
# Jade Daily Pulse — {Brand Name}
**{Day, Month DD, YYYY}** · Generated {HH:MM} local

---

## 1. The dominant narrative
{2–3 sentences naming the single loudest thing being said about the brand right now. Lead with the narrative, not the volume. Follow with 2 direct quotes, each on its own line with attribution: source + URL.}

> "Quote here." — *r/SkincareAddiction, [link](URL)*

> "Quote here." — *@username on TikTok, [link](URL)*

## 2. Three tensions
{Three bullets, each naming a tension in how the brand is perceived. A tension = two things both true that pull against each other. Not "people love it / some hate it" — that's a split, not a tension. Format: bold the tension in 6–10 words, then one sentence of color with a source.}

- **{Tension headline}.** {One sentence with evidence and source URL.}
- **{Tension headline}.** {One sentence with evidence and source URL.}
- **{Tension headline}.** {One sentence with evidence and source URL.}

## 3. Where the world disagrees with your messaging
{The gap between how the brand positions itself (from brand-profile.md `positioning:`) and what consumers actually say. One paragraph, 3–5 sentences. Be specific — name the messaging claim and the contradicting signal. If there's no meaningful gap today, say so plainly — don't pad.}

## 4. One early signal
{One thing happening at the edge that nobody on the brand's team is tracking yet. Could be: a creator gaining traction with their audience, a sub-narrative forming in comments, a Reddit thread climbing, a new use case emerging, a competitor making a quiet move. One paragraph + source URL. This is the section the reader will forward to their team.}

---

### Competitor pulse
{3–5 one-line bullets — competitor name, what happened, why it might matter to this brand. Skip if nothing meaningful surfaced.}

- **{Competitor}** — {what happened}. {Why it matters for this brand in 6–10 words.}
- **{Competitor}** — {what happened}. {Why it matters for this brand in 6–10 words.}

---
*Built with [Jade](https://thejade.shop) — daily intel agents for consumer brands.*
```

## Voice & length rules

- **Total length:** the body (excluding competitor pulse) fits on one phone screen. Aim for ~400 words.
- **Opinionated, not hedged.** "The dominant narrative is X" — not "There appears to be some indication that X may be." If you're not sure, say what's most likely and move on.
- **No padding.** If a section has nothing real to report today, say "Quiet day on this front" in one line. Never invent.
- **Quotes are non-negotiable for section 1.** If you genuinely can't find quotes, write "Couldn't find quotable sentiment today" and explain why in one sentence (e.g., "brand was off-cycle this week").
- **No marketing language.** Never write "exciting," "innovative," "leading," "premium." Strip it.
- **Mobile-first formatting.** Short paragraphs. No tables. Bold for scanability.

## After writing

1. Print the full memo to the chat so the user sees it immediately.
2. Tell the user the file path it was saved to.
3. If this is the first run (no prior memos exist in `memos/`), remind the user they can schedule daily runs by typing `/schedule` in Cowork and choosing "daily" at their preferred time. Note that scheduled runs only fire while the laptop is awake and the Claude Desktop app is open.
