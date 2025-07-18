# Rule Files Formatting Standards

## File Naming Conventions
- Use kebab-case for file names (e.g., `file-name.xml`)
- Append `-optimized` to optimized versions of files (e.g., `file-name-optimized.xml`)
- Use appropriate file extensions:
  - `.xml` for XML-based rule files
  - `.md` for Markdown-based rule files

## XML Structure and Formatting
- Use a single root element that describes the content (e.g., `<TOOLS_AND_FILE_OPERATIONS>`)
- Group related rules under semantic section tags (e.g., `<CRITICAL>`, `<FILE_OPERATIONS>`)
- Use consistent indentation (2 spaces)
- Use ALL_CAPS for tag names
- Use proper XML entity escaping (e.g., `&lt;` for `<`, `&gt;` for `>`)
- Use comments to separate major sections (`<!-- Section Title -->`)

## Markdown Structure and Formatting
- Use a YAML frontmatter for metadata when appropriate
- Use proper heading hierarchy (H1 for title, H2 for major sections, etc.)
- Use bold (`**text**`) for emphasis of critical information
- Use code formatting (`` `code` ``) for tool names and commands
- Use numbered lists for sequential steps
- Use bullet lists for non-sequential items
- Use code blocks with triple backticks for examples

## Rule Identification
- Use consistent ID prefixes for different rule categories:
  - `CS` for coding standards
  - `FS` for favouring simplicity
  - `FO` for file operations
  - `MERM` for Mermaid diagram rules
  - `GO` for Golang-specific rules
  - `DK` for Docker-specific rules
  - `TEST` for testing requirements
  - `EH` for error handling

## Content Organization
- Place critical/important rules at the top
- Group related rules together
- Use consistent terminology across all files
- Maintain a clear hierarchy of information

## Best Practices
- Keep rule descriptions concise and clear
- Avoid redundancy between files
- Use examples sparingly and only when they add value
- Ensure all rules have a clear purpose and are actionable

These standards ensure consistency across all rule files, making them easier to maintain, understand, and follow.
