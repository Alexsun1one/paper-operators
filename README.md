# Paper Operators / 纸片人

> 一个中文优先的 Codex Skill：把文章里的判断、转折和复杂关系，变成清楚、好看、有动作感的纸片人正文配图。

[English](README.en.md)

Paper Operators 面向写作者、产品人、研究者、教师、创作者，以及所有需要把复杂想法讲清楚的人。它不是一个「可爱小人」画风包，而是一套文章配图工作流：先读懂文章里真正值得画的那句话，再让无脸纸片人亲手完成关键动作。

纸片人会装框、捕光、牵线、检视、开闸、照料、称重、归档、修补。它不是站在旁边卖萌，而是在图里把抽象概念做出来。

<p align="center">
  <img src="examples/images/readme/06-materials-before-conclusion.jpg" alt="先把材料摊开，再下结论" width="100%">
</p>

## 它解决什么问题

很多 AI 文章配图会掉进两个坑：要么好看但空泛，要么清楚但像 PPT。

Paper Operators 想要的是另一种状态：

- 读者三秒内知道这张图在讲什么
- 画面有纸张、器具、路径和动作，不是冰冷图标
- 中文标签默认可读，不再只给空白占位框
- 同一篇文章里的多张图风格统一，但每张图又贴合自己的段落
- 角色只在有用时出现，不能为了可爱而硬塞

一句话判断：如果把纸片人拿掉，图还是同样清楚，那这张图就不该画纸片人。

## 示例图

<table>
  <tr>
    <td width="50%">
      <img src="examples/images/readme/01-readable-chinese-route.jpg" alt="中文路线示例" width="100%">
      <br>
      <sub><strong>中文标签路线。</strong>观点、关系、状态、文字和结果沿着同一条路径展开。</sub>
    </td>
    <td width="50%">
      <img src="examples/images/readme/02-aerial-paper-stage-hero.jpg" alt="高空纸模舞台" width="100%">
      <br>
      <sub><strong>高空纸模舞台。</strong>适合系统、产品、城市、路线和多对象关系。</sub>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <img src="examples/images/readme/03-art-attention-frame.jpg" alt="艺术审美装框示例" width="100%">
      <br>
      <sub><strong>艺术与审美。</strong>纸片人可以是装框员、捕光员、调色员，而不是工程流程图里的小工人。</sub>
    </td>
    <td width="50%">
      <img src="examples/images/readme/04-life-boundary-room.jpg" alt="生活心理边界房间" width="100%">
      <br>
      <sub><strong>生活与心理。</strong>边界、照料、记忆和情绪天气，可以变成房间、屏风、纸条和路径。</sub>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <img src="examples/images/readme/05-ai-town-systems.jpg" alt="AI 系统小镇" width="100%">
      <br>
      <sub><strong>产品、AI 与系统。</strong>团队、校验、上线、证据和路线，可以被组织成一个可读的桌面世界。</sub>
    </td>
    <td width="50%">
      <img src="examples/images/readme/07-chat-copilot-agent.jpg" alt="从问答到派活" width="100%">
      <br>
      <sub><strong>从问答到派活。</strong>Chat、Copilot、Agent 的差异，不是名词差异，而是工作闭环差异。</sub>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <img src="examples/images/readme/08-agent-launch-six-forces.jpg" alt="Agent 上场六股力量" width="100%">
      <br>
      <sub><strong>Agent 上场。</strong>不是一匹马，是模型、上下文、工具、生态、成本和企业需求一起动。</sub>
    </td>
    <td width="50%">
      <img src="examples/images/readme/09-agent-service-results.jpg" alt="从旧 SaaS 到 Agent 代办" width="100%">
      <br>
      <sub><strong>Agent 代办。</strong>牌桌从“用工具”变成“买结果”，配图也要画出付费对象的变化。</sub>
    </td>
  </tr>
</table>

说明：README 里展示的是为 GitHub 加载速度压缩过的预览图，不代表实际生成图的清晰度。旧版 PNG 示例仍保留在 [`examples/images/`](examples/images/) 目录，新加入的首页样图放在 `examples/images/readme/`。

## 适合谁

适合：

- 公众号、博客、newsletter、长文作者
- 产品、AI、商业、工程、教育、研究类内容
- 艺术评论、文化文章、个人经验、心理和生活类文章
- 需要「有人在做这件事」而不是只有箭头和方框的解释图
- 想为一篇文章生成一组统一但不单调的正文图

不适合：

- 只需要 logo、贴纸、表情包或装饰性 mascot
- 一张普通截图、表格或图表就能说清楚的内容
- 纸片人只能站在旁边凑气氛，不能参与核心动作的场景

## 工作流

1. 从文章里找出最值得画的 source anchor：一句话、一个转折、一个冲突或一个判断。
2. 写清楚读者看完图应该明白什么。
3. 判断领域和语气：艺术、文化、生活、产品、商业、工程、教育、心理等。
4. 选择纸片人的动作：装框、捕光、牵线、检视、开闸、照料、称重、归档、修补。
5. 回答 `what breaks if removed`，确认纸片人不是装饰。
6. 选择纸模世界：画廊工作台、边界房间、纸片小镇、档案桌、路线图、剖面图、货架矩阵等。
7. 写出短而可读的中文标签。
8. 生成一张图，并检查清晰度、动作、文字、构图和风格漂移。

规划输出通常长这样：

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

## 安装

把 Skill 目录复制到 Codex skills 目录：

```bash
mkdir -p ~/.codex/skills
cp -R paper-operators ~/.codex/skills/paper-operators
```

重启 Codex 后即可使用：

```text
用 $paper-operators 给这篇文章规划 3 张正文配图，先不要生成图。
```

也可以直接生成一张：

```text
用 $paper-operators 根据下面这段文字生成一张 16:9 正文配图。

文字：
好的审美不是装饰，而是把注意力放到正确的位置。
```

## 示例提示词

规划一篇文章的图包：

```text
用 $paper-operators 给下面这篇文章规划 3 张正文配图，先不要生成图。

要求：
- 中文读者优先
- 每张图都给 source anchor、reader takeaway、operator family、what breaks if removed
- 至少一张不是工程/产品图，要贴合文章领域

文章：
{paste article}
```

生成产品 / AI 系统配图：

```text
用 $paper-operators 生成一张产品/AI 系统配图。

Source anchor:
我不是在问一个 AI，而是在组织一群 AI 完成一条可验证的路线。

要求：
- operator family 选 Thread Runner + Lens Keeper
- 高空纸模城镇/工作台，蓝色路径从想法穿过 AI 团队、检查点、上线场景
- 必须出现短中文标签：想法、团队、校验、上线
```

生成艺术评论配图：

```text
用 $paper-operators 生成一张艺术评论配图。

Source anchor:
好的审美不是装饰，而是把注意力放到正确的位置。

要求：
- operator family 选 Frame Setter / Light Catcher
- 画廊工作台、装框、光卡、色票、留白
- 不要画成流程图、漏斗、节点网络
```

更多示例见 [`examples/prompts.md`](examples/prompts.md)。

## 关注后续

这个仓库放的是可复用的 Skill 和示例。更完整的拆解、提示词、文章配图复盘、AI 写作和产品实践，我会继续写在公众号里。

如果你也关心这些问题：怎么让 AI 图不再像模板、怎么把文章里的判断画清楚、怎么把 Codex Skill 做成真正可复用的工作流，欢迎关注「正在逐渐AI化」。

<p align="center">
  <img src="assets/wechat-official-account.png" alt="微信搜一搜：正在逐渐AI化" width="720">
</p>

## 仓库结构

```text
paper-operators/
├── README.md
├── README.en.md
├── LICENSE
├── NOTICE.md
├── assets/
│   └── wechat-official-account.png
├── examples/
│   ├── prompts.md
│   └── images/
│       └── readme/
├── docs/
│   └── style-notes.md
└── paper-operators/
    ├── SKILL.md
    ├── agents/openai.yaml
    ├── references/
    └── assets/examples/
```

外层仓库给人读，内层 `paper-operators/` 是真正安装到 Codex 里的 Skill。

## License

MIT. See [`LICENSE`](LICENSE).
