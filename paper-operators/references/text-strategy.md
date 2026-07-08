# Text Strategy

Use this reference whenever labels or sentence strips matter.

The model should generate only the text that the image itself must own.

## Label Budget

- Simple article figure: 3-6 short labels.
- Story/book card: 4-8 beat labels.
- Data story scene: 3-5 category/state labels plus exact values only if readable.
- Reference-informed explainer: labels for parts, mechanisms, or cues that would otherwise be ambiguous.
- Series: keep label vocabulary stable across images.

## Good Label Shapes

Prefer:

- nouns attached to objects: `SOURCE`, `CHOICE`, `RISK`
- verbs attached to actions: `CHECK`, `FILTER`, `ROUTE`
- states attached to chips or gates: `PENDING`, `VERIFIED`, `BLOCKED`
- story beats: `CALL`, `COST`, `RETURN`, `CHANGE`

Avoid:

- full sentences as labels
- abstract stage names such as `INPUT PHASE`
- fake UI labels
- tiny captions on busy texture
- labels that repeat what the image already shows

## Exact Text Block

For final prompts, state:

```text
Exact text: include only these labels: "A", "B", "C".
No other text, no fake paragraphs, no extra legend, no watermark.
```

If the image needs a title or explanatory line, decide whether the outer layout should own it. Most README/social/slide titles should stay outside.

## Repair Policy

If the image is good but labels are wrong:

1. Try one regeneration with a stricter exact-text block.
2. Shorten labels and place them on larger quiet plaques.
3. If text is still unstable and the surrounding layout can own the text, regenerate with numbered markers and put the explanation outside.

Do not silently accept misspelled labels in showcase, README, education, science, data, or public article assets.

