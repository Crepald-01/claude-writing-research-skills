---
name: email-drafter
description: Summarizes an email thread and drafts a reply in a requested tone, flagging any facts the thread does not contain. Use when the user pastes an email or thread and asks for a reply, follow-up, decline, apology, or help answering a message, or asks what a thread is about.
---

# Email Drafter

Use this skill to turn a pasted email thread into a clear summary and a ready-to-send reply. The goal is a draft the user can send after reading it once, with nothing invented and nothing important missing.

## When to use it

Use this skill when the user:
- Pastes one email or a full thread and asks for a reply.
- Asks for a follow-up, reminder, decline, acceptance, apology, or escalation.
- Asks what a thread is about, what is still open, or what they owe someone.
- Asks to make a reply "shorter", "firmer", "warmer", or "more formal" after a first draft.

Do not use it for writing a new cold email with no thread to reply to. That is a plain writing task, though the same tone rules apply.

## Before you draft

Check for these inputs. If one is missing and it changes the reply, ask one short question. Otherwise proceed and note the assumption.

1. **The thread.** Read every message, oldest first. Emails often quote earlier messages, so do not treat the quoted text as new content.
2. **The sender's role relative to the user.** Is the sender a client, manager, colleague, vendor, recruiter, or stranger? This sets the default formality.
3. **The user's goal.** Yes, no, need more time, negotiate, or just acknowledge? If the user has not said, infer the most likely goal from the latest message and state it in one line.
4. **The tone.** Use the tone the user asks for. If none is given, use polite and neutral, and say which tone you chose.
5. **The user's name and sign-off.** Use it only if provided. Never guess a name from the email address.

## Steps

1. **Map the thread.** For each message, record: sender, date, what they asked or stated, and whether it was answered. Note any message that the user sent and still needs a response.
2. **Find the open items.** List every question, request, deadline, and decision pending. A thread often has more than one. Check the most recent message first, then earlier ones for requests that were never answered.
3. **Write the thread summary.** Use 2 to 4 bullets covering the topic, the state of the conversation, and the open items. Include dates and figures exactly as written in the thread.
4. **Decide the reply's job.** Each reply should do one of these: answer, confirm, decline, ask for something, delay, or apologize. If it must do several, put the most urgent first.
5. **Draft the body.**
   - Open with a direct response to the latest message, not a pleasantry about it. A short thank-you is fine when it fits the tone.
   - Answer each open item in the order the sender raised them, or lead with the most important item.
   - For facts the thread does not contain (a price, a date, a yes or no on a commitment the user has not made), use [CONFIRM: what is needed] instead of inventing it.
   - Keep sentences short. Prefer 3 to 6 sentences for a simple reply and up to two short paragraphs for a complex one.
   - End with one clear next step: a question, a date, or a statement of what happens next. Do not end with an open-ended "let me know your thoughts" unless no other next step exists.
6. **Write the subject line.** If the thread has a subject, keep it, and add "Re:" only if it is not already there. If the user is starting a new topic inside the thread, offer a new subject line.
7. **Check the draft.** Before you return it, confirm:
   - Every question in the latest message is answered or marked [CONFIRM].
   - No commitment, date, price, or number appears that was not in the thread or from the user.
   - The tone matches what was requested throughout, not just in the first line.
   - The length fits the reply's job.
8. **Offer one variation** only if the user's goal is ambiguous, such as a firm and a gentle version of a decline. Otherwise return one draft.

## Tone guide

- **Formal:** full sentences, titles where known, no contractions, clear closing such as "Kind regards."
- **Friendly:** contractions allowed, first names if the thread uses them, one brief warm line.
- **Firm:** state the position in the first sentence, give a concrete deadline or condition, no apology unless the user is at fault.
- **Apologetic:** name the specific issue, take responsibility without groveling, say what will change or be fixed.
- **Neutral (default):** plain, polite, no emotion words, no filler.

## Edge cases

- **Angry or hostile sender.** Do not mirror the anger. Acknowledge the concern in one sentence, answer the factual points, and move to next steps. Flag it in the notes if the user may want to involve someone else before replying.
- **Legal, financial, or medical content.** Draft the reply, but note that the user should check any commitment, figure, or legal wording before sending.
- **Multiple recipients (reply all).** Note who is copied. Do not include anything the user might not want shared with everyone on the thread, and flag it if the thread includes a message that looks private.
- **Forwarded emails with no clear request.** Ask what the user wants to do with it. Do not guess a reply.
- **Non-English thread.** Reply in the language of the latest message unless the user asks for another language. Mention the language in one line.

## Output format

Return the response in this order and use these headings:

**Thread summary**
- Topic, state of the conversation, and open items, in 2 to 4 bullets.

**Draft reply**
Subject: (only if needed)

[Body text, ready to paste]

**Notes** (include only if relevant)
- [CONFIRM] items and what the user needs to provide.
- Tone chosen, if the user did not specify one.
- Any warning, such as a commitment that needs review or a copied recipient who should not see the reply.

## Rules

- Never invent facts, dates, prices, names, or commitments. Use [CONFIRM] placeholders.
- Do not add a signature unless the user supplies their name or signature block.
- If the user gives a length, follow it exactly.
- Do not add apologies, thanks, or pleasantries the user did not ask for and the tone does not need.
- Keep quoted text out of the draft unless the user specifically wants to quote a line back.
- If the user asks you to send the email, explain that this skill only drafts it. The user sends it.

## Example

Input: a client asks whether a project can be delivered by 15 May. The user wants to say yes but has not confirmed the date with their team.

Output:

**Thread summary**
- Client asked on 2 May whether the project can be delivered by 15 May.
- No reply sent yet; this is the only open question.
- Deadline requested: 15 May.

**Draft reply**
Subject: Re: Project delivery timeline

Hi Anna,

Thanks for checking. I can confirm delivery by [CONFIRM: 15 May or the date your team agrees]. I will send a written schedule by [CONFIRM: day] so you can plan your side.

Best,
[CONFIRM: your name]

**Notes**
- The date is not confirmed. Check it with your team before sending.
- Tone: friendly and professional, since the thread is informal.
