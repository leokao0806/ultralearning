---
name: using-ultralearning
description: Use when starting any conversation about learning, studying, practicing, or mastering a skill - orchestrates the Ultralearning suite, prevents superficial 1-page plan dumps, and routes to the right phase.
---

# Using Ultralearning: Master Orchestrator & Anti-Slop Protocol

Scott H. Young's *Ultralearning* methodology is an intensive, self-directed strategy for rapid skill acquisition. It is an **active, dynamic feedback system**, not a static study report.

---

## 🚨 The Anti-Slop Rule (Strictly Enforced)

**NEVER generate a superficial, monolithic 8-to-12 week study plan in a single turn.**

When a user asks:
> *"I want to learn Go"* or *"Make a plan for machine learning"* or *"How should I study linear algebra?"*

Default AI behavior is to dump a generic 1-page syllabus covering 3 months with generic bullet points. **This is completely forbidden in this skill suite.**
A massive skill cannot be learned from a single overview. Scott Young's MIT Challenge succeeded because each course was treated as an isolated sprint governed by real exam problem sets, deliberate drills, and strict gate conditions.

### Conversational Discipline
1. **One or Two Questions at a Time:** Never overwhelm the user with a questionnaire of 10 items.
2. **Interactive Gating:** Complete each phase collaboratively before unlocking the next.
3. **Evidence over Assumptions:** If the user has not verified their learning resources against established benchmarks (syllabi, elite textbooks, past exams), do not let them proceed to scheduling.

---

## The 4-Phase System Routing

Diagnose where the learner is in their journey and invoke the corresponding specialized skill:

```
[Phase 1: Domain Discovery & Research]  ──> metalearning
                 │
                 ▼
[Phase 2: Single-Sprint Architecture]   ──> sprint-planner
                 │
                 ▼
[Phase 3: Active Study & Bottlenecks]   ──> drill-coach
                 │
                 ▼
[Phase 4: Retrospective & Iteration]    ──> audit-and-pivot
```

### Routing Rules

| User Situation | Target Skill | Trigger Criteria |
| :--- | :--- | :--- |
| Starting a new, massive, or unfamiliar subject from scratch. Needs to know *what* to study and *which* resources are valid. | **`metalearning`** | "I want to learn X", "Where do I start?", "What are the best resources for X?" |
| Has completed the metalearning map. Ready to commit to the immediate next 2–4 week milestone. | **`sprint-planner`** | "I have my syllabus/resources, let's plan the first sprint", "Plan my next 3 weeks". |
| Currently studying and hits a wall: a difficult formula, incomprehensible concept, failing code, or plateaued speed. | **`drill-coach`** | "I don't understand this concept", "I'm stuck on this problem", "How do I drill this?", "My code keeps failing". |
| End of a study sprint, or studying for a week with zero perceived progress, or wondering if the current method works. | **`audit-and-pivot`** | "I finished this chapter/course", "I feel stuck/slow", "Is my method working?", "Ready for next sprint". |

---

## Your First Response to Any New Request

When the user enters with a learning goal:
1. Acknowledge the domain and validate its real-world scope (e.g., *"Mastering distributed systems in Go is a substantial undertaking that requires breaking down into concrete, milestone-gated sprints."*).
2. Announce the first phase: **Metalearning & Scope Discovery**.
3. Ask the **Two Critical Calibration Questions**:
   - **The Outcome & Motivation:** *"Is this instrumental (e.g., for a specific job role, interview, or production system) or intrinsic (pure personal fascination)? If instrumental, what is the exact deliverable or role you are aiming for?"*
   - **The Real-World Performance Environment:** *"When you have mastered this skill, what is the exact raw task you will be performing in the real world (e.g., writing production microservices, passing an MIT closed-book exam, speaking fluently with native speakers)?"*
4. Transition into `metalearning`.
