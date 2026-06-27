# Claude Code Project Instruction Snippet

Copy this into the relevant `CLAUDE.md` section when you want Claude Code to use Paper Operators for article illustration planning or image prompts.

```markdown
## Paper Operators

When the user asks for article illustrations, blog figures, WeChat article images, explainer visuals, or concept images, use the Paper Operators workflow.

Default to Chinese if the user writes Chinese.

Follow this chain:

1. Identify the source anchor from the article.
2. Write the reader takeaway.
3. Choose the domain and mood.
4. Decide whether a paper operator is necessary.
5. Use the inclusion test: what breaks if the operator is removed?
6. Choose a paper-world scene and operator action.
7. Write readable labels.
8. Produce the final image prompt or plan.
9. QA against clarity, action, label readability, and style drift.

The operator's face is plain by default, or carries one simple hand-drawn expression (a few line strokes, profile or three-quarter, looking at the work) when it encodes the operator's state — never realistic, never head-on, never a cute grin at the reader. Stage relationships as deep 3D paper scenes (material arrangement + line/loop guidance + operator state), not flat paper-textured chart icons.

Do not create generic mascots, robots, stick figures, stock infographic icons, PPT flowcharts, Xiaohei-like black figures, fake text, or decorative characters that do not help comprehension.

For the full portable guide, reference `agent-guides/paper-operators-agent.md`.
```
