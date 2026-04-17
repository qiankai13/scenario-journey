# Templates

Use these output patterns based on the user's requested format.

## 1. Standard Template

```md
## Scenario Definition

- User:
- Context:
- Goal:
- Success criteria:
- Constraints:
- Assumptions:

## Journey

### Stage 1: [Name]

- Behavior:
- Intent:
- Psychology:
- System response:
- Friction:
- Opportunity:

### Stage 2: [Name]

- Behavior:
- Intent:
- Psychology:
- System response:
- Friction:
- Opportunity:

## Key Judgments

- Biggest breakpoint:
- Lowest emotional point:
- Main decision hesitation point:
- Main information gap:
- Main system mismatch:
- Best AI intervention point:
- Highest-priority optimization stage:

## Design Recommendations

### Recommendation 1

- Action:
- Expected impact:
- Relative effort:
- Dependencies:

### Recommendation 2

- Action:
- Expected impact:
- Relative effort:
- Dependencies:

### Recommendation 3

- Action:
- Expected impact:
- Relative effort:
- Dependencies:

## Technical Capability Requirements

- Perception:
- Data:
- Reasoning:
- Execution:
- Interaction support:
- Governance:
- Performance:
```

## 1.5. Minimum Input Checklist

Use this when the user input is vague and you need to show what is known vs inferred.

```md
## Input Check

- Known:
- Missing:
- Assumptions used:
- Confidence level:
```

## 2. Matrix Template

Use this when the user asks for a matrix, whiteboard-ready view, or PPT-friendly journey table.

Default to the compact version below unless the user explicitly needs the expanded journey-map view.

### Compact Matrix

```md
| Attribute \\ Stage | Stage 1: Trigger | Stage 2: Enter | Stage 3: Explore | Stage 4: Decide | Stage 5: Execute | Stage 6: Complete / Review |
| --- | --- | --- | --- | --- | --- | --- |
| Behavior |  |  |  |  |  |  |
| Intent |  |  |  |  |  |  |
| Psychology / Emotion |  |  |  |  |  |  |
| System response |  |  |  |  |  |  |
| Friction / Risk |  |  |  |  |  |  |
| Opportunity |  |  |  |  |  |  |
| AI / System intervention |  |  |  |  |  |  |
| Technical requirement |  |  |  |  |  |  |
```

### Expanded Matrix

If the matrix is for a more classic journey-map presentation, add these rows:

```md
| Touchpoints |  |  |  |  |  |  |
| Channels |  |  |  |  |  |  |
| Thoughts / Quotes |  |  |  |  |  |  |
| Emotion trend / score |  |  |  |  |  |  |
| Target experience |  |  |  |  |  |  |
| One-line tension |  |  |  |  |  |  |
```

## 3. AI-Native Stage Template

Use this when the scenario explicitly involves system intelligence or cross-app orchestration.

```md
### Stage [N]: [Name]

- Behavior:
- Intent:
- Psychology:
- System response:
- Friction:
- Opportunity:
- Signals:
- Inference:
- AI action:
- Risk:
- User control point:
- Trust threshold:
- Reversibility:
```

## 4. PPT Structure Template

Use this when the user wants a slide-ready output.

```md
1. Slide 1: Scenario definition
   User, context, goal, success criteria, constraints

2. Slide 2: Journey overview
   4-7 stages with one-line summary per stage

3. Slide 3: Full journey matrix
   Stage columns x analysis rows

4. Slide 4: Key tensions and breakpoints
   Biggest breakpoint, emotional low point, hesitation point, mismatch

5. Slide 5: Design priorities
   Priority stage, why it matters, expected gains

6. Slide 6: AI intervention strategy
   Recommend vs confirm vs automate vs stay silent

7. Slide 7: Technical capability requirements
   Perception, data, reasoning, execution, interaction support, governance, performance
```

## 4.5. Visualization Handoff Template

Use this when another skill or tool will turn the analysis into a visual journey map.

```md
## Visualization Handoff

### Stage 1: [Name]

- Touchpoints:
- Channels:
- Actions:
- Thoughts:
- Emotion trend or score:
- Pain points:
- Opportunities:
- One-line tension:
- Target experience:
- Technical support needed:
```

## 5. Prioritization Prompt

If the user asks "which part should we optimize first", answer with:

```md
## Priority Judgment

- First priority stage:
- Why now:
- What changes in user experience:
- What business or usage metric it likely affects:
- What minimum product change is enough to validate it:
```

## 6. QA Prompt

Use this before final delivery when the output must go into a document, review, or deck.

```md
## QA Check

- Is this one task chain rather than a broad lifecycle?
- Do the stages follow time?
- Does every stage include behavior, intent, psychology, system response, friction, and opportunity?
- Is the biggest breakpoint explicit?
- Is the priority stage explicit?
- If AI is involved, are intervention timing and user control boundaries explicit?
- Do the technical requirements clearly come from the journey analysis?
- Do the technical requirements map back to the key journey problems rather than forming a separate checklist?
```
