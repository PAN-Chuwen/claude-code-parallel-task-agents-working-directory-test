# Multi-Environment Parallel Analysis Demo

This repository demonstrates Claude Code's parallel Task agent capabilities for analyzing multiple environments simultaneously.

## Use Case

Navigate to this directory and run Claude Code with the specific prompt to see parallel analysis in action:

```bash
cd ~/claude-code-parallel-task-agents-working-directory-test && claude
```

Then use this prompt:

```
Analyze multiple environment configurations in parallel
```

## What This Demonstrates

Claude Code will create multiple Task agents that work in parallel to:
- Analyze three different environment configurations (dev, staging, production)
- Each agent uses `cd` to navigate to its assigned directory
- Generate comprehensive reports for each environment
- Work simultaneously rather than sequentially

This showcases Claude Code's ability to handle complex multi-environment analysis tasks efficiently through parallel execution.