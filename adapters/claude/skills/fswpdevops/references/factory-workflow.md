# Agent factory workflow

A loop where an agent builds and automated checks decide. Use it when an agent writes the change. Humans own the issue and the approval.

## Loop

1. **Issue first.** Every change starts as a written issue: the problem, then acceptance criteria (how we know it is fixed). No issue, no work. Keep issues small and well described.
2. **Tests first.** Write or name the tests that prove each criterion before any code. Use what the repo already runs: PHPCS, PHPUnit, Plugin Check, a block or e2e test. The merge gate only knows what the tests know, so a criterion with no test is not covered; say so in the issue.
3. **Own worktree and branch.** The agent works in its own worktree on its own branch, then opens a PR that links the issue.
4. **CI runs the tests.** On failure the result goes back to the agent to fix. Allow a bounded number of tries (default 3), then stop and report what failed and what was tried.
5. **Merge gate.** Merge only when all three hold: tests passed, review approved, scope matches the issue (nothing extra, nothing missing).
6. **Human review on every PR.** Whoever requested the change is not the one who approves it. No PR merges without a review, and no setup skips review.
7. **Holdout scenarios (optional, larger work).** Acceptance tests the building agent never sees, kept with the reviewer and run against the PR. A failure goes back as a plain description of the broken behaviour, not the test itself.
8. **Start small.** One agent, small issues, review always on. Add agents or holdouts only after the small loop runs cleanly.

## Issue template

```
Problem: what is wrong or missing, for whom
Acceptance criteria:
- [ ] criterion, each checkable by a test
Tests: file or command that proves each criterion
Out of scope: what this change must not touch
```
