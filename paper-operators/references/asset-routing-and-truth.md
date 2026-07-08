# Asset Routing And Truth

Use this reference before final prompt writing when the source is more than a single article sentence: a book, story, report, chart, slide, screenshot, science topic, historical object, brand, or social-card package.

Paper Operators is a visual reasoning system, not only a style. The first question is not "what should it look like?" but "what job must this image do in the final artifact?"

## Core Rule

Keep the paper operator only when the operator's physical action clarifies the meaning.

If the final need is an exact chart, a full slide layout, a full social card, a logo, or a decorative center image where no action is needed, do not force Paper Operators to own the whole job. Use Paper Operators for the reasoning image, and let the surrounding layout, chart, PPT, or card system do its own work.

## Asset Roles

Pick one role before choosing the scene.

### Article Figure

Use for one section, claim, tension, or turn inside an essay.

- Visual job: make one argument memorable.
- Best form: one operator performing one relation.
- Text ownership: short object labels inside the image; paragraph explanation stays outside.

### Story Or Book Card

Use for a whole story, chapter, biography, case study, or book explainer.

- Visual job: compress characters, turning points, consequence, and transformation.
- Best form: one dense single-image multi-beat card, unless the narrative truly needs a series.
- Text ownership: labels for beats, characters, forces, or choices; no plot paragraphs inside the image.
- Operator job: reveal, guide, archive, light, or transform the story arc.

### Data Story Scene

Use when the content includes numbers, rankings, benchmark results, project metrics, or a chart screenshot, but the final image should explain the meaning rather than replace a rigorous chart.

- Visual job: show what the data means and why it matters.
- Best form: a compact chart/table object embedded in a paper scene, with the operator inspecting, weighing, highlighting, or routing the key comparison.
- Truth rule: list every value that appears in the image. Do not let the image model invent numbers, categories, dates, or axes.
- If exact axes and values are the whole artifact, use a native chart or PPT/chart workflow instead; Paper Operators can create the surrounding interpretation scene.

### Center Illustration For A Card Or Slide

Use when another system will handle title, subtitle, body copy, platform ratio, or slide layout.

- Visual job: be the central image well.
- Best form: no large title inside the image; leave safe margins and avoid dense text.
- Text ownership: only labels needed to understand the objects. Outer layout owns headline and commentary.
- Ratio: ask for the target image well if known; otherwise default to 16:9 horizontal.

### Reference-Informed Explainer

Use for science, history, culture, geography, specific brands, model families, artifacts, devices, species, buildings, or anything visually easy to get wrong.

- Visual job: make the thing recognizable without copying an external image.
- Best form: symbolic paper scene with stable visual cues translated into the Paper Operators world.
- Reference rule: gather stable cues, not style. Use references to avoid wrong parts, wrong era, wrong mechanism, or confused silhouettes.
- Record uncertainty when exactness matters.

## Routing Questions

Answer these before prompt writing:

```text
asset role:
final container: article / README / social card / slide / doc / knowledge base / other
display well or ratio:
text ownership: inside image / outside layout / both
truth constraints: exact labels / exact numbers / historical or scientific cues / brand cues / none
reference need: yes/no and why
operator necessity:
if not Paper Operators, better owner:
```

## Cognitive Anchors For Long Sources

For a long article, chapter, book, transcript, report, or deck, do not illustrate every paragraph.

Pick 1-6 cognitive anchors:

- the opening question
- the main transformation
- the central tradeoff
- the hidden mechanism
- the evidence or data turn
- the emotional or moral choice
- the closing payoff

For each anchor, decide whether it becomes:

- one standalone figure
- one panel in a story/book card
- one image in a chained series
- a data story scene
- no image because text explains it better

## Truth Handling

Some images can be approximate; some cannot.

### Must Be Exact

- chart values
- labels specified by the user
- names, dates, places, product names, model names
- scientific part labels
- historical route labels when they carry the point
- brand or icon cues when recognition matters

Put exact requirements explicitly in the final prompt:

```text
Exact text: include only these labels: "A", "B", "C".
Exact data: show these values and no others: A=12, B=8, C=5.
Do not invent extra categories, dates, axes, legends, or labels.
```

### Can Be Symbolic

- mood
- paper props
- metaphor world
- operator pose
- visual emphasis
- non-critical background objects

## What To Refuse Or Reroute

Reroute away from Paper Operators when:

- the user only needs a strict chart with exact axes and values
- a screenshot or table already explains the point better
- the paper operator would be decorative
- the asset is a complete social card or slide layout rather than the center illustration
- the topic requires photo-real documentary accuracy
- the user needs a logo, icon system, sticker, or brand mark

In these cases, say the better owner plainly: native chart, PPT skill, social-card skill, code-rendered diagram, image edit, or ordinary documentation.

## QA Additions

Before delivery, check:

- The chosen asset role is visible in the result.
- Text ownership is respected: no headline stuffed into the image when an outer layout should own it.
- Exact labels and data are not invented, misspelled, or swapped.
- Reference-informed cues are recognizable but not copied from a source image.
- The operator action is still necessary after routing.
- The image remains readable at the intended display size.

