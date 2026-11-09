---
name: audit-and-pivot
description: Use weekly or when hitting plateaus - measures rate-of-learning, tests for illusion of competence, checks 80/20 difficulty sweet spot, and executes experiments (resource pivot, A/B methods, constraint imposition).
---

# Audit & Pivot: Calibration, Verification & Strategic Experimentation

Ultralearning is not stubborn adherence to a failing plan. Scott Young's MIT Challenge and language sprints required dynamic, aggressive course correction whenever the **marginal rate of return** began to diminish.

Use this skill at two mandatory junctures:
1. **The Weekly Retrospective:** A 15-minute diagnostic at the end of each study week.
2. **The Sprint Gate Certification:** Evaluating whether the Gate Condition was met before unlocking the next sprint.

---

## Part 1: The Diagnostic Audit Matrix

Conduct this audit with the learner. Review their logged hours and actual outputs against these four diagnostic tests:

### Test 1: The Rate-of-Learning Velocity Check
* **Diagnostic Question:** *"Has the rate of new comprehension or problem-solving speed noticeably flattened over the last 5–7 days?"*
* **Analysis:** If the learner is putting in hours but progress has ground to near zero, continuing the current method is futile (Diminishing Marginal Utility). A tactical pivot is mandatory.

### Test 2: The Directness Ratio Check (Principle 3)
* **Diagnostic Question:** *"Of the hours logged this week, what exact percentage was spent directly producing the artifact or writing closed-book solutions vs. passively reading or watching videos?"*
* **Passing Threshold:** $\ge 60\%$ direct practice.
* **Failure Flag:** If $< 50\%$ direct practice, the learner has slipped into **passive proxy learning (Tutorial Hell)**. Prescribe an immediate total ban on video/text reading for 3 days.

### Test 3: The Illusion-of-Competence Audit (Principle 5)
* **Diagnostic Question:** *"Can you reproduce the core concepts or solve standard exercises on a blank piece of paper with all references closed?"*
* **Failure Flag:** If the learner understands while looking at notes but fails when closed-book, they are suffering from recognition bias rather than recall mastery. Prescribe immediate **Free Recall / Question-Book** drills.

### Test 4: The 80/20 Difficulty Sweet Spot Check (Principle 6)
* **Diagnostic Question:** *"What percentage of your practice attempts resulted in errors or friction?"*
* **Calibration:**
  * If error rate $< 10\%$: Practice is too easy. Raise difficulty or introduce time limits.
  * If error rate $> 40\%$: Cognitive overload. Break down into atomic components via `drill-coach`.
  * Sweet spot: $15\% - 25\%$ error rate.

---

## Part 2: Strategic Experimentation (Principle 9: When to Pivot)

If the audit detects stagnation or diminishing returns, execute one of these structured experiments:

### 1. The Resource Pivot
If a primary textbook or course has produced diminishing returns after 10–15 hours of sincere effort, **drop it immediately**.
* Return to the benchmark list compiled in `metalearning`.
* Select an alternate pedagogical source with a different cognitive style (e.g., transition from an abstract mathematical text to an implementation-first book, like moving from Tanenbaum to *Beej's Guide to Network Programming*).

### 2. The Technique A/B Test
Run a controlled 3-day split test:
* Divide target concepts or problem sets into Group A and Group B.
* Apply Strategy 1 (e.g., Anki spaced flashcards) to Group A.
* Apply Strategy 2 (e.g., Free recall + Feynman diagrams) to Group B.
* Measure retention on day 4 closed-book; double down on the winning strategy.

### 3. Introduce Novel Constraints
Best performance breakthroughs occur within tight boundaries:
* **Tool Constraints:** Write the system without using third-party packages or standard helper libraries.
* **Time Constraints:** Cut exercise time limits by 50% to force pattern recognition.
* **Format Constraints:** Explain or sketch system state machines exclusively on a whiteboard without IDE tools.

---

## Part 3: The Sprint Gate Evaluation Protocol

When a learner completes the scheduled weeks of a Sprint:

1. **Evaluate the Gate Condition defined in `sprint-planner`:**
   - Did the test suite achieve the required pass rate?
   - Did the closed-book exam meet the target percentage ($\ge 80\%$)?
   - Was the direct artifact deployed and validated?
2. **The Verdict:**
   - **PASS:** Formally certify completion. Document lessons learned. Invoke `sprint-planner` to architect Sprint $N+1$.
   - **FAIL / INCOMPLETE:** Do NOT allow progression to the next sprint. Identify the failing subsystem, schedule a 3-to-5 day targeted remediation sprint via `drill-coach`, and re-test.
