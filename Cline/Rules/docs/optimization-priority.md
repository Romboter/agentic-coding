# Optimization Priority Order

## Priority Ranking (Highest to Lowest)

1. **`new-task-rules.md`** (11,315 bytes)
   - Largest core file
   - Very verbose with many redundant explanations
   - High impact on context usage
   - Potential for 70% reduction

2. **`sams-main-clinerules.xml`** (4,202 bytes)
   - Core file that other files depend on
   - Contains redundant explanations
   - Medium-high impact on context usage

3. **`file-operations-rules.xml` + `tooling-rules.xml`** (2,577 bytes combined)
   - Significant overlap in purpose
   - Can be consolidated into a single file
   - Medium impact on context usage

4. **`mermaid-rules.xml`** (1,093 bytes)
   - Contains verbose theme definitions
   - Referenced by `new-task-rules.md`
   - Medium-low impact on context usage

5. **`spelling-rules.xml`** (904 bytes)
   - Implements principle #6 from `sams-main-clinerules.xml`
   - Low impact on context usage

6. **`repeat-back-rules.xml`** (424 bytes)
   - Smallest file
   - No dependencies with other files
   - Very low impact on context usage

## Adhoc Files (If Needed)

- **`_ollama-modelfile-conversion.md`** (40,042 bytes)
- **`_create-mcp-server-rules.md`** (17,255 bytes)
- **`_cline-for-slides.md`** (7,066 bytes)
- **`_cline-memory-bank.md`** (3,974 bytes)
- **`_self-reflection-rules.md`** (2,621 bytes)
- **`_confidence-rating.xml`** (2,075 bytes)
- **`_qwen-nothink.md`** (11 bytes)

## Optimization Approach

1. Start with the largest files first for maximum impact
2. Focus on files with redundant explanations and examples
3. Consolidate related files to reduce duplication
4. Preserve core functionality while reducing verbosity
