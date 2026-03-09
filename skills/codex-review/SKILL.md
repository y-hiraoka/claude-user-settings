---
name: codex-review
description: Request a code review from Codex CLI. If the user indicates they would like a code review using Codex, you should execute this skill.
---

## How to Request a Code Review in Codex

Based on the user's instructions and the flow of the conversation, determine which differences you want Codex to review and specify the CLI options accordingly.

- Review uncommitted changes

  ```bash
  codex review --uncommitted
  ```

- Review the differences between the current branch and a specific base branch

  ```bash
  codex review --base some/branch
  ```

- Review the differences between two specific branches

  ```bash
  codex review "Review differences between branch-a and branch-b."
  ```

## Fix the problem

Codex assigns the following priority levels as a result of the review:

- [P0] Critical
- [P1] High
- [P2] Moderate
- [P3] Low
- [P4] Negligible

As a rule, you should act as follows for each priority level:

- [P0] Start fixing the problem immediately
- [P1] Inform the user about the problem and ask if they want to fix it
- [P2] Inform the user about the problem and ask if they want to fix it
- [P3] Just inform the user about the problem
- [P4] Just inform the user about the problem
