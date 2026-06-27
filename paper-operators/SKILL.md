---
name: paper-operators
description: Generate or plan publish-grade 16:9 article illustrations using folded-paper action characters, with Chinese-first article/body-image workflows. Use when a user wants Chinese or English article illustrations, blog figures, explainer visuals, social/article images, or concept images where a small paper person should physically perform the core idea. Especially useful for turning abstract claims, emotions, cultural ideas, art criticism, product thinking, systems, workflows, tensions, boundaries, transformations, relationships, and evidence into clear high-angle paper-model scenes, as single figures or chained multi-image series. Do not use for generic mascots, cute stickers, Xiaohei-style black figures, stock PPT infographics, or image requests where no action character helps comprehension.
---

# Paper Operators / 纸片人

Paper Operators turns an article idea into a tactile paper-stage illustration where a small folded-paper person performs the core conceptual action.

默认面向中文文章配图；用户使用英文时再切换英文输出。Use this skill to create a consistent article-illustration style: paper people, physical metaphors, readable labels, clear reader paths, and domain-aware tools. The character is never decoration. If removing the paper operator does not weaken the image, do not use one.

## Workflow

1. Read the article, excerpt, topic, or image-edit request.
2. Identify one source anchor: the sentence, paragraph, claim, tension, turn, or feeling that deserves a visual.
3. Read the user's real intent with `references/intent-reading.md`: who reads it, what they should feel, the author's stance, and the content-specific particulars that must appear. The image must fit THIS document, not the topic in general.
4. Name the core relationship the image must show, using `references/relationship-grammar.md`: connection, sequence, dependency, causality, feedback, contrast, tradeoff, hierarchy, transformation, boundary, divergence, or tension. Choose the relationship before the operator; precision comes from rendering the exact relation, direction, condition, and state.
5. Choose the domain and mood: art, culture, personal essay, business, product, engineering, education, psychology, finance, history, lifestyle, or another field.
6. Choose the core action: pull, frame, reveal, block, tune, fold, sort, mend, weigh, arrange, carry, shelter, distill, balance, light, archive, or transform.
7. Decide whether a Paper Operator is necessary using the inclusion test.
8. Before locking the default metaphor, diverge with `references/creative-divergence.md`: sketch a few candidate worlds and converge on the one that fits this content most precisely — do not reflexively reuse route-table, gallery, or room.
9. Select one operator family from `references/operator-library.md` that can physically perform the relationship; use the Operator × Relationship map when unsure.
10. Choose the composition mode with `references/composition-modes.md`: one dense single-image-multi-beat composition (e.g. four river crossings on one terrain) vs a multi-image series — pick what the content's own structure demands, not a default.
11. Assemble the scene from the kit in `references/primitives.md`, and encode status, degree, and state precisely with `references/state-coding.md`. Reuse the same primitive for the same meaning so the image stays consistent.
12. Adapt the world, props, palette, texture, and typography using `references/domain-adaptation.md`.
13. Write readable labels in the user's language. For simple Chinese figures, use 3-6 short labels; for complex multi-state figures, use more labels when they clarify paths, states, contrasts, or groups. Prefer short labels, but allow one readable sentence strip when it materially improves comprehension.
14. Build the final image prompt using `references/prompt-template.md`.
15. Generate or edit one image at a time.
16. When the article needs more than one image, plan the set with `references/series-and-chaining.md` so the figures share a world, operator, palette, and a progressing throughline instead of reading as N unrelated pictures.
17. Run QA with `references/qa-checklist.md`, and run the **Swap Test** from `references/variation-engine.md`: if the image could move onto a different article unnoticed, it is not precise enough. Regenerate if the operator is decorative, the style drifts, the relationship collapses into a generic arrow, the image feels template-locked, labels are missing, or the idea is unclear.
18. For README, portfolio, or showcase images, include at least one non-engineering domain when possible: art, culture, life, psychology, education, food, travel, or personal essays. The skill should not look like it only draws workflows.

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
- folded-paper people with a calm plain face by default, or one simple hand-drawn expression (a few line strokes for brows/eyes and mouth, profile or three-quarter) when it encodes the operator's state; never realistic, never head-on, never Xiaohei white-dot eyes
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

- **Relationship first** (`references/relationship-grammar.md`): name the exact relationship the image must show, then render its direction, condition, and state. This is what stops every image from collapsing into a generic left-to-right arrow. A precise relationship is the difference between "two things with a line" and "B depends on A, and breaks without it." Express the relation as a deep 3D paper scene — material arrangement, line or loop guidance, and the operator's state — not as a flat paper-ified chart icon (see "Relationships As Scenes, Not Chart Icons" in `references/style-dna.md`).
- **Primitives as the kit** (`references/primitives.md`): build every scene from a known set of paper parts — carriers, surfaces, enclosures, optics, measures, state containers, label containers, and the paper-person construction kit. One primitive carries one meaning; reuse the same primitive for the same meaning so a set of images feels like one world.
- **State coding for precision** (`references/state-coding.md`): show status, degree, and quality without extra text — color semantics, path thickness and texture, elevation, gate posture, edge condition, light, and degree. Keep an encoding budget: pick the one or two encodings that carry the article's precision and let the rest stay neutral.
- **Series for chaining** (`references/series-and-chaining.md`): when an article needs several images, chain them into one argument. Keep the operator, palette, and label style constant; advance one throughline ribbon across the set; introduce a small motif early and pay it off at the end.

These layers compose: pick the relationship, render it with primitives and state coding, and when there are multiple images, chain them with a shared throughline.

## Flexibility & Precision

The fastest way this skill dies is sameness: the first image wows, but after repeated use everything "feels the same" and stops being interesting. That boredom is a precision failure, not a style problem. The cure is to fit each image to THIS specific content and the user's real intent — when every image is built from its own article's particulars, no two look alike, because no two articles are the same. Do not be rigid; do not reprint a default scene. Four references hold this line.

- **Read intent, not just words** (`references/intent-reading.md`): infer the audience, the desired feeling, the author's stance, and the one sentence they would stake everything on; pull the content-specific particulars that must appear. Translate "what they said" into "what they need" — a request for a "flowchart" may really want a feeling.
- **Diverge before you default** (`references/creative-divergence.md`): sketch a few candidate metaphor worlds and converge on the one that fits this content most precisely, instead of reflexively reusing route-table / gallery / room. Precision beats novelty.
- **Choose the composition mode** (`references/composition-modes.md`): decide between one dense single-image-multi-beat composition and a multi-image series by the content's own structure. A campaign that crosses one river four times is one map, not four pictures.
- **Run the variation engine** (`references/variation-engine.md`): keep the semantic invariants fixed (relationship, operator action, DNA) and let content-driven axes vary (camera, world, pose, palette accent, expression).

The test that ties them together is the **Swap Test**: if the image could move onto a different article on the same topic without anyone noticing, it has failed — a precise image is locked to its document. Regenerate until the Swap Test fails for every neighboring article.

## Output Contract

For planning, return:

```text
source anchor:
reader takeaway:
intent (audience · feeling · author stance · the one sentence to keep):
domain and mood:
relationship type:
core action:
operator decision:
what breaks if removed:
operator family:
metaphor world (after divergence; why this beats the default):
composition mode (single dense image / series; why):
primitives and state coding:
composition:
labels (mandatory; 3-6 for simple figures, more when complex states/paths/groups need them; optional one-sentence strip if helpful):
series plan (only when planning more than one image):
final image prompt:
QA risks (include the Swap Test):
```

For generation, produce one image at a time and report:

- image path
- intended placement
- one-line purpose
- native label status: confirm whether labels/sentence strips are rendered inside the image, intentionally omitted, or externally overlaid because the user requested post-production
- whether it passes QA or needs regeneration

## References

- `references/style-dna.md`: the visual identity and anti-copy rules.
- `references/intent-reading.md`: read the user's real intent and the content-specific particulars so the image fits THIS document, not the topic in general.
- `references/relationship-grammar.md`: the 12 relationship families, their visual encoding, and how to render them precisely instead of as generic arrows.
- `references/operator-library.md`: operator families, action verbs, and the Operator × Relationship map.
- `references/creative-divergence.md`: diverge to several candidate metaphor worlds, then converge on the one that fits the content most precisely.
- `references/primitives.md`: the composable kit of atomic paper parts, label containers, and the paper-person construction kit.
- `references/state-coding.md`: the precise visual encoding system for status, degree, and quality.
- `references/domain-adaptation.md`: how to adapt paper operators to art, culture, life, business, technical, and other topics.
- `references/composition-modes.md`: choose one dense single-image-multi-beat composition vs a series; single-image layouts for multi-step stories.
- `references/series-and-chaining.md`: how to chain a set of images into one connected argument with a shared throughline.
- `references/variation-engine.md`: defeat sameness through precision; semantic invariants vs content-driven variables; the Swap Test.
- `references/prompt-template.md`: planning and final generation prompt templates.
- `references/qa-checklist.md`: acceptance and regeneration rules.
