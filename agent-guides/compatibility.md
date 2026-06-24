# Compatibility Notes

Paper Operators has two layers:

1. **Workflow layer**: article analysis, source anchor selection, operator inclusion test, composition, labels, final prompt, and QA.
2. **Rendering layer**: the image model that turns the final prompt into pixels.

The workflow layer is portable across agent tools. The rendering layer depends on the image model.

## Portable Files

These files are intentionally tool-neutral:

- `agent-guides/paper-operators-agent.md`
- `examples/prompts.md` after replacing `$paper-operators` with a plain instruction such as `请按 Paper Operators 工作流处理`

They are plain Markdown and do not require Codex Skill metadata, frontmatter, custom commands, MCP, or a specific runtime.

## Tool-Specific Files

These files are adapters:

- `paper-operators/`: Codex Skill package.
- `agent-guides/claude-code.md`: snippet for `CLAUDE.md`.
- `agent-guides/cursor-rule.mdc`: Cursor rule template with Cursor-style frontmatter.

Hermes Agent, OpenClaw, and other agent systems should be able to use `paper-operators-agent.md` as a project instruction or workflow prompt unless they publish a stricter package format. They do not need to understand Codex Skill metadata to use the method.

For Hermes Agent and OpenClaw, treat Paper Operators as:

- a reusable workflow prompt
- a project-level instruction
- a planning layer that produces figure specs and final renderer prompts

Then send the final prompt to whatever image renderer that agent can call.

## Expected Behavior In Other Agents

A compatible agent should be able to:

- keep Chinese output when the user writes Chinese
- identify a source anchor from article text
- answer `what breaks if removed`
- choose a domain-specific paper operator
- write a final image prompt
- avoid generic mascots, PPT charts, stock icons, robots, and Xiaohei-like figures
- hand off to an image renderer if it cannot generate images itself

## Rendering Quality

The final image quality depends on the renderer.

Strong image models can usually handle the full Paper Operators style, including paper texture, readable labels, high-angle composition, and operator action.

Weaker image models may need a reduced version:

- fewer labels
- simpler composition
- blank label containers for later typography
- one operator and one action
- post-production text overlay in Figma, Canva, Photoshop, Pillow, or another layout tool

Do not judge the workflow only by a weak renderer's first image. Judge whether the agent produced a clear source anchor, action, composition, label plan, and QA risks.
