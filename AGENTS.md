# Agent Instructions

## Project Technical Overview

See `openspec/` for product requirements and technical architecture details.

We use red/green TDD for all development.

## Package Manager

Always use **pnpm** — never npm or yarn.

## Testing Rules

- Use red/green TDD for all development.
- Tests MUST cover the functionality being implemented.
- NEVER ignore the output of the system or the tests — logs and messages often contain CRITICAL information.
- Test output MUST be pristine to pass. No unexpected warnings or errors in output.
- If logs are supposed to contain errors, capture and assert on them.
- Tests must cover affected functionality at the appropriate level (unit, integration, and/or E2E). All three are expected for feature work; smaller changes should test at whatever level is meaningful.

## Workflow

- Use the OpenSpec workflow in `openspec/` for structured changes.
- **Worktrees**: After creating a git worktree, copy `.env` from the main repo root into the worktree root so that tests, previews, and builds work as expected. When working in worktrees, only copy `.env` (not `.env.production`) to the worktree.