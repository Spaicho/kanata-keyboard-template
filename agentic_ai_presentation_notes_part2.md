# Agentic AI Presentation Notes — Part 2

## Shock moments / surprise moments

This section should show both capability and risk.

### Shock story #1 — AI exposed a major security issue while writing a login integration test
Story essence:

- The task was simple: create an integration test for a web app UI.
- The goal was to test login and verify landing on the right page depending on the user.
- The app used SSO / OAuth.
- The AI found a way to spoof identities and enter with the identity of any user.
- This revealed a serious security issue.

Why it matters:

- AI can behave like an aggressive tester / accidental red teamer.
- Routine dev tasks can surface real vulnerabilities.

Strong line:

**I asked for a login test. I got a security finding.**

### Shock story #2 — AI discovered DB access path by itself
Story essence:

- The goal was to create tests for each user profile, where different profiles enable different features.
- The AI was not explicitly told to connect to the database.
- Credentials were not explicitly given in the prompt.
- It found connection details in config files.
- It reused the same JDBC driver / patterns used by the application.
- It wrote the necessary code / script.
- It inspected the database schema.
- It crafted SQL queries.
- It identified useful profiles and users to test.

Why it matters:

- The agent inferred intent and found its own path to the result.
- It used the latent capability surface already present in the repo / environment.
- This is both powerful and alarming.

Best punchline:

**The surprise was not only what the AI could do. The surprise was what our environment silently allowed.**

Other useful lines:

- **If it's in the repo or runtime, assume the agent can and will use it.**
- **The AI was only as powerful as the access we had already left lying around.**

---

## Workflow evolution

This section should be story + learning.

### Phase 1 — One chat, long planning
- started in VS Code with one chat on the side
- spent 2 or 3 days planning to make sure the plan was solid
- then moved from planning mode to agent mode for implementation

### Phase 2 — Two chats / parallel side work
- planning and implementation both took time
- opened a second chat to do something else in parallel
- used it for environment issues or urgent work

### Phase 3 — Four agents in parallel
- realized it was possible to use more agents
- ended up with four agents, about one per repo
- asked another agent to read the plan and extract tasks that could be done in parallel
- learned that many tasks were too small to justify a dedicated agent

### Real bottleneck
- not the AI
- not the number of agents
- the real bottleneck became human context switching
- constantly re-reading prompts and responses to reload context
- each agent handled a different repo / problem

Strong lines:

- **I thought the bottleneck was agent capacity. It turned out to be my brain.**
- **My brain became the queue.**
- **I scaled execution faster than I scaled my own context-switching capacity.**

### What actually improved output
The best improvements came from workflow design, not from blindly adding more agents.

Important lessons:

- task sizing matters
- independent tasks benefit most from parallel agents
- tiny tasks are often not worth their own agent
- chunking beats asking an agent to rewrite a giant file at once
- good defaults and guardrails matter
- context design matters more than clever prompting at scale

Strong line:

**I thought prompting was the main skill. It turned out context design was the real multiplier.**

---

## Copilot instructions, custom prompts, and workflow mechanics

### Copilot instructions / persistent repo guidance
Used for:

- coding conventions
- architecture constraints
- warnings / pitfalls
- instructions such as: do not write giant files in one shot, edit in chunks
- commit and review rules

### Task prompt / chat request
Used for:

- immediate task intent
- acceptance criteria
- success conditions for the current request

### Reusable slash prompts / custom prompts
Example:

- `/prepare-commit`
- after a session, it organizes changes into logical commits
- proposes detailed commit messages
- waits for review
- never commits automatically

Important guardrail:

**No commit before human review.**

### Skills and custom agents
- did not feel much need to use skills or custom agents
- believed workflow and guardrails mattered more
- had seen claims or discussion online suggesting many custom agents do not necessarily improve output quality proportionally

### Copilot CLI
- recently started using Copilot CLI
- it feels like a different product from IDE Copilot
- especially interesting in autopilot-like mode

---

## Personal workflow and ergonomics

### Voice instead of typing
- used vocal interaction instead of typing
- similar to people on the frontier like Peter / OpenClaw workflows

Good line:

**I stopped treating the agent like a text box and started talking to it.**

### Stack Overflow habit change
One very good proof point:

**I went to Stack Overflow one time in two weeks.**

Why it lands:

- instantly relatable
- shows the daily loop changed
- generic browser search was replaced by contextual reasoning inside the repo and toolchain

Other phrasing:

- **In two weeks, I opened Stack Overflow once.**
- **I replaced generic search with contextual problem-solving inside my own codebase.**

---

## External signal: Peter / OpenClaw / frontier workflows

This can be included as a "this is not just me" section.

Themes to mention:

- multi-screen / desk setup
- multiple concurrent agents
- voice workflow
- very high visible shipping velocity / many public projects

Use carefully:

- do not make it idol worship
- make it a signal that the workflow frontier is shifting

Good framing line:

**I'm not showing this because it looks cool. I'm showing it because it previews a different job.**

