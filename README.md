# Paper Operators / 纸片人

> A Chinese-first Codex Skill for turning article ideas into clear, tactile, paper-stage illustrations.

Paper Operators is built for people who write, explain, publish, teach, ship products, or make sense of complicated ideas. It turns an abstract sentence into a 16:9 article illustration where a small faceless paper person physically performs the core action: framing, lighting, routing, inspecting, filtering, caring, weighing, archiving, or repairing.

It is not a mascot pack. It is a visual thinking tool.

<p align="center">
  <img src="examples/images/05-readable-chinese-route.png" alt="Paper Operators readable Chinese route example" width="100%">
</p>

## What This Skill Does

- Finds the sentence, conflict, turn, or judgment in an article that is worth visualizing.
- Chooses a paper-world metaphor that matches the domain: art, culture, life, product, business, engineering, AI, education, or psychology.
- Uses paper operators only when their action improves comprehension.
- Produces readable Chinese or English labels by default, instead of empty label boxes.
- Keeps a consistent visual language across a whole article package without making every image look the same.

The rule is simple: if removing the paper operator does not weaken the image, the operator should not be there.

## Gallery

<table>
  <tr>
    <td width="50%">
      <img src="examples/images/01-aerial-paper-stage-hero.png" alt="High-angle paper stage" width="100%">
      <br>
      <sub><strong>High-angle paper stage.</strong> Good for systems, products, routes, cities, and multi-object scenes.</sub>
    </td>
    <td width="50%">
      <img src="examples/images/02-art-attention-frame.png" alt="Art attention frame" width="100%">
      <br>
      <sub><strong>Art and attention.</strong> Paper operators become frame setters, light catchers, and color tuners.</sub>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <img src="examples/images/03-life-boundary-room.png" alt="Life boundary room" width="100%">
      <br>
      <sub><strong>Life and psychology.</strong> Boundaries, care, memory, and emotional weather become rooms and paper objects.</sub>
    </td>
    <td width="50%">
      <img src="examples/images/04-ai-town-systems.png" alt="AI town systems" width="100%">
      <br>
      <sub><strong>Product, AI, and systems.</strong> Routes, teams, checkpoints, and evidence become a readable tabletop world.</sub>
    </td>
  </tr>
</table>

## Why It Exists

Most AI-generated article images fail in one of two ways: they are pretty but vague, or they are clear but look like a slide deck.

Paper Operators tries to sit in the better middle:

- clear enough to explain the idea in three seconds
- warm enough that readers want to keep looking
- structured enough to support long-form writing
- distinctive enough to make a publication feel owned

The style borrows the discipline of diagrams, the warmth of paper craft, and the editorial restraint of a good magazine figure. It does not copy Xiaohei-style black figures, white-dot eyes, blob mascots, generic stick people, robots, stock icons, or PPT infographics.

## When To Use It

Use Paper Operators for:

- WeChat articles, blogs, newsletters, and long-form essays
- product thinking, AI workflows, business judgment, engineering notes
- art criticism, cultural essays, personal writing, psychology, education
- explainers that need more humanity than arrows and boxes
- visual packages where several images should feel related

Avoid it when:

- the image only needs a logo, icon, sticker, or decorative mascot
- a simple chart or screenshot would explain the point better
- the operator would stand beside the idea instead of acting on it

## How It Works

1. Pick one source anchor from the article.
2. Decide what the reader should understand after seeing the image.
3. Choose the domain and mood.
4. Select a paper operator family.
5. Answer `what breaks if removed`.
6. Choose a scene: gallery table, boundary room, paper town, archive desk, route map, cutaway, shelf matrix, or another paper-world setup.
7. Add readable labels in the user's language.
8. Generate one image, then check clarity, action, text, composition, and style drift.

Planning output includes:

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

## Install

Copy the Skill directory into your Codex skills folder:

```bash
mkdir -p ~/.codex/skills
cp -R paper-operators ~/.codex/skills/paper-operators
```

Restart Codex, then call it by name:

```text
用 $paper-operators 给这篇文章规划 3 张正文配图，先不要生成图。
```

Or generate one image directly:

```text
用 $paper-operators 根据下面这段文字生成一张 16:9 正文配图。

文字：
好的审美不是装饰，而是把注意力放到正确的位置。
```

## Example Prompts

Plan an article package:

```text
用 $paper-operators 给下面这篇文章规划 3 张正文配图，先不要生成图。

要求：
- 中文读者优先
- 每张图都给 source anchor、reader takeaway、operator family、what breaks if removed
- 至少一张不是工程/产品图，要贴合文章领域

文章：
{paste article}
```

Generate a product or AI system image:

```text
用 $paper-operators 生成一张产品/AI 系统配图。

Source anchor:
我不是在问一个 AI，而是在组织一群 AI 完成一条可验证的路线。

要求：
- operator family 选 Thread Runner + Lens Keeper
- 高空纸模城镇/工作台，蓝色路径从想法穿过 AI 团队、检查点、上线场景
- 必须出现短中文标签：想法、团队、校验、上线
```

Generate an art essay image:

```text
用 $paper-operators 生成一张艺术评论配图。

Source anchor:
好的审美不是装饰，而是把注意力放到正确的位置。

要求：
- operator family 选 Frame Setter / Light Catcher
- 画廊工作台、装框、光卡、色票、留白
- 不要画成流程图、漏斗、节点网络
```

More examples live in [`examples/prompts.md`](examples/prompts.md).

## Follow The Work

这个仓库放的是可复用的 Skill 和示例。更完整的拆解、提示词、文章配图复盘、AI 写作和产品实践，我会继续写在公众号里。

如果你也关心这些问题：怎么让 AI 图不再像模板、怎么把文章里的判断画清楚、怎么把 Codex Skill 做成真正可复用的工作流，欢迎关注「正在逐渐AI化」。

<p align="center">
  <img src="assets/wechat-official-account.png" alt="微信搜一搜：正在逐渐AI化" width="720">
</p>

## Repository

```text
paper-operators/
├── README.md
├── LICENSE
├── NOTICE.md
├── assets/
│   └── wechat-official-account.png
├── examples/
│   ├── prompts.md
│   └── images/
├── docs/
│   └── style-notes.md
└── paper-operators/
    ├── SKILL.md
    ├── agents/openai.yaml
    ├── references/
    └── assets/examples/
```

The outer repository is for people reading the project. The inner `paper-operators/` directory is the actual Codex Skill.

## License

MIT. See [`LICENSE`](LICENSE).

## English Summary

Paper Operators is a Codex Skill for generating article illustrations with faceless folded-paper action characters. It creates tactile paper-stage diagrams where a small paper figure physically performs the core idea: framing, lighting, routing, inspecting, filtering, caring, weighing, archiving, or repairing.

Use it for Chinese or English article body images, blog illustrations, concept visuals, and explainer figures. Do not use it for generic mascots, stickers, Xiaohei-style black figures, stock infographic icons, or decorative AI art that does not help readers understand the article.
