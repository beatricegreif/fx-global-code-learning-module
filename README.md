# AI-Assisted Learning Module: FX Global Code

**Personal project (2026) · Beatrice Greif, CFA**

Status: completed (November 2026)

## Goal
A trader or supervisor new to the FX Global Code needs a short, reliable way to learn its key principles. This project tests whether an AI assistant can produce that learning content, and what controls are needed before such content can be trusted.

## Approach
1. **Requirements:** define the learner, the learning goals and the acceptance criteria ([01_requirements.md](01_requirements.md)).
2. **Content:** use an AI assistant to write short explanations and quiz questions on selected principles ([02_content/](02_content/)).
3. **Validation:** check every explanation and answer against the official text of the Code and log each error with its severity ([03_validation/error_log.csv](03_validation/error_log.csv)).
4. **Lessons learned:** summarise what the AI got wrong, why, and which controls would be needed in a real e-learning product ([04_lessons_learned.md](04_lessons_learned.md)).

The prompts used are documented in [prompts.md](prompts.md).

## Scope
Six principles from the **Execution** (11 Pre-Hedging, 14 Mark Up, 17 Last look) and **Information Sharing** (19 and 20 Confidential Information, 22 Market Colour) sections of the FX Global Code, version updated December 2024. The full Code is not reproduced here; it is published by the Global Foreign Exchange Committee (GFXC) at [globalfxc.org](https://www.globalfxc.org).

## Results
| | |
|---|---|
| Items validated | 6 explanations, 18 quiz questions |
| Errors found | 7: 0 High, 4 Medium, 3 Low |
| Wrong answer keys | 0 |
| Fixed in Run B (with source) | All Medium-severity items |

**Key findings**
- The main risk was not invented facts but **paraphrases that shift the meaning** and **omitted core conditions**.
- One misconception about Principles 19 and 20 appeared **systematically** in both runs.
- The AI's **self-flags of uncertainty helped but did not identify the actual errors**.
- With web search, the AI relied on **secondary sources and an outdated 2021 reference**, not on the current Code.
- **Providing the official text** fixed all Medium-severity errors.

Full details: [04_lessons_learned.md](04_lessons_learned.md)

## Why this project
I worked 11 years as an FX trader and led an FX Global Code project at Erste Group Bank with around 20 stakeholders from Compliance, Legal, Trading and Technology. This project combines that subject knowledge with requirements, testing and AI, and shows how I validate AI output before using it.

_No internal or confidential material from any former employer is used in this project._
