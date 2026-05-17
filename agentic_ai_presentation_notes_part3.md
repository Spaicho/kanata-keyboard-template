# Agentic AI Presentation Notes — Part 3

## Historical framing

### AI as a compiler-like moment
Idea:

- the advent of AI feels like the advent of compilers
- compilers opened programming to many more people, not just assembly programmers
- they raised the abstraction level
- one historical maturity milestone was self-hosting / bootstrapping: a compiler compiling its own code
- similarly, now LLMs can help build LLM systems

Important nuance:

- compilers are deterministic
- LLMs are probabilistic
- the analogy is strongest at the level of abstraction shift and workflow change, not identical behavior

Good lines:

- **AI feels like a compiler moment for our generation.**
- **A new abstraction layer changes who can build and what can be built.**
- **Compilers became self-hosting; now AI is helping build AI.**

---

## Resistance and cultural shift

There is an image of an old-school retro developer that could be used as a visual.
Use it carefully.

Best angle:

- not mocking people
- show that resistance is understandable

Fears people may have:

- quality concerns
- security concerns
- loss of craft
- feeling replaced
- distrust of hype

Good response:

**The answer is not denial. The answer is learning how to work well with it.**

---

## Spotify provocative slide idea

There is also a Spotify headline screenshot about best developers not having written a line of code since December thanks to AI.

How to use it:

- as a provocative conversation starter
- not as a literal "nobody codes anymore" claim
- the real point is that the job is shifting from typing to specifying, steering, reviewing, and shipping

Good framing:

- **When 'writing code' stops being the main job**
- **Old: write code. New: describe -> generate -> review -> ship.**

---

## The 5 pillars from the Agentic AI Engineering video

Use these as the operating model across all 4 use cases.

Pillars:

1. Context Engineering
2. Agentic Validation
3. Agentic Tooling
4. Agentic Code Bases
5. Compound Engineering

Useful framing:

**The 4 use cases show where AI creates value. The 5 pillars show how to make that value reliable and repeatable.**

Rough practical mapping:

- big migration / refactoring -> code bases, validation, compounding
- massive analysis / reporting -> tooling, context, compounding
- UI/UX app design -> context, validation, tooling
- production issue investigation -> context, tooling, validation

---

## Recommended presentation structure

### Presentation shape
Use slides as the backbone, with a few carefully chosen demo islands.

Do not constantly jump between:

- slides
- IDE
- browser
- Excel
- logs
- chats

Better rhythm:

**Claim -> Artifact / Demo -> Lesson**

### Recommended demo islands
1. setup / MCP / multi-repo workspace
2. Excel inventory / impact file
3. dashboard / UI result

Keep the production investigation mostly as a prepared artifact, not a risky live deep dive.

### Recommended slide sequence
1. Title / opening
2. Thesis: work-model shift
3. Pivot moment: migration we couldn't do until now
4. Why this is big: changed feasibility
5. Why modernization matters more now: code for humans and agents
6. Four use-case pillars
7. Five pillars / operating model
8. Setup / operating table
9. Workflow evolution: one chat to four agents
10. Real bottleneck: human context switching
11. What actually improved output
12. Use case 1: big migration and refactoring
13. Use case 2: massive analysis and Excel artifact
14. Use case 3: UX process to implemented dashboard
15. Use case 4: production investigation
16. Shock moments: security + DB self-discovery
17. Daily work changed: Stack Overflow once in two weeks
18. Historical analogy: compiler moment
19. Resistance is normal
20. Closing

### Use-case artifacts to show
Use case 1:
- workspace with many repos open
- migration chat / plan / before-after snippets

Use case 2:
- Excel file with color-coded sheets
- thorough analysis output

Use case 3:
- finished implemented dashboard in browser
- maybe a nod to UX process

Use case 4:
- production investigation chat / thread
- cross-domain analysis across code, SQL, scripts, docs, logs

---

## Suggested talk track ideas / recurring punchlines

- **This is not a tooling upgrade. It is a work-model shift.**
- **The headline is not speed. The headline is changed feasibility.**
- **We write for humans and agents.**
- **Maintainability is throughput.**
- **The surprise was not only what the AI could do. The surprise was what our environment silently allowed.**
- **Different roles, same shift.**
- **The biggest shift is not that AI writes code. The biggest shift is that it changes what one person can understand, attempt, and deliver.**

---

## Canva workflow notes

If using Canva instead of PowerPoint Copilot:

- use Canva for layout / visual draft, not for inventing the whole argument
- generate a first short draft from a concise prompt
- manually insert real proof artifacts afterward
- export to PPTX later if needed

Short Canva prompt:

Create a professional presentation for engineers and managers about agentic AI in software engineering. Tone: modern, credible, ambitious. Core message: this is not just better autocomplete, it is changing feasibility, workflow, and decision-making. Include sections on: aha migration story, why code must be written for humans and agents, four use cases (legacy migrations, massive analysis/reporting, UI/UX app design, production issue investigation), workflow evolution from one chat to multiple agents, surprise/security moments, and a strong closing about how AI changes what one person can deliver. Use clean layouts with room for screenshots and demo artifacts.

Shorter version:

Professional presentation for engineers and managers on agentic AI in software work. Show that AI changes feasibility, workflow, and decision-making, not just coding speed. Include: migration/refactoring, large-scale analysis/reporting, UI/UX app design, production issue investigation, workflow evolution, surprise/security moments, and a strong conclusion. Clean modern style with room for screenshots.

---

## Final reminder on presentation style

This should not be a pure demo.
This should not be a pure slide deck.

Best version:

**A story-driven deck with proof artifacts.**

That gives:

- clarity
- credibility
- interactivity
- strong visuals
- practical lessons

