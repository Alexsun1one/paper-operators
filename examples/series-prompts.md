# Series Prompts / 串联示例提示词

多图正文配图示例。每个系列包含：文章前提、串联计划、逐张终稿提示词。提示词风格对齐 [`prompts.md`](prompts.md)。

Codex 用户写 `用 $paper-operators ...`；其他 Agent 可替换为「请按 Paper Operators 工作流处理」。

提示：纸片人默认平脸；需要让读者读出操作员状态时，可加极简手绘表情（两条线当眉/眼、一条线当嘴，侧脸看着活），并随主路径推进。详见 `paper-operators/references/state-coding.md` 的「操作员表情状态」。

---

## 系列 A — 产品 / AI 系统（4 张）

**文章前提：** 从一个人提问，到组织一群 Agent 交付一条可验证的结果。

**串联计划**

| 张次 | 角色 | 关系 | 主路径状态 |
|------|------|------|------------|
| 1 | 开场(问答) | 问题 → 意图 | 蓝色工带松散，从「想法卡」垂落 |
| 2 | 展开(派活/团队) | 意图 → 分工 | 工带拉紧，分岔到 Agent 工位 |
| 3 | 转折(校验/风险) | 产出 → 检验 | 工带经检验闸门，风险枝标记 |
| 4 | 收束(交付结果) | 检验 → 交付 | 工带落入交付托盘，校验章盖印 |

- **共享世界：** 高空纸模工作台 / 微型路线城镇
- **Operator：** Thread Runner + Lens Keeper（同一位牵线员，折叠纸身、炭笔轮廓）
- **表情（状态编码）：** 默认平脸，随主路径推进——图1 平静、图2 凝神、图3 受压（眉头压紧）、图4 舒展落定；极简手绘线条、侧脸看着活，避开恐怖谷
- **Palette：** 纸白、墨灰、通道蓝；证据琥珀（校验）、风险珊瑚（分支）
- **标签风格：** 路线吊牌 +  stitched 纸签
- **Motif：** 小校验章 — 图 3 未盖，图 4 盖在交付卡上

### 图 1 — 开场(问答)

```text
用 $paper-operators 生成系列第 1/4 张 16:9 正文配图（产品/AI 系统串联 · 开场）。

Source anchor:
从一个人提问，到组织一群 Agent 交付一条可验证的结果。

Reader takeaway:
问题先被收成一张可执行的意图卡，蓝色工带从这里出发。

Domain and mood:
产品 / AI 系统；清晰、克制、可验证

Core action:
pull — 牵线员把松散工带从想法卡上拉起来

Paper operator:
- operator family: Thread Runner / 牵线员
- action: 弯腰拉起蓝色 carrier ribbon，ribbon 一端系在「想法卡」上
- object acted on: 想法卡 + 松散工带
- relation clarified: 个人提问如何变成可路由的意图
- what breaks if removed: 问题与后续路线失去连接起点
- appearance: 米白折叠纸身、炭笔轮廓、折叠瓦片头、无眼无嘴、通道蓝语义色标
- scale: 约占画面高度 12%

Metaphor world:
高空纸模工作台，左侧一张「想法卡」纸签，右侧空工位待填；smooth blue carrier ribbon 从想法卡垂落、松散。

Composition:
- 单焦点：想法卡 + 牵线员拉带动作
- 高空俯视纸模景深
- 工带起点清晰，终点留白暗示后续
- 中文标签：想法、提问、意图、待路由

Style:
- tactile paper model, editorial diagram
- restrained palette: 纸白、墨灰、quiet gray、passage blue
- 不要 PPT 流程图、不要机器人头、不要节点网络图标
- 不要 Xiaohei 黑 blob、不要白点眼

Quality target:
publish-grade 正文配图，三秒读懂：一个问题刚被收成意图，工带准备出发。
```

### 图 2 — 展开(派活/团队)

```text
用 $paper-operators 生成系列第 2/4 张 16:9 正文配图（产品/AI 系统串联 · 展开）。

Source anchor:
从一个人提问，到组织一群 Agent 交付一条可验证的结果。

Reader takeaway:
同一条蓝色工带被拉紧，分岔到多个 Agent 纸工位，各负一段任务。

Domain and mood:
产品 / AI 系统；协作、分工、路线清晰

Core action:
route — 牵线员把工带分岔到 Agent 工位

Paper operator:
- operator family: Thread Runner / 牵线员（与图 1 同一纸片人身份）
- action: 站在路线分叉口，把 carrier ribbon 拉紧并分到三个 Agent 纸牌工位
- object acted on: 分岔工带 + Agent 工位纸牌
- relation clarified: 一个意图如何被拆成可并行的工作段
- what breaks if removed: 团队分工失去可视路径
- appearance: 与图 1 相同：米白折叠纸身、炭笔轮廓、折叠瓦片头、通道蓝色标

Metaphor world:
延续图 1 工作台：工带已从「想法卡」拉紧延伸过来（handoff：图 1 松散末端 = 图 2 拉紧起点）；三个 Agent 纸牌工位沿工带排列，每工位一张 stitched 任务签。

Composition:
- 单焦点：分岔口 + 牵线员分带动作
- 蓝色 carrier ribbon 为主路径，分三支
- 中文标签：意图、Agent A、Agent B、Agent C、分工、拉紧

Style:
- 与系列一致：高空纸模、纸白墨灰通道蓝
- Agent 工位是纸牌+吊牌，不是机器人头像
- 不要 dashboard 卡片墙、不要 stock icon

Quality target:
publish-grade，三秒读懂：同一条工带进入团队分工。
```

### 图 3 — 转折(校验/风险)

```text
用 $paper-operators 生成系列第 3/4 张 16:9 正文配图（产品/AI 系统串联 · 转折）。

Source anchor:
从一个人提问，到组织一群 Agent 交付一条可验证的结果。

Reader takeaway:
产出必须经过检验闸门；风险枝被标出，小校验章尚未盖下。

Domain and mood:
产品 / AI 系统；审慎、可验证、有张力

Core action:
inspect — Lens Keeper 检视员在闸门处检验，Thread Runner 持工带等候

Paper operator:
- operator family: Thread Runner + Lens Keeper（两位，关系明确：路线 + 检验）
- action: Lens Keeper 用 translucent lens 检视工带上的产出卡；Thread Runner 持工带在闸门侧
- object acted on: 检验闸门 + 产出卡 + 风险 coral 标记枝
- relation clarified: 协作产出如何被验证、风险如何被看见
- what breaks if removed: 「可验证」承诺失去视觉证据
- motif: 小校验章放在闸门旁，尚未盖印（callback 铺垫）

Metaphor world:
延续系列工作台：工带从 Agent 工位汇入检验闸门；一条 risk coral 纸枝从侧道伸出，贴「风险」吊牌。

Composition:
- 单焦点：检验闸门 + 检视动作
- 工带经闸门，状态：待校验
- 中文标签：产出、检验、风险、待盖印、校验章

Style:
- 系列一致 palette；证据 amber 用于检验区、risk coral 用于风险枝
- 不要 glowing AI brain、不要 security 盾牌 stock icon

Quality target:
publish-grade，三秒读懂：产出到闸门，验证尚未完成。
```

### 图 4 — 收束(交付结果)

```text
用 $paper-operators 生成系列第 4/4 张 16:9 正文配图（产品/AI 系统串联 · 收束）。

Source anchor:
从一个人提问，到组织一群 Agent 交付一条可验证的结果。

Reader takeaway:
工带落入交付托盘，校验章盖在结果卡上——从提问到可验证交付，路线闭环。

Domain and mood:
产品 / AI 系统；完成、可信、收束

Core action:
place — 牵线员把工带末端放入交付托盘

Paper operator:
- operator family: Thread Runner / 牵线员（系列同一身份）
- action: 把 carrier ribbon 末端放入交付托盘，校验章已盖在「结果卡」上（motif payoff）
- object acted on: 交付托盘 + 结果卡 + 已盖校验章
- relation clarified: 整条路线如何收束为可交付、已验证的结果
- what breaks if removed: 文章论点「可验证交付」失去终点
- motif payoff: 图 3 未盖的校验章，此刻盖在结果卡上

Metaphor world:
延续系列：工带从检验闸门延伸落入右侧交付托盘；growth mint 轻标记「完成」；整体 quiet、editorial。

Composition:
- 单焦点：交付托盘 + 盖印结果卡
- 工带状态：已交付、拉直、落位
- 中文标签：结果、交付、已校验、闭环、可验证
- 可选一条短句纸签：从提问到可验证的结果

Style:
- 系列一致：高空纸模、纸白墨灰通道蓝、证据 amber 校验章
- 不要庆祝 confetti、不要 mascot 举手

Quality target:
publish-grade，三秒读懂：路线闭环，结果已验证交付。
```

---

## 系列 B — 艺术评论（3 张）

**文章前提：** 好的审美不是装饰，而是把注意力放到正确的位置。

**串联计划**

| 张次 | 角色 | 关系 | 主路径状态 |
|------|------|------|------------|
| 1 | 开场(杂乱素材) | 素材 → 待整理 | 蓝色工带穿过散乱纸屑堆 |
| 2 | 动作(装框/捕光/调色) | 素材 → 被处理 | 工带经画框+光卡，色票对齐 |
| 3 | 收束(被看见的作品) | 处理 → 呈现 | 工带止于装框作品，光落在焦点 |

- **共享世界：** 画廊工作台 Gallery workbench
- **Operator：** Frame Setter / Light Catcher（装框员 + 捕光员，同一纸身语言）
- **Palette：** 纸白、墨灰、通道蓝；growth mint 用于完成光区
- **标签风格：** 画廊 plaque 展签
- **Motif：** 空画框 → 装入作品 → 被光照亮的完成框

### 图 1 — 开场(杂乱素材)

```text
用 $paper-operators 生成系列第 1/3 张 16:9 正文配图（艺术评论串联 · 开场）。

Source anchor:
好的审美不是装饰，而是把注意力放到正确的位置。

Reader takeaway:
工作台上一堆未整理的素材——审美问题首先是注意力还没被放到该放的地方。

Domain and mood:
艺术 / 评论；克制、专业、有判断

Core action:
survey — 装框员站在散乱素材前，尚未动手

Paper operator:
- operator family: Frame Setter / 装框员
- action: 面对散乱的 paper scraps、色票碎纸、裁切角，手持空画框尚未落下
- object acted on: 散乱素材堆 + 空画框
- relation clarified: 「杂乱」是审美工作尚未开始的可见状态
- what breaks if removed: 后续装框/捕光失去对比起点
- appearance: 米白折叠纸身、炭笔轮廓、无五官、小 semantic tab

Metaphor world:
高空视角画廊工作台：裁切角、色票碎纸、未命名 paper scraps 散
；smooth blue carrier ribbon 松散穿过素材堆；空画框 lean 在桌边。

Composition:
- 单焦点：散乱素材 vs 空画框
- 不要流程图、不要 funnel
- 中文标签：素材、未整理、空框、待聚焦

Style:
- tactile paper model, gallery workbench
- restrained palette: 纸白、墨灰、passage blue
- 不要 PPT、不要节点网络

Quality target:
publish-grade，三秒读懂：审美工作尚未开始，素材待被聚焦。
```

### 图 2 — 动作(装框/捕光/调色)

```text
用 $paper-operators 生成系列第 2/3 张 16:9 正文配图（艺术评论串联 · 动作）。

Source anchor:
好的审美不是装饰，而是把注意力放到正确的位置。

Reader takeaway:
装框员把素材装入画框，捕光员调整光卡——注意力正在被放到正确位置。

Domain and mood:
艺术 / 评论；专注、工艺感、判断进行中

Core action:
frame + light — 装框 + 捕光

Paper operator:
- operator family: Frame Setter + Light Catcher（两位协作，同一纸身语言）
- action: Frame Setter 把选中的 composition 装入 mat board；Light Catcher 持 translucent light card 调整光照
- object acted on: 画框 + mat board + light card + 对齐的 color strips
- relation clarified: 审美作为动作——装框、捕光、色票对齐
- what breaks if removed: 「放到正确位置」只剩抽象口号
- handoff: 图 1 空框此刻正在装入作品

Metaphor world:
延续画廊工作台：blue carrier ribbon 拉紧，经画框工位和光卡工位；paper palette 色票已对齐。

Composition:
- 单焦点：装框 + 光卡动作
- 中文标签：装框、捕光、色票、对齐、聚焦中

Style:
- 系列一致：高空纸模、gallery plaque 展签
- 不要 engineering gate、不要 dashboard

Quality target:
publish-grade，三秒读懂：注意力正在被装框和光线放到该放之处。
```

### 图 3 — 收束(被看见的作品)

```text
用 $paper-operators 生成系列第 3/3 张 16:9 正文配图（艺术评论串联 · 收束）。

Source anchor:
好的审美不是装饰，而是把注意力放到正确的位置。

Reader takeaway:
完成的作品被框住、被光照亮——审美让正确的东西被看见。

Domain and mood:
艺术 / 评论；完成、安静、有被看见的分量

Core action:
reveal — 捕光员让光落在装框作品上

Paper operator:
- operator family: Light Catcher / 捕光员（Frame Setter 可退至侧影或离场）
- action: 持 light card，让 growth mint 柔光落在已装框作品上
- object acted on: 完成装框的作品 + 光区
- relation clarified: 审美终点不是装饰，而是作品被正确呈现
- what breaks if removed: 文章收束失去可视 payoff
- motif payoff: 图 1 的空框，此刻框住被照亮的作品

Metaphor world:
延续画廊工作台：blue carrier ribbon 止于装框作品；周围 quiet margin；plinth 展签。

Composition:
- 单焦点：被光照亮的装框作品
- generous quiet zones
- 中文标签：作品、被看见、留白、完成
- 可选短句纸签：把注意力放到正确的位置

Style:
- 系列一致 palette；growth mint 光区
- editorial, tactile, publishable
- 不要 cute mascot、不要 stock gallery icon

Quality target:
publish-grade，三秒读懂：审美收束为「被看见」。
```

---

## 系列 C — 生活 / 心理（3 张）

**文章前提：** 边界不是把人推远，而是给关系留出可以呼吸的房间。

**串联计划**

| 张次 | 角色 | 关系 | 主路径状态 |
|------|------|------|------------|
| 1 | 开场(被淹没) | 自我 → 过载 | 工带缠绕，天气卡写「阴」、灯灭 |
| 2 | 动作(立屏风/挪云) | 过载 → 分界 | 工带拉直，屏风立起，云被放到架上 |
| 3 | 收束(可呼吸的房间) | 分界 → 空间 | 工带松落至呼吸区，灯重亮、天气卡转「晴」 |

- **共享世界：** 软边界房间 Soft boundary room
- **Operator：** Boundary Keeper / Care Folder（边界员 + 照料员）
- **Palette：** 纸白、墨灰、通道蓝；quiet gray 用于「沉重」元素
- **标签风格：** stitched 便签 + 小 weather card
- **Motif：** 天气卡（阴→晴）+ 暖灯（灭→亮）—— 原元素串联

### 图 1 — 开场(被淹没)

```text
用 $paper-operators 生成系列第 1/3 张 16:9 正文配图（生活/心理串联 · 开场）。

Source anchor:
边界不是把人推远，而是给关系留出可以呼吸的房间。

Reader takeaway:
小房间里请求与情绪堆叠，人尚未被隔开——需要先看见「被淹没」的状态。

Domain and mood:
生活 / 心理；温暖但不幼稚、真实、略沉

Core action:
hold — 边界员被堆叠的便签和 request cards 包围，尚未立屏风

Paper operator:
- operator family: Boundary Keeper / 边界员
- action: 站在纸模小房间中央，被便签、信封、request cards 堆绕；blue carrier ribbon 缠绕打结
- object acted on: 便签堆 + 缠绕工带 + weather card（阴）+ 未亮的 paper lamp
- relation clarified: 没有边界时，关系空间被请求淹没
- what breaks if removed: 后续「呼吸房间」失去对比
- motif 引入: weather card 写「阴」；lamp 灭

Metaphor world:
高空视角 soft boundary room：纸屏风尚未立起；椅子、便签、weather card、未亮暖灯。

Composition:
- 单焦点：便签堆 + 缠绕工带
- 温暖 paper texture，不要 KPI 图表
- 中文标签：请求、堆叠、阴、未亮、待分界

Style:
- tactile paper model, intimate editorial
- restrained palette: 纸白、墨灰、passage blue、quiet gray
- 不要 flowchart、不要 engineering node

Quality target:
publish-grade，三秒读懂：关系空间被淹没，边界尚未建立。
```

### 图 2 — 动作(立屏风/挪云)

```text
用 $paper-operators 生成系列第 2/3 张 16:9 正文配图（生活/心理串联 · 动作）。

Source anchor:
边界不是把人推远，而是给关系留出可以呼吸的房间。

Reader takeaway:
边界员立起软屏风，照料员把沉重的蓝灰云放到架子上——分界是动作，不是冷漠。

Domain and mood:
生活 / 心理；温柔、有决断、正在恢复空间

Core action:
place + separate — 立屏风 + 挪走沉重的云

Paper operator:
- operator family: Boundary Keeper + Care Folder（两位，同一纸身语言）
- action: Boundary Keeper 立起 paper screen；Care Folder 把 quiet gray 蓝灰云放到 side shelf
- object acted on: 软屏风 + 蓝灰云 + 拉直的 carrier ribbon
- relation clarified: 边界作为物理动作——隔开、挪开、让出空间
- what breaks if removed: 「边界」读成抽象概念而非可做的动作
- handoff: 图 1 缠绕工带此刻被拉直

Metaphor world:
延续 soft boundary room：屏风已立；一侧 request 区、一侧留白；weather card 仍为「阴」；lamp 微亮。

Composition:
- 单焦点：立屏风 + 挪云
- 中文标签：屏风、挪开、沉重、分界、拉直

Style:
- 系列一致：高空纸模、stitched 便签
- 温暖但不 cute sticker
- 不要 chart、不要 gate icon

Quality target:
publish-grade，三秒读懂：边界正在建立，空间开始恢复。
```

### 图 3 — 收束(可呼吸的房间)

```text
用 $paper-operators 生成系列第 3/3 张 16:9 正文配图（生活/心理串联 · 收束）。

Source anchor:
边界不是把人推远，而是给关系留出可以呼吸的房间。

Reader takeaway:
屏风后留出可呼吸区域，暖灯亮、天气卡转晴——边界让关系有空间，而非推远人。

Domain and mood:
生活 / 心理；安静、透气、收束、有温度

Core action:
shelter — 照料员在可呼吸区放置空 chair，灯亮

Paper operator:
- operator family: Care Folder / 照料员
- action: 在屏风后的 breathing zone 放置 empty chair，点亮 paper lamp
- object acted on: 可呼吸区 + 空椅 + 亮灯 + weather card（晴）
- relation clarified: 边界终点是「可呼吸的房间」，不是隔绝
- what breaks if removed: 文章论点「留出空间」失去可视 payoff
- motif payoff: weather card「阴→晴」；lamp 灭→亮

Metaphor world:
延续 soft boundary room：blue carrier ribbon 松落至 breathing zone；屏风侧 quiet margin；茶、空椅、亮灯。

Composition:
- 单焦点：可呼吸区 + 亮灯
- generous quiet zones
- 中文标签：可呼吸、留白、晴、亮灯、房间
- 可选短句纸签：给关系留出可以呼吸的房间

Style:
- 系列一致 palette；growth mint 轻标记「呼吸区」
- editorial, tactile, warm but not childish
- 不要 mascot 挥手、不要 Xiaohei

Quality target:
publish-grade，三秒读懂：边界收束为可呼吸的关系空间。
```

---

## 批量规划提示（串联专用）

```text
用 $paper-operators 给下面这篇文章规划一个 N 张正文配图系列，先不要生成图。

要求：
- 先读 references/series-and-chaining.md
- 给出 article throughline、set length、shared world/operator/palette/label style
- 每张图：role、anchor、relation、operator+action、throughline state、labels
- 填写 continuity checklist
- 至少一张非工程/产品图（若文章领域允许）

文章：
{paste article}
```
