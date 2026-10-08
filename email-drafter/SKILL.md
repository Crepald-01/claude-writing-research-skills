---
name: email-drafter
description: Drafts email replies in a requested tone, with a short summary of the thread. Use when the user pastes an email thread and asks for a reply, a follow-up, or help answering a message.
---

# Email Drafter

## Steps

1. Read the full thread, oldest message first. Note who sent each message, what was asked, and what is still open.
2. Write a summary of the thread in 2 to 4 bullet points: the topic, the open questions, and any deadlines.
3. Identify the tone requested (for example: formal, friendly, firm, apologetic). If no tone is given, use a polite, neutral tone and say so.
4. Draft the reply:
   - Open by addressing the most recent message directly.
   - Answer every open question. If a question cannot be answered from the thread, mark it with [CONFIRM] instead of inventing an answer.
   - Keep it short. Prefer 3 to 6 sentences unless the user asks for more.
   - End with a clear next step or question.
5. Offer one alternative subject line if the thread has none, or if the user asks for a new subject.

## Rules

- Never invent facts, dates, prices, or commitments. Use [CONFIRM] placeholders instead.
- Do not add a signature unless the user provides their name.
- If the user asks for a specific length, follow it.

## Output format

**Thread summary**
- bullet points

**Draft reply**
Subject: (if needed)
Body text

**Notes** (only if there are [CONFIRM] items)
