# Plan Mode in VS Code

Source: [planAgentProvider.ts](https://github.com/microsoft/vscode/blob/main/extensions/copilot/src/extension/agents/vscode-node/planAgentProvider.ts)

Its behavior is essentially:

- Discovery: invoke the built-in `Explore` subagent to inspect the codebase, find analogous implementations, and identify blockers. For independent areas, it explicitly tells the model to launch 2–3 Explore subagents in parallel.
- Alignment: use `vscode/askQuestions` to resolve substantial ambiguity rather than making big assumptions.
- Design: produce a detailed implementation plan including dependencies/parallel steps, verification, relevant functions/types, full file paths, scope boundaries, and decisions.
- Refinement: update the plan based on feedback until the user approves it.
- It saves the persistent working plan into `/memories/session/plan.md` using the VS Code memory tool.

The prompt also contains hard constraints along the lines of:

> “STOP if you consider running file editing tools — plans are for others to execute.”

and

> “The only write tool you have is … memory for persisting plans.”
