# AGENTS

This file outlines how AI agents interact with the repository.

- **Codex Setup:** Refer to `docs/CODEX_SETUP.md` for context initialization.
- **Workflow:** Agents should follow `docs/AI_DEVELOPMENT_WORKFLOW.md`.
- Agents must NOT commit directly to main.
- Follow Conventional Commits.
- Include proper tests and lint checks (once implemented) before requesting reviews.

## Working with other agents

Three agents work on this project: Claude Code, Codex and Antigravity. All three read this file (Claude through `CLAUDE.md`).

- The agent given the task is the lead. Only the lead edits files, and it chooses another agent for a read-only review when a second view helps.
- Before starting, the lead reads `HANDOFF.md`. Before stopping, it adds an entry: what it did, what is unfinished, what the next agent should check.
- Reviewers return their feedback as text and edit nothing, including `HANDOFF.md`.
- Each agent can be asked for a review from the terminal (run from the project root; the commands are launchers in `~/.local/bin`):
  - Claude: `claude -p "<prompt>" < /dev/null`
  - Codex: `codex exec --sandbox read-only "<prompt>"`
  - Antigravity: `agy -p "<prompt>"`
