# Agentic AI Presentation Notes — Part 1

## Core intent of the presentation

This presentation is for colleagues and managers about using agentic AI for big migrations and refactoring of very old codebases across tens of Git repositories.

The presentation should feel **big**: not just "AI helps code faster," but that this is a real shift in the history of software work. There is a before and after.

Key overarching message:

- This is not just a tooling upgrade.
- This is not just better autocomplete.
- This is a **work-model shift**.
- It changes feasibility, workflow, decision-making, and what one person can deliver.
- It affects everyone's work, not just coders.
- It will affect work first, then because work shapes daily life, it affects life too.

Useful recurring lines:

- **This is not a tooling upgrade. It is a work-model shift.**
- **The headline is not speed. The headline is changed feasibility.**
- **Different roles, same shift.**
- **Maintainability is throughput.**
- **We now write for humans and agents.**
- **The bottleneck moved from typing to orchestration and judgment.**

---

## Audience and positioning

Audience includes:

- engineers
- tech leads
- architects
- managers
- potentially people beyond pure coding roles

The talk should show that AI is not limited to one niche. It helps with:

- modernization
- understanding systems
- product design and delivery
- production support and investigation

So the audience should leave thinking:

- this is bigger than a coding assistant
- this changes daily work
- everyone should care

---

## Four main use-case pillars

These are the backbone of the presentation.

### 1) Big migration and refactoring
Examples:

- javax -> jakarta
- Spring Boot 2 -> 3
- iBatis / eBatis -> MyBatis
- Spring XML -> annotations
- Playwright integration tests

Message:

Agentic AI is a force multiplier for large-scale legacy modernization across many repositories.

### 2) Massive analysis across codebases and live systems
Examples:

- analyzing codebases
- GitLab API analysis
- Kubernetes live pods
- config and services
- scraping webapps to gather data scattered across pages
- cross comparing findings
- generating very thorough Excel files with color code and beautiful sheets

Message:

AI is not only for generating code. It can also build visibility and understanding across complex systems.

### 3) Designing a very professional UI/UX app
Examples:

- starting from a thorough UX process
- helping across design steps
- helping through implementation
- delivering a polished dashboard or app

Message:

AI can help all along the product creation lifecycle, not just in backend legacy work.

### 4) In-depth production bug / issue analysis
Examples:

- codebases
- SQL
- databases
- scripts
- bash
- Confluence
- Control-M
- logs

Message:

AI can act as a cross-domain investigator in messy real-world incidents and analysis.

### Summary line for the four use cases

**Refactor. Analyze. Design. Diagnose.**

or

**Build. Understand. Modernize. Troubleshoot.**

---

## Aha moments / pivot moments

### Aha moment #1 — iBatis/eBatis to MyBatis
This is one of the strongest stories in the talk.

Story essence:

- There was a migration from eBatis / iBatis to MyBatis.
- It spanned several codebases and hundreds of thousands of lines.
- 3 to 4 developers worked on it.
- About 6 months were spent.
- In the end, it was abandoned because it was too complex.
- Later, using agentic AI, the same class of migration was handled by one person in about a week.

This was the moment of:

**"Oh my God, it's happening."**

Why it matters:

- It demonstrates a before/after moment.
- It proves changed feasibility.
- It is not just speed. It is a strategic shift in what can realistically be attempted.

Possible framing lines:

- **The migration we couldn't do — until now.**
- **That was the moment I realized the rules had changed.**
- **This was my before-and-after moment in software history.**

### Aha moment #2 — EHCache 2 -> 3? No, jump to Caffeine
Story essence:

- There was a cache migration need around EHCache version 2.
- The obvious old-world thinking would have been EHCache 2 -> 3.
- But the question became: why remain on that framework at all?
- EHCache was no longer the state of the art.
- In the old world, switching to a different framework entirely would have felt too hard and too costly.
- With AI, it became realistic to leap directly to Caffeine.

Why it matters:

- AI does not just accelerate implementation.
- It changes the economics of technical decisions.
- It allows optimizing for the best target state, not just the easiest incremental path.

Strong lines:

- **From minimal change to best change.**
- **AI changes the cost model, so we can optimize for the best target state.**
- **Code is getting cheaper. Decision quality matters more.**
- **The bottleneck is moving from coding to judgment.**

---

## Why modernization matters more than before

Key message:

**We do not write code for humans only anymore. We write for humans and agents.**

Implications:

- codebases must be easier to navigate for agents
- repos should have README files / markdown onboarding docs
- architecture and constraints should be more explicit
- naming and structure matter more
- up-to-date dependencies matter more
- stale undocumented code hurts more than before

This is not just developer nicety. It has leverage.

Good framing:

- every repository should have an agent onboarding surface
- a well-documented repo is now executable context
- documentation is not just for human onboarding anymore; it enables automation

Compounding effect:

- each refactoring / cleanup makes future refactoring easier
- each iteration improves agent understanding
- code quality now compounds twice: for humans and for agents

Strong line:

**Maintainability is no longer just a cost. It is throughput.**

