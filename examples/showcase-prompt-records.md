# Showcase Prompt Records

This file records reusable public examples. It is intentionally compact: enough to reproduce the reasoning, not a full private generation log.

## A Christmas Carol Story Card

asset name: `showcase-story-card-christmas-carol`
asset role: story/book card
source anchor: Scrooge changes after seeing his past, present, and possible future, then choosing generosity.
relationship type: transformation / moral choice
operator family: Light Catcher / Archive Tender
truth constraints: labels only: `SCROOGE`, `PAST`, `PRESENT`, `FUTURE`, `CHOICE`, `CHANGE`, `GENEROSITY`
output path: `examples/images/showcase/showcase-story-card-christmas-carol.png`
README preview: `examples/images/readme/v2-story-card-christmas-carol.jpg`
caption: A familiar story compressed into character, turning points, consequence, and transformation.
QA result: accepted; readable labels, clear arc, operator reveals transformation.

## Apollo 11 Reference-Informed Explainer

asset name: `showcase-reference-apollo-11`
asset role: reference-informed explainer
source anchor: Apollo 11 is understandable as a chain of real mission objects: Saturn V, Columbia, Eagle, landing, return.
relationship type: sequence / transformation
operator family: Thread Runner / Archive Tender
truth constraints: labels only: `SATURN V`, `COLUMBIA`, `EAGLE`, `LANDING`, `RETURN`, `APOLLO 11`
reference cues: tall Saturn V, cone-shaped command module, angular lunar module with landing legs and gold foil-like facets, gray Moon, blue Earth return arc, splashdown capsule.
output path: `examples/images/showcase/showcase-reference-apollo-11.png`
README preview: `examples/images/readme/v2-reference-apollo-11.jpg`
caption: Real-world cues translated into a paper-stage explainer without copying source imagery.
QA result: accepted; labels are correct, no extra text, mission objects recognizable.

## Project Status Data Story

asset name: `showcase-data-story-status-board`
asset role: data story scene
source anchor: A data story uses exact metric objects plus operator action to explain what needs attention.
relationship type: tension / triage
operator family: Tradeoff Weigher / Gate Builder
truth constraints: exact labels and values only: `OPEN 12`, `AT RISK 5`, `BLOCKED 2`, `DONE 31`, `REVIEW`
output path: `examples/images/showcase/showcase-data-story-status-board.png`
README preview: `examples/images/readme/v2-data-story-status-board.jpg`
caption: A small metric board becomes an action-oriented triage story without losing the numbers.
QA result: accepted; exact values match, no extra numbers, operator action clarifies risk review.

