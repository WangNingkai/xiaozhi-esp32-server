---
name: agent-tool-logic-optimization
description: Workflow command scaffold for agent-tool-logic-optimization in xiaozhi-esp32-server.
allowed_tools: ["Bash", "Read", "Write", "Grep", "Glob"]
---

# /agent-tool-logic-optimization

Use this workflow when working on **agent-tool-logic-optimization** in `xiaozhi-esp32-server`.

## Goal

Optimize agent backend logic and improve tool invocation accuracy, including prompt and function adjustments.

## Common Files

- `main/manager-api/src/main/java/xiaozhi/modules/agent/service/impl/AgentServiceImpl.java`
- `main/xiaozhi-server/agent-base-prompt.txt`
- `main/xiaozhi-server/core/connection.py`
- `main/xiaozhi-server/plugins_func/functions/*.py`

## Suggested Sequence

1. Understand the current state and failure mode before editing.
2. Make the smallest coherent change that satisfies the workflow goal.
3. Run the most relevant verification for touched files.
4. Summarize what changed and what still needs review.

## Typical Commit Signals

- Update agent service implementation logic in Java backend.
- Modify agent prompt templates for better tool descriptions.
- Adjust Python core connection logic for tool usage.
- Refactor or enhance specific tool function scripts.

## Notes

- Treat this as a scaffold, not a hard-coded script.
- Update the command if the workflow evolves materially.