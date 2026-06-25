# Example Prompts / 示例提示词

Codex 用户可以写 `用 $paper-operators ...`。

Claude Code、Cursor、Hermes Agent、OpenClaw 或其他 Agent 工具，可以把 `$paper-operators` 换成：

```text
请按 Paper Operators 工作流处理下面这篇文章。
```

如果你的 Agent 没有读过本仓库，先把 [`agent-guides/paper-operators-agent.md`](../agent-guides/paper-operators-agent.md) 放进项目规则或自定义指令。

## 先规划，不生成

```text
用 $paper-operators 给下面这篇文章规划 3 张正文配图，先不要生成图。

要求：
- 中文读者优先
- 每张图都给 source anchor、reader takeaway、operator family、what breaks if removed
- 至少一张不是工程/产品图，要贴合文章领域

文章：
{paste article}
```

## 生成一张正文图

```text
用 $paper-operators 根据下面这段文字生成一张 16:9 正文配图。

重点：高空纸模视角、立体元素、蓝色主路径、中文标签像贴纸/展签一样排布。纸片人必须执行核心动作，不要站旁边装饰。

文字：
好的审美不是装饰，而是把注意力放到正确的位置。
```

## 艺术文章

```text
用 $paper-operators 生成一张艺术评论配图。

Source anchor:
好的审美不是装饰，而是把注意力放到正确的位置。

要求：
- operator family 选 Frame Setter / Light Catcher
- 画廊工作台、装框、光卡、色票、留白
- 不要画成流程图、漏斗、节点网络
```

## 生活/心理文章

```text
用 $paper-operators 生成一张生活/心理文章配图。

Source anchor:
边界不是把人推远，而是给关系留出可以呼吸的房间。

要求：
- operator family 选 Boundary Keeper 或 Care Folder
- 小房间、软屏风、椅子、便签、天气卡
- 温暖但不幼稚，不要 KPI 图表
```

## 情绪整理房间

```text
用 $paper-operators 生成一张 16:9 生活/心理文章正文配图。

Source anchor:
把情绪放回合适的位置，关系才重新有了可以呼吸的空间。

要求：
- operator family 选 Boundary Keeper / Care Folder
- 纸片人在雨后房间里移动一朵沉重的蓝灰云，把它放到架子上
- 房间里有屏风、便签、天气卡、茶、暖灯
- 不要工程词、不要节点网络、不要流程图
- 可以少量中文标签，但画面必须先靠动作和空间读懂
```

## 产品/AI/系统文章

```text
用 $paper-operators 生成一张产品/AI 系统配图。

Source anchor:
我不是在问一个 AI，而是在组织一群 AI 完成一条可验证的路线。

要求：
- operator family 选 Thread Runner + Lens Keeper
- 高空纸模城镇/工作台，蓝色路径从想法穿过 AI 团队、检查点、上线场景
- 必须出现短中文标签：想法、团队、校验、上线
- 复杂度由文章决定：如果需要多状态，就用颜色/路径/标签把状态管理清楚；不要无意义堆城市细节
```

## 文字更多但仍清楚

```text
用 $paper-operators 生成一张带中文字的正文配图。

Source anchor:
好图不是更复杂，而是让关系、状态和文字一起变清楚。

要求：
- 高空纸模视角，蓝色主路径
- 必须有可读中文，不要空标签
- 可以使用 5-10 个短标签，按路径、状态、对象分组
- 可以加一条短句作为底部纸条说明
- 不要伪中文、不要密密麻麻、不要 PPT 流程图
```
