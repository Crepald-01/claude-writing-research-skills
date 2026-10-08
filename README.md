# Claude Skills

A small collection of Claude skills for writing and research work. Each skill is a folder containing a `SKILL.md` file, which tells Claude when to use the skill and how to carry out the task.

## Skills

| Skill | What it does | Use it when |
|---|---|---|
| [email-drafter](email-drafter/SKILL.md) | Summarizes an email thread and drafts a reply in a requested tone. Marks unknown facts with `[CONFIRM]` instead of guessing. | You paste an email thread and need a reply or follow-up. |
| [document-summarizer](document-summarizer/SKILL.md) | Condenses a long PDF or report into a one-page brief with a table of key figures and their source sections. | You have a long document and need the key findings and numbers. |
| [research-brief-writer](research-brief-writer/SKILL.md) | Writes a sourced overview of a topic, separating points of agreement from expert disagreement and noting gaps. | You need background on a topic, with sources and an honest view of the debate. |

## Installation

Copy the skill folders you want into your Claude skills directory, keeping each `SKILL.md` inside its own folder:

```
skills/
├── email-drafter/
│   └── SKILL.md
├── document-summarizer/
│   └── SKILL.md
└── research-brief-writer/
    └── SKILL.md
```

Or download the repository as a zip, extract it, and copy the folders.

## Design principles

- **No invented facts.** Each skill asks for or flags missing information rather than filling gaps.
- **Sources are visible.** Summaries keep track of where figures and claims came from.
- **Fair treatment of disagreement.** Contested topics are presented as positions with their evidence, without a personal verdict.

## Contributing

Open an issue or a pull request with a change to a `SKILL.md` file. Keep the frontmatter (`name` and `description`) accurate, since the description decides when Claude uses the skill.

## License

Add a license here before publishing if you plan to share the skills publicly.
