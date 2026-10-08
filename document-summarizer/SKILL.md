---
name: document-summarizer
description: Condenses long PDFs, reports, papers, and similar documents into a one-page brief with key findings, a table of figures traced to their source sections, and noted limitations. Use when the user provides a long document and asks for a summary, brief, key takeaways, executive summary, or the main numbers from it.
---

# Document Summarizer

Use this skill to turn a long document into a one-page brief that a busy reader can trust. Every figure in the brief must trace to the document, and the brief must say clearly what the document does not establish.

## When to use it

Use this skill when the user:
- Provides a PDF, report, paper, white paper, policy, audit, or long memo and asks for a summary.
- Asks for "key figures", "main takeaways", "the numbers that matter", or an executive summary.
- Asks for a brief to share with someone who will not read the original.

Do not use it for a question about one specific passage, which is a lookup task. Do not use it to critique or fact-check the document, which needs a separate review.

## Before you summarize

1. **Confirm access.** Check that the full text is available. If the document is scanned and the text is unreadable, say which pages are affected and ask whether the user can supply a text version. Do not summarize pages you could not read.
2. **Identify the purpose and audience.** Is the document informing, persuading, reporting results, or recording a decision? Who is it for? This decides which findings to emphasize. If the user has said who the brief is for, use that.
3. **Note the date and version.** Figures change between editions. Record the publication or data date on the first line of the brief.
4. **Check the scope.** If the document is very long (over about 60 pages), ask whether the user wants the whole document or specific sections. If they do not reply, summarize the executive summary, introduction, conclusions, and any section with a substantial number of figures, and say which sections you covered.

## Steps

1. **Read the full document,** including tables, figure captions, appendices, and footnotes. Numbers often appear in footnotes or appendices and are not repeated in the main text.
2. **Map the structure.** List the main sections and the page range of each. You will cite sections in the brief, so keep this list.
3. **Extract the figures.** For every number that matters to the document's argument or decisions, record:
   - The metric and its unit.
   - The value exactly as written, including the currency, the base year, and any qualifier such as "approximately" or "preliminary".
   - The period or date it refers to.
   - The page or section where it appears.
   If two places in the document give different values for the same metric, record both, note the difference, and do not pick one silently.
4. **Identify the findings.** Separate what the author found or concluded from what the author is recommending and from what the author only assumed or hopes will happen. Keep these labels distinct in the brief.
5. **Identify the limitations.** Look for stated caveats, sample sizes, scope limits, data gaps, conflicts of interest disclosed by the author, and anything marked as preliminary or not reviewed.
6. **Draft the brief** using the structure below. Target about 300 to 450 words. Do not pad it to reach that length. A shorter accurate brief is better than a longer one with filler.
7. **Check the brief against the source.** For each figure in the table, confirm it matches the source value and section. For each finding, confirm the author actually made that claim, not a version of it that you inferred.

## Output structure

**Title and source**
Document title, author or organization, publication or data date, and page count if known.

**Purpose** (1 to 2 sentences)
What the document sets out to do and who it is for.

**Key findings** (3 to 5 bullets)
The main conclusions the author draws. Use the author's position, and attribute it: "The report concludes that..." Do not present a finding as established fact if the author framed it as an estimate or a possibility.

**Key figures** (table)

| Metric | Value | Period or date | Source section |
|---|---|---|---|

Include only the figures that bear on the findings. Aim for 5 to 10 rows. Keep values exactly as written in the document.

**Recommendations or next steps** (2 to 4 bullets)
What the author recommends, stated as the author stated it. Mark any recommendation that is conditional, such as "if funding is approved."

**Limitations and open questions** (1 to 3 bullets)
What the document does not cover, where the data is weak, and what a reader would need to know before relying on it. Include any caveats the author gives.

## Rules

- Use only figures that appear in the document. If the user asks for a figure that is missing, say that it is not in the document. Do not calculate or estimate one unless the user asks, and if you do, label it as your calculation and show the inputs.
- Keep the author's wording for numbers, dates, and units. Do not round, convert currencies, or change date formats unless asked.
- Keep the author's conclusions separate from your summary. Do not add your own opinion, evaluation, or prediction.
- Do not summarize a section you could not read. Name it in the limitations.
- If a figure is in a chart or image, read the value only if it is clearly labeled. Otherwise say the value could not be read reliably.
- If the document contains an error you notice, such as an arithmetic mismatch between two tables, flag it in the limitations rather than correcting it.

## Adjusting length and focus

- If the user asks for a shorter brief, keep the title, purpose, and key figures, and cut the rest to one line each.
- If the user asks for a particular focus (for example, "only the financial figures"), limit the table and findings to that focus, and state the focus under the title.
- If the user asks for a brief for a specific audience, change the emphasis but not the facts. Do not remove a limitation to make the brief more persuasive.

## Example

Input: a 40-page annual sustainability report, requested as a one-page brief for a board meeting.

Output (abbreviated):

**Title and source**
Annual Sustainability Report 2025, Example Co. Published March 2026. 40 pages.

**Purpose**
Reports the company's emissions, energy use, and progress against its 2025 targets, and sets out goals for 2030.

**Key findings**
- The report states that Scope 1 and 2 emissions fell compared with 2024.
- It attributes most of the reduction to a change in energy supplier, not to operational efficiency.

**Key figures**

| Metric | Value | Period | Source section |
|---|---|---|---|
| Scope 1 and 2 emissions | 41,200 tCO2e | 2025 | Section 3.1, Table 4 |
| Scope 1 and 2 emissions | 48,900 tCO2e | 2024 | Section 3.1, Table 4 |

**Limitations and open questions**
- Scope 3 emissions are excluded and the report says they are "under review."
- Table 4 and the executive summary differ on the 2024 baseline; the table value is used here.
