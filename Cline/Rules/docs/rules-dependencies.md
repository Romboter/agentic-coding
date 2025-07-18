# Rules Files Dependencies Analysis

## Core Files
- `sams-main-clinerules.xml`: Contains fundamental principles and coding rules that other files may build upon
  - Principle #5 about context window usage is referenced by `new-task-rules.md`
  - Principle #6 about British English is related to `spelling-rules.xml`
  - Simplicity principles are foundational to other rules

## Related File Groups

### Task Management
- `new-task-rules.md`: Heavily references context window monitoring (from `sams-main-clinerules.xml`)
- Uses Mermaid diagrams (relies on `mermaid-rules.xml` for formatting)

### Tool Usage
- `file-operations-rules.xml` and `tooling-rules.xml`: Significant overlap in purpose
  - Both deal with tool usage and file operations
  - Natural candidates for merging
  - No other files depend on their specific structure

### Formatting and Presentation
- `mermaid-rules.xml`: Referenced by `new-task-rules.md` for diagram formatting
- `spelling-rules.xml`: Implements principle #6 from `sams-main-clinerules.xml`

### Standalone Rules
- `repeat-back-rules.xml`: No dependencies with other files
- `adhoc/_self-reflection-rules.md`: Meta-relationship with all rules files but no direct dependencies

## Optimization Implications

1. **Safe to Merge**: `file-operations-rules.xml` and `tooling-rules.xml`
2. **Requires Careful Modification**: `new-task-rules.md` (due to its verbosity and references to other rules)
3. **Core File**: `sams-main-clinerules.xml` (changes here may affect other files)
4. **Independent Files**: `repeat-back-rules.xml` and most adhoc files can be optimized independently
