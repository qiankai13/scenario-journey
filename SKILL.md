---
name: scenario-journey
description: Use when a user asks to analyze a scenario, user journey, customer journey, experience map, touchpoint map, service blueprint, service flow, AI-native interaction path, or a key product experience chain, especially when the input is vague and needs to be rewritten into stages, tensions, intervention points, design priorities, and technical capability requirements for documents, PPTs, or cross-team reviews.
---

# Scenario Journey

## Overview

Turn a vague scenario into a journey that supports product decisions, interaction design, AI intervention design, and technical planning.

This skill is not a journey-map generator. It is a scenario decomposition and opportunity-identification workflow.

## When to Use

Use this skill when the user provides any of the following:

- A vague scenario description that needs to be made concrete
- A key product flow that needs optimization
- A cross-step mobile or multi-app task experience
- An AI-native scenario where the system should intervene in stages
- A journey analysis that must be expressed in Markdown, a matrix, a document, or a PPT outline
- A request framed as journey map, experience map, touchpoint map, or service blueprint, but where the real need is structured analysis rather than just a visual

Typical prompts include:

- "分析用户在通勤路上快速处理多个消息与任务的体验旅程"
- "为什么用户在配置系统级 AI 助手时中途放弃"
- "请分析从通知进入任务处理的体验旅程，并找出优化点"
- "拆解用户发起跨 App 目标任务时，AI 应该如何分阶段介入"

Do not use this skill for:

- Pure page inventories
- Feature lists without a time-based scenario
- Broad narratives like "analyze the user's whole day"

If the user explicitly wants a visual deck or slide output, keep this skill as the analysis layer first, then hand off to a presentation or PPT skill for the rendering layer.

## Non-Negotiables

Always enforce these rules:

- Start with `who + context + goal`. Never start from screens or features.
- Use time progression as the main axis. Do not organize by page.
- Each stage must include behavior, intention, psychology or emotion, system response, friction, and opportunity.
- Do not stop at description. Make judgments.
- Always identify the most important breakpoint and the most valuable optimization stage.
- If AI or system intelligence is involved, explicitly analyze where the system should intervene, where it should confirm, where it should automate, and where it should stay quiet.
- Map experience findings into technical capability requirements.
- Separate `analysis` from `rendering`. First build the analytical model, then compress it for matrix, PPT, or whiteboard formats.

## Workflow

### 1. Rewrite the scenario

Rewrite the input into one precise proposition:

`A certain user, in a certain context, wants to complete a certain goal, and goes through a multi-stage experience process.`

Always define:

- User role
- Triggering context
- Core goal
- Success criteria
- Constraints

If the user gives a broad scenario, compress it into a single task chain before continuing.

### 1.5. Gather the minimum working inputs

Before going deep, check whether you have enough information to produce a defensible journey.

Core inputs:

- Stages or a way to infer them
- User actions or behaviors
- Goal and success criteria
- Pain points or evidence of friction

Useful optional inputs:

- Touchpoints or channels
- Representative thoughts or quotes
- Emotional direction or rough highs and lows
- Existing solution constraints
- Desired output mode: prose, matrix, PPT, or AI-native design view

If the input is incomplete, infer cautiously and mark assumptions rather than pretending certainty.

### 2. Break the journey into 4-7 stages

Use time progression, not UI structure.

Common stage patterns:

- Trigger
- Enter
- Explore
- Compare or decide
- Execute
- Complete
- Review or follow-up

Not every analysis needs all of them, but the sequence must explain how the experience evolves.

When the final format is matrix or PPT, also track these optional stage-level fields if they add value:

- `Touchpoints`: where the user interacts with the system or service
- `Channels`: app, system UI, store, message, email, voice, physical context
- `Thoughts`: short first-person paraphrases or quotes
- `Emotion level`: a rough relative score or label, only if it helps comparison

### 3. Fill every stage with six required fields

For each stage, provide:

- `Behavior`: what the user is doing
- `Intent`: what the user is actually trying to achieve
- `Psychology`: what the user is feeling, fearing, or hesitating about
- `System response`: what the product or system does now
- `Friction`: what blocks, slows, confuses, or risks failure
- `Opportunity`: what should change in design or system behavior

Do not output bare action steps. The psychology and friction are mandatory.

### 4. Make experience judgments

After the stages, explicitly judge:

- Biggest breakpoint
- Lowest emotional point
- Main decision hesitation point
- Main information gap
- Main system mismatch
- Best AI intervention point, if applicable
- Highest-priority stage to optimize

State why each judgment matters.

### 5. Translate experience into design moves

Turn the judgments into concrete product or interaction decisions:

- Which stage to optimize first
- What interaction ability to add or remove
- What system ability to add
- What feedback, confirmation, or guidance should change
- Which metrics or experience outcomes are likely to improve

Avoid generic advice like "simplify the flow" unless it is tied to a specific stage and mechanism.

When relevant, distinguish between:

- Interaction changes
- System capability changes
- Operational or service changes
- AI intervention strategy changes

### 6. Translate experience into technical capability requirements

Infer the underlying system requirements needed to support the target experience.

Always cover these dimensions when relevant:

- `Perception`: context, device state, environment, user state, signal capture
- `Data`: history, preferences, task context, cross-app state, cross-device sync
- `Reasoning`: intent recognition, stage detection, priority, prediction, risk judgment
- `Execution`: app orchestration, system actions, automation chains, background continuation
- `Interaction support`: overlays, progressive confirmation, low-interruption reminders, result feedback, interruption handling
- `Governance`: permissions, rollback, explainability, authorization boundaries, auditability
- `Performance`: latency, weak-network tolerance, stability, background continuity, on-device responsiveness

The goal is to translate experience language into architecture language.

## Delivery Modes

Choose the lightest format that still supports the decision.

- `Analytical prose`: best for product thinking, reviews, and design alignment
- `Matrix`: best for workshops, whiteboards, and cross-functional comparison
- `PPT outline`: best when the analysis will be turned into slides
- `Visualization handoff`: best when another skill or tool will render the final journey map

If the user asks for a journey-map-style deliverable, do not jump directly into layout instructions. First stabilize the scenario definition, stage model, and priority judgment.

## Visualization Handoff

If this analysis will later be rendered as a journey map, provide a compressed handoff layer in addition to the main analysis.

Recommended handoff fields by stage:

- Stage name
- Touchpoints
- User actions
- User thoughts
- Emotion trend or score
- Pain points
- Opportunities
- Target experience
- Technical support needed

This keeps the analytical core intact while making the result renderable in PPT, whiteboards, or other visualization tools.

## Output Rules

By default, produce the following sections:

1. `Scenario definition`
2. `Stage-by-stage journey`
3. `Key judgments`
4. `Design recommendations`
5. `Technical capability requirements`

If the user asks for a matrix, PPT structure, or AI-native enhancement, use the templates in [references/templates.md](./references/templates.md).

If the user asks for a presentation-ready artifact, include both:

- The core analytical judgment
- The compressed handoff structure for the visualization layer

## Default Output Shape

### Scenario Definition

Include:

- User
- Context
- Goal
- Success criteria
- Constraints

### Stage-by-Stage Journey

Prefer 4-7 stages. For each stage include:

- Stage name
- Behavior
- Intent
- Psychology or emotion
- System response
- Friction or risk
- Opportunity

### Key Judgments

Must include:

- Biggest breakpoint
- Lowest emotional point
- Best AI intervention point, if relevant
- Highest-priority optimization stage

### Design Recommendations

Give a prioritized set of recommendations tied to the judged stages.

### Technical Capability Requirements

Group requirements by perception, data, reasoning, execution, interaction support, governance, and performance.

## QA Checklist

Before finalizing, verify:

- The scenario has been narrowed to one task chain, not a whole day or broad lifecycle
- The stages follow time progression rather than page structure
- Every stage includes behavior, intent, psychology, system response, friction, and opportunity
- The output contains judgments, not just observations
- The highest-priority stage is explicit and defended
- AI intervention timing and boundaries are explicit when AI is involved
- Technical capability requirements are derived from the journey, not pasted in as a generic checklist
- If a matrix or PPT handoff is included, the compressed fields still match the main analytical judgment

## AI-Native Extension

If the scenario involves AI or system intelligence, add these fields where useful:

- `Signals`: what the system can perceive
- `Inference`: what the AI infers from those signals
- `AI action`: what the system should do
- `Risk`: what can go wrong
- `User control point`: where the user authorizes, confirms, edits, or interrupts

Also judge intervention style:

- Recommend
- Confirm
- Auto-execute
- Stay silent

## Quality Bar

Good output should:

- Collapse broad narratives into one clear task chain
- Expose real tension, not just visible steps
- Show where the system should appear and where it should not
- Prioritize instead of flattening every issue
- Be directly reusable in a document, a workshop, or a review

Bad output typically:

- Repeats the user's wording without sharpening it
- Lists pages instead of a journey
- Describes actions without intentions or emotions
- Lists all problems equally
- Mentions AI without specifying intervention timing or boundaries

## Response Style

Write like a senior product and experience architect:

- Direct
- Specific
- Structured
- Decisive

Do not use filler. Do not write empty framework language. Every section should help someone decide what to optimize and what capabilities must exist to support it.
