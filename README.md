# 🗂️ Slotwise Status Planner

![Status](https://img.shields.io/badge/status-archived-lightgrey)
![Type](https://img.shields.io/badge/type-web%20app-blue)
![Focus](https://img.shields.io/badge/focus-scheduling%20logic-orange)
![Stack](https://img.shields.io/badge/stack-vanilla%20JS%20%7C%20HTML%20%7C%20CSS-green)
![UI](https://img.shields.io/badge/UI-responsive-success)

A **slot-based planning and assignment tool** designed to manage workforce availability and distribute responsibilities fairly across time intervals.

This project focuses on **time-slot modeling**, **fair distribution logic**, and **clear operational UX**, without relying on external APIs or backend services.

---

## ⚠️ Project Status

> **Archived / Transition Phase**

The original business context this tool was built for has been **officially discontinued**.  
As a result, this repository is no longer being developed under its initial domain (*slotwise-status-planner*).

However, the **core logic and UI architecture remain solid and reusable**.

I am currently considering **refactoring and transforming this project into a more generic scheduling / availability planning tool**, such as:

- Workforce shift planner  
- On-call / incident rotation planner  
- Generic time-slot allocation utility  

This repository represents a **completed iteration**, not an abandoned prototype.

---

## ✨ Key Features

- Slot-based time modeling (including cross-midnight slots)
- Employee availability matrix (checkbox + presets)
- Shift preset system with automatic slot filling
- Fair assignment engine with:
  - streak limitation
  - category balancing
  - workload distribution
- Modal handling for over-capacity scenarios
- Clean, responsive UI
- Multi-theme CSS architecture (gray / light / dark ready)

---

## 🧠 Case Study — Why This Project Exists

### Problem

Operational teams often struggle with:
- uneven workload distribution
- repetitive task assignments
- manual shift planning errors
- unclear visibility of who is available when

Most solutions are either:
- too manual (spreadsheets)
- too heavy (enterprise tools)
- or lack fairness logic

---

### Solution Approach

This project models the problem as:

> **People × Time Slots × Assignable Units**

Key design decisions:
- **Frontend-only architecture** for speed and portability
- **Deterministic assignment engine** instead of randomness
- **State-driven UI**, allowing instant recalculation
- **Human-first UX**, minimizing repetitive clicks

---

### Assignment Logic (Simplified)

- Track last assigned category per employee
- Prevent long streaks of the same category
- Penalize repeated actions and overload
- Prefer least-used candidates per slot
- Relax rules only when no valid candidate exists

This ensures:
- fairness over time
- predictable behavior
- explainable results

---

## 🧩 Tech Stack

- **HTML5** — semantic layout
- **CSS3** — custom design system + theming
- **Vanilla JavaScript**
  - state management
  - scheduling logic
  - DOM rendering
- No frameworks
- No external dependencies
- No backend


---

## 🔮 Future Direction (Planned)

If continued, this project will likely evolve into:

- **Generic Shift / Availability Planner**
- Domain-agnostic terminology
- Export options (CSV / JSON)
- Minor UX polishing
- Possible modularization of the assignment engine

---

## 🧾 Final Note

This project is intentionally **left in a complete, stable state**.

While the original use case ended, the work itself was not discarded.  
Instead of forcing continuation without purpose, I chose to **close this chapter cleanly** and leave room for a meaningful transformation.

> *“Not every finished project needs to keep running — some just need to be finished properly.”*


