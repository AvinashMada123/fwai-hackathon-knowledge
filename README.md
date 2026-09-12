# FWAI Hackathon — Knowledge Base

A static knowledge base for answering live participant questions about the Freedom With AI hackathon/bootcamp — on Zoom, WhatsApp, or anywhere else. Open this folder with Claude Code and ask it questions the way you'd ask a colleague; it answers from the files in `knowledge/`, not from guesswork or live dashboard data.

## What's in here

- `CLAUDE.md` — tells Claude how to behave when answering questions from this repo.
- `knowledge/00-overview.md` — what the program is, who it's for.
- `knowledge/01-schedule.md` — the 4-day structure and session timing.
- `knowledge/02-submissions-scoring.md` — how submissions, grading, points, and the leaderboard work.
- `knowledge/03-access-membership.md` — who gets access, the Diamond tier, DeepSeek API keys.
- `knowledge/04-rules-and-gotchas.md` — the questions that come up most, answered directly.
- `knowledge/05-channels.md` — Zoom, WhatsApp, the in-app bot, attendance fallback.
- `knowledge/99-proposed-not-live.md` — a planned future program, kept separate so it's never mistaken for what's live today.

## Install (one-time, on Kundan's computer)

**1. Install Claude Code** (skip if already installed):

```bash
npm install -g @anthropic-ai/claude-code
```

This needs Node.js installed first. If `npm` isn't recognized, install Node from [nodejs.org](https://nodejs.org) first, then re-run the command above.

**2. Clone this repository:**

```bash
git clone https://github.com/AvinashMada123/fwai-hackathon-knowledge.git
cd fwai-hackathon-knowledge
```

This is a **private** repository — Animesh needs to add your GitHub account as a collaborator first (Settings → Collaborators on the repo), and you'll need to be logged into GitHub (via `git` credentials or the GitHub CLI) for the clone to work.

**3. Log in to Claude Code** (one-time, opens a browser to sign in with your Claude account):

```bash
claude
```

## Day-to-day use

Every time you want to answer questions during a call:

1. Open a terminal.
2. `cd` into the cloned folder.
3. Run:
   ```bash
   claude
   ```
4. Ask your question in plain language, e.g. "someone's asking why their submission got capped at 5 out of 100" or "what time is Sunday's session." Claude will answer from the knowledge files.

You can leave this terminal window open throughout a call and keep asking follow-up questions.

## Keeping it accurate

This is a **static snapshot** — it does not read live dashboard data (scores, attendance, individual participant status). When a program detail changes (schedule, pricing, rules), someone edits the relevant file in `knowledge/`, commits, and pushes:

```bash
git add -A
git commit -m "Update: <what changed>"
git push
```

Anyone else using the repo should then run `git pull` before their next call to get the update.

## What this is not

- Not a live data connection — it won't know an individual participant's score, submission status, or rank. For that, check the dashboard directly.
- Not a public FAQ — this repo is private and should stay that way; some of the content (pricing, internal caveats) isn't meant for participants to read directly.
