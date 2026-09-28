# AI Model Restriction & Logging Instructions

> **[REQUIRED CONFIGURATION FOR USER]**  
> **TARGET_MODEL_NAME:** `Claude Opus 5.5`  
> **STRICT_MODE:** `ENABLED`

---

## 1. Strict Model Enforcement Protocol

### Rule 1.1: Assigned Model Usage Only

- The AI **MUST ONLY** use the model specified in the `TARGET_MODEL_NAME` configuration field above.
- The AI is **STRICTLY FORBIDDEN** from switching to or delegating sub-tasks to any other model or smaller fallback variants unless explicitly authorized by the user in writing.
- If the AI detects an automatic model downgrade or switch during execution, it must log an alert in the performance log and flag the mismatch to the user.

---

## 2. Mandatory Output Requirement: `DEVELOPMENT_LOG.md`

Along with the generated project files, the AI **MUST** create and output a separate file named `DEVELOPMENT_LOG.md` inside the project root directory.

---

## 3. Structure & Contents of `DEVELOPMENT_LOG.md`

The generated log file must strictly follow this markdown structure:

```markdown
# Project AI Execution & Model Performance Log

## 1. Model Metadata

- **Assigned Model Name:** [Exact value from TARGET_MODEL_NAME configuration]
- **Execution Model Version / Snapshot:** [Insert Version/Build ID if available]
- **Execution Date & Time:** [Insert Timestamp]
- **Enforcement Status:** [Pass (Only assigned model was used) / Warning (Model mismatch detected)]

---

## 2. Model Selection & Rationale

- **Primary Reason for Model Assignment:** Explaining why this model was specified for this task (e.g., strong code generation abilities, precise UI styling capabilities).
- **Task Alignment:** How the model handled complex UI animations and mathematical logic.

---

## 3. Model Performance Metrics Over Time

| Phase   | Sub-Task                              | Latency / Time Taken | Accuracy / Output Quality | Tokens Used (Est.) | Issues / Errors Encountered |
| :------ | :------------------------------------ | :------------------- | :------------------------ | :----------------- | :-------------------------- |
| Phase 1 | UI Layout & CSS Keyframes             | [Time]               | [High/Med/Low]            | ~[Token Count]     | [None / Description]        |
| Phase 2 | JS Logic & Math Engine                | [Time]               | [High/Med/Low]            | ~[Token Count]     | [None / Description]        |
| Phase 3 | Keyboard Mapping & Micro-interactions | [Time]               | [High/Med/Low]            | ~[Token Count]     | [None / Description]        |

---

## 4. Execution Decisions & Architectural Rationale

- **Decision 1:** [Why a specific CSS animation approach was chosen]
- **Decision 2:** [How floating-point precision was handled in math execution]
- **Decision 3:** [Layout strategy chosen for responsive display]

---

## 5. Model Performance Summary

- **Strengths Demonstrated:** [Key highlights of model execution]
- **Weaknesses / Bottlenecks:** [Any areas where code needed self-correction]
- **Final Evaluation Score:** [Self-assessment score out of 10 for model output quality]
```

---

## 4. Final Delivery Checklist

When delivering the final solution, the AI must provide:

1. The completed project source files (`index.html`, `styles.css`, `script.js` OR single app file).
2. The standalone `DEVELOPMENT_LOG.md` file populated with real metadata from the build session.
