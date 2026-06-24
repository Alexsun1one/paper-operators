# Smoke Test For A New Agent

Use this test when you want to know whether a non-Codex agent has actually understood Paper Operators.

## Prompt

```text
请按 Paper Operators 工作流处理下面这句话，先不要生成图，只输出规划和最终生图提示词。

句子：
从问答到派活，Agent 的变化不是更会聊天，而是开始承担一段可检查的工作。
```

## Expected Output Shape

A compatible agent should return something close to:

```text
source anchor:
从问答到派活，Agent 的变化不是更会聊天，而是开始承担一段可检查的工作。

reader takeaway:
Agent 的关键变化是从回答问题变成承接目标、规划、调用工具、保留记忆并交付结果。

domain and mood:
AI/product explanation, clear, workbench-like, not cute.

core action:
Thread Runner pulls a blue work ribbon from Chat/Copilot into an Agent execution board.

operator decision:
use operator: yes

what breaks if removed:
Without the operator pulling the work ribbon, the shift from passive answering to active delegation becomes just a static comparison chart.

operator family:
Thread Runner + Lens Keeper

metaphor world:
high-angle paper workbench with three zones: Chat 问答, Copilot 辅助, Agent 执行.

composition:
left-to-right transformation, blue carrier ribbon, execution board with goal/planning/tools/memory/delivery cards.

labels:
Chat 问答, Copilot 辅助, Agent 执行, 目标, 规划, 工具, 记忆, 交差

final image prompt:
...

QA risks:
Chinese labels may blur; if renderer is weak, reduce labels or leave blank label containers for overlay.
```

## Fail Signals

The agent probably did not understand the guide if it:

- only writes a pretty generic prompt
- skips `what breaks if removed`
- draws a cute mascot standing beside a chart
- turns the idea into a normal PPT flowchart
- ignores Chinese labels
- does not mention renderer limitations or QA risks
