---
name: sprint-planner
description: Use to plan a focused 2-4 week learning sprint - defines exact chapters/lectures, direct practice artifacts, daily deep work blocks, and strict pass/fail gate conditions.
---

# Sprint Planner: Granular Milestone Architecture

In ultralearning, **you never plan a 6-month journey in detail.** Learning velocity is non-linear: you will encounter unforeseen roadblocks and unexpected breakthroughs. 

Sprint Planner schedules **exactly one sprint at a time (typically 2 to 4 weeks)** with relentless precision. Future sprints remain rough placeholders until the current sprint's Gate Condition is passed.

---

## The 4 Golden Rules of an Ultralearning Sprint

1. **The Horizon Limit:** Maximum 4 weeks. Standard is 2 to 3 weeks.
2. **The Direct Performance Anchor (Principle 3):** At least 60% of all hours must be spent directly building, coding, translating, or solving problems without notes—not passively reading or watching videos.
3. **The Unambiguous Gate Condition:** The sprint CANNOT conclude based on "time spent." It must conclude with an objective, pass/fail evaluation (e.g., *"Score $\ge 80\%$ on MIT 6.824 Lab 2 tests"* or *"Complete 20 dynamic programming problems closed-book in under 20 minutes each"*).
4. **No Gate, No Next Sprint:** If the learner fails the gate, they do NOT move to Sprint 2. They invoke `drill-coach` or `audit-and-pivot` to troubleshoot and re-test.

---

## Interactive Planning Workflow

Work through these steps with the user:

### Step 1: Sprint Scope & Deliverable Definition
Ask the user:
* **Sprint Name & Number:** (e.g., *Sprint 1: Concurrency Primitives & Network Protocols*).
* **Duration:** (e.g., 2 weeks, 15 hours/week = 30 hours).
* **The Single Direct Deliverable:** What exact functioning artifact or test paper proves this sprint was mastered?

### Step 2: Resource Assignment (Down to the Chapter/Lab)
Demand extreme specificity. Reject vague inputs like *"study networking"*:
* Book: Exactly which chapters? (e.g., *Tanenbaum Computer Networks, Chapters 3.1–3.4*)
* Lectures: Exactly which video/audio numbers?
* Problem sets: Exactly which problems (e.g., *Exercises 12, 15, 18, 22*)?

### Step 3: Define the Gate Condition (Milestone Test)
Formulate the exact pass/fail criteria:
* **Type A (Project / Code):** Public GitHub repository with CI passing 100% of automated integration tests under network partition simulations.
* **Type B (Exam / Problem Set):** Closed-book timed test from a historical university final exam with passing score $\ge 80\%$.
* **Type C (Performance):** Recorded uninterrupted 15-minute dialogue with a native tutor strictly in the target language.

### Step 4: Schedule Deep Work Blocks
Map the hours into concrete weekly slots:
* Schedule 90–120 minute high-focus blocks.
* Match cognitive arousal to difficulty (Yerkes-Dodson): Quiet environment, zero notifications for abstract conceptual work; energetic music allowed for repetitive syntax/drills.
* Enforce the **5-Minute Rule** for days with high starting friction.

---

## Output Artifact: `sprint-contract-sprint-[N].md`

Generate the formal contract for the user:

```markdown
# 📋 Ultralearning Sprint Contract: Sprint [N]

> **Focus Domain:** [Domain]  
> **Sprint Horizon:** [Start Date] ──> [Target End Date] ([X] Weeks)  
> **Total Committed Hours:** [X] Hours ([X] hrs/week)  

---

## 1. Primary Direct Deliverable
* **Target Output:** [e.g., A concurrent HTTP/1.1 file server supporting range requests and connection pooling built in raw Go with zero third-party dependencies.]

---

## 2. Granular Learning Curriculum
* **Primary Reading:** [Textbook name, exact chapters]
* **Primary Lectures/Codebases:** [Exact URLs, repos, or lab assignments]
* **Closed-Book Problem Sets:** [Specific problem numbers to solve without checking solutions]

---

## 3. Strict Gate Condition (Pass/Fail)
> ⚠️ **You cannot begin Sprint [N+1] until this gate is certified.**
* **Evaluation Standard:** [Exact test, benchmark, or exam]
* **Passing Threshold:** [Score, test suite pass rate, or mentor sign-off]
* **Verification Method:** [Closed-book simulation / public deployment verification]

---

## 4. Weekly Execution Blocks

### Week 1 ([Date] - [Date])
* **Block 1 (Mon 07:00-09:00):** [Exact task]
* **Block 2 (Tue 07:00-09:00):** [Exact task]
* **Block 3 (Wed 07:00-09:00):** [Exact task]
* **Block 4 (Thu 07:00-09:00):** [Exact task]
* **Block 5 (Sat 09:00-12:00):** [Mid-sprint direct implementation milestone]

### Week 2 ([Date] - [Date])
* [Follow same structure, ending with the Gate Evaluation session]

---

## 5. Daily Active Protocols
* **Retrieval Protocol:** Notes taken exclusively as Question-Book items. Daily 15-minute Anki review before starting new material.
* **Struggle Protocol:** Minimum 15-minute struggle timer before consulting hints, docs, or solutions.
```

When Sprint execution begins, if the user hits an impassable bottleneck or mental roadblock, invoke **`drill-coach`**.  
At the end of the sprint, invoke **`audit-and-pivot`** to review results and certify the gate.
