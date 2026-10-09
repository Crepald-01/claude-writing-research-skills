---
name: meeting-notes-to-actions
description: Turn messy meeting notes, transcripts, or voice-memo dumps into a clean summary with decisions, action items (owner and deadline), and open questions. Use when the user shares meeting notes or a transcript and wants follow-ups.
---

# Meeting notes to action items

## Output structure
1. **Summary**: 2–3 sentences on what the meeting was for and what was reached.
2. **Decisions**: one line each, stating what was decided and by whom if known.
3. **Action items**: table with columns Task | Owner | Due | Status.
4. **Open questions**: anything raised but not resolved.

## Rules
- Only include an owner if one was named or clearly implied. Write "Unassigned" otherwise.
- Only include a due date if one was stated. Write "Not set" otherwise. Do not invent dates.
- Merge duplicate tasks that were phrased differently in different parts of the notes.
- Turn vague items ("look into pricing") into a concrete next step ("Compare three pricing tiers, owner: unassigned") and flag that it was reworded.
- Keep the summary under 100 words. Do not reproduce the transcript.
- If the notes are too sparse to identify owners or dates, say so and list what is missing instead of guessing.
