# Paper Operators / 纸片人

中文优先的 Codex Skill，用纸片人做文章正文配图。

它不是一个通用「可爱小人」画风包。Paper Operators 的核心是：让无脸纸片人亲手完成文章里的关键动作，把抽象判断变成可看的纸模场景。

![Paper Operators hero](examples/images/05-readable-chinese-route.png)

## 它适合做什么

- 公众号、博客、长文里的 16:9 正文配图
- 把抽象观点画成一眼懂的视觉隐喻
- 给艺术、文化、生活、产品、商业、工程、AI 等文章生成统一但不单调的图包
- 需要「有人在做这件事」而不是只有流程箭头的解释图

## 为什么叫纸片人

纸片人不是 mascot，也不是站在旁边增加可爱度的小角色。

每张图里，它必须执行一个核心动作：

- 装框、捕光、调色
- 牵线、检视、开闸
- 照料、折叠、设边界
- 归档、修补、称重

如果把纸片人拿掉，图还是同样清楚，那这张图就不该用纸片人。

## 视觉风格

Paper Operators 默认使用高空纸模信息场景：

- 高空或微俯视视角，像桌面上的微缩纸模舞台
- 立体纸片、卡片、标签、装订环、路径带、镜片、灯卡、门、框、托盘
- 复杂度由文章自己决定：先选最小足够复杂度，但复杂关系可以画复杂图
- 必须有文字：简单图用 3-6 个短中文标签；复杂图可以更多，但要分组、贴近对象、读得清
- 主路径、连线、状态和层级要清楚；复杂可以，但不能乱
- 纸片人无脸、无眼、无嘴，不复制小黑的黑色 blob 身体或白点眼

默认不要生成空白标签图。只有用户明确要「后期叠字」或文字必须 100% 可编辑时，才使用 blank label containers。

默认效果应该像这样：有主路径、有状态、有短中文标签，也有完整句子作为低层说明，但不会变成密密麻麻的伪文字。

![Readable Chinese route](examples/images/05-readable-chinese-route.png)

高空纸模模式：更适合系统、产品、城市、路线和多对象文章。

![Aerial paper stage](examples/images/01-aerial-paper-stage-hero.png)

## 示例

艺术与审美：纸片人不是工程角色，而是装框员、捕光员、调色员。

![Art attention frame](examples/images/02-art-attention-frame.png)

生活与心理：纸片人可以整理边界、照料记忆、搬运情绪天气。

![Life boundary room](examples/images/03-life-boundary-room.png)

产品、AI、系统：纸片人可以牵引路径、检视证据、把抽象流程变成空间。

![AI town systems](examples/images/04-ai-town-systems.png)

## 安装

把 `paper-operators/` 这个 Skill 目录复制到 Codex skills 目录：

```bash
mkdir -p ~/.codex/skills
cp -R paper-operators ~/.codex/skills/paper-operators
```

重启 Codex 后即可使用：

```text
用 $paper-operators 给这篇文章规划 3 张正文配图，先不要生成图。
```

或直接生成：

```text
用 $paper-operators 根据下面这段文章生成一张 16:9 正文配图。
```

## 工作流

1. 找到文章里最值得画的一句话、转折、冲突或判断。
2. 判断领域：艺术、文化、生活、产品、商业、工程、教育等。
3. 选择动作：装框、捕光、牵线、检视、开闸、照料、称重、归档等。
4. 回答 `what breaks if removed`，确认纸片人不是装饰。
5. 写出 3-6 个短标签，让读者不猜谜。
6. 生成一张复杂度匹配文章的图：简单观点用简单图，多状态/多关系文章可以用复杂图。
7. 检查：三秒能否读懂、动作是否成立、文字是否清楚漂亮、是否滑向 PPT 或 mascot。

## 仓库结构

```text
paper-operators/
├── README.md
├── LICENSE
├── NOTICE.md
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

Skill 本体只保留 AI 执行任务需要的内容。README、docs、examples 属于开源仓库说明，不会增加 Skill 运行时上下文负担。

## English

Paper Operators is a Codex Skill for generating article illustrations with faceless folded-paper action characters. It creates tactile paper-stage diagrams where a small paper figure physically performs the core idea: framing, lighting, routing, inspecting, filtering, caring, weighing, archiving, or repairing.

Use it for Chinese or English article body images, blog illustrations, concept visuals, and explainer figures. Do not use it for generic mascots, stickers, Xiaohei-style black figures, or stock infographic icons.
