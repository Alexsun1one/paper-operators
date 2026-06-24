# Agent Integration Guides

Paper Operators is packaged as a Codex Skill, but the method is portable.

Use [`paper-operators-agent.md`](paper-operators-agent.md) as the generic instruction pack for tools that do not understand Codex Skills directly.

This directory also includes:

- [`claude-code.md`](claude-code.md): a compact snippet you can paste into `CLAUDE.md`.
- [`cursor-rule.mdc`](cursor-rule.mdc): a project rule template for Cursor.

## Suggested Mapping

| Tool | How to use Paper Operators |
| --- | --- |
| Codex | Install `paper-operators/` into `~/.codex/skills/paper-operators`. |
| Claude Code | Paste [`claude-code.md`](claude-code.md) into the relevant `CLAUDE.md` section, or reference the full portable guide. |
| Cursor | Copy [`cursor-rule.mdc`](cursor-rule.mdc) into `.cursor/rules/paper-operators.mdc`, or adapt the full portable guide. |
| Hermes Agent | Use the guide as a reusable agent instruction/workflow prompt. |
| OpenClaw | Use the guide as a custom workflow or project-level agent instruction. |
| Other agents | Use the guide anywhere the agent accepts system, project, or task instructions. |

The important part is not the tool name. The important part is that the agent follows the same workflow: source anchor, reader takeaway, operator inclusion test, domain adaptation, final prompt, and QA.
