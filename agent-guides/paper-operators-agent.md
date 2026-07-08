# Paper Operators Portable Agent Guide

Use this guide when an agent tool does not support Codex Skills directly.

You can paste it into a project instruction file, custom agent prompt, Cursor rule, Claude Code project note, Hermes Agent instruction, OpenClaw workflow, or any other agent system that can read repository guidance.

This guide is plain Markdown on purpose. It does not depend on Codex Skill metadata, `$paper-operators` syntax, MCP tools, a specific image model, or any particular agent runtime.

## Mission

Turn essays, books, stories, systems, reports, and evidence into clear, tactile, paper-stage visual cards.

The image should show a folded-paper operator physically performing the source's core conceptual action: framing, lighting, routing, inspecting, filtering, caring, weighing, archiving, repairing, or transforming.

This is not a mascot style. The operator is useful only when the action helps the reader understand the idea.

## Default Language

Use Chinese by default when the user writes Chinese.

Use English when the user writes English or explicitly asks for English output.

## Workflow

1. Read the article, excerpt, topic, or image request.
2. Pick one source anchor: a sentence, conflict, turn, claim, tension, or feeling worth visualizing.
3. State the reader takeaway in one sentence.
4. Route the asset: article figure, story/book card, data story scene, center illustration, or reference-informed explainer. Decide final container, display ratio, text ownership, exact truth constraints, and whether another tool should own the job.
5. For stories/books, identify protagonist, conflict, turning point, choice, consequence, and transformation. For data scenes, write exact labels and values before prompting. For scientific, historical, brand, artifact, or other visually specific topics, gather stable factual/visual cues before prompting.
6. Choose the domain and mood: art, culture, life, product, business, engineering, AI, education, psychology, history, finance, or another field.
7. Choose the core action: pull, frame, reveal, block, tune, fold, sort, mend, weigh, arrange, carry, shelter, distill, balance, light, archive, or transform.
8. Run the inclusion test:

```text
paper operator:
- use operator: yes/no
- source anchor:
- domain:
- relationship type:
- core action:
- object acted on:
- relation clarified:
- what breaks if removed:
- operator family:
- forbidden drift:
```

9. Use a paper operator only if `what breaks if removed` is concrete.
10. Build a high-angle paper-model scene with readable labels. Keep headlines, long explanations, citations, and platform-specific text outside the image unless the image truly owns them.
11. When the piece needs more than one image, plan them as a connected series (see Depth Layers).
12. Generate or plan one image at a time.
13. Check the output against the QA rules below, including truth constraints and failure patterns.

If the current agent cannot generate images, stop at the final image prompt and clearly say which image model or renderer should receive it.

## Visual DNA

- 16:9 horizontal article body image by default.
- High-angle tabletop paper-model scene.
- Folded-paper people, no black blob body. The face is plain by default, or carries one simple hand-drawn expression (a few line strokes for brows/eyes and mouth, profile or three-quarter, looking at the work) when it encodes the operator's state — effort, focus, strain, relief, care. Keep it abstract to avoid the uncanny valley; never realistic, never head-on, never Xiaohei white-dot eyes.
- Tactile paper, card tabs, trays, labels, gates, frames, ribbons, shelves, boxes, folders, scales, lenses, light cards.
- Stage relationships as deep 3D paper scenes — material arrangement, line or loop guidance, and operator state — not as flat paper-textured chart icons.
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

## Depth Layers

These ideas give the method its depth. The full reference files live in the repo, but the concepts travel on their own.

- **Asset routing and truth.** Decide whether this is an article figure, story/book card, data story scene, center illustration, or reference-informed explainer. Record final container, display ratio, text ownership, exact data/label/reference constraints, and whether another tool should own the job. (Full guide: `paper-operators/references/asset-routing-and-truth.md`.)
- **Relationship first.** Before choosing an operator, name the exact relationship the image must show: connection, sequence, dependency, causality, feedback loop, contrast, tradeoff, hierarchy, transformation, boundary, divergence, or tension. Then render its direction, condition, and state. This is what stops an image from collapsing into a generic left-to-right arrow. (Full grammar: `paper-operators/references/relationship-grammar.md`.)
- **Story cards, data stories, reference explainers.** For stories/books, show protagonist, conflict, choice, consequence, and transformation; for data, preserve exact values while showing implication; for science/history/brands/artifacts, gather stable cues before prompting. (Full guides: `story-card-grammar.md`, `data-story-scenes.md`, `reference-informed-explainers.md`.)
- **Primitives as the kit.** Build every scene from a known set of paper parts — carriers and paths, surfaces and holders, enclosures and boundaries, optics and light, measures and tools, state containers, and label containers. One primitive carries one meaning; reuse the same primitive for the same meaning so a set of images feels like one world. (Full kit: `paper-operators/references/primitives.md`.)
- **State coding for precision.** Show status, degree, and quality without extra text: color semantics, path thickness and texture, elevation, gate posture, edge condition, light, and degree. Keep an encoding budget — pick the one or two encodings that carry the point and let the rest stay neutral. (Full system: `paper-operators/references/state-coding.md`.)
- **Series for chaining.** When an article needs several images, chain them into one argument: keep the operator, palette, and label style constant, advance one throughline ribbon across the set, and introduce a small motif early that pays off at the end. (Full guide: `paper-operators/references/series-and-chaining.md`; worked examples: `examples/series-prompts.md`.)

These layers compose: pick the relationship, render it with primitives and state coding, and when there are multiple images, chain them with a shared throughline.

A further layer keeps the output from going stale (`paper-operators/references/intent-reading.md`, `creative-divergence.md`, `composition-modes.md`, `variation-engine.md`): read what THIS document actually wants (audience, feeling, stance, the one sentence to keep), diverge the metaphor before defaulting, choose the right composition (a single dense image with several beats — like four river crossings on one map — vs a series), and build each image around its own content. Apply the **Swap Test**: if the image could move onto a different article on the same topic without anyone noticing, it is not precise enough — regenerate. The drift from first-use "wow" to repeated-use "boring" is a precision failure, not a style problem.

## Output Contract

For planning, return:

```text
source anchor:
reader takeaway:
asset role:
final container and display ratio:
text ownership:
truth constraints and reference needs:
domain and mood:
core action:
operator decision:
what breaks if removed:
operator family:
metaphor world:
composition:
labels:
final image prompt:
prompt record (for public/reusable assets):
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
- Exact data, names, scientific parts, historical cues, or reference-specific objects are wrong or invented.
- The image contains a title, paragraph, citation, or long legend that should belong to the outer layout.
- The main path, state change, or reader takeaway is unclear.
- The scene uses engineering props for a non-engineering article without a reason.
- The image is charming but does not explain the source anchor.

Pass only when:

- The source anchor is visible in the image logic.
- The action is physically legible.
- The labels help instead of clutter.
- A reader can understand the main idea in about three seconds.
- The image feels like a paper-stage article illustration, not a generic AI graphic.
