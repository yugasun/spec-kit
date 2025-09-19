---
description: Review and validate the implementation plan artifacts for completeness, consistency, and constitutional compliance.
---

Given the implementation plan to review provided as an argument, do this:

1. Load and analyze the implementation plan:

   - Read the implementation plan file at IMPL_PLAN path
   - Verify all required sections are present and complete
   - Check that no "NEEDS CLARIFICATION" placeholders remain
   - Validate Progress Tracking shows phases 0-1 complete

2. Read the constitution at `/memory/constitution.md` to verify constitutional compliance.

3. Validate generated artifacts exist and are complete:

   - Check Phase 0: Verify research.md exists and contains technical decisions
   - Check Phase 1: Verify required artifacts based on project type:
     - data-model.md (if entities required)
     - contracts/ directory with API specifications (if applicable)
     - quickstart.md with test scenarios
     - Agent-specific template file (CLAUDE.md, .github/copilot-instructions.md, etc.)

4. Perform consistency checks:

   - Verify technical decisions in research.md align with plan context
   - Check that data model entities match those referenced in contracts
   - Ensure quickstart scenarios cover main user stories from feature spec
   - Validate that all dependencies and constraints are realistic and achievable

5. Constitutional compliance review:

   - Verify Constitutional Check section shows no violations
   - Confirm complexity is justified if architecture exceeds simple patterns
   - Check that performance goals and constraints are realistic
   - Ensure technical approach follows established patterns and best practices

6. Readiness assessment:

   - Confirm plan is ready for Phase 2 (/tasks command)
   - Identify any missing information or inconsistencies
   - Validate that implementation approach is feasible within constraints

7. Generate review report:
   - Document findings, issues, and recommendations
   - Rate plan completeness (Ready/Needs Revision/Major Issues)
   - Provide specific action items if revisions needed
   - Confirm branch status and next steps

Use absolute paths with the repository root for all file operations to avoid path issues.
