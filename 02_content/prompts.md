# Prompts and Method

## Source and scope
- **Source:** FX Global Code, version updated December 2024, published by the GFXC.
- **Principles in scope:**

| Section | Principle | Topic |
|---|---|---|
| Execution | 11 | Pre-Hedging |
| Execution | 14 | Mark Up |
| Execution | 17 | Last look |
| Information Sharing | 19 | Identifying and limiting access to Confidential Information |
| Information Sharing | 20 | Disclosure of Confidential Information to external parties |
| Information Sharing | 22 | Market Colour |

## Test design
- **Run A (without source):** the AI writes the content from its own knowledge. This shows what a typical user would get and which errors occur.
- **Run B (with source):** for each item with a High severity error in Run A, the AI gets the official text of that principle and rewrites the item. This shows whether grounding in the source fixes the error.
- Each run is done in a **new chat**, so earlier answers don't influence the result.
- Tool, model and date are recorded for each run.

| Run | Tool / model | Date |
|---|---|---|
| A | _to fill in_ | _to fill in_ |
| B | _to fill in_ | _to fill in_ |

## Prompt 1: Explanation (Run A)
```
You are writing a short e-learning module for junior FX traders and supervisors
who are new to the FX Global Code.

Explain Principle [NUMBER] of the FX Global Code ([TOPIC]) in plain English.
- Maximum 150 words.
- State what the principle requires and why it matters.
- Include one short practical example from an FX dealing desk.
- Do not add requirements that are not in the Code.
- If you are unsure about any point, say so explicitly.
```

## Prompt 2: Quiz questions (Run A, same chat as Prompt 1)
```
Write 3 multiple-choice questions on Principle [NUMBER] of the FX Global Code.
- 4 answer options each, exactly one correct.
- Wrong options should be plausible but clearly wrong according to the Code.
- At least one question should be a short practical scenario.
- After each question, give the correct answer and a one-sentence explanation
  that refers to the Code.
```

## Prompt 3: Correction with source (Run B, new chat)
```
Below is the official text of Principle [NUMBER] of the FX Global Code
(version updated December 2024).

[PASTE THE PRINCIPLE TEXT]

Rewrite the following explanation / question so that it is fully consistent
with this text. Use only the text above. Mark every change you make.

[PASTE THE ITEM WITH THE ERROR]
```

## Validation rules
1. Check every statement against the official text of the principle, not against memory.
2. Use the illustrative examples in Annex 1 of the Code to check scenario questions.
3. Log every deviation in `03_validation/error_log.csv`, even small ones.
4. Apply the severity levels from `01_requirements.md` (High / Medium / Low).
