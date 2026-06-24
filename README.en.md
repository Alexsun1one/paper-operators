# Paper Operators

> A Chinese-first agent workflow for turning article ideas into clear, tactile, paper-stage illustrations.

[中文](README.md)

Paper Operators is built for people who write, explain, publish, teach, ship products, or make sense of complicated ideas. It turns an abstract sentence into a 16:9 article illustration where a small faceless paper person physically performs the core action: framing, lighting, routing, inspecting, filtering, caring, weighing, archiving, or repairing.

This repository includes a ready-to-install Codex Skill, but the method is not Codex-only. Claude Code, Cursor, Hermes Agent, OpenClaw, or any agent tool that supports project rules, custom instructions, or workflow prompts can use the same guide.

It is not a mascot pack. It is a visual thinking tool.

<p align="center">
  <img src="examples/images/readme/06-materials-before-conclusion.jpg" alt="Lay out the material before drawing conclusions" width="100%">
</p>

## What This Skill Does

- Finds the sentence, conflict, turn, or judgment in an article that is worth visualizing.
- Chooses a paper-world metaphor that matches the domain: art, culture, life, product, business, engineering, AI, education, or psychology.
- Uses paper operators only when their action improves comprehension.
- Produces readable Chinese or English labels by default, instead of empty label boxes.
- Keeps a consistent visual language across a whole article package without making every image look the same.

The rule is simple: if removing the paper operator does not weaken the image, the operator should not be there.

## Gallery

<table>
  <tr>
    <td width="50%">
      <img src="examples/images/readme/01-readable-chinese-route.jpg" alt="Readable Chinese route" width="100%">
      <br>
      <sub><strong>Readable Chinese route.</strong> Claim, relation, state, text, and outcome unfold along one path.</sub>
    </td>
    <td width="50%">
      <img src="examples/images/readme/02-aerial-paper-stage-hero.jpg" alt="High-angle paper stage" width="100%">
      <br>
      <sub><strong>High-angle paper stage.</strong> Good for systems, products, routes, cities, and multi-object scenes.</sub>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <img src="examples/images/readme/03-art-attention-frame.jpg" alt="Art attention frame" width="100%">
      <br>
      <sub><strong>Art and attention.</strong> Paper operators become frame setters, light catchers, and color tuners.</sub>
    </td>
    <td width="50%">
      <img src="examples/images/readme/04-life-boundary-room.jpg" alt="Life boundary room" width="100%">
      <br>
      <sub><strong>Life and psychology.</strong> Boundaries, care, memory, and emotional weather become rooms and paper objects.</sub>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <img src="examples/images/readme/05-ai-town-systems.jpg" alt="AI town systems" width="100%">
      <br>
      <sub><strong>Product, AI, and systems.</strong> Routes, teams, checkpoints, and evidence become a readable tabletop world.</sub>
    </td>
    <td width="50%">
      <img src="examples/images/readme/07-chat-copilot-agent.jpg" alt="From Q&A to delegated work" width="100%">
      <br>
      <sub><strong>From Q&A to delegated work.</strong> Chat, Copilot, and Agent differ by work loop, not by naming.</sub>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <img src="examples/images/readme/08-agent-launch-six-forces.jpg" alt="Agent launch with six forces" width="100%">
      <br>
      <sub><strong>Agents entering the field.</strong> It is not one horse; models, context, tools, ecosystem, cost, and enterprise demand move together.</sub>
    </td>
    <td width="50%">
      <img src="examples/images/readme/09-agent-service-results.jpg" alt="From old SaaS to agent service outcomes" width="100%">
      <br>
      <sub><strong>Agent service outcomes.</strong> The table shifts from using tools to buying results.</sub>
    </td>
  </tr>
</table>

Note: the images shown in this README are compressed previews for faster GitHub loading. They do not represent the full sharpness of the generated originals. Earlier PNG examples remain in [`examples/images/`](examples/images/), while the new homepage examples live in `examples/images/readme/`.

## Why It Exists

Most AI-generated article images fail in one of two ways: they are pretty but vague, or they are clear but look like a slide deck.

Paper Operators tries to sit in the better middle:

- clear enough to explain the idea in three seconds
- warm enough that readers want to keep looking
- structured enough to support long-form writing
- distinctive enough to make a publication feel owned

The style borrows the discipline of diagrams, the warmth of paper craft, and the editorial restraint of a good magazine figure. It does not copy Xiaohei-style black figures, white-dot eyes, blob mascots, generic stick people, robots, stock icons, or PPT infographics.

## When To Use It

Use Paper Operators for:

- WeChat articles, blogs, newsletters, and long-form essays
- product thinking, AI workflows, business judgment, engineering notes
- art criticism, cultural essays, personal writing, psychology, education
- explainers that need more humanity than arrows and boxes
- visual packages where several images should feel related

Avoid it when:

- the image only needs a logo, icon, sticker, or decorative mascot
- a simple chart or screenshot would explain the point better
- the operator would stand beside the idea instead of acting on it

## How It Works

1. Pick one source anchor from the article.
2. Decide what the reader should understand after seeing the image.
3. Choose the domain and mood.
4. Select a paper operator family.
5. Answer `what breaks if removed`.
6. Choose a scene: gallery table, boundary room, paper town, archive desk, route map, cutaway, shelf matrix, or another paper-world setup.
7. Add readable labels in the user's language.
8. Generate one image, then check clarity, action, text, composition, and style drift.

Planning output includes:

```text
source anchor:
reader takeaway:
domain and mood:
core action:
operator decision:
what breaks if removed:
operator family:
metaphor world:
composition:
labels:
final image prompt:
QA risks:
```

## Integrations

### Codex

Copy the Skill directory into your Codex skills folder:

```bash
mkdir -p ~/.codex/skills
cp -R paper-operators ~/.codex/skills/paper-operators
```

Restart Codex, then call it by name:

```text
Use $paper-operators to plan three article body illustrations for this essay. Do not generate images yet.
```

Or generate one image directly:

```text
Use $paper-operators to generate a 16:9 article body illustration from the paragraph below.

Text:
Good taste is not decoration. It is placing attention in the right place.
```

### Other Agent Tools

If you use Claude Code, Cursor, Hermes Agent, OpenClaw, or another agent tool, you do not need to force it into the Codex Skill format.

Use this portable instruction pack:

[`agent-guides/paper-operators-agent.md`](agent-guides/paper-operators-agent.md)

Suggested mapping:

| Tool | How to use it |
| --- | --- |
| Claude Code | Use [`agent-guides/claude-code.md`](agent-guides/claude-code.md), or paste the portable guide into the relevant `CLAUDE.md` section. |
| Cursor | Use [`agent-guides/cursor-rule.mdc`](agent-guides/cursor-rule.mdc), or adapt the portable guide into a project rule. |
| Hermes Agent | Use it as a reusable workflow prompt / agent instruction. |
| OpenClaw | Use it as a custom workflow or project-level agent instruction. |
| Other agents | Paste it wherever the tool accepts system, project, or task instructions. |

The important chain is: `source anchor -> reader takeaway -> operator inclusion test -> domain adaptation -> final prompt -> QA`.

Hermes Agent and OpenClaw should be able to use this method as long as they can read or paste ordinary project instructions. Give them [`agent-guides/paper-operators-agent.md`](agent-guides/paper-operators-agent.md) as a workflow prompt or project-level instruction. They do not need to understand the Codex Skill package format to perform article analysis, composition planning, label design, and final prompt generation.

Important: what transfers across agents is the analysis, composition, and prompt workflow. Final image quality still depends on the image model. Claude Code, Cursor, Hermes Agent, and OpenClaw can plan the figure and produce the final renderer prompt; if they do not have a strong image model available, hand that prompt to a better renderer. See [`agent-guides/compatibility.md`](agent-guides/compatibility.md), and use [`agent-guides/smoke-test.md`](agent-guides/smoke-test.md) to check whether a new agent actually follows the workflow.

## Example Prompts

Plan an article package:

```text
Use $paper-operators to plan three article body illustrations for the following essay. Do not generate images yet.

Requirements:
- Chinese readers first
- For each image, include source anchor, reader takeaway, operator family, and what breaks if removed
- At least one image should not be an engineering/product diagram; adapt it to the essay's domain

Essay:
{paste article}
```

Generate a product or AI system image:

```text
Use $paper-operators to generate a product / AI system illustration.

Source anchor:
I am not asking one AI. I am organizing a group of AIs to complete a verifiable route.

Requirements:
- operator family: Thread Runner + Lens Keeper
- high-angle paper town / workbench
- a blue route from idea to AI team, checkpoint, and launch scene
- include short Chinese labels: 想法, 团队, 校验, 上线
```

Generate an art essay image:

```text
Use $paper-operators to generate an art criticism illustration.

Source anchor:
Good taste is not decoration. It is placing attention in the right place.

Requirements:
- operator family: Frame Setter / Light Catcher
- gallery workbench, frame placement, light card, color swatches, quiet negative space
- do not turn it into a flowchart, funnel, or node network
```

More examples live in [`examples/prompts.md`](examples/prompts.md).

## Follow The Work

This repository contains the reusable Skill and examples. Longer breakdowns, prompt notes, article illustration reviews, AI writing practice, and product work will continue on my WeChat official account.

If you care about making AI images less generic, making article judgment visible, and turning agent workflows into reusable systems, search for 「正在逐渐AI化」 on WeChat.

<p align="center">
  <img src="assets/wechat-official-account.png" alt="WeChat search: 正在逐渐AI化" width="720">
</p>

## Repository

```text
paper-operators/
├── README.md
├── README.en.md
├── LICENSE
├── NOTICE.md
├── assets/
│   └── wechat-official-account.png
├── agent-guides/
│   ├── claude-code.md
│   ├── compatibility.md
│   ├── cursor-rule.mdc
│   ├── README.md
│   ├── paper-operators-agent.md
│   └── smoke-test.md
├── examples/
│   ├── prompts.md
│   └── images/
│       └── readme/
├── docs/
│   └── style-notes.md
└── paper-operators/
    ├── SKILL.md
    ├── agents/openai.yaml
    ├── references/
    └── assets/examples/
```

The outer repository is for people reading the project and for portable agent instructions. The inner `paper-operators/` directory is the ready-to-install Codex Skill.

## License

MIT. See [`LICENSE`](LICENSE).
