---
name: metalearning
description: Use before starting any new learning domain - conducts deep interview on motivation, executes syllabus benchmarking (MIT OCW, authoritative textbooks), CFP decomposition, and ruthless exclusion.
---

# Metalearning: Domain Discovery & Curriculum Reverse-Engineering

Metalearning is drawing the map before setting off. Without rigorous metalearning, learners waste dozens of hours reading outdated tutorials, studying irrelevant subfields, or falling into the illusion of progress.

**Do not write a weekly calendar in this skill.** This skill produces only one artifact: the **Metalearning Map Canvas**. Once completed and approved by the user, route to `sprint-planner`.

---

## The Interactive Protocol (Step-by-Step)

Work through these 5 steps with the user collaboratively. **Do not execute all steps in one message.**

```
[Step 1: Motivation & Target Environment]
                   │
                   ▼
[Step 2: The 10% Research Budget]
                   │
                   ▼
[Step 3: Curriculum Benchmarking]
                   │
                   ▼
[Step 4: The CFP Decomposition]
                   │
                   ▼
[Step 5: Ruthless Emphasize / Exclude]
                   │
                   ▼
[Artifact: Metalearning Map Canvas] ──> handoff to sprint-planner
```

---

### Step 1: Motivation & Target Environment Verification
Ask the user:
1. **Instrumental vs. Intrinsic:**
   - *If Instrumental:* What specific job, promotion, exam, or commercial deliverable requires this? Have you verified that this skill actually produces that outcome (e.g., analyzed real job listings or talked to a senior engineer)?
   - *If Intrinsic:* What specific aesthetic, intellectual, or personal curiosity drives you?
2. **Direct Environment (Principle 3):**
   - What will the real-world performance look like? (e.g., *"I will sit at an empty terminal and build a distributed key-value store without looking at tutorials"* vs. *"I will read a book on Go"*).

*Wait for user response before proceeding to Step 2.*

---

### Step 2: The 10% Research Budget
Establish the quantitative scope:
* Calculate: $\text{Total Hours} = \text{Target Weeks} \times \text{Hours/Week}$.
* The **10% Rule:** You are allocated exactly $10\%$ of total project time for upfront curriculum investigation and resource scouting.
  * *Example:* For a 100-hour commitment (10 hrs/week for 10 weeks), research is capped at 10 hours.
* **Diminishing Returns Warning:** Researching beyond 10% is procrastination disguised as preparation. Once a viable canonical syllabus is found, research must stop.

---

### Step 3: Curriculum Benchmarking (Reverse-Engineering)
Do not improvise a learning path from random blog posts. Establish an authoritative **Benchmark Standard**:
* **Academic standard:** Top university syllabus (MIT OpenCourseWare, Stanford CS, Berkeley EECS).
* **Industry/Practitioner standard:** The gold-standard textbook and its official problem sets (e.g., *Designing Data-Intensive Applications* by Kleppmann; *Operating Systems: Three Easy Pieces*).
* **Direct Project standard:** A canonical open-source project or challenge repo (e.g., Build Your Own Redis, MIT 6.824 Lab assignments).

*Review candidate resources with the user and select exactly ONE primary textbook/syllabus and ONE primary practical assignment suite.*

---

### Step 4: The CFP Decomposition (Concepts, Facts, Procedures)
Deconstruct the target subject into three distinct cognitive buckets:

| Category | What It Is | How It Must Be Mastered | Examples in Computer Science |
| :--- | :--- | :--- | :--- |
| **Concepts** | Ideas and relational mental models that must be *understood deeply*. | Feynman Technique, first-principles derivation, concrete-to-abstract analogizing. | Virtual memory, Raft consensus, closures, pointers, relational normalization. |
| **Facts** | Discrete arbitrary information that must be *memorized*. | Anki / Spaced Repetition Systems (SRS), atomic cards. | CLI flags, standard library API methods, HTTP status codes, syntax rules. |
| **Procedures** | Physical or mental actions that must become *automatic*. | Deliberate drills, time-slicing, high-repetition feedback. | Debugging with GDB/pprof, writing unit tests, refactoring, touch-typing syntax. |

*Collaboratively brainstorm the CFP items with the user.*

---

### Step 5: Ruthless Emphasize / Exclude (The 80/20 Knife)
The biggest mistake in learning is trying to learn everything. Ask the user:
1. **Emphasize (Core 20%):** Which subskills directly enable building the primary direct deliverable?
2. **Exclude (The Noise 80%):** Which modules, theoretical tangents, legacy tools, or nice-to-haves will be **strictly forbidden** during this project?

---

## Output Artifact: `metalearning-canvas.md`

Synthesize the findings into an artifact in the user's workspace or brain:

```markdown
# Metalearning Map: [Domain Name]

## 1. Parameters & Motivation
- **Type:** Instrumental / Intrinsic
- **Direct Target Artifact:** [Measurable real-world output]
- **Time Commitment:** [X] Total Hours | Research Budget (10%): [X] Hours

## 2. Benchmark Curriculum & Primary Resources
- **Benchmark Source:** [MIT OCW / Canonical Book / Exam]
- **Primary Textbook/Guide:** [Title & Author]
- **Primary Practice Ground:** [Repo / Lab suite / Problem set]

## 3. CFP Breakdown
- **Core Concepts (Feynman):** [Item 1, Item 2, Item 3]
- **Core Facts (Anki/SRS):** [Item 1, Item 2, Item 3]
- **Core Procedures (Drill):** [Item 1, Item 2, Item 3]

## 4. Strategic Scope
- **Emphasize (Priority Focus):** [2-3 high-leverage areas]
- **Exclude (Banned from Scope):** [Explicitly skipped modules]
```

Once the user approves this canvas, invoke **`sprint-planner`** to architect Sprint 1.
