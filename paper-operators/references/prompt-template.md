# Prompt Template

Use one image at a time.

## Planning Template

```text
Use $paper-operators. First plan, do not generate yet.

Source anchor:
{quote / paragraph / concept}

Return:
- reader takeaway
- domain and mood
- core action
- whether to use a Paper Operator
- what breaks if removed
- operator family
- metaphor world
- composition
- label plan
- final generation prompt
- QA risks
```

## Final Generation Prompt

```text
Generate one standalone 16:9 horizontal article illustration in the Paper Operators style.

Article context:
{one sentence}

Source anchor:
{specific claim, sentence, or paragraph}

Reader takeaway:
{one sentence}

Domain and mood:
{art / culture / personal essay / business / product / engineering / education / finance / other; mood}

Core action:
{pull / frame / reveal / block / tune / fold / sort / mend / weigh / arrange / carry / shelter / distill / balance / light / archive / transform}

Paper operator:
- use one folded-paper operator, not a mascot.
- operator family: {Thread Runner / Lens Keeper / Gate Builder / Frame Setter / Color Tuner / Light Catcher / Archive Tender / Care Folder / Boundary Keeper / Weather Reader / Stack Mason / Residue Sweeper / Tradeoff Weigher}.
- action: {physical verb}.
- object acted on: {carrier / frame / light card / palette / archive / note / boundary / scale / layer / map / evidence card}.
- relation clarified: {what the action explains}.
- what breaks if removed: {the relation becomes less clear}.
- appearance: off-white folded-paper body, charcoal outline, folded tile head, small semantic color tab, one domain-specific tool.
- expression: plain by default, or one simple hand-drawn expression (a few line strokes for brows/eyes and mouth) when it encodes the operator's state — {neutral / effort / focus / strain / relief / satisfaction / care}; profile or three-quarter, looking at the work, never realistic, never head-on, never Xiaohei white-dot eyes.
- scale: secondary to the idea, usually 8-18% of canvas height.

Metaphor world:
{domain-specific world from domain-adaptation.md}

Composition:
- one focal module
- generous margins
- calm paper-stage depth
- clear start/change/result or before/action/after
- labels attached to objects, paths, frames, tabs, trays, or surfaces
- complexity should match the article: use the simplest sufficient form, but allow complex multi-state scenes when route, label, and state coding stay clear
- if using aerial paper-stage mode: high-angle tabletop miniature scene, dimensional paper props, smooth blue carrier ribbon, beautiful readable label plaques arranged near objects

Style:
- tactile paper model, editorial diagram, clear handcrafted quality
- restrained palette: paper, ink, quiet gray, one domain accent, plus passage/evidence/risk/growth only if meaningful
- no PPT look, no stock icons, no fake dense text
- no Xiaohei-like black blob body, no white-dot eyes, no tiny thin legs
- expression is allowed only as a state signal (effort, focus, strain, relief, care); no cute mascot grin aimed at the reader, no robot, avatar, silhouette, generic stick figure, or sticker behavior
- relations should be staged as deep 3D paper scenes (material arrangement + line/loop guidance + operator state), not flattened into paper-textured chart icons

Text:
Mandatory readable labels:
- include readable labels in the user's language
- for simple Chinese figures, use 3-6 short labels, usually 2-6 characters each
- for complex multi-state figures, add enough short labels to make states, paths, contrasts, and groups clear
- allow one readable sentence strip when it sharpens the takeaway
- attach labels to physical objects as tabs, plaques, route signs, gallery captions, sentence strips, or stitched cards
- do not leave labels blank unless the user explicitly requests post-production overlay
- do not generate dense fake text

Quality target:
publish-grade article body figure, clear in three seconds, visually memorable, elegant, domain-specific, not childish.
```

## Chinese-First Aerial Paper-Stage Prompt Add-On

Append this block when the user asks for the newer polished style:

```text
Use high-angle aerial paper-stage composition: a miniature tabletop paper-model scene with raised paper objects, cards, trays, tags, frames, gates, lenses, rooms, shelves, or route stations. Let complexity match the article: simple ideas stay simple; complex relationships may use more states, paths, and objects when the route remains legible. Use a smooth blue carrier ribbon as the main reader path if the concept has movement or transformation. Arrange Chinese labels as physical objects: readable plaques, stitched tags, hanging labels, paper tabs, gallery captions, or route signs. Avoid dense fake Chinese and avoid empty label placeholders unless post-production overlay is explicitly requested.
```

## Image Edit Prompt

```text
Use $paper-operators to edit this image.

Keep:
- core idea
- paper-stage material
- folded-paper operator identity (plain or one simple state expression)

Fix:
- make the operator perform the core action
- remove mascot behavior or decorative standing
- make labels shorter, clearer, and attached to the right objects
- make the domain-specific tool clearer
- improve focal hierarchy and quiet space
```
