# Rules Index

This document serves as a master index for all rule files, providing a quick reference to find specific rules and understand their relationships.

## Overview of Rule Files

| File | Purpose | Key Contents |
|------|---------|--------------|
| [`sams-main-clinerules-optimized.xml`](#sams-main-clinerules) | Core principles and coding standards | Critical principles, coding rules, language-specific rules |
| [`new-task-rules-optimized.md`](#new-task-rules) | Context window management and task handoff | Context monitoring, task breakdown, handoff process |
| [`tools-and-file-operations-optimized.xml`](#tools-and-file-operations) | Tool usage and file operations | File operation rules, available tools, best practices |
| [`mermaid-rules-optimized.xml`](#mermaid-rules) | Mermaid diagram formatting | Diagram rules, standard theme definitions |
| [`repeat-back-rules.xml`](#repeat-back-rules) | Rule verification process | Initial conversation verification |
| [`spelling-rules.xml`](#spelling-rules) | Spelling standards | British English spelling rules |

## Rule Categories

### Critical Principles
- **Simplicity**: Favour concise, straightforward solutions (Priority 1)
- **Tool Usage**: Prioritise using available tools over manual approaches (Priority 2)
- **Best Practices**: Follow language-specific best practices (Priority 3)
- **Verification**: Verify all changes before completing tasks (Priority 4)
- **Context Management**: Start new task when context window exceeds 70% (Priority 5)
- **British English**: Use British English spelling in all outputs (Priority 6)

### Coding Standards
- **CS001-CS009**: General coding standards and practices
- **FS001-FS004**: Rules for favouring simplicity
- **GO001-GO002**: Golang-specific rules
- **DK001**: Docker-specific rules
- **TEST001-TEST003**: Testing requirements
- **EH001-EH002**: Error handling and git rules

### File Operations
- **FO001-FO002**: Rules for file operations
- Available tools: `write_to_file`, `read_file`, `replace_in_file`, `search_files`, `list_files`

### Task Management
- Context window monitoring
- Task breakdown in Plan Mode
- Task handoff process
- Required context components

### Diagram Formatting
- **MERM001-MERM004**: Mermaid diagram formatting rules
- Standard theme definitions for consistent styling

## <a id="sams-main-clinerules"></a>sams-main-clinerules-optimized.xml

Core principles and coding standards that form the foundation of all other rules.

**Key Rules:**
- 6 critical principles in priority order
- General coding rules (CS001-CS009)
- Simplicity rules (FS001-FS004)
- Language-specific rules for Golang and Docker
- Testing requirements (TEST001-TEST003)

## <a id="new-task-rules"></a>new-task-rules-optimized.md

Guidelines for context window management and task handoff workflow.

**Key Components:**
- Context window monitoring (75% threshold)
- Plan Mode task breakdown process
- Task handoff process and template
- Required context components
- Best practices for maintaining continuity

## <a id="tools-and-file-operations"></a>tools-and-file-operations-optimized.xml

Rules and guidelines for tool usage and file operations.

**Key Components:**
- File operation rules (FO001-FO002)
- Available file operation tools
- Additional useful tools (fetch_url, library_docs, etc.)
- Best practices for tool usage

## <a id="mermaid-rules"></a>mermaid-rules-optimized.xml

Rules for creating and formatting Mermaid diagrams.

**Key Components:**
- Mermaid formatting rules (MERM001-MERM004)
- Standard theme definitions for consistent styling

## <a id="repeat-back-rules"></a>repeat-back-rules.xml

Process for verifying understanding of rules at the start of conversations.

**Key Components:**
- Rule verification process for new conversations

## <a id="spelling-rules"></a>spelling-rules.xml

Standards for consistent spelling across all outputs.

**Key Components:**
- British English spelling rules
- Common American to British English conversions

## Quick Rule Lookup

| If you need to... | Refer to... |
|-------------------|-------------|
| Understand core principles | `sams-main-clinerules-optimized.xml` |
| Follow coding standards | `sams-main-clinerules-optimized.xml` (CS001-CS009) |
| Create simple, elegant solutions | `sams-main-clinerules-optimized.xml` (FS001-FS004) |
| Manage context window usage | `new-task-rules-optimized.md` |
| Hand off tasks effectively | `new-task-rules-optimized.md` |
| Use file operation tools | `tools-and-file-operations-optimized.xml` |
| Create Mermaid diagrams | `mermaid-rules-optimized.xml` |
| Verify rule understanding | `repeat-back-rules.xml` |
| Use correct spelling | `spelling-rules.xml` |

This index provides a comprehensive overview of all rule files and their relationships, making it easier to find specific rules and understand the overall rule structure.
