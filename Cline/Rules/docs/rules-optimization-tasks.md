# Rules Optimization Task List

## Phase 1: Analyze and Prepare
- [x] 1. Create a backup directory for original rules files
- [x] 2. Identify dependencies between rules files
- [x] 3. Determine priority order for optimization (based on size and impact)

## Phase 2: Optimize High-Impact Files
- [x] 4. Simplify `new-task-rules.md` (highest priority - very verbose)
   - Remove redundant explanations
   - Condense examples
   - Preserve core instructions
   - Reduce by ~70%

- [x] 5. Streamline `sams-main-clinerules.xml`
   - Removed unnecessary whitespace and formatting
   - Consolidated redundant rules
   - Converted to more compact format
   - Created `sams-main-clinerules-optimized.xml` with a 19% size reduction (4,202 → 3,406 bytes)

## Phase 3: Consolidate Related Rules
- [x] 6. Merge `file-operations-rules.xml` and `tooling-rules.xml`
   - Created unified `tools-and-file-operations-optimized.xml` file
   - Removed overlapping concepts and redundancy
   - Standardized format with clear sections
   - Combined size: 2,577 bytes → Merged file: 2,018 bytes (22% reduction)

- [x] 7. Optimize `mermaid-rules.xml`
   - Created `mermaid-rules-optimized.xml`
   - Properly escaped XML entities
   - Maintained all essential rules and theme definitions
   - File size optimization was minimal as original was already compact

## Phase 4: Address Minor Rules
- [x] 8. Evaluate and potentially modify `repeat-back-rules.xml`
   - Task skipped as per user request
   - Original file is already compact (424 bytes)

- [x] 9. Review `adhoc/_self-reflection-rules.md`
   - Task skipped as per user request to proceed to Phase 5

## Phase 5: Create Unified Structure
- [x] 10. Develop consistent formatting across all rules
   - Created `formatting-standards.md` with comprehensive guidelines
   - Defined standards for file naming, XML structure, Markdown formatting
   - Established rule ID conventions and content organization principles
   - Documented best practices for rule creation and maintenance
- [x] 11. Create a master index file for quick reference
   - Created `rules-index.md` with comprehensive overview of all rule files
   - Organized rules by categories and provided quick lookup tables
   - Added detailed descriptions of each rule file's purpose and key contents
   - Included cross-references between related rules
- [x] 12. Implement conditional loading mechanism (if possible)
   - Created `rules-loading-config.json` as a blueprint for conditional loading
   - Defined core rules, context-dependent rules, and language-specific rules
   - Specified loading priorities and dependencies between rules
   - Outlined different loading strategies based on context window usage
   - Provided implementation notes for system-level integration

## Phase 6: Testing and Validation
- [x] 13. Verify all optimized rules maintain original intent
   - Created `rules-verification.md` with comprehensive verification results
   - Verified each optimized file against its original counterpart
   - Confirmed all essential rules and requirements are preserved
   - Validated new supporting files for accuracy and completeness
- [x] 14. Measure context usage reduction
   - Created `context-usage-reduction.md` with detailed analysis
   - Calculated total size reduction: 9,860 bytes (48.1%)
   - Estimated token reduction: ~2,465 tokens (1.3% of context window)
   - Analyzed optimization efficiency and conditional loading impact
   - Provided visualization of file size reductions
- [x] 15. Document optimization process for future reference
   - Created `optimization-guide.md` with comprehensive documentation
   - Outlined the complete optimization approach and methodology
   - Detailed step-by-step process for future optimization efforts
   - Documented lessons learned and best practices
   - Provided recommendations for future work
