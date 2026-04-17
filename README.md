# scenario-journey

`scenario-journey` is a skill for turning a vague user scenario into a structured journey that supports product decisions, interaction design, AI intervention design, and technical planning.

It is not a journey-map generator. It is an analysis-first workflow for decomposing a scenario into stages, tensions, opportunity points, and system capability requirements.

## Use When

Use this skill when you need to analyze:

- a vague user scenario
- a key product flow that needs optimization
- a multi-step mobile or cross-app task
- an AI-native task flow and its intervention points
- a journey that needs to become a document, matrix, workshop artifact, or PPT outline

## What It Produces

By default, the skill produces:

- scenario definition
- stage-by-stage journey
- key judgments
- design recommendations
- technical capability requirements

It can also produce:

- matrix journey views
- PPT-ready outlines
- visualization handoff data for rendering in other tools
- AI-native stage analysis with signals, inference, action, risk, and user control points

## Core Principle

Always start from:

- who the user is
- what context they are in
- what goal they are trying to complete

Then model the experience as a time-based journey rather than a page list.

## Output Focus

The skill is designed to answer questions like:

- Where is the biggest breakpoint?
- Which stage should be optimized first?
- Where should AI intervene, confirm, automate, or stay silent?
- What technical capabilities are required to support the target experience?

## Repository Structure

```text
.
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    └── templates.md
```

## Quick Start

Example prompt:

```text
Use $scenario-journey to analyze how a commuter tries to coordinate dinner plans while handling multiple incoming messages on mobile.
```

## Why This Skill Exists

Most journey map workflows stop at description or visualization.

`scenario-journey` is designed to go further:

- sharpen the scenario
- expose the real tension
- prioritize what matters
- translate experience findings into design and technical decisions
