# Lessons Learned

## Summary
Across 6 principles, 6 explanations and 18 quiz questions, validation found **7 errors: 0 High, 4 Medium, 3 Low**. No quiz answer key was wrong. The Medium errors were not invented facts: they were omissions of core conditions and paraphrases that shifted the meaning. All Medium errors were fixed in Run B once the official text was provided.

## Findings

**1. The most frequent risk is wording that sounds right but is not.**
The AI replaced "lack of sophistication" with "lack of expertise" (P14) and described Market Colour as information that "stays general" instead of "effectively aggregated and anonymised" (P22). Both read naturally and would pass a quick review, but each changes what the learner understands the principle to require.

**2. One misconception was systematic, not random.**
In both runs of Principle 19, the AI stated that disclosure is covered by Principle 20 rather than Principle 19, and in the second run it used this to justify leaving out a core rule (disclosure only to parties with a valid reason, never where misuse is likely). A confident error that leads to deliberate omission is harder to spot than a visible mistake.

**3. Self-flags of uncertainty help, but do not replace validation.**
Every run ended with a note on accuracy. The flags pointed to the right areas in several cases, but they did not identify the actual problem: in P14 the flagged option did contain an error, yet the flag did not mention the shift in meaning. In P20 the AI claimed it had verified the content against the current Code; that content was in fact correct, but the claim itself could only be confirmed by checking.

**4. Web access did not mean access to the authoritative source.**
In the runs where the AI searched the web, it relied on secondary material (ECB and ACI pages, GFXC materials and a 2021 consultation paper), not on the Code itself. One review note asked for validation against the "2021 text", although the current version dates from December 2024. Following the AI's own advice literally would have meant checking against an outdated source.

**5. Validation needs more than the principle text.**
Several items were only verifiable with the Code's Annex 1 examples (P14, P17) or its definitions (the Foreword's definition of "Market Participant" covers both firms and personnel). A validator working from the principles alone could wrongly mark correct content as an error.

**6. Grounding in the source fixed the errors.**
In Run B, the AI rewrote each Medium-severity item with the official text pasted in. All three items were corrected without introducing new errors.

## Controls a real e-learning product would need
- **Generate from the source:** provide the official text of the current version to the AI rather than relying on its own knowledge or web search.
- **Pin the version:** record which version of the Code each item is based on, and re-check all items when the Code is updated.
- **Expert review before release:** a subject-matter expert checks every item against the principle, the Annex examples and the definitions, using a checklist per principle.
- **Error log with severity:** document every deviation and require that no High-severity error remains open.
- **Use the Code's terminology:** keep a short glossary aligned with the Code, so paraphrases do not drift in meaning.
- **Separate background from requirements:** label any context that goes beyond the Code (for example, the history behind it).

## Limitations
- Small sample: 6 principles, one AI tool, one validator.
- Test conditions were not fully uniform: web search was active in some runs, and Principle 19 was first run outside incognito mode. These deviations are documented in `prompts.md`.
- Low-severity errors were documented but not corrected in Run B.
