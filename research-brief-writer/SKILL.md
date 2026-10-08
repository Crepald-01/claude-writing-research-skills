---
name: research-brief-writer
description: Writes a sourced research brief on a topic, separating what sources agree on from where experts disagree, with each position attributed and gaps in the evidence named. Use when the user asks for a research brief, background overview, literature summary, state of knowledge on a topic, or a summary of what is known and debated about a subject.
---

# Research Brief Writer

Use this skill to produce a short, sourced brief that tells the reader what is known, what is contested, and what remains unknown on a topic. The brief must be fair to competing positions, must cite its claims, and must not give a personal verdict on questions that are still open.

## When to use it

Use this skill when the user:
- Asks for background on a topic, a history, or an overview of current knowledge.
- Asks what experts think about a question, or where a debate stands.
- Needs a brief to prepare for a meeting, a decision, an article, or a study.
- Asks for a comparison of positions on a contested policy, scientific, or historical question.

Do not use it for a question with a single documented answer, such as a date or a definition. Answer those directly, with one source.

## Before you research

1. **Pin down the question.** Restate the topic as a question the brief will answer, in one sentence. Example: "Topic: remote work and productivity" becomes "What does the evidence say about how remote work affects productivity, and where do researchers disagree?"
2. **Set the scope.** Decide on the time range (for example, studies from the last ten years), the geographic focus, and the population or sector if relevant. If the topic is very broad, choose the most useful angle and state in the brief what you left out.
3. **Check for a stated purpose.** Is the brief for a decision, a general reader, a student, or a specialist? This sets the depth and vocabulary. Default to a general educated reader.
4. **Check the currency.** Some topics change within months, such as regulations, prices, or AI capabilities. For these, prioritize sources from the past six months and state the date of the most recent source.

## Steps

1. **Gather sources.** Find at least three independent sources for each major claim. Rank them by reliability:
   - Highest: primary data, official statistics, peer-reviewed studies, original legal or policy texts, and primary historical records.
   - Middle: reputable reviews, systematic reviews, expert reports from recognized institutions, and quality journalism that cites primary sources.
   - Lowest: opinion pieces, company marketing, blogs, and forums. Use these only to show that a view exists, and label them as such.
   Record for each source: title, author or publisher, date, type, and link.
2. **Read the sources, not just the abstracts.** Check the methods, sample, scope, and limitations. A conclusion can be stronger or weaker than its abstract suggests.
3. **Group the findings.** Put each relevant finding under one of three headings: points of agreement, points of disagreement, and open questions. A finding goes under agreement only if most credible sources reach it independently.
4. **Map each disagreement.** For each one, record:
   - The specific claim in dispute, stated neutrally.
   - Each position, stated in its strongest version.
   - Who holds each position, with sources.
   - The evidence each side relies on, and its main weakness.
   - Whether the disagreement is about facts, methods, values, or definitions. A disagreement about definitions is often resolved by stating the definition used.
5. **Note the gaps.** Record what the evidence does not settle: missing data, studies that have not been done, results that have not been replicated, and places where all sources share the same assumption.
6. **Check for bias.** Note who funded or produced each source where that is disclosed, and any strong institutional stake in the answer. Do not dismiss a source for its funding alone, but say where it matters to the reading.
7. **Write the brief** using the structure below. Then check it against the rules in the next section.

## Output structure

**Topic and scope**
One sentence stating the question the brief answers and the scope (time range, region, or population).

**Summary**
Three to five sentences. Give the state of the evidence in the first sentence, the main disagreement in the second, and the main gap in the third.

**What sources agree on**
Three to six bullets. Each bullet is one finding, with the sources that support it in brackets, for example [1, 4].

**Where experts disagree**
One subsection per disagreement, with a bold label. For each:
- **The question:** the disputed claim, stated neutrally.
- **Position A:** the view, the people or sources who hold it, and the evidence it rests on.
- **Position B:** the same structure.
- **Why they differ:** the main reason, such as different data, different definitions, different time periods, or different values.

**Gaps and uncertainty**
Two to four bullets naming what the evidence does not establish, and what kind of research would close each gap.

**Sources**
A numbered list. Each entry: title, author or publisher, date, and link. Match the numbers used in the brief.

## Rules

- **Cite every factual claim.** If you cannot source a claim, leave it out or mark it "unverified."
- **Attribute opinions.** Write "the report argues" or "critics contend," not a bare statement. A claim made by one source is not a fact of the field.
- **Give each position its strongest version.** Write the case the way its best advocate would make it, then note the main criticism. Do not write a position as a straw man.
- **Do not state a personal conclusion on contested questions.** You may say which position has more direct evidence on a narrow factual point, if the sources support it. On value questions or unresolved empirical questions, lay out the positions and leave the weighing to the reader.
- **Keep the brief under 600 words** unless the user asks for more. If the topic needs more, offer a longer version or a list of further reading.
- **State the date of the newest source** and say if the topic is fast-changing.
- **Do not present a single study as settled.** Say "one study found" when the finding rests on one source.
- **Keep quotations short.** Paraphrase in your own words, and use a direct quote only when the exact wording matters, and keep it brief.
- **Do not invent sources, authors, dates, or links.** If you cannot verify a source, say so rather than providing a citation.

## Handling thin or conflicting evidence

- **Little evidence exists.** Say so in the first sentence of the summary, list the few sources you found, and do not extrapolate beyond them.
- **Sources contradict each other on a fact (not an interpretation).** Check the primary source behind each. If the conflict remains, report both figures with their sources and say the conflict is unresolved.
- **Expert consensus is strong.** State it as consensus, cite the bodies or reviews that show it, and note any dissenting views that exist. Do not manufacture a disagreement to appear balanced.
- **The topic is politically or morally contested.** Describe the positions and the evidence each side uses. Do not characterize one side's motives. Use neutral terms that each side would accept as a fair description of its own view where possible.

## Example

Input: "Give me a brief on whether intermittent fasting helps with weight loss compared with regular calorie restriction."

Output (abbreviated; the source entries are placeholders showing the format, not real citations, and a real brief must use sources you have checked):

**Topic and scope**
What does the evidence show about intermittent fasting compared with continuous calorie restriction for weight loss in adults, based on controlled trials from the last ten years?

**Summary**
Several randomized trials find that intermittent fasting and continuous calorie restriction produce similar weight loss when calories are matched. Researchers disagree on whether fasting windows add any benefit beyond the calorie reduction itself. Long-term adherence data are limited, and most trials last under a year.

**What sources agree on**
- When total calories are matched, the two approaches produce similar average weight loss [1, 2].
- Many participants find both approaches hard to sustain beyond a year [2, 3].

**Where experts disagree**
- **The question:** Does timing of eating add a benefit beyond calorie reduction?
- **Position A:** Some researchers report small additional effects on appetite or metabolic markers, and argue that timing matters for some people [4].
- **Position B:** Others find no meaningful difference after adjusting for calories and argue the effect is explained by eating less [1].
- **Why they differ:** Trials use different fasting schedules, sample sizes are small, and some studies do not control for total intake.

**Gaps and uncertainty**
- Few trials last longer than a year.
- Most participants are not representative of the general population.

**Sources**
1. Example, A. (2024). Title of trial. Journal. https://...
