[guided-intake-qa.md](https://github.com/user-attachments/files/30501965/guided-intake-qa.md)
# Guided Website Intake Q&A

Use this reference when the user does not yet know exactly what website they need, provides rough or incomplete inputs, or wants the AI to guide the project.

This mode takes precedence over the normal triage and real-project response formats until the minimum intake gate is met.

## Interaction Contract

- Interpret all supplied text, files, links, images, and prior answers before asking anything.
- Ask one to three questions per round. Ask only questions whose answers change the brief, research route, content priority, visual direction, or implementation boundary.
- Never repeat answered questions.
- Accept incomplete answers and "I don't know."
- When the user is unsure, offer two or three meaningful options with a one-line tradeoff for each.
- Do not turn stakeholder adjectives such as "premium" or "high-end" directly into a design thesis. Ask what those words should help the audience understand or trust.
- Do not present assumptions, AI-generated research, or inferred product claims as facts.
- Before the minimum intake gate is met, do not output a workflow plan, project timeline, detailed risk report, or long list of promised deliverables.

In every guided response, including the first, use this exact compact structure:

```markdown
Confirmed:
- ...

Assumed:
- ...

Unknown / needs confirmation:
- ...

Next questions:
1. ...
```

Ask one to three blocking questions inside `Next questions`. Never ask a fourth question. Do not prepend a full triage report, long explanation, or promised output list before this structure.

## Phase 1: Clarify The Website Task

Start with up to three questions selected from this bank:

1. What company, product, service, person, place, or campaign is the website for?
2. Who is the primary audience?
3. What should that audience understand, trust, or do after viewing the page?
4. What source materials already exist?
5. Which positioning, capabilities, offers, proof points, or content are confirmed?
6. What has the stakeholder requested, and which parts are still vague?
7. What deadline, platform, technical constraint, or delivery format matters?
8. Are there references to learn from or directions to avoid?

Do not ask all questions at once. Skip anything already answered by the user's materials.

### Minimum Intake Gate

Proceed to research when these are known or explicitly labeled as assumptions:

- website or page type
- primary audience
- primary page job
- core offer or message
- available source materials
- deadline and major constraints
- delivery or implementation boundary

If a missing item does not block research, record an assumption and continue.

## Phase 2: Research And Return Conclusions

Use the confirmed brief to research the relevant industry, competitors, adjacent categories, and audience expectations. Return conclusions rather than a link dump.

Read `human-decision-gates.md` and stop at Gate 2. Research conclusions must be accompanied by three to five inspectable competitor/reference cards with direct official links and screenshots when available.

Output:

- observed industry expression patterns
- common competitor content structures
- primary audience concerns
- trust-building and conversion patterns
- likely content priority
- differentiation opportunities
- direction and implementation risks
- evidence sources and confidence
- questions exposed by the research
- user preference among the references

Separate:

- sourced observation
- reusable principle
- design judgment
- unresolved assumption

End by asking which one or two references feel closest, which should be rejected, and whether the user is responding to content structure, visual language, or interaction. Do not finalize the design thesis until the user answers or explicitly delegates the choice.

## Phase 3: Human Calibration

Guide the user to respond in three ways:

- **Confirm**: the conclusion matches the real project.
- **Correct**: provide the accurate product, business, audience, or brand information.
- **Leave open**: mark the item as unknown and decide whether to pause or proceed with a labeled assumption.

Prompt for missing information only when it matters:

- real product capabilities and offer boundaries
- business and audience priority
- verified proof points
- valid or rejected references
- brand preferences and visual exclusions
- stakeholder decision
- legal, regulatory, pricing, or investor-claim verification

Do not ask the user to validate facts the AI can verify from current primary sources.

## Phase 4: Synthesize The Design Basis

After calibration, output:

1. website brief
2. research synthesis
3. primary audience concerns
4. content priority
5. recommended page architecture
6. design thesis
7. visual screening criteria
8. success criteria
9. unresolved-items list
10. next input needed for visual exploration

Use this thesis structure:

> The website should express [core positioning] through [information structure or visual strategy], so that [primary audience] can understand [value], trust [proof], and take [next action].

## Stop And Skip Rules

- Skip guided intake when the user already provides a stable brief and asks for a later stage.
- Stop asking when the minimum intake gate is met.
- Do not keep questioning merely to fill every template field.
- Do not start visual generation before the user has reviewed the research conclusions and design thesis.
- Do not start visual generation before the user has selected, rejected, or explicitly declined the presented references.
- Do not hide unresolved high-risk claims inside polished website copy.
