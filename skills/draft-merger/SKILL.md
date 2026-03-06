---
name: draft-merger
description: "Merge multiple drafts of the same document into one polished final version. Use this skill whenever the user provides 2 or more versions/drafts of a document and wants them combined, merged, consolidated, or synthesized into a single piece. Triggers on phrases like: 'merge these drafts', 'combine these versions', 'I have multiple drafts', 'pick the best one and combine', '把这几份稿子合并', '合并稿子', '整合稿子', '多份稿子', or whenever the user uploads/shares multiple files that are clearly different versions of the same content. Also trigger when user says 'merge', 'combine', 'consolidate', 'integrate', 'synthesize' in the context of documents or writing. Do NOT use for merging code, data, or files that aren't text documents."
---

# Draft Merger

This skill merges multiple drafts of the same document into one cohesive, polished final version. The process has three stages: **select a base draft**, **enrich it with content from other drafts**, then **polish the final result**.

## Stage 1: Read and Assess All Drafts

Read every draft the user has provided. As you read, build a mental map of:

- **Structure**: How is each draft organized? What sections does it have?
- **Strengths**: What does each draft do particularly well? (e.g., stronger argument, richer examples, more vivid language, better flow, more complete coverage)
- **Unique content**: What does each draft contain that the others lack?
- **Quality signals**: Depth of analysis, clarity of language, logical coherence, factual richness, emotional resonance

After reading all drafts, briefly summarize your assessment to the user — one sentence per draft capturing its character and main strength.

## Stage 2: Select the Base Draft

**If the user specified which draft to use as the base**, respect their choice without argument.

**If no base is specified**, identify the strongest draft yourself. The best base is typically the one with:
- The clearest overall structure and logical flow
- The strongest central argument or narrative
- The most polished language
- The broadest coverage of the topic

Tell the user which draft you've selected as the base and why, in 2–3 sentences. Invite them to override your choice if they prefer a different base. If they want a different base, switch to it before continuing.

## Stage 3: Enrich with Content from Other Drafts

Go through the other drafts systematically and identify content worth incorporating into the base. Ask yourself for each passage:

- **Is it absent from the base?** Only add genuinely missing content — not near-duplicates of what's already there.
- **Does it add value?** Strong examples, supporting evidence, nuanced arguments, key context, important caveats, vivid descriptions — these are worth adding. Filler, repetition, or weaker versions of existing content are not.
- **Does it fit naturally?** Find the right place in the base draft where the new content belongs. If it disrupts the flow badly, it may not be worth including.

As you identify valuable additions, integrate them into the draft. Aim for seamless insertion — the reader should not be able to tell which draft a given sentence came from.

**What to look for in other drafts:**
- Sections or paragraphs that cover aspects the base glosses over or omits entirely
- Better examples or more concrete illustrations of a point already made
- Stronger evidence, data, or citations
- Useful context (background, definitions, qualifications) that the base assumes the reader knows
- A compelling conclusion or introduction that the base lacks
- Distinctive phrasing or turns of phrase that are genuinely better than the base

**What to leave out:**
- Content that contradicts the base's argument (unless the contradiction is meaningful and worth surfacing — if so, flag it)
- Near-duplicate content that makes the same point less clearly
- Material that's tangential or off-topic relative to the base's focus
- Anything that would bloat the document without adding substance

## Stage 4: Polish the Final Draft

Once the base has been enriched, do a polishing pass over the whole document:

1. **Coherence and flow**: Read the document end-to-end as a new reader would. Fix any seams where inserted content disrupts the flow. Smooth transitions between sections.
2. **Eliminate redundancy**: Remove any passages that now repeat each other due to the merging process.
3. **Consistency**: Ensure consistent terminology, tense, tone, and voice throughout. If the drafts used different styles (formal vs. casual), choose the appropriate register and apply it uniformly.
4. **Language quality**: Improve sentence-level clarity. Fix awkward phrasing, tighten wordy sentences, and strengthen weak word choices — but don't over-edit. Preserve the author's voice.
5. **Structure**: Verify that the document structure still makes sense. Reorder sections if the merge revealed a better logical sequence.

## Output

Present the merged draft in full. After it, include a brief **Merge Notes** section (a short bulleted list) summarizing:
- Which draft was used as the base and why
- The most significant additions from other drafts
- Any notable editorial decisions (e.g., you chose not to include a section from Draft B because it contradicted the core argument)
- Any open questions for the user (e.g., "Draft C had an alternate conclusion — I used Draft A's, but let me know if you'd prefer the other")

## Handling Edge Cases

**Very similar drafts**: If the drafts are nearly identical, say so upfront. Focus the merge on selecting the best phrasing sentence-by-sentence rather than adding whole sections.

**Very different drafts**: If the drafts take fundamentally different approaches (e.g., different angles, audiences, or arguments), flag this before merging. Ask the user which direction they want to go, or whether they want a synthesis that draws from both approaches.

**Contradictions**: If two drafts make conflicting factual claims, point this out rather than silently choosing one. Let the user decide which is correct.

**Language mix**: If drafts are in different languages, confirm with the user which language the final draft should be in before proceeding.

**User-specified additions**: If the user says "also make sure to include X from Draft 2", honor that explicitly and call it out in the Merge Notes.
