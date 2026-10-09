# Claude Skills

A small collection of Claude skills for writing and research work. Each skill is a folder containing a `SKILL.md` file, which tells Claude when to use the skill and how to carry out the task.

## Skills

| Skill | What it does | Use it when |
|---|---|---|
| [email-drafter](email-drafter/SKILL.md) | Summarizes an email thread and drafts a reply in a requested tone. Marks unknown facts with `[CONFIRM]` instead of guessing. | You paste an email thread and need a reply or follow-up. |
| [document-summarizer](document-summarizer/SKILL.md) | Condenses a long PDF or report into a one-page brief with a table of key figures and their source sections. | You have a long document and need the key findings and numbers. |
| [research-brief-writer](research-brief-writer/SKILL.md) | Writes a sourced overview of a topic, separating points of agreement from expert disagreement and noting gaps. | You need background on a topic, with sources and an honest view of the debate. |
| [meeting-notes-to-actions](meeting-notes-to-actions/SKILL.md) | Turns meeting notes or transcripts into decisions, action items with owners and dates, and open questions. | You have meeting notes and need follow-ups. |
| [email-triage](email-triage/SKILL.md) | Sorts a batch of emails into reply now, reply later, delegate, or ignore, and drafts urgent replies. Never sends. | You have a backlog of email to process. |
| [spreadsheet-formulas](spreadsheet-formulas/SKILL.md) | Writes, explains, and debugs Excel and Google Sheets formulas, including common error codes. | You need a formula or an error fixed. |
| [data-cleaning](data-cleaning/SKILL.md) | Standardizes messy CSV or spreadsheet data and logs every change, leaving the original untouched. | You have a tabular file that is inconsistent. |
| [resume-tailoring](resume-tailoring/SKILL.md) | Adapts a resume to a job posting using only experience already in it, with a gap report. | You have a resume and a job description. |
| [interview-prep](interview-prep/SKILL.md) | Generates likely interview questions, answer structures, and feedback on practice answers. | You have an upcoming interview. |
| [code-review](code-review/SKILL.md) | Reviews code for bugs, security issues, edge cases, and readability, ranked by severity. | You want a review before merging. |

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
