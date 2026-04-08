<div align="center">
  <h1>⚙️ Skills Samples Repository</h1>
  <p><em>Advanced Agentic AI Automation & Developer Tools</em></p>
</div>

---

> [!NOTE]
> This repository curates a comprehensive collection of advanced "Skills" tailored for autonomous coding AI agents. These capabilities orchestrate everything from persistent log tracking and changelog automation to deep integrations with modern libraries like GSAP, Vercel patterns, and Postgres.

## 🚀 Overview

The **Skills Management Example** project acts as a centralized brain for context-aware workflows. By defining precise workflows, rulesets, and prompts, this suite of tools effectively drives agentic coding assistants to act with deterministic rigor in any codebase. 

## ✨ Key Capabilities

### 🗂️ Workflow & Documentation
- **context-logger**: Persistently logs all prompts and actions to ensure continuity and system memory.
- **changelog-generator**: Interrogates commit histories to automate `docs/CHANGELOG.md` updates.
- **database-documenter**: Maintains up-to-date data dictionaries and ER models as the database evolves.
- **functional-documenter**: Keeps system requirements, business rules, and UI workflows synchronized in `docs/FUNCTIONAL_DOCS.md`.
- **create-readme**: Reconstructs concise, aesthetically appealing project documentation.

### 🎨 Frontend & Design
- **frontend-design**: Engineers robust, production-grade, and beautifully stylized UI layouts that avoid generic AI aesthetics.
- **vercel-react-best-practices**: Guides the application of Next.js and React performance optimization guidelines curated directly from Vercel Engineering.

### 🎭 GSAP Animation Suite
Our comprehensive official GSAP tools teach agents exact implementations for modern web animation:
- **gsap-core**: Mastering timelines, tweens, defaults, and the core API.
- **gsap-scrolltrigger**: Implementing robust scroll-driven, layered, and pinned animations.
- **gsap-react** & **gsap-frameworks**: Managing scoping, cleanup on unmount, and React/Vue workflows.
- **gsap-plugins** & **gsap-utils**: Interfacing with Flip, Draggable, Snap, Helper utilities, etc.
- **gsap-performance**: Advanced techniques for reducing jank, managing `will-change`, and avoiding layout thrashing.

### 💽 Backend & DevOps
- **neon-postgres**: Handles connection, platform management, and data handling tailored for Neon Serverless Postgres.
- **committer**: Organizes structured, clean Git commits for precise version control workflows.
- **skill-creator**: A meta-skill that allows the AI to self-author, benchmark, and evaluate new behaviors autonomously!

## ⚙️ Structure & Mechanism

Each skill directory (e.g., `.agents/skills/`) contains an overarching `SKILL.md` coupled with configuration rules and robust references. AI agents recursively parse these files when triggered by specific prompt heuristics, overriding basic behaviors with highly refined engineering methodologies.
