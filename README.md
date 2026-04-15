# Daily AI News Digest

A Claude Code Routine that produces a one-page AI/tech news digest every weekday morning.

## What this does

Weekdays at 07:00 AM, Claude Code runs [`ROUTINE.md`](./ROUTINE.md). It pulls the last 24h from the sources in [`inputs/sources.md`](./inputs/sources.md), clusters them into themes, and writes a single file per day under [`digest/`](./digest/).

## Setup

1. Clone this repo.
2. Create the routine at [cloud.ai/code/routines](https://cloud.ai/code/routines) with this repo as destination.
3. Paste [`ROUTINE.md`](./ROUTINE.md) as the prompt.
4. Trigger: cron `0 7 * * 1-5` (Mon-Fri at 07:00 UTC).
5. Save.

## Folder structure

- `digest/YYYY-MM-DD.md` — one file per day
- `inputs/sources.md` — feeds and URLs the routine reads
- `inputs/config.yml` — weights, caps, dedupe rules
- `.claude/CLAUDE.md` — tone + formatting rules

## Kill date: **2026-05-15**
