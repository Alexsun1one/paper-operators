# Data Story Scenes

Use this reference when the source includes numbers, rankings, metrics, benchmark results, charts, tables, survey counts, project status, or evidence summaries.

Paper Operators should not pretend to be a rigorous chart renderer. Its job is to turn data into a readable story scene while preserving the facts that appear in the image.

## Data Contract

Before prompting, write:

```text
data source:
chart or metric type:
exact labels:
exact values:
unit:
order:
highlight:
uncertainty:
what the data means:
```

If values cannot be read, ask for data or mark them approximate. Do not invent values to make the scene prettier.

## When To Use Paper Operators

Use Paper Operators when:

- the data needs interpretation, not only plotting
- one comparison, bottleneck, risk, or turn matters most
- a human reader needs a story about what to do next
- the chart can be a physical object inside the scene

Use a native chart / PPT / code-rendered diagram instead when:

- exact axes are the primary deliverable
- the chart must be editable
- there are many values or dense labels
- the final artifact will be audited as a statistical chart

## Composition Patterns

### Compact Chart + Operator

- Put a small chart/table/card as a physical object.
- The operator highlights, weighs, inspects, stamps, routes, or blocks the key point.
- Keep the chart simple: 3-5 categories, one unit, one highlight.

### Risk Board

- Use columns, chips, flags, and a review stamp.
- Good for project status, QA, bugs, incidents, and launch readiness.
- The operator moves a risk chip or stamps the final state.

### Evidence Scale

- Put two or more evidence piles on a scale.
- Good for tradeoffs, strategy, model comparison, claims, and decisions.
- Labels should state evidence roles, not generic `pros` and `cons` unless that is the article's language.

### Before / After Metric Scene

- Show an old state, intervention, and new state.
- Use exact before/after values.
- The operator should physically transform, repair, or route the metric object.

## Prompt Requirements

For every data story prompt, include:

```text
Exact data: show only these values: ...
Exact labels: include only these labels: ...
Do not add extra categories, numbers, axes, dates, legends, or fake sources.
If a number cannot fit clearly, omit it rather than inventing or shrinking it.
```

## QA

Reject if:

- any value is wrong
- category order is swapped
- the image adds fake numbers or fake sources
- the scene hides the chart
- the operator does not clarify the data meaning
- it looks like a spreadsheet screenshot with paper texture

Accept if:

- the main data point is visible in three seconds
- exact values and labels match the contract
- the operator action explains the implication
- the image works as a data story even if the surrounding article is not visible

