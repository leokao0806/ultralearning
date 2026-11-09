<p align="center">
  <img src="assets/logo.png" width="120" height="120" alt="Ultralearning Logo">
</p>

<h1 align="center">⚡ Ultralearning</h1>

<p align="center">
  <strong>A modular skills framework bringing Scott Young's Ultralearning methodology to AI coding agents.</strong>
</p>

<p align="center">
  <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License: MIT"></a>
  <a href="https://github.com/leokao0806/ultralearning"><img src="https://img.shields.io/badge/Agents-Claude%20Code%20|%20Antigravity%20|%20Cursor%20|%20Codex-success" alt="Supported Agents"></a>
</p>

> [!NOTE]
> **Attribution:** This project is an open-source AI agent skill suite implementation of the **Ultralearning** framework created by **Scott H. Young** in his book *[Ultralearning: Master Hard Skills, Outsmart the Competition, and Accelerate Your Career](https://www.scotthyoung.com/blog/ultralearning/)* (Harper Business, 2019). All core pedagogical principles and methodologies are the intellectual work of Scott H. Young.

---

## 🛑 Why Traditional AI Study Plans Fail

Most AI assistants fail miserably at learning plans because they are built as **passive report generators**:
* You ask: *"I want to learn Go and distributed systems."*
* The AI immediately dumps a generic, superficial 12-week bulleted list in 5 seconds.
* It assumes learning is linear, ignores prerequisites, includes zero verification, and offers no mechanism when you hit an inevitable plateau.

**Real Ultralearning is a dynamic, high-rigor discipline.** Scott Young didn't conquer the 4-year MIT Computer Science curriculum in 12 months by reading a 1-page syllabus—he tackled it **one course at a time**, anchored by official final exams, aggressive feedback, deliberate drills, and continuous methodological pivots.

Modeled after the modular philosophy of [Superpowers](https://github.com/obra/superpowers), this framework splits learning into **5 interactive, specialized skills** with strict conversational gating.

---

## 🧩 The 5 Modular Skills

```text
                               ┌─────────────────────────────┐
                               │     using-ultralearning     │
                               │  (Master Orchestrator /     │
                               │   Anti-Slop Gatekeeper)     │
                               └──────────────┬──────────────┘
                                              │
                 ┌────────────────────────────┼────────────────────────────┐
                 ▼                            ▼                            ▼
   ┌───────────────────────────┐┌───────────────────────────┐┌───────────────────────────┐
   │       metalearning        ││      sprint-planner       ││        drill-coach        │
   │  (Domain Discovery &      ││  (Single-Sprint Plan &    ││  (Bottleneck Isolation &  │
   │   Reverse Engineering)    ││   Gate Architecture)      ││   Feynman Sparring)       │
   │  - Deep motivation verify ││  - Max 2-4 week horizon   ││  - 15-min struggle timer  │
   │  - 10% research budget    ││  - Concrete textbook/labs ││  - Socratic Feynman test  │
   │  - CFP decomposition      ││  - Pass/Fail Gate check   ││  - 5 deliberate drill types│
   │  - Ruthless 80/20 pruning ││  - Daily deep work blocks ││  - Rate-limiting bottleneck│
   └───────────────────────────┘└───────────────────────────┘└───────────────────────────┘
                                              │
                                              ▼
                               ┌─────────────────────────────┐
                               │       audit-and-pivot       │
                               │  (Velocity Audit, Sweet     │
                               │   Spot & Strategic Pivot)   │
                               │  - Learning rate check      │
                               │  - 80/20 difficulty balance │
                               │  - Resource / A-B pivots    │
                               │  - Gate evaluation          │
                               └─────────────────────────────┘
```

### 1. `using-ultralearning` (The Root Orchestrator)
* **The Anti-Slop Rule:** Strictly forbids dumping monolithic plans.
* Diagnoses where you are in your journey and routes you to the correct phase.
* Enforces back-and-forth conversational discipline (1-2 questions at a time).

### 2. `metalearning` (Phase 1: Reverse-Engineering the Map)
* **Deep Motivation Calibration:** Distinguishes instrumental (career/exam) from intrinsic goals.
* **The 10% Rule:** Allocates exactly 10% of total project hours to upfront syllabus and benchmark research.
* **Curriculum Benchmarking:** Reverse-engineers elite university syllabi (MIT OCW, Stanford) or canonical textbooks.
* **CFP Analysis:** Deconstructs the domain into **Concepts** (to understand), **Facts** (to memorize via Anki/SRS), and **Procedures** (to drill).
* **Ruthless Exclusion:** Identifies the 20% core and explicitly bans the 80% secondary noise.

### 3. `sprint-planner` (Phase 2: Granular Milestone Architecture)
* **The Horizon Limit:** Plans **only ONE sprint** at a time (2 to 4 weeks).
* **Direct Performance Anchor:** At least 60% of time must be hands-on artifact creation, not reading.
* **The Strict Gate Condition:** Defines an objective, pass/fail test (e.g., scoring $\ge 80\%$ on a closed-book past exam, or passing 100% of network partition unit tests). You cannot advance to Sprint 2 until Sprint 1's gate is certified.

### 4. `drill-coach` (Phase 3: The Bottleneck Elimination Engine)
* **The 15-Minute Struggle Rule:** Forbids giving direct answers until you have actively struggled for 15 minutes.
* **Interactive Feynman Sparring:** Roleplays as an inquisitive 10-year-old child; catches technical jargon and forces plain-language analogies until intuition is rock-solid.
* **5 Deliberate Drill Archetypes:** Time-slicing, cognitive component isolation, the copycat method, the magnifying glass, and prerequisite chaining.

### 5. `audit-and-pivot` (Phase 4: Calibration & Strategic Experimentation)
* **Rate-of-Learning Check:** Detects when your progress velocity approaches zero (diminishing marginal returns).
* **Illusion-of-Competence Audit:** Tests whether you can reproduce knowledge on blank paper with all books closed.
* **Difficulty Sweet Spot:** Calibrates tasks to maintain the 80% success / 20% error zone.
* **Strategic Pivots:** Replaces ineffective textbooks, runs A/B learning strategy experiments, or imposes new artificial constraints.

---

## 🚀 Installation

Install across any major AI Agent runtime:

### 1. Antigravity (Google / Gemini)
Install the plugin directly via the CLI:
```bash
agy plugin install https://github.com/leokao0806/ultralearning
```

### 2. Claude Code
Install as a plugin:
```bash
/plugin install leokao0806/ultralearning
```
*Or clone into local skills:*
```bash
git clone https://github.com/leokao0806/ultralearning.git ~/.claude/skills/ultralearning
```

### 3. Cursor
Clone into your project's agent skills:
```bash
git clone https://github.com/leokao0806/ultralearning.git .agents/skills/ultralearning
```

### 4. OpenAI Codex / Other Agents
Clone into the universal cross-runtime skills directory:
```bash
git clone https://github.com/leokao0806/ultralearning.git ~/.agents/skills/ultralearning
```

---

## 💬 How to Use: A Real-World Walkthrough

### Scenario 1: Starting a Massive New Skill
You tell your agent:
> *"I want to master Go and distributed systems using ultralearning."*

* **Bad Agent:** Dumps 12 bulleted weeks of topics in one message.
* **Ultralearning Agent (`using-ultralearning`):**
  1. Acknowledges the scale of the domain.
  2. Invokes `metalearning`.
  3. Asks: *"Is this for a specific backend engineering role or personal curiosity? What exact production system do you want to build at the end?"*
  4. Once answered, guides you through benchmarking (e.g., MIT 6.824 syllabus), CFP decomposition, and 10% research budgeting.
  5. Produces the `metalearning-canvas.md` before routing to `sprint-planner`.

### Scenario 2: Planning the First Sprint
Once the map is approved:
* Agent invokes `sprint-planner`.
* Plans **only Sprint 1 (2 weeks)**:
  * Readings: *The Go Programming Language, Ch 1–4*.
  * Direct Deliverable: A concurrent TCP chat server with heartbeat protocols.
  * Gate Condition: Closed-book implementation of the server passing an automated stress test with 500 concurrent connections.
* Generates `sprint-contract-sprint-1.md`.

### Scenario 3: Hitting a Wall Mid-Study
During Week 1, you get stuck on Go channels and race conditions:
> *"I don't understand CSP and channel select statements. My code keeps deadlocking."*

* Agent invokes `drill-coach`.
* Enforces the **15-minute Struggle Timer**.
* Runs the **Interactive Feynman Test**: *"Explain channel deadlocks to me like I'm 10 years old. No CS jargon allowed."*
* Catches your hand-waving and designs an isolated **Cognitive Component Drill**: 5 synthetic deadlock puzzles on paper.

### Scenario 4: Weekly Review & Milestone Certification
At the end of Sprint 1:
> *"I finished Sprint 1, let's see where I stand."*

* Agent invokes `audit-and-pivot`.
* Runs the 4 diagnostic tests: Directness ratio, closed-book test, rate of learning, and error rate sweet spot.
* Tests the Gate Condition:
  * If passed $\longrightarrow$ Certifies milestone and triggers `sprint-planner` for Sprint 2.
  * If failed $\longrightarrow$ Diagnoses the failure mode and designs a 3-day targeted remediation drill before allowing you to proceed.

---

## 📚 Attribution & Acknowledgments

This project is an open-source AI agent implementation inspired by and built directly upon the methodology developed by **Scott H. Young** in his bestselling book:

> **[*Ultralearning: Master Hard Skills, Outsmart the Competition, and Accelerate Your Career*](https://www.scotthyoung.com/blog/ultralearning/)**  
> by Scott H. Young (Harper Business, 2019)

All core pedagogical concepts, the 9 principles, and project structuring techniques are the intellectual work of Scott H. Young. This repository serves as an operational translation that equips autonomous AI coding agents to act as ultralearning coaches and curriculum architects for human learners.

We strongly encourage everyone using this skill to purchase and read the original book!

---

## 📄 License

MIT License © 2026 [Leo Kao](https://github.com/leokao0806). Feel free to adapt and share!
