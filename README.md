# fable-mode

An agent skill that makes Claude Opus work with the habits of Claude Fable: find the real cause, check facts instead of guessing, finish the whole task, test the result, and report in plain language.

A text file cannot copy another model's raw capability. Most of what users notice on everyday work is habit: was the work finished, was it checked, was the cause found, can the report be read cold. This skill writes those habits down, each with its reason, so the agent can apply them with judgment in new situations.

## Install

```sh
git clone https://github.com/DaganGera/fable-mode ~/.claude/skills/fable-mode
```

Claude Code loads it when a session starts on Opus, or when you say "fable mode", "work like Fable" or "be more thorough". To load it every time, add a line to `~/.claude/CLAUDE.md` telling the agent to load `fable-mode` before the first non-trivial task.

## What it covers

- **How to think**: check facts, find the cause, consider more than one explanation.
- **How to build**: small exact edits, no extras, run what you wrote.
- **How to finish**: complete the whole task, work through errors, stop only for a real reason.
- **How to speak**: lead with the result, plain language, honest about what was and was not verified.
- **Check before you end a turn**: a short list of questions to answer first.

It works in any agent that reads `SKILL.md` files.

## License

MIT
