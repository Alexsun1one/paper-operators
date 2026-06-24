# Paper Operators Portable Agent Guide

Use this guide when an agent tool does not support Codex Skills directly.

You can paste it into a project instruction file, custom agent prompt, Cursor rule, Claude Code project note, Hermes Agent instruction, OpenClaw workflow, or any other agent system that can read repository guidance.

This guide is plain Markdown on purpose. It does not depend on Codex Skill metadata, `$paper-operators` syntax, MCP tools, a specific image model, or any particular agent runtime.

## Mission

Turn article ideas into clear, tactile, paper-stage illustrations.

The image should show a faceless folded-paper operator physically performing the article's core conceptual action: framing, lighting, routing, inspecting, filtering, caring, weighing, archiving, repairing, or transforming.

This is not a mascot style. The operator is useful only when the action helps the reader understand the idea.

## Default Language

Use Chinese by default when the user writes Chinese.

Use English when the user writes English or explicitly asks for English output.

## Workflow

1. Read the article, excerpt, topic, or image request.
2. Pick one source anchor: a sentence, conflict, turn, claim, tension, or feeling worth visualizing.
3. State the reader takeaway in one sentence.
4. Choose the domain and mood: art, culture, life, product, business, engineering, AI, education, psychology, history, finance, or another field.
5. Choose the core action: pull, frame, reveal, block, tune, fold, sort, mend, weigh, arrange, carry, shelter, distill, balance, light, archive, or transform.
6. Run the inclusion test:

```text
paper operator:
- use operator: yes/no
- source anchor:
- domain:
- core action:
- object acted on:
- relation clarified:
- what breaks if removed:
- operator family:
- forbidden drift:
```

7. Use a paper operator only if `what breaks if removed` is concrete.
8. Build a high-angle paper-model scene with readable labels.
9. Generate or plan one image at a time.
10. Check the output against the QA rules below.

If the current agent cannot generate images, stop at the final image prompt and clearly say which image model or renderer should receive it.

## Visual DNA

- 16:9 horizontal article body image by default.
- High-angle tabletop paper-model scene.
- Faceless folded-paper people: no eyes, no mouth, no black blob body.
- Tactile paper, card tabs, trays, labels, gates, frames, ribbons, shelves, boxes, folders, scales, lenses, light cards.
- A blue carrier ribbon/path can guide the reader through the image.
- Use readable labels by default.
- For simple Chinese figures, use 3-6 short labels.
- For complex figures, use more labels only when they clarify paths, states, contrasts, or groups.
- One readable sentence strip is allowed when it sharpens the takeaway.
- Avoid dense paragraphs, fake tiny text, PPT flowcharts, stock icons, generic robots, mascots, and Xiaohei-like black figures.

## Domain Adaptation

For art or design writing, use frame setters, light catchers, color tuners, gallery tables, plinths, frames, light cards, and color strips.

For personal essays or psychology writing, use boundary rooms, folded memories, weather cards, soft screens, chairs, notes, and care folders.

For product, business, or AI writing, use route runners, lens keepers, gates, scales, check trays, task boards, model cards, and result boxes.

For engineering or systems writing, use cutaways, bridges, relay paths, failure branches, repair loops, evidence trays, and interface cards.

Always let the article choose the operator's tool and world. Do not force engineering props into art, culture, life, or emotional essays.

## Output Contract

For planning, return:

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

For prompt-only agents, return the same planning block plus a final renderer prompt.

For agents with image generation, produce one image at a time and report:

```text
image path:
intended placement:
one-line purpose:
QA result:
```

## Renderer Handoff

When another tool will render the image, pass this compact handoff:

```text
renderer task:
- aspect ratio: 16:9 horizontal
- source anchor:
- reader takeaway:
- paper operator action:
- scene:
- labels:
- style DNA:
- forbidden drift:
- final prompt:
```

Prefer a strong image model for final rendering. Weaker models can still use the workflow, but should reduce text density, use fewer labels, or leave blank label containers for post-production typography.

## QA Rules

Regenerate or revise if:

- The paper operator is decorative.
- Removing the operator would not weaken comprehension.
- The image becomes a generic mascot, robot, stick figure, PPT chart, or stock infographic.
- The labels are missing, unreadable, fake, or floating without objects.
- The main path, state change, or reader takeaway is unclear.
- The scene uses engineering props for a non-engineering article without a reason.
- The image is charming but does not explain the source anchor.

Pass only when:

- The source anchor is visible in the image logic.
- The action is physically legible.
- The labels help instead of clutter.
- A reader can understand the main idea in about three seconds.
- The image feels like a paper-stage article illustration, not a generic AI graphic.
