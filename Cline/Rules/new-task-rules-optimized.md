---
description: Context window management and task handoff workflow
version: 1.1
tags: ["context-management", "new-task"]
globs: ["*"]
---
# Task Handoff Strategy

## Context Window Monitoring

**CRITICAL**: Monitor context window usage in environment details. When usage exceeds 75% (e.g., 150K/200K tokens), initiate task handoff:

1. Complete current logical step
2. Use `ask_followup_question` to offer creating a new task
3. If approved, use `new_task` with comprehensive handoff instructions

## Plan Mode Task Breakdown

In Plan Mode:

1. **Initial Analysis**: Understand full scope, identify components, consider challenges
2. **Task Decomposition**: Break into logical subtasks, prioritize based on dependencies
3. **Create Roadmap**: Present numbered subtasks with dependencies (use Mermaid diagrams when helpful)
4. **Get Approval**: Confirm subtask priorities, starting point, then request Act Mode toggle

## Task Handoff Process

In Act Mode:

1. **Identify Handoff Points**:
   - Subtask completion
   - Logical stopping point
   - Context window exceeds 75%
   - Task scope expansion

2. **Handoff Steps**:
   - Summarize accomplishments
   - State remaining work
   - Use `ask_followup_question` to offer new task creation

3. **Create New Task**:
   ```xml
   <new_task>
   <context>
   # Task Continuation: [Brief Title]

   ## Completed Work
   - [Key accomplishments]
   - [Files modified/created]
   - [Important decisions]

   ## Current State
   - [Project state]
   - [Running processes]
   - [Key files status]

   ## Next Steps
   - [Remaining tasks]
   - [Implementation details]
   - [Known challenges]

   ## Reference Information
   - [Documentation links]
   - [Important patterns]
   - [User preferences]

   Please continue by [specific next action].
   </context>
   </new_task>
   ```

## Required Context Components

Always include:

- **Project Context**: Goals, architecture, tech stack
- **Implementation Details**: Files modified, components implemented, patterns
- **Progress Tracking**: Completed items, remaining items, blockers
- **User Preferences**: Coding style, approaches, priorities

## Best Practices

1. **Maintain Continuity**: Consistent terminology, reference decisions
2. **Preserve Context**: Include relevant code snippets, reference files
3. **Clear Next Actions**: Begin with actionable step, prioritize tasks
4. **Document Assumptions**: Note areas needing user input
5. **Optimize for Resumability**: Structure for immediate continuation

## When to Use Task Handoffs

1. Context window exceeds 75%
2. Long-running projects
3. Complex implementations with distinct phases
4. Switching focus areas
5. Different expertise needed for different parts
