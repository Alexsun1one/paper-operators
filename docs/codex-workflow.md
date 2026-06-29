# Codex Workflow

Paper Operators is an open-source visual reasoning skill for turning essays, book chapters, product ideas, and complex systems into tactile paper-stage illustrations.

The repository is intentionally shaped as a Codex-native workflow, not a loose prompt collection. The maintainable unit is the loop:

```text
source text -> visual reasoning -> final image prompt -> Codex render -> artifact review -> rule update -> public example
```

## What Codex Does

Codex is used as the maintainer workstation for this project:

- read and revise the Skill files
- plan figures from long-form writing
- generate final image prompts
- render showcase images
- inspect the generated assets
- update README examples and agent guides
- keep Codex, Claude Code, Cursor, and portable-agent instructions aligned

The most important part is the feedback loop. When an image looks generic, has weak text, or fails to match the article, the fix is written back into the workflow as a rule, reference, prompt template, or QA check.

## Why This Is Useful OSS

Most people can ask an image model for "an illustration," but they struggle to get a picture that actually explains an idea. Paper Operators gives them a reusable method:

1. find the source anchor
2. name the relationship
3. decide whether a paper operator is necessary
4. choose a content-specific metaphor world
5. encode state and labels
6. render
7. run QA and the Swap Test

That makes the output more teachable than a gallery of nice prompts. A writer, teacher, newsletter author, indie builder, or product person can reuse the method on their own material.

## Cross-Agent Path

Paper Operators is a Codex Skill, but the workflow also ships as portable instructions:

- Codex: install `paper-operators/` into `~/.codex/skills/paper-operators`
- Claude Code: use `agent-guides/claude-code.md`
- Cursor: use `agent-guides/cursor-rule.mdc`
- Other agents: use `agent-guides/paper-operators-agent.md`

The planning workflow transfers across tools. Final rendering quality depends on the available image model. In testing for this project, Codex has produced the strongest full-image results: paper texture, object depth, readable labels, and clear operator action.

## What More OpenAI Support Would Unlock

API credits and extended Codex access would be used for public-facing OSS work:

- build a wider example gallery from real essays, books, product notes, and educational explainers
- publish more failure-to-rule writeups, so people see how generic images become precise ones
- add more smoke tests for cross-agent compatibility
- maintain English and Chinese docs with matched examples
- improve label reliability, series consistency, and prompt-to-image QA

The goal is not to produce a private art style. The goal is to make a reusable method for visual reasoning with AI images.

## Current Public Evidence

- Public repo: <https://github.com/Alexsun1one/paper-operators>
- Installable Codex Skill: `paper-operators/SKILL.md`
- Portable agent guide: `agent-guides/paper-operators-agent.md`
- Showcase originals: `examples/images/showcase/`
- README previews: `examples/images/readme/`
- QA rules: `paper-operators/references/qa-checklist.md`

