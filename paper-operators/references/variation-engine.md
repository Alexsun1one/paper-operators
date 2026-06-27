# Variation Engine / 变化引擎

Use this reference when repeated Paper Operators output starts to feel the same. The failure mode is not "needs more randomness." The failure mode is **template-lock**: the skill stops reading the article and starts reprinting a default scene. The cure is **precision** — build each image from THIS content's specifics, and variation follows naturally because no two articles are the same.

## The Sameness Trap / 同质化陷阱

First use wows. Repeated use bores. The reader stops seeing the article in the image and starts seeing the skill's default template.

**Symptoms of template-lock:**

- **Same camera every time:** high-angle tabletop, identical tilt, identical margin ratio, operator always bottom-left or always center-right.
- **Same layout every time:** three cards on a blue ribbon, equal-weight panels, route-table staging regardless of the claim.
- **Same operator pose every time:** standing beside the scene, one hand on ribbon, neutral posture, no state change across articles.
- **Same palette every time:** passage blue + off-white + one mint tab, even when the article is about risk, warmth, loss, or art.
- **Same world every time:** gallery workbench, route table, soft boundary room, archive table, or miniature town — pasted onto every domain.
- **Same props by habit:** gates, funnels, nodes, and workflow cards in art essays, personal essays, and food writing.

**The tell:** "This image could illustrate almost any article." If swapping the labels would not break the scene, the image is not precise enough. Sameness is a precision failure, not a missing randomness knob.

## The Precision Principle / 精准原则

Build each image from THIS content's specifics:

- **Source anchor:** the exact sentence, tension, turn, or feeling that earns the figure — not a generic topic keyword.
- **Relationship:** the exact relation, direction, condition, and state from `references/relationship-grammar.md` — not a default left-to-right arrow.
- **Domain props:** tools, surfaces, and metaphor world drawn from the article's own field — not engineering props by default.
- **Emotional temperature:** calm, urgent, fragile, playful, heavy, or resolved — encoded in posture, light, edge condition, and expression when needed.

Read the article with `references/intent-reading.md` before choosing camera, world, or props. Precision is what makes images different; sameness is what happens when the skill skips reading.

### The Swap Test / 换文测试

After planning or generating, ask:

```text
If I moved this image onto a different article in the same genre,
would anyone notice the mismatch?
```

- **Pass:** the image fails on another article because its props, relation, labels, and operator action belong to THIS anchor.
- **Fail → regenerate:** the scene is generic enough to swap articles without loss. Template-lock confirmed.

The Swap Test is a regenerate trigger, not a nice-to-have. Run it before accepting any image in a repeated-use workflow.

## Invariants vs Variables / 不变 vs 可变

Not every axis should move. Vary the wrong things and the image breaks correctness. Vary nothing and the skill prints the same poster forever.

### NEVER vary / 语义不变

These carry meaning. Changing them for "variety" breaks the image:

- **Relationship being shown:** connection, dependency, tradeoff, boundary, etc. — chosen from the anchor, not rotated for freshness.
- **Operator action and state:** the physical verb and what it acts on; the operator performs the relation, not a default "hold ribbon" pose.
- **Label meaning:** short labels attached to the correct objects; do not swap label text to fake diversity while keeping the same scene.
- **Style DNA:** folded-paper material, charcoal outline, faceless-or-simple-expression rule, restrained palette logic, 3D paper-stage depth — not flat chart icons, not mascots, not PPT infographics (see `references/style-dna.md`).

If an axis change would make a correct reader misread the relation, it is an invariant. Keep it.

### SHOULD vary, driven by content / 随内容变化

These SHOULD differ image to image because different content naturally demands different staging. Do not randomize them; derive them from the anchor, domain, and relation.

| Axis / 轴 | Content-driven menu |
| --- | --- |
| Camera angle & height / 机位 | steep bird's-eye for overview; shallow isometric for hand-work; low three-quarter for intimacy; side-elevated for comparison trays |
| Composition & focal placement / 构图 | operator on-path vs at gate vs at scale; asymmetric weight; one focal module with quiet zones; foreground action vs recessed archive |
| Operator pose & expression / 姿态 | leaning into pull, crouched at repair, arms extended at bridge, still at weigh; one simple line expression only when state needs reading |
| Metaphor world & props / 隐喻世界 | gallery plinth, kitchen board, ledger table, weather shelf, stage wing, clinic tray, garden bed — from the article domain, not a default room |
| Palette accent / 色标 | passage blue for routes; evidence amber for proof; risk coral for failure branches; growth mint for payoff; one focus accent per image |
| Motif / 母题 | stamp, lamp, empty frame, weather card, note tag — one recurring primitive when the set needs continuity (`references/series-and-chaining.md`) |
| Lighting direction / 光向 | top-left editorial wash; side light on frame or lens; dim recess for hidden layers; warm strip on the deliverable |
| Depth staging / 景深 | foreground gate, mid-stage operator, back shelf; raised active layer, recessed done layer |
| Label-container style / 标签容器 | stitched tags, gallery plaques, route signs, hanging labels, sentence strip — match domain and set, not one default tab shape |

Pick axes from the article. Two images about different claims should diverge on several rows without breaking DNA.

## Where Legitimate Variation Comes From / 合法变化来源

Variation is a downstream symptom of precision. Pursue it in this priority order:

### (a) Content-fidelity / 内容忠实 — primary source

Different anchors, relations, domains, and emotional beats naturally yield different images. This is the main engine. Before touching "make it different," ask whether the image is built from THIS content yet. If not, fix precision first.

Use `references/intent-reading.md` to lock anchor and takeaway. Use `references/composition-modes.md` to pick a staging mode that fits the relation — not the skill's favorite layout.

### (b) Deliberate contrast-with-previous / 与前图对照 — within a set

When planning 2–6 images, each new figure should differ from the last on **≥2 axes** (camera, focal placement, operator action, prop cluster, palette accent, throughline state) while keeping shared world, operator identity, palette base, and label style constant.

This links directly to `references/series-and-chaining.md` **Continuity Dimensions**: what stays constant vs what changes per image. Contrast-with-previous is legitimate when it serves the argument progression — not when it randomizes the set into unrelated posters.

### (c) Divergence exploration / 隐喻分叉 — when the anchor allows

When the article supports multiple valid metaphor worlds, explore alternatives with `references/creative-divergence.md`. Run parallel candidates; keep the one that passes the Swap Test and QA. Divergence is exploration of fit, not dice rolls.

### NOT a source: blind randomization / 盲目随机

Random camera, random palette, random props with no anchor reason is not variation — it is noise. Random ≠ precise. If the only reason to change an axis is "we used that last time," derive the change from content or from deliberate set contrast, not from a variation knob.

## The Two-Renders Test / 双次渲染测试

Run the same finalized prompt twice (same anchor, relation, domain, labels). Compare:

| Outcome | Meaning |
| --- | --- |
| **Visibly different, both correct, both precise** | Healthy: the skill reads content, not a frozen template; hand-built paper imperfection allows natural drift within DNA. |
| **Nearly identical** | Template-lock: composition, pose, world, and props are over-constrained; loosen content-driven axes (camera, props, focal placement), not semantic invariants. |
| **Different but one misfits the content** | Over-variation: an axis moved without anchor reason; roll back the axis that broke the Swap Test. |

Use the two-renders test during skill tuning, not as an excuse to accept a wrong image. Both renders must pass QA and the Swap Test.

## Anti-Template Checklist / 反模板清单

Before accept, confirm:

- [ ] Source anchor is THIS article's sentence/tension, not a genre keyword.
- [ ] Relationship is named and visible; a plain arrow would lose meaning.
- [ ] Domain props and metaphor world come from the article field — no habitual route-table/gallery/room without cause.
- [ ] Operator physically performs the relation; pose and tool match the action verb.
- [ ] Camera, composition, and focal placement fit the claim — not the skill's default layout.
- [ ] Palette accent encodes state or domain — not the same mint tab on every image.
- [ ] Swap Test passed: image would fail on a different article.
- [ ] Scene is a deep 3D paper stage — not a flat paper-textured chart icon.
- [ ] Labels are short, attached, and meaningful — not generic placeholders.
- [ ] In a set: ≥2 axes change from previous image; shared DNA stays constant (`references/series-and-chaining.md`).

## Accept / Regenerate

### Accept

- The image could only illustrate THIS anchor; the Swap Test passes.
- Variation across recent outputs comes from different content specifics — camera, & relations, domain props, and staging — not from the same template with label swaps.
- Camera, composition, operator pose, props, and accent color are content-driven; at least two axes would change if the anchor changed.
- Style DNA holds: folded-paper operator, restrained palette, 3D tactile stage, faceless-or-simple-expression rule, readable attached labels.
- In a series, contrast-with-previous is deliberate: ≥2 axes change per image while world, operator identity, and label style stay constant; throughline progresses.
- Two-renders test (when run): both outputs are visibly different yet both precise — or a single render is accepted because planning already locked content-specific axes.

### Regenerate

- **Swap Test fail:** image could sit on another article; generic three-card ribbon layout; habitual gallery/route-table/room world regardless of domain.
- **Template-lock:** same camera, pose, palette, and prop cluster as the last three outputs with only label changes.
- **Random drift:** camera, props, or palette changed with no anchor reason; image no longer fits the content.
- **False variation:** labels swapped but scene unchanged; cosmetic palette rotation while composition stays frozen.
- **Two-renders test fail:** identical outputs from the same prompt — skill is template-locked; regenerate with explicit content-driven axes from `references/composition-modes.md` and domain props.
- **Invariant broken:** relation collapsed to generic arrow; operator decorative; engineering props in non-engineering article; flat chart icon instead of 3D scene; mascot expression or Xiaohei drift.

### Repair moves

If template-lock is suspected:

```text
Re-read the source anchor with intent-reading. Name the exact relationship. List three domain-specific props the article mentions or implies. Pick camera and focal placement from composition-modes that fit the relation — not the default high-angle three-card layout. Regenerate. Run Swap Test before accept.
```

If two-renders test shows identical outputs:

```text
Lock invariants (relationship, operator action, label meaning, DNA). Explicitly vary ≥2 content-driven axes: metaphor world, camera height, operator pose, prop cluster, or palette accent. Regenerate twice and compare.
```

If variation broke precision:

```text
Identify which axis moved without anchor reason. Restore invariants. Regenerate from THIS content's source anchor, relationship, and domain props only. Pass Swap Test before accept.
```
