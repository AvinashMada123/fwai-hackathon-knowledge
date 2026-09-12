# Session starter prompt (end-to-end)

One-time setup, not a prompt:
1. Install Node.js if you don't have it, then run `npm install -g @anthropic-ai/claude-code`.
2. Accept the GitHub collaborator invite for this repo (check your email, or [github.com/AvinashMada123/fwai-hackathon-knowledge/invitations](https://github.com/AvinashMada123/fwai-hackathon-knowledge/invitations)).
3. Make sure `git` can access your GitHub account (run `gh auth login` once, or just try the clone below and follow the sign-in prompt it gives you).

Every time you want to use it: open a terminal, run `claude` in any folder, and paste this whole prompt as your first message:

```
Set up and run my FWAI hackathon coach knowledge base, then help me answer live participant questions.

1. If the folder "fwai-hackathon-knowledge" doesn't already exist in the current directory, clone it:
   git clone https://github.com/AvinashMada123/fwai-hackathon-knowledge.git
   If it already exists, cd into it and run "git pull" instead to get the latest version.

2. cd into fwai-hackathon-knowledge, then read CLAUDE.md and every file in knowledge/.

3. Once you've read them, tell me you're ready, then wait for my questions.

For each question I paste in after that:
- Give me a short, spoken-ready answer (1-4 sentences) I can say or type straight to the participant.
- Base it only on the files in knowledge/. If it's not covered, tell me plainly instead of guessing.
- If the question needs their personal data (their score, submission status, rank), tell me to check the dashboard instead of guessing.
```

Then just paste each participant's question as it comes in, e.g. "someone's asking why their submission got capped at 5/100" — Claude will answer from the knowledge base.
