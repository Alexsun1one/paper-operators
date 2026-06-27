# Intent Reading / 意图读取

This is the layer that makes the image fit the user's ACTUAL idea and THIS specific document — not the literal words, and not a generic same-feeling picture. Read it before building the prompt, alongside `references/relationship-grammar.md`.

## The Precision Mandate

An image that fits "any article on this topic" is a failure. It must fit THIS document — this author, this argument, this turn, this reader.

First use wows because it is novel: a paper operator physically performing an idea is unfamiliar, so any competent scene feels fresh. Repeated use bores because it stops being specific. When every image renders the topic in general — "burnout, so a tired figure", "growth, so a rising stack" — the operator becomes wallpaper. The novelty wears off and the sameness shows through. The boredom is not a style problem; it is a precision failure.

The fix is precision to content + intent. Render the particular thing the author actually means, for the particular reader they are writing to.

**The Swap Test / 换文测试** (shared with `references/variation-engine.md`): could this image move onto a different article — a neighboring post on the same topic — without anyone noticing it no longer fits? If yes, it is not precise enough. A precise image is locked to its document: swap the article and the image is visibly wrong.

Use this test as the bar for "specific". It is the single fastest way to catch a generic result before it ships.

## Intent Dimensions To Infer / 要推断的意图维度

The user rarely states these, but the image must serve them. Infer each from the article and the request.

- **Audience / 读者**: peers, beginners, executives, the emotionally invested, or 小红书 scrollers. A diagram for peers may be dense; the same idea for beginners needs one clear action; for the emotionally invested it needs warmth and room; for scrollers it needs one legible beat that survives a thumbnail.
- **Desired feeling / 期望感受**: reassured, provoked, impressed, comforted, or seen. The image should leave the reader feeling this — not just understanding the topic.
- **Author's stance / 作者立场**: confident, vulnerable, critical, or selling. Stance sets the operator's posture and expression: a confident author's operator works with assurance; a vulnerable author's operator shelters something fragile; a critical author's operator exposes or weighs; a selling author's operator reveals a clear gain.
- **Register / 语气**: serious, warm, playful, elegant, or intimate. Register sets palette warmth, line quality, and label tone.
- **The real job / 真正任务**: explain, persuade, move, be saved-and-shared (收藏转发), or earn a tap (封面点击). The job decides what the image optimizes for — clarity, a turn, an emotion, a quotable still, or a stop-scroll beat.
- **The one sentence / 一句话**: the single sentence the author would stake everything on. Find it. The image should serve that sentence above all else.

State the inferred dimensions in one compact line in the plan, e.g. `intent: beginners · reassured · vulnerable · warm · move · "你不是不够努力，是方向错了"`. This line is what keeps the rest of the build honest.

## Content-Specific Extraction / 内容特征提取

Precision lives in the concrete particulars of THIS document. Pull them out and make sure they appear, so the figure is unmistakably about this piece and nothing else.

Extraction checklist:

```text
content particulars:
- the specific object: the literal thing this article is about (not the category)
- the specific turn: the article's pivot, reversal, or "actually..." moment
- the specific number: the figure, ratio, count, or date the author leans on
- the specific tension: the exact two forces this piece holds, named in its words
- the specific stake: what the reader gains or loses if the claim is true
- the author's own word: a distinctive phrase or image the author repeats
```

Not every article yields all six; pull what is there. Then bind at least the strongest two into the scene as labeled paper objects or operator actions. If the extracted turn is "四渡赤水 was about exhausting the pursuer, not crossing rivers", the image must show the encirclement loosening — not four generic crossings.

The test: read the extracted particulars back, then ask whether the planned image could be drawn without them. If it could, the image is still generic. Push the particulars into the operator's action, the props, and the labels until the Swap Test fails for any neighboring article.

## Signals To Read / 要读的信号

Infer intent from what the document and its context show:

- **Tone**: analytical, warm, critical, melancholic, playful, urgent, elegant, intimate (see `references/domain-adaptation.md` for how tone sets the world).
- **Platform**: 公众号 long-form (rewards depth and a clean focal module), 小红书 (rewards one warm legible beat that survives a small thumbnail), blog or newsletter (rewards a precise explanatory figure), slide (rewards a single dominant relation). Platform shifts composition energy and label density.
- **Word choice**: formal vs colloquial, technical vs plain, certain vs hedged. Match the label register to the author's diction.
- **Emphasis and repetition**: what the author returns to is the anchor. Repeated words are usually the article's true subject, even when the title points elsewhere.
- **Anxiety**: what the author defends, qualifies, or pre-empts ("我知道有人会说...") reveals the real stake and often the desired feeling.
- **Emotional temperature**: hot (urgent, raised) wants higher composition energy and a sharper accent; cool (reflective, settled) wants quiet space, lower contrast, and a calmer operator.

## When To ASK vs INFER / 何时问，何时推断

Default: infer. State the assumption in one line, and proceed. A confident, specific guess that is 90% right beats a survey that stalls the work. Most articles give enough signal to read intent without asking.

Ask 1–2 sharp clarifying questions ONLY when a wrong guess is costly or irreversible:

- client-critical or publish-critical wording, where a mis-rendered phrase has real cost
- a sensitive emotional or medical topic, where the wrong feeling is harmful (grief, illness, loss, mental health)
- a specific brand, real person, or named product that must be depicted correctly

When you do ask, ask one or two pointed questions, each with a default already chosen, e.g. "这篇的读者是同行还是入门者？默认按入门者做。" Never interrogate with a multi-question survey. Never ask what you can infer.

## Map "What They Said" → "What They Need" / 字面 → 真实需求

The request names a form; the author needs an effect. Translate it.

- An essayist asking for "a flowchart / 流程图" usually wants a feeling, not a flowchart — render the emotional arc, not the boxes.
- "四渡赤水" wants the genius and relief of escaping encirclement — the pursuer exhausted, the loop slipping open — not merely four river crossings.
- A burnout essay wants room-to-breathe — a cleared surface, a single quiet operator setting things down — not a productivity chart.
- A product launch wants the shift in what the reader pays for — the old object set aside, the new value lifted forward — not a feature grid.
- A "data report / 数据复盘" by a vulnerable author wants the human cost or relief behind the number, not a dashboard.
- A "vs / 对比" piece by a critical author wants the verdict's weight, not two neutral panels — the scale already tilting.

The pattern: the named form is the author's guess at a solution. Read past it to the effect, then choose the operator and relationship that deliver the effect. Map the effect to a relationship in `references/relationship-grammar.md`, not to the literal form.

## Adapt The Image To Intent / 按意图调整画面

Same content + different intent → different operator expression, palette warmth, composition energy, and label tone. The anchor stays; the rendering changes.

Worked example — one anchor, two intents. Anchor: "我离职了 / I quit my job."

- **Intent A — reassured, warm, for the emotionally invested (move).** Operator gently folds a heavy work-badge into a small note and sets it down on a cleared table; one window opens to soft light. Palette warm, low contrast, generous quiet space. Operator in three-quarter view with an eased brow. Labels soft and few: `放下`, `留白`, one sentence strip `这一步不是失败`. Composition energy low and settled.
- **Intent B — provoked, confident, for peers (persuade).** Operator cuts a taut tether between a labeled `稳定` slab and a `机会` route, the freed route springing forward. Palette cooler with one sharp accent on the cut; higher contrast. Operator mid-action, decisive. Labels crisp tabs: `沉没成本`, `真实收益`, `下一步`. Composition energy higher, the cut as the focal beat.

Both are on-DNA, both are precise to the content, and neither would pass the other's Swap Test — that is the point. Use the intent line to pick which way the same anchor renders. For deliberate alternates of one brief, hand off to `references/variation-engine.md`; for choosing the composition energy itself, see `references/composition-modes.md`; when the literal read feels tired and the brief invites a fresh angle, see `references/creative-divergence.md`.

## Accept / Regenerate

Accept if:

- The image serves the inferred intent: the right audience, feeling, stance, register, and job.
- The image is locked to the specific content: at least two extracted particulars (object, turn, number, tension, stake, or the author's own word) are present as objects, actions, or labels.
- It passes the Swap Test: moving it to a neighboring article on the same topic would be visibly wrong.
- The named form was translated to the needed effect, not rendered literally.
- The intent line is recorded in the plan and the image visibly honors it.

Regenerate if:

- The image merely renders the literal words ("flowchart" → boxes; "growth" → a generic rising stack).
- It fits any article on the topic — it passes the Swap Test by being swappable.
- It mismatches the audience or the desired feeling (a cold chart for the emotionally invested; a dense peer diagram for 小红书 scrollers).
- It ignores the author's stance (a confident operator on a vulnerable essay; a neutral panel on a critical verdict).
- It serves the topic in general instead of the one sentence the author would stake everything on.
- No extracted particular survived into the image, so the figure is about the category, not the piece.
