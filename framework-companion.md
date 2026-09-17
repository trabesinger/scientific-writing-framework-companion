# Multi-Level Framework for Scientific Writing — Companion and Prompt Library

**A companion to:** Trabesinger, A. (2026). *Multi-level framework for scientific writing* (Version 1.3) [Report]. Zenodo. https://doi.org/10.5281/zenodo.18642949

**License:** CC BY-SA 4.0 — free to use, adapt, and share with attribution.

---

## About this document

The [Framework PDF](https://doi.org/10.5281/zenodo.18148137) sets out four hierarchical levels of scientific writing — manuscript, section, paragraph/sentence, word — as a single-page visual reference. It assumes some familiarity with the underlying concepts (hourglass structure, thematic progression, signposting) but works as a standalone checklist even without that background.

This document expands each level into working detail, in two parts:

1. **The framework itself** — the same checklists, written out in full, for direct use by a writer or editor.
2. **A prompt library** — every checklist item converted into a ready-to-use instruction for a large language model, so the framework can be applied directly in an AI-assisted writing or editing session. This isn't specific to any one AI assistant; the prompts work as plain instructions for whichever tool you use.

Read top to bottom for writing. Work bottom to top for editing — fix structure before polishing words.

This document gives you the diagnostic categories. Applying them to your own manuscript — with feedback on the judgment calls where they overlap or conflict — is what the [scientific writing workshops](https://reinschrift.ch) are for.

---

## The four levels

| Level | Focus | Key questions |
|-------|-------|---------------|
| **Manuscript** | Story arc, overall narrative | Why? What? So what? |
| **Section** | Structure and function of each part | Does each section do its job? |
| **Paragraph/Sentence** | Flow, coherence, signposting | Is the logic visible and connected? |
| **Word** | Economy, precision, formality | Is every word earning its place? |

---

## Level 1: Manuscript

The manuscript level concerns the overall story and how it's conveyed to different readers.

### Story structure: Why? / What? / So what?

Every scientific paper must answer three questions:

1. **Why?** — What is the problem, gap, or motivation?
2. **What?** — What did you do? What did you find?
3. **So what?** — Why does it matter? What are the implications?

Can you articulate the paper's story in three sentences (why/what/so what)? Is the "so what" compelling and specific, not generic? Does the narrative thread run clearly from introduction through discussion?

### Abstract quality

The abstract must be self-contained and tell the complete story in miniature. Does it follow the hourglass structure (broad → narrow → broad)? Can a non-specialist grasp the significance? Are the main findings stated, not just hinted at?

### Figure strategy

Can you understand the paper's main message from figures alone? Does each figure have a clear purpose in the narrative? Are figures referenced at appropriate points in the text?

### Reader hierarchy

Different readers engage at different depths:

| Reader type | What they read | What they need |
|-------------|----------------|----------------|
| Quick reader | Title, abstract, figures | Complete story in compressed form |
| General reader | + Introduction, conclusions | Context and significance |
| Specialist | Full text | Methods, details, nuance |

Does each level work for its intended reader?

A useful additional test: can a *newcomer to the subfield* — typically a first-year PhD student or a talented MSc student — use the supplementary material (SI) to reproduce the work? The SI should contain everything specific to this paper that is not available elsewhere: detailed protocols, parameters, derivations, code, and data. Standard background knowledge belongs in textbooks and the literature; paper-specific knowledge belongs in the SI.

---

## Level 2: Section

Each major section has a specific function. Evaluate whether it fulfils that function.

### Title

Is it specific and informative? Does it convey the main finding or contribution? Avoid generic titles, question titles (usually), and overly clever titles.

### Abstract

Structure (hourglass):
1. **Opening** — Broad context, why this matters
2. **Background** — More specific context, state of the field
3. **Gap/Problem** — What's missing, what's the question
4. **"Here we..."** — The pivot from problem to solution. This statement marks the transition from what is missing to what this paper delivers. It should be specific enough that a reader could reconstruct the paper's core contribution from it alone. Everything before it establishes why the paper is needed; everything after it is the payoff.
5. **Key findings** — Main results, stated clearly
6. **Implications** — So what? Broader significance

**Common failure mode — the grant-proposal abstract:** In general-audience journals, a frequent error is an abstract structured as broad field context → methodological approach → vague gesture at results. This reads like a grant proposal and buries the finding. The corrective is to lead with the result (or at minimum, the surprise), and use the "Here we…" pivot to introduce the approach. Ask: *could a reader state the main finding after reading only the abstract?* If not, the abstract needs refining.

### Introduction

Function: lead the reader from broad context to your specific question. Does it establish the gap in knowledge? Is the "funneling" smooth (broad → narrow)? Does it end with a clear statement of what this paper will do? Is it appropriately concise?

### Results

Each results paragraph should have a clear narrative function: open by stating the question or observation the paragraph addresses, present the evidence or finding, and close by spelling out the connection to what follows.

Is the logic between consecutive observations made explicit, or does the reader have to infer it? Are paragraphs presenting data, or telling a story with data as evidence? Is the main finding of each paragraph clear from its opening sentence? Are figures and tables placed appropriately? Is the connection between methods and results clear? Are placeholders, incomplete passages, and author notes removed before submission?

**A common failure mode:** results paragraphs that describe what a figure shows rather than what the data mean. The figure caption does the former; the results text should do the latter. Each paragraph should make a scientific statement and use the figure as evidence, not narrate its contents.

### Discussion

Function: interpret results, address limitations, connect to broader context. Does it open with the main finding, framed in terms of its interpretation or significance — not merely restating what was observed? The opening sentence of the Discussion should advance the reader's understanding, not replay the Results section. Are alternative explanations considered? Are limitations acknowledged honestly? Does it connect findings to the field (funnel back out)?

### Conclusions

Is it specific to this work, not generic statements? Forward-looking where appropriate? Free of new story elements not introduced earlier?

### Methods

Is there sufficient detail for reproduction? Is the organization logical — sequential by experimental procedure, or grouped by technique?

### Supplementary information

Supplementary information (SI) extends the main text without disrupting its flow. Use it for methodological detail beyond what the main Methods section can accommodate while remaining readable; extended figures, tables, and derivations that support but do not drive the main narrative; raw or processed datasets; and code and analysis scripts.

Is everything needed to reproduce the results available — either in the main text, the SI, or a linked repository? Are datasets deposited in an appropriate repository (e.g., Zenodo, Figshare, an institutional repository)? Is code available in a version-controlled repository (e.g., GitHub) with sufficient documentation to run it? Is there a data availability statement, and, if required by the journal, a code availability statement? Does the SI have its own internal logic, or is it a dumping ground? Careful reviewers and readers will read it.

### Verb tense by section

Different sections use different tenses by convention:

| Section | Tense | Rationale |
|---------|-------|-----------|
| Introduction | Present | Established knowledge is treated as current fact |
| Methods | Past | Describes what was done |
| Results | Past | Describes what was found |
| Discussion | Present | Interprets findings in relation to current knowledge |
| Conclusions | Present | States what is now known |

Within the Introduction, prior work is often referenced in past tense ("Smith et al. showed…"), switching to present for the accepted state of knowledge ("It is now understood that…"). Mixed tense within a section usually signals a structural problem.

---

## Level 3: Paragraph and sentence

This level concerns flow, coherence, and the logical structure of argument.

### Paragraph structure

Each paragraph should have a clear role in the argument, open with a topic sentence stating its main point, contain one main idea (the "paragraph = unit of thought" principle), and connect logically to the previous and next paragraphs. Can you summarize each paragraph in one sentence? If not, it may need splitting or refocusing.

### Signposting

Signposts guide readers through the argument: transitions between paragraphs ("However", "In contrast", "Building on this"), section openings that preview content, and explicit statements of structure ("We address three questions..."). Could a reader skim only the first sentence of each paragraph and follow the argument?

### Thematic progression

Sentences should connect logically through given–new structure: each sentence picks up an element from the previous sentence (given) and introduces new information (new); the "new" of one sentence often becomes the "given" of the next.

Example of poor flow:
> "The enzyme was purified. Column chromatography was used. Three fractions showed activity."

Example of good flow:
> "The enzyme was purified using column chromatography. This procedure yielded three fractions. Each fraction showed distinct activity levels."

### One message per sentence

Avoid overloaded sentences with multiple clauses. Split complex ideas across multiple sentences. The reader should grasp your point on first reading.

### Decluttering

Remove redundant phrases ("in order to" → "to"), weak openings ("It is important to note that..."), excessive hedging (keeping appropriate hedging), and unnecessary nominalizations ("make a measurement" → "measure").

---

## Level 4: Word

The finest level of polish — but only worth attention once higher levels are sound.

### Economy

Use short words where they work as well as long ones. Cut words that add no meaning. Prefer active voice, usually.

| Wordy | Concise |
|-------|---------|
| in order to | to |
| due to the fact that | because |
| a large number of | many |
| at the present time | now |
| in the event that | if |
| it is possible that | perhaps / may |

### Clarity and precision

Use precise technical terms correctly. Avoid ambiguous pronouns (unclear "this", "it", "they"). Define acronyms on first use. Be specific: "increased significantly (p < 0.01)" not "increased a lot".

### Hedging and certainty

Calibrate the strength of claims precisely to what the evidence supports. Under-hedging overstates; over-hedging undermines the contribution.

| Stronger claim | Weaker claim |
|----------------|--------------|
| prove, demonstrate | suggest, indicate |
| show | appear to show |
| confirm | are consistent with |
| the data establish | the data are compatible with |

Is every claim in the paper at the right point on this spectrum? "Suggest" where the evidence is strong is as misleading as "prove" where it is not.

### Objectivity and formality

Scientific writing should be objective (focus on evidence, not feelings), formal (appropriate register for an academic audience), and cautious where appropriate ("suggests" vs "proves"). Avoid hyperbole ("groundbreaking", "revolutionary"), colloquialisms, and first person where it draws attention from the work.

### Crutch phrases

Certain phrases recur so frequently in scientific writing that they have lost communicative force.

**Vague evaluative language** — these tell the reader how to feel rather than showing why the result matters: "intriguing", "fascinating", "exciting", "elegant", "remarkable", "striking", "notable". Replace with a specific statement of *why* the finding is significant.

**Introduction crutches:** "in recent years", "over the past decades", "has been extensively studied", "is receiving great interest", "plays an important role in science and technology". These substitute for genuine contextualization. State specifically what has been established, by whom, and what remains open.

**Conclusion crutches:** "further research is needed", "opens new avenues", "paves the way for", "sheds light on", "lays the groundwork for", "provides a platform for". These are placeholders for a genuine forward-looking statement. Say specifically what the next step is, or what question this work now makes answerable.

**Redundancies:** "past history", "future plans", "completely eliminate", "still remains", "end result", "brief summary", "absolutely essential". Cut the redundant word.

### Non-native-speaker patterns

Many manuscripts written by non-native English speakers share characteristic constructions worth flagging:

**Filler phrases** — wordy constructions with leaner equivalents:

| Wordy | Concise |
|-------|---------|
| in order to | to |
| due to the fact that | because |
| in the case of | for |
| with regard/respect to | on, about |
| in terms of | (often deletable) |
| it can be seen that | (delete; state the observation directly) |
| on the other hand | (only valid if "on the one hand" appeared earlier) |

**Stiff or over-Latinate constructions** — where simpler phrasing would serve equally well. Prefer short Anglo-Saxon words where they carry the same meaning: "use" not "utilize", "show" not "demonstrate" (unless demonstrating is specifically what was done), "find" not "identify" where no identification process is implied.

**Vague referents** — unclear use of "this", "it", or "they" without an unambiguous antecedent. Every demonstrative should have a referent the reader can identify without re-reading.

### Hyphens, en-dashes, and em-dashes

**Hyphens** (-) join compound modifiers before a noun ("high-resolution image", "well-established method") but are dropped when the modifier follows the verb ("the image is high resolution"). Also used in prefixes where needed for clarity ("re-examine", "co-author").

**En-dashes** (–) are used for ranges ("pp. 10–25", "2019–2023") and for compound terms where the elements are of equal weight and both are free-standing ("Bose–Einstein condensate", "cost–benefit analysis").

**Em-dashes** (—) mark a parenthetical aside or a strong break in a sentence. Spacing conventions vary by house style; follow the target journal.

Are hyphens, en-dashes, and em-dashes used consistently and correctly throughout? Inconsistent dash usage is a common copy-editing flag.

### -ize/-ise spellings

*New Hart's Rules* endorses **-ize** spellings as the Oxford scholarly convention ("organize", "recognize", "characterize") — one of several legitimate house-style choices, alongside -ise, used by different publishers. What matters is consistency: pick one convention and apply it throughout, following the target journal's house style where specified.

Exceptions that are always -ise regardless of house style: "advertise", "advise", "comprise", "revise", "supervise", and others where -ise is part of the root, not a suffix.

---

## Using the framework

### For writing (top-down)

1. Start at manuscript level: articulate your story (why/what/so what).
2. Plan sections: outline each section's purpose and content.
3. Draft paragraphs: write topic sentences first, then fill in.
4. Polish words: only after structure is sound.

### For editing (bottom-up)

1. Word level: fix obvious errors, tighten prose.
2. Sentence/paragraph level: check flow, signposting, paragraph unity.
3. Section level: verify each section fulfils its function.
4. Manuscript level: step back — does the story work?

### For grant proposals

The framework applies with adaptation:
- **Why** becomes: Why is this research needed? Why now? Why you?
- **What** becomes: What will you do? What is your approach?
- **So what** becomes: What will the impact be?

Track record and feasibility thread through the entire narrative in competitive grant schemes, not just in a designated section. Panels assess not only *what* will be done and *why it matters*, but *why this PI/team is the one to do it*. The same manuscript-level question — "so what?" — applies here to the applicant's positioning: why now, why this approach, why you? Narrative CVs and fellowship statements follow many of the same structural principles as grant proposals, with similar hourglass logic and story arc.

### For teaching

The framework supports progressive disclosure: introduce levels sequentially, use exemplar texts at each level, have students diagnose texts before revising, and build from manuscript-level thinking downward.

---

## Quick reference checklist

**Manuscript level**
- [ ] Story is clear: why / what / so what
- [ ] Abstract is self-contained and complete
- [ ] Figures tell the story independently
- [ ] Narrative thread runs throughout

**Section level**
- [ ] Title is specific and informative
- [ ] Introduction funnels from broad to specific
- [ ] Results presented objectively
- [ ] Discussion interprets without over-claiming
- [ ] Conclusions are specific, not generic
- [ ] Methods and SI enable reproduction

**Paragraph/sentence level**
- [ ] Each paragraph has one main idea
- [ ] Topic sentences are clear
- [ ] Signposting guides the reader
- [ ] Thematic progression connects sentences
- [ ] No overloaded sentences

**Word level**
- [ ] Prose is concise
- [ ] Technical terms used precisely
- [ ] No ambiguous pronouns
- [ ] Appropriate formality and hedging

---

## Appendix: Prompt library for AI-assisted writing and editing

Every checklist question above converts directly into an instruction for a large language model. The pattern is simple: prefix a checklist item with "Check whether…", "Help me ensure…", or "Analyse this text for…", paste in your draft, and ask.

The prompts below are organized by level so you can work top-down (writing) or bottom-up (editing), and are phrased generically — they work with any AI assistant, not a specific one.

### Manuscript-level prompts
- "Summarize the story of this paper in three sentences: why, what, so what. Then tell me if that story is compelling and specific rather than generic."
- "Check whether my abstract follows the hourglass structure — broad context, narrowing to the specific contribution, then broadening back out to implications."
- "Read only the abstract and figures of this draft, then tell me what you understand the paper's main finding to be. Does that match what I intended?"
- "Check whether a newcomer to this subfield — a first-year PhD student — could use the supplementary material to reproduce this work. Flag anything missing."

### Section-level prompts
- "Is this title specific and informative, or could it apply to many other papers? Suggest three alternatives that name the actual finding."
- "Check whether this abstract reads like a grant proposal — broad context, then methods, then a vague gesture at results — rather than leading with the finding."
- "Does this Introduction funnel smoothly from broad context to the specific gap this paper addresses? Does it end with a clear statement of what the paper does?"
- "Check whether this Methods section has enough detail for another researcher to reproduce the work."
- "For each paragraph in this Results section, tell me: what is the main finding, is it stated in the opening sentence, and does the paragraph interpret the data or merely narrate what a figure shows?"
- "Does this Discussion open by interpreting the main finding, or does it just restate the Results? Check whether limitations are acknowledged and alternative explanations considered."
- "Check whether these Conclusions are specific to this work rather than generic, and whether any new claims appear that weren't introduced earlier in the paper."
- "Check the verb tense in each section against convention: present for Introduction/Discussion/Conclusions, past for Methods/Results. Flag any inconsistencies."

### Paragraph/sentence-level prompts
- "For each paragraph, extract the topic sentence. Tell me if it accurately previews the paragraph's content, and if each paragraph contains only one main idea."
- "Check the signposting in this text — could a reader follow the argument by skimming only the first sentence of each paragraph?"
- "Analyse the thematic progression between sentences in this passage. Flag any place where the connection between consecutive sentences requires the reader to infer a missing link."
- "Find any overloaded sentences with multiple competing clauses and suggest how to split them."
- "Find weak openings, redundant phrases and unnecessary nominalizations in this text, and suggest leaner alternatives."

### Word-level prompts
- "Check this text for crutch phrases — vague evaluative words ('intriguing', 'remarkable', 'elegant') and generic introduction/conclusion filler ('has been extensively studied', 'opens new avenues'). Suggest specific replacements."
- "Check whether the strength of each claim in this text matches the strength of the evidence — flag any over-claiming ('prove', 'demonstrate') or under-claiming ('may possibly suggest') that doesn't fit."
- "Check this text for common non-native-English patterns: filler phrases like 'in order to' or 'with regard to', over-Latinate word choices, and vague pronoun references without a clear antecedent."
- "Check hyphen, en-dash, and em-dash usage in this text for consistency."
- "Check -ize/-ise spelling consistency throughout this document."

---

## References and resources

- Framework PDF: Trabesinger, A. (2026). *Multi-level framework for scientific writing* (Version 1.3). Zenodo. https://doi.org/10.5281/zenodo.18642949
- This companion document is licensed CC BY-SA 4.0 — free to use, adapt, and share with attribution.
