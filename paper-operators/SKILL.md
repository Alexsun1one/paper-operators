---
name: paper-operators
description: Generate or plan publish-grade 16:9 article illustrations using faceless folded-paper action characters, with Chinese-first article/body-image workflows. Use when a user wants Chinese or English article illustrations, blog figures, explainer visuals, social/article images, or concept images where a small paper person should physically perform the core idea. Especially useful for turning abstract claims, emotions, cultural ideas, art criticism, product thinking, systems, workflows, tensions, boundaries, transformations, and evidence into clear high-angle paper-model scenes. Do not use for generic mascots, cute stickers, Xiaohei-style black figures, stock PPT infographics, or image requests where no action character helps comprehension.
---

# Paper Operators / 纸片人

Paper Operators turns an article idea into a tactile paper-stage illustration where a small faceless paper person performs the core conceptual action.

默认面向中文文章配图；用户使用英文时再切换英文输出。Use this skill to create a consistent article-illustration style: paper people, physical metaphors, readable labels, clear reader paths, and domain-aware tools. The character is never decoration. If removing the paper operator does not weaken the image, do not use one.

## Workflow

1. Read the article, excerpt, topic, or image-edit request.
2. Identify one source anchor: the sentence, paragraph, claim, tension, turn, or feeling that deserves a visual.
3. Choose the domain and mood: art, culture, personal essay, business, product, engineering, education, psychology, finance, history, lifestyle, or another field.
4. Choose the core action: pull, frame, reveal, block, tune, fold, sort, mend, weigh, arrange, carry, shelter, distill, balance, light, archive, or transform.
5. Decide whether a Paper Operator is necessary using the inclusion test.
6. Select one operator family from `references/operator-library.md`.
7. Adapt the world, props, palette, texture, and typography using `references/domain-adaptation.md`.
8. Write readable labels in the user's language. For simple Chinese figures, use 3-6 short labels; for complex multi-state figures, use more labels when they clarify paths, states, contrasts, or groups. Prefer short labels, but allow one readable sentence strip when it materially improves comprehension.
9. Build the final image prompt using `references/prompt-template.md`.
10. Generate or edit one image at a time.
11. Run QA with `references/qa-checklist.md`; regenerate if the operator is decorative, the style drifts, complexity is unmanaged, labels are missing, or the idea is unclear.
12. For README, portfolio, or showcase images, include at least one non-engineering domain when possible: art, culture, life, psychology, education, food, travel, or personal essays. The skill should not look like it only draws workflows.

## Inclusion Test

Before adding a paper person, answer:

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
labels (mandatory; 3-6 for simple figures, more when complex states/paths/groups need them; optional one-sentence strip if helpful):
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
- `references/operator-library.md`: operator families and action verbs.
- `references/domain-adaptation.md`: how to adapt paper operators to art, culture, life, business, technical, and other topics.
- `references/prompt-template.md`: planning and final generation prompt templates.
- `references/qa-checklist.md`: acceptance and regeneration rules.
