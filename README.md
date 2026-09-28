# Project-AIX

A small educational experiment on how Claude handles instructions from a GitHub repo.

## What this is

This repo is a test, not a product. It contains two instruction files:

| File | Purpose |
|:-----|:--------|
| `project_instructions.md` | A simple task: build a colorful, animated calculator |
| `ai_logging_model_enforcement_instructions.md` | A rule requiring a specific model and an honest log of which model ran |

The goal was to learn:

- what "installing" instructions in Claude actually means,
- whether a text file can change which model answers,
- how Claude behaves when a file pushes it to claim something it can't verify.

## What I found

- A text file cannot change which model runs. The app chooses the model before the model reads anything.
- Claude built the task but did not falsify the log. It reported the model mismatch instead of writing "Pass".
- Pasting a repo link only affects that one chat turn. Persistent instructions need real mechanisms such as `CLAUDE.md` or skills in Claude Code.

## Read the full write-up

I wrote about the experiment, the findings, and what I learned here:

**[Read the blog on Medium](https://medium.com/@rohit.gupta1604004/a5efe1cb8dd9)**

## Note

This was done for learning purposes only. Nothing in this repo is malicious, and it should not be used to test real harmful tasks.
