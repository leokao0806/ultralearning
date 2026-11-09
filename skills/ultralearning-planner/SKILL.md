---
name: ultralearning-planner
description: Use when the user wants to design, structure, audit, or optimize an intensive, self-directed learning plan or study project using Scott Young's Ultralearning framework and cognitive science principles.
---

# Ultralearning Planner

An operational engine for designing aggressive, self-directed learning projects based on Scott H. Young's *Ultralearning* methodology and empirical cognitive science (Karpicke, Roediger, Bjork, Ericsson).

This skill guides you through transforming vague learning desires (e.g., "I want to learn machine learning") into an actionable, high-velocity blueprint built around direct practice, cognitive decomposition, active retrieval, and deliberate drill.

---

## Core Planning Workflow

Follow this 6-phase sequence when consulting with a learner:

```
[Phase 1: Project Intake & Goal Calibration]
                │
                ▼
[Phase 2: Metalearning & CFP Decomposition]
                │
                ▼
[Phase 3: Directness & Drill Engine Design]
                │
                ▼
[Phase 4: Retrieval, Retention & Feedback Systems]
                │
                ▼
[Phase 5: Blueprint Generation & Schedule Assembly]
                │
                ▼
[Phase 6: Mid-Project Audit & Bottleneck Triage]
```

---

## Phase 1: Project Intake & Goal Calibration

Extract clear parameters before designing the curriculum. If the user's initial prompt is broad, ask targeted diagnostic questions to clarify:

1. **Specific Measurable Target:**
   - Reject generic goals: *"I want to learn Rust."*
   - Require tangible outcomes: *"Build an in-memory distributed key-value store with Raft consensus in Rust that passes Jepsen partition tests."*
2. **Motivation Classification:**
   - **Instrumental (Functional):** Driven by career pivot, job promotion, or exam qualification. Mandate early validation: has the user verified that acquiring this specific skill will yield the desired career payoff?
   - **Intrinsic (Essential):** Driven by intellectual curiosity or personal fulfillment. Prioritize personal interest over external industry standards.
3. **Time Budget & Constraints:**
   - Define exact timeframe: Start date, end date, and hours per week.
   - Calculate total project hours ($H = \text{weeks} \times \text{hours/week}$).
   - Enforce the **10% Metalearning Rule**: Dedicate $0.10 \times H$ to upfront research, curriculum mapping, and benchmark comparison before starting active practice.

---

## Phase 2: Metalearning & CFP Decomposition

Deconstruct the target subject using the **Concepts, Facts, Procedures (CFP)** framework. Refer to [references/principles-deep-dive.md](./references/principles-deep-dive.md#1-metalearning-first-draw-a-map) for theoretical details.

### 1. Build the CFP Matrix
* **Concepts (To Understand):** Mental models, relational logic, and theories requiring deep semantic integration. 
  * *Strategy:* Feynman Technique, conceptual proofs, derivation from first principles.
* **Facts (To Memorize):** Discrete units of arbitrary information (syntax, commands, terms, constants, formulas).
  * *Strategy:* Spaced Repetition Systems (SRS / Anki), atomic flashcards, mnemonic encoding.
* **Procedures (To Practice):** Actions, algorithmic routines, and motor skills that must become automatic.
  * *Strategy:* Deliberate drill, high-repetition loops, time-slicing.

### 2. Benchmarking & Strategic Pruning
* **Benchmarking:** Reverse-engineer established curricula (e.g., top university course syllabi, standard reference textbooks, industry qualification standards).
* **Emphasize vs. Exclude:**
  * **Emphasize (The Core 20%):** Highlight the highest-leverage subskills directly required to build the target deliverable.
  * **Exclude (The Noise):** Ruthlessly cut modules, theoretical rabbit holes, and outdated topics that do not serve the immediate direct outcome.

---

## Phase 3: Direct Practice & Drill Engine Design

Ensure the learner does not hide in passive proxy learning (watching video lectures, rereading notes).

### 1. Establish the Direct Practice Vehicle
Choose the primary mode of direct practice:
* **Project-Based Learning:** Creating a functioning production artifact (app, paper, portfolio, musical piece).
* **Immersive Environment:** Total immersion where secondary crutches are removed.
* **Flight Simulator:** High-fidelity simulated environments mirroring real-world constraints when direct execution is costly.
* **The Overkill Standard:** Raising the performance bar above normal baseline (e.g., presenting publicly, timed competition).

### 2. Map the Direct-Then-Drill Bottleneck Loops
Identify anticipated bottlenecks and match them with tactical drill types:
* **Time Slicing:** Isolate the single hardest micro-sequence and repeat it until frictionless.
* **Cognitive Component Isolation:** Drill a single cognitive layer (e.g., syntax drills without architectural design; pronunciation without grammar).
* **The Copycat:** Clone a master reference for 90% of the work to isolate and drill the remaining 10% creative component.
* **Prerequisite Chaining:** Tackle an advanced challenge; upon failure, step back one prerequisite link, drill it to fluency, and re-engage.

---

## Phase 4: Retrieval, Retention & Feedback Systems

Build the cognitive reinforcement architecture to defeat the forgetting curve and accelerate skill correction.

### 1. Retrieval Engine (Testing over Rereading)
* **The Question-Book Method:** Require notes to be recorded exclusively as questions with hidden answers, not descriptive summaries.
* **Closed-Book Sprints:** Ban documentation and AI assistants during the first attempt at solving a problem; force brain retrieval before consulting docs.
* **Free-Recall Audits:** Enforce a 5-minute blank-sheet recall session after every study block.

### 2. Long-Term Retention Protocols
* **Spacing:** Daily 15-minute SRS flashcard maintenance to prevent decay.
* **Proceduralization:** Convert high-friction tasks into recurring muscle memory workflows.
* **Overlearning:** Practice core procedures 50% beyond the point of initial mastery.

### 3. Feedback Loop Calibration
* Establish tight feedback loops across the **Feedback Triad**: Outcome (did it run?), Informational (what broke?), and Corrective (expert diagnosis).
* Calibrate task difficulty to maintain an **80/20 sweet spot** (80% success, 20% informative struggle).

---

## Phase 5: Blueprint Generation & Schedule Assembly

Synthesize the analysis into a formal project document using the template in [resources/project-blueprint-template.md](./resources/project-blueprint-template.md).

The generated output must include:
1. **Executive Summary & Scope:** Measurable target deliverable, timeline, total hours.
2. **Metalearning Map:** Full CFP decomposition table, benchmark sources, emphasize/exclude list.
3. **Direct Practice Specification:** Real-world deliverables, milestone deadlines.
4. **Targeted Drills & Bottleneck Protocols:** Isolated drill exercises for anticipated choke points.
5. **Retrieval & Retention Schedule:** Anki deck parameters, Question-Book structure, spacing intervals.
6. **Weekly Phase-by-Phase Roadmap:** Clear weekly breakdown of focus areas, hours, and direct milestones.

Provide the user with the weekly tracking template from [resources/weekly-execution-tracker.md](./resources/weekly-execution-tracker.md) to log deep work blocks, struggle timer breakthroughs, and weekly retrospectives.

---

## Phase 6: Mid-Project Audit & Bottleneck Triage

When a user reports struggles or plateaus during project execution, consult [references/troubleshooting-bottlenecks.md](./references/troubleshooting-bottlenecks.md) and execute the diagnostic protocol:

1. **Procrastination / Resistance:** Apply the 5-Minute Commitment Rule and micro-scaffolding. Calibrate arousal levels based on task complexity (Yerkes-Dodson).
2. **Illusion of Competence:** Check if the user is passively rereading or watching tutorials. Switch immediately to closed-book free recall and direct coding.
3. **Transfer Failure:** If the user excels at textbook problems but cannot build independently, replace practice exercises with end-to-end direct project building.
4. **Plateaus & Diminishing Returns:** Execute the Direct-Then-Drill cycle to isolate the rate-limiting step, or run an A/B experimentation sprint.
5. **Post-Project Decision:** Guide the user to choose between **Maintenance** (low-intensity spaced repetition), **Re-learning** (scheduled refresher sprints), or **Mastery** (advancing to unique personal style and edge experimentation).
