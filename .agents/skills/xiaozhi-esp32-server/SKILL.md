```markdown
# xiaozhi-esp32-server Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill provides guidance on contributing to the `xiaozhi-esp32-server` Python codebase. It covers established coding conventions, workflow automation for optimizing agent logic and tool invocation, and testing patterns. Whether you're improving backend logic, refining prompts, or adding new features, this guide will help you align with the project's standards.

## Coding Conventions

### File Naming
- Use **snake_case** for all Python files.
  - Example: `core_connection.py`, `plugin_utils.py`

### Import Style
- Use **relative imports** within modules.
  - Example:
    ```python
    from .utils import parse_request
    ```

### Export Style
- Use **named exports** (explicitly define what is exported).
  - Example:
    ```python
    def connect_agent(...):
        ...
    __all__ = ['connect_agent']
    ```

### Commit Patterns
- Commit messages are freeform, usually around 37 characters.
  - Example: `fix: improve tool invocation accuracy`

## Workflows

### Agent Tool Logic Optimization
**Trigger:** When you want to improve agent search logic, refine tool invocation, or adjust prompt handling.  
**Command:** `/optimize-agent-tool-logic`

**Steps:**
1. **Update agent service logic in Java backend**
   - Edit: `main/manager-api/src/main/java/xiaozhi/modules/agent/service/impl/AgentServiceImpl.java`
   - Example:
     ```java
     // Refactor tool selection logic
     public void optimizeToolInvocation() {
         // Improved logic here
     }
     ```
2. **Modify agent prompt templates**
   - Edit: `main/xiaozhi-server/agent-base-prompt.txt`
   - Example:
     ```
     # Add clearer tool descriptions for agents
     ```
3. **Adjust Python core connection logic**
   - Edit: `main/xiaozhi-server/core/connection.py`
   - Example:
     ```python
     def invoke_tool(tool_name, params):
         # Enhanced parameter validation
         ...
     ```
4. **Refactor or enhance tool function scripts**
   - Edit: `main/xiaozhi-server/plugins_func/functions/*.py`
   - Example:
     ```python
     def new_tool_function(...):
         # Improved logic for new tool
         ...
     ```

## Testing Patterns

- **Framework:** Unknown (no specific framework detected)
- **Test File Pattern:** Files named with `.test.` in the filename.
  - Example: `core_connection.test.py`
- **Best Practice:** Place test functions in files matching the pattern and ensure they cover new or modified logic.

## Commands

| Command                        | Purpose                                                      |
|--------------------------------|--------------------------------------------------------------|
| /optimize-agent-tool-logic     | Optimize agent backend logic and tool invocation workflows    |
```
