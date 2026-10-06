# Maeve AI Decision Workspace

A speculative design exploration for [Maeve by Secfi](https://secfi.com/maeve): turning an AI equity assistant from a chatbot into a **decision workspace**, so that people deciding whether to exercise their startup options can see what drives the answer, what the AI knows and assumes, and where the recommendation would change.

> Concept prototype with fictional data and a heuristic model. Not tax, legal or investment advice. Based only on Secfi's public product materials; not affiliated with Secfi.

## What's here

| File | What it is |
|---|---|
| [`maeve_pitch_deck.html`](maeve_pitch_deck.html) | 8-slide deck: benchmark, design principles & scope, page structure, live demo, feature walkthroughs |
| [`maeve_decision_workspace_v2.html`](maeve_decision_workspace_v2.html) | The interactive workspace prototype (current version, embedded in the deck) |
| [`maeve_decision_workspace_demo.html`](maeve_decision_workspace_demo.html) | First prototype, kept for comparison |

All files are self-contained HTML. Clone the repo and open them in a browser; keep them in the same folder so the deck can embed the demo.

## The idea

**From designing a chatbot to designing a workspace.** For a high-stakes, often irreversible financial decision, a fluent answer in chat isn't enough. The workspace turns the conversation into a shared decision model the user can inspect and change:

**Calibrated mental model → grounded decision → calibrated trust → long-term partnership with Secfi**

The layout borrows the agent-workspace frame that Secfi's users (engineers, PMs and designers) already know from Claude Code and Codex. The repo becomes the user's financial position, tests become decision boundaries, and commits become saved decisions.

## Design principles

1. **Simple by default, inspectable on demand.** Show one direction first; reasons, options and sources sit one layer down.
2. **Show the boundary, not just the outcome.** Say *"Above $22, waiting wins"* instead of *"83% confident"*.
3. **Every number says where it came from.** Verified, calculated, assumed and AI-estimated values never look the same.
4. **Ask only what can flip the answer.** Inputs that only refine precision can wait.

## Try the demo

1. Drag **Current 409A** past the $22 line. The direction flips from *Partial exercise* to *Wait*, and the panel explains why.
2. Open **How sure is this?** It starts with what still needs a check.
3. Click **Answer 2 questions**, then **Run calculation**.
4. **Save decision**, and let Maeve watch the events that would make you revisit it.

## Built with

Plain HTML, CSS and JavaScript, prototyped with Claude Code. Design tokens were sampled from Secfi's web app; DM Sans and Newsreader stand in for Matter and Reckless.
