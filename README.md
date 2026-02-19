# Why this solves a problem
## Token Budgeting
- By using a "Mini" model as the entry point, you handle the messy, long-form brainstorming without burning through your Claude 3.5 Opus or Sonnet quota.
- Only the "compressed" result is passed forward.

## Design Guardrails
- The agent is explicitly told to "Fail" a request if it doesn't align with your Tailwind/Alpine.js standards, preventing technical debt before a single line of code is written.

## The "Sub-Agent" Workflow
- In 2026, VS Code agents can call one another. By using the handoff property, you create a pipeline:
  - PO $\rightarrow$ Optimizer (Mini model, cheap, enforces standards)
  - Optimizer $\rightarrow$ Strategist (Mid model, defines logic)
  - Strategist $\rightarrow$ Architect (High model, writes code)

## How to use it 
- When your PO has a "big idea," they should open the agent picker and select ```context-optimizer```.
- They can paste their entire brain-dump there. The agent will then hand back a refined version that is "ready for the machines."
