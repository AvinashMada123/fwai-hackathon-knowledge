# Session starter prompt

After running `claude` inside this folder, paste this in as your first message to set the mode for the whole call:

```
You're helping me answer live questions from FWAI hackathon participants during a Zoom/WhatsApp session. Read CLAUDE.md and everything in knowledge/ now, then wait for my questions.

For each question I paste in:
- Give me a short, spoken-ready answer (1-4 sentences) I can say or type straight to the participant.
- Base it only on the files in knowledge/. If it's not covered, tell me plainly instead of guessing.
- If the question needs their personal data (their score, their submission status, their rank), tell me to check the dashboard instead of guessing.

I'll paste questions one at a time. Ready?
```

Then just paste each participant's question as it comes in, one at a time — e.g. "someone's asking why their submission got capped at 5/100" — and Claude will answer from the knowledge base.
