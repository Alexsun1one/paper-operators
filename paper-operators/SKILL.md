---
name: paper-operators
description: Generate or plan publish-grade 16:9 article illustrations using faceless folded-paper action characters, with Chinese-first article/body-image workflows. Use when a user wants Chinese or English article illustrations, blog figures, explainer visuals, social/article images, or concept images where a small paper person should physically perform the core idea. Especially useful for turning abstract claims, emotions, cultural ideas, art criticism, product thinking, systems, workflows, tensions, boundaries, transformations, relationships, and evidence into clear high-angle paper-model scenes, as single figures or chained multi-image series. Do not use for generic mascots, cute stickers, Xiaohei-style black figures, stock PPT infographics, or image requests where no action character helps comprehension.
---

# Paper Operators / 纸片人

Paper Operators turns an article idea into a tactile paper-stage illustration where a small faceless paper person performs the core conceptual action.

默认面向中文文章配图；用户使用英文时再切换英文输出。Use this skill to create a consistent article-illustration style: paper people, physical metaphors, readable labels, clear reader paths, and domain-aware tools. The character is never decoration. If removing the paper operator does not weaken the image, do not use one.

## Workflow

1. Read the article, excerpt, topic, or image-edit request.
2. Identify one source anchor: the sentence, paragraph, claim, tension, turn, or feeling that deserves a visual.
3. Name the core relationship the image must show, using `references/relationship-grammar.md`: connection, sequence, dependency, causality, feedback, contrast, tradeoff, hierarchy, transformation, boundary, divergence, or tension. Choose the relationship before the operator; precision comes from rendering the exact relation, direction, condition, and state.
4. Choose the domain and mood: art, culture, personal essay, business, product, engineering, education, psychology, finance, history, lifestyle, or another field.
5. Choose the core action: pull, frame, reveal, block, tune, fold, sort, mend, weigh, arrange, carry, shelter, distill, balance, light, archive, or transform.
6. Decide whether a Paper Operator is necessary using the inclusion test.
7. Select one operator family from `references/operator-library.md` that can physically perform the relationship; use the Operator × Relationship map when unsure.
8. Assemble the scene from the kit in `references/primitives.md`, and encode status, degree, and state precisely with `references/state-coding.md`. Reuse the same primitive for the same meaning so the image stays consistent.
9. Adapt the world, props, palette, texture, and typography using `references/domain-adaptation.md`.
10. Write readable labels in the user's language. For simple Chinese figures, use 3-6 short labels; for complex multi-state figures, use more labels when they clarify paths, states, contrasts, or groups. Prefer short labels, but allow one readable sentence strip when it materially improves comprehension.
11. Build the final image prompt using `references/prompt-template.md`.
12. Generate or edit one image at a time.
13. When the article needs more than one image, plan the set with `references/series-and-chaining.md` so the figures share a world, operator, palette, and a progressing throughline instead of reading as N unrelated pictures.
14. Run QA with `references/qa-checklist.md`; regenerate if the operator is decorative, the style drifts, complexity is unmanaged, labels are missing, the relationship collapses into a generic arrow, or the idea is unclear.
15. For README, portfolio, or showcase images, include at least one non-engineering domain when possible: art, culture, life, psychology, education, food, travel, or personal essays. The skill should not look like it only draws workflows.

## Inclusion Test

Before adding a paper person, answer:

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

Use an operator only when `what breaks if removed` is concrete. Good answers include:

- "The connection path loses agency."
- "The boundary no longer reads as a decision."
- "The hidden layer is no longer being inspected."
- "The artwork no longer feels curated, repaired, tuned, or reframed."

Weak answers include:

- "It looks more fun."
- "It adds personality."
- "It fills empty space."

## Default Style

Read `references/style-dna.md` before generating final images.

Core visual DNA:

- Chinese-first article illustration unless the user asks otherwise
- high-angle tabletop paper-model scene when the user wants the newer polished style
- adaptive complexity: choose the simplest sufficient form, but allow complex multi-state scenes when the article needs them and the path/status system stays clear
- mandatory readable labels by default: short Chinese/English labels attached to objects; use 3-6 for simple figures and more for complex multi-state figures when the extra labels make the route clearer
- faceless folded-paper people, no eyes, no mouth
- off-white paper body, charcoal outline, small semantic color tabs
- tactile paper, translucent tools, light shadows, quiet editorial composition
- flowing blue carrier ribbon/path for the main reader route when useful
- labels arranged as tabs, plaques, hang tags, gallery captions, route signs, sentence strips, or stitched cards; do not leave the image text-empty
- one paper operator, one tool, one core action
- 16:9 horizontal article body image by default
- generous margins and clear focal hierarchy
- concise Chinese or English labels attached to objects
- no Xiaohei-like black blob body, white-dot eyes, tiny thin legs, or deadpan monster identity
- no generic stick figure, robot, avatar, office worker, mascot sticker, or PPT icon set

## Domain Adaptation

Paper Operators are not only for engineering diagrams.

For an art article, the operator may hang a frame, tune a color strip, hold a light card, restore a torn composition, arrange plinths, or reveal a hidden brush rhythm.

For a personal essay, the operator may fold a memory, carry a small weather panel, shelter a fragile note, untangle a ribbon of choices, or place an empty chair.

For business or product writing, the operator may route a carrier line, filter a funnel, weigh a tradeoff, stack a roadmap, or stamp a decision.

For technical writing, the operator may inspect a cutaway, bridge a handoff, block a failure branch, or repair a loop.

Always let the article choose the operator's tool and world. Do not force engineering props into art, culture, life, or emotional essays.

## Depth Layers

Four references give the skill its depth. Reach for them in this order.

- **Relationship first** (`references/relationship-grammar.md`): name the exact relationship the image must show, then render its direction, condition, and state. This is what stops every image from collapsing into a generic left-to-right arrow. A precise relationship is the difference between "two things with a line" and "B depends on A, and breaks without it."
- **Primitives as the kit** (`references/primitives.md`): build every scene from a known set of paper parts — carriers, surfaces, enclosures, optics, measures, state containers, label containers, and the paper-person construction kit. One primitive carries one meaning; reuse the same primitive for the same meaning so a set of images feels like one world.
- **State coding for precision** (`references/state-coding.md`): show status, degree, and quality without extra text — color semantics, path thickness and texture, elevation, gate posture, edge condition, light, and degree. Keep an encoding budget: pick the one or two encodings that carry the article's precision and let the rest stay neutral.
- **Series for chaining** (`references/series-and-chaining.md`): when an article needs several images, chain them into one argument. Keep the operator, palette, and label style constant; advance one throughline ribbon across the set; introduce a small motif early and pay it off at the end.

These layers compose: pick the relationship, render it with primitives and state coding, and when there are multiple images, chain them with a shared throughline.

## Output Contract

For planning, return:

```text
source anchor:
reader takeaway:
domain and mood:
relationship type:
core action:
operator decision:
what breaks if removed:
operator family:
metaphor world:
primitives and state coding:
composition:
labels (mandatory; 3-6 for simple figures, more when complex states/paths/groups need them; optional one-sentence strip if helpful):
series plan (only when planning more than one image):
final image prompt:
QA risks:
```

For generation, produce one image at a time and report:

- image path
- intended placement
- one-line purpose
- native label status: confirm whether labels/sentence strips are rendered inside the image, intentionally omitted, or externally overlaid because the user requested post-production
- whether it passes QA or needs regeneration

## References

- `references/style-dna.md`: the visual identity and anti-copy rules.
- `references/relationship-grammar.md`: the 12 relationship families, their visual encoding, and how to render them precisely instead of as generic arrows.
- `references/operator-library.md`: operator families, action verbs, and the Operator × Relationship map.
- `references/primitives.md`: the composable kit of atomic paper parts, label containers, and the paper-person construction kit.
- `references/state-coding.md`: the precise visual encoding system for status, degree, and quality.
- `references/domain-adaptation.md`: how to adapt paper operators to art, culture, life, business, technical, and other topics.
- `references/series-and-chaining.md`: how to chain a set of images into one connected argument with a shared throughline.
- `references/prompt-template.md`: planning and final generation prompt templates.
- `references/qa-checklist.md`: acceptance and regeneration rules.
