# Requirements: FX Global Code Learning Module

## 1. User and need
| Item | Description |
|---|---|
| Primary user | A junior FX trader, sales person or supervisor who is new to the FX Global Code |
| Need | Understand the key principles on execution and information sharing in about 30 minutes |
| Context | Self-study, on screen, no prior knowledge of the Code assumed |

## 2. Learning goals
After the module, the learner can:
1. Explain in their own words what each selected principle requires.
2. Recognise in a short practical scenario whether conduct is in line with the Code.
3. Name where to find the official text for further detail.

## 3. Scope
- **In scope:** Principles 11, 14 and 17 (Execution) and 19, 20 and 22 (Information Sharing) of the FX Global Code, version updated December 2024.
- **Out of scope:** the full Code, legal interpretation, firm-specific policies.

## 4. Deliverables
| # | Deliverable | Format |
|---|---|---|
| D1 | One short explanation per principle (max. 150 words) | Markdown |
| D2 | 2–3 multiple-choice questions per principle, with answer and explanation | Markdown |
| D3 | Error log of the validation | CSV |
| D4 | Lessons learned | Markdown |

## 5. Acceptance criteria
| ID | Criterion |
|---|---|
| AC1 | Every explanation is consistent with the official text of the Code; no statement goes beyond it. |
| AC2 | Every quiz question has exactly one correct answer, which can be traced to the Code's text. |
| AC3 | Wrong answer options are plausible but clearly wrong according to the Code. |
| AC4 | The language is plain English, understandable without prior knowledge. |
| AC5 | Every error found is logged with ID, item, description, severity and fix. |
| AC6 | No item with a "High" severity error remains unfixed in the final version. |

## 6. Severity levels for the error log
| Severity | Definition | Example |
|---|---|---|
| High | Factually wrong or misleading about what the Code requires | The AI states a practice is prohibited when the Code allows it under conditions |
| Medium | Incomplete or imprecise in a way that could confuse the learner | A key condition of a principle is missing |
| Low | Wording, style or clarity issue | Jargon not explained |

## 7. Risks
- **Hallucination:** the AI invents requirements or principle numbers that do not exist.
- **Overstatement:** the AI presents the Code as law; it is a voluntary set of principles.
- **Outdated version:** the AI relies on an earlier version of the Code.
