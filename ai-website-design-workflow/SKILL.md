---
name: ai-website-design-workflow
description: Use when designing, auditing, validating, prototyping, handing off, or implementing a website, landing page, product homepage, brand homepage, portfolio case page, campaign page, or marketing site from incomplete inputs, no mature PRD, unclear information architecture, weak research, uncertain visual direction, unclear AI implementation path, or a final Figma/mockup-to-web build. Guides Codex through input triage, website brief creation, research synthesis, design thesis definition, visual direction prompts, AI output sampling, implementation path validation, public website copy, designer/Figma handoff, Figma-to-web implementation, prototype QA, and workflow retrospective.
---

# AI Website Design Workflow

Use this skill to turn rough website inputs into a staged, evidence-aware design process. It is not an automatic website generator. AI expands breadth; the designer makes depth judgments and final decisions.

## Core Rules

- Separate **facts**, **assumptions**, **design judgments**, and **unknowns** in every stage.
- Ask only for inputs that block the current stage. Otherwise make a clearly labeled assumption and continue.
- Keep each decision traceable to user input, source evidence, design thesis, visual constraints, or prototype observations.
- Do not let AI-generated visuals override the brief, thesis, audience, or content priority.
- Do not treat prototypes or generated HTML as production frontend code unless the user explicitly asks for production implementation.
- Extract reusable principles from references; do not copy brands, layouts, copy, proprietary diagrams, or unsupported metrics.
- Separate **public website copy** from **internal design/process notes**. Final website pages must sound like an external company, product, solution, or campaign page, not like a design rationale, style comparison, skill validation, or prototype report.
- When source materials mix business content and visual instructions, extract the business claims, product capabilities, solutions, audiences, CTAs, and proof points first. Apply visual instructions only when the user asks for them.
- Normalize required names, product terms, and banned old terms before final delivery. Run a content pass to catch stale names and internal labels.
- When the user provides a final Figma design or mockup, treat that design as the visual source of truth. Inspect it before coding, map sections and responsive rules, and implement with fidelity rather than reinterpreting the earlier AI prototype.

## Operating Modes

### Real Project Mode

When the user asks to run the website process for a real project, proceed stage by stage. Stop after each stage with:

- stage output
- assumptions made
- risks
- `next input needed`

Continue only when the next stage is not blocked or the user asks you to proceed.

### Single Stage Mode

When the user asks for one stage only, run that stage and keep the output compatible with later stages.

### Validation / Dry-run Mode

When the user asks to validate, audit, test, or improve this workflow as a reusable skill, run the full workflow in one pass using labeled assumptions. Include the stage gates and failure signals, but do not rely on project memory unless the user explicitly asks for a project-specific validation.

## Workflow

### 0. Triage The Website Task

Use `references/input-triage-template.md` when the project type, audience, page job, risk level, or workflow route is unclear.

Output:

- project type
- primary audience
- page job
- input quality
- risk level
- recommended workflow route
- assumptions and blockers

### 1. Create Website Brief

Use `references/brief-template.md` when inputs are incomplete, scattered, stakeholder-written, AI-generated, or missing a mature PRD.

Output:

- input summary
- what is known
- evidence status
- missing information
- constraints
- website brief
- success criteria
- next input needed

### 2. Research And Define Design Thesis

Use `references/research-to-design-thesis.md` when the task needs competitor review, industry references, brand references, category positioning, or current-market proof.

Output:

- research evidence table
- common patterns
- differentiation opportunities
- design thesis
- content priority
- direction risks
- source and assumption notes

### 3. Generate Visual Prompts And Direction

Use `references/visual-prompt-template.md` when the design thesis needs to become visual directions, moodboard search terms, image prompts, website-generation prompts, or style constraints.

Output:

- visual keywords
- moodboard search terms
- meaningfully different visual directions
- screening criteria
- chosen direction or fusion route
- visual constraint package
- reusable generation prompt
- negative prompt

### 3.5 Sample AI Outputs

Use `references/ai-output-sampling-template.md` when prompts need to be tested visually before choosing an implementation path.

Output:

- selected prompt runs
- capture checklist
- observations
- keep/reject notes
- prompt drift
- evidence needed for path validation

Skip this stage only when the user explicitly wants abstract prompts without generated examples, or when no visual generation/prototype route is available yet.

### 4. Validate AI Implementation Paths

Use `references/ai-path-validation-matrix.md` when comparing ways to generate or prototype the page, such as prompt-to-HTML, prompt-to-image, reference generation, DESIGN.md generation, style-skill generation, manual design plus AI coding, Figma-to-code, or no-code builders.

Output:

- project weighting
- validation matrix
- evidence gaps
- strengths and limits per path
- what each path may influence
- recommended path
- decision record

### 5. Deepen The Design

Use `references/design-deepening-template.md` after a path is chosen and the designer needs a stronger page structure, design system seed, hero definition, component inventory, motion plan, or decision log.

Output:

- page architecture
- section-by-section intent
- hero definition
- design system seed
- component inventory
- AI element prompts
- motion rules
- decision log

### 5.5 Create Publishable Website Copy

Use `references/public-website-content-pass.md` before or during prototype implementation when any page copy, HTML content, Framer prompt, Figma text, or no-code page content will be shown as the website itself.

Output:

- content source map
- public page narrative
- section-by-section public copy
- product and solution capability copy
- CTA and conversion copy
- name normalization list
- unsupported or risky claims
- internal-language removal checklist

### 5.6 Prepare Human Design Deepening Handoff

Use `references/designer-deepening-handoff.md` when the AI/Codex prototype, prompt sample, or direction page is intended to become input for the designer's Figma refinement rather than the final page.

Output:

- chosen direction summary
- what the designer should keep, reject, and explore
- public content package
- Figma frame / breakpoint requirements
- component and asset handoff checklist
- unresolved design decisions

### 6. Implement From Final Design

Use `references/figma-to-web-implementation.md` when the user provides a Figma design, Figma MCP access, design link, exported screenshot, or final mockup and asks Codex to implement the page as HTML/CSS/React/Framer-compatible code.

Output:

- design inspection notes
- implementation boundary
- section and component mapping
- responsive rules
- asset extraction or replacement plan
- code implementation
- fidelity gaps and follow-up fixes

### 7. Validate Prototype Quality

Use `references/prototype-qa-checklist.md` when the user has a Figma design, HTML prototype, screenshot, code output, no-code preview, or implementation preview.

Output:

- required verification evidence
- visual restoration checklist
- responsive checklist
- motion and interaction notes
- accessibility and readability notes
- public-content checks
- handoff boundary
- fix priorities

### 8. Retrospect And Improve The Workflow

Use `references/workflow-retrospective-template.md` after one real project run or a skill validation run.

Output:

- run summary
- stage review
- what worked
- what failed or felt unstable
- human judgments AI could not replace
- skill updates needed
- do-not-generalize notes
- next-version notes

## Quality Standards

Evaluate outputs with these standards:

- **Brand fit**: the direction matches the company, product, audience, and page job.
- **Industry fit**: visuals and wording reflect the domain instead of generic template language.
- **Information control**: structure, priority, and page rhythm are clear.
- **Public copy integrity**: final page text describes the real offer, product capabilities, solutions, services, and CTAs; it does not expose design process, style references, validation labels, or prototype caveats.
- **Differentiation**: the page avoids indistinct stock-tech, stock-brand, or one-note aesthetics.
- **Feasibility**: ideas can translate into real sections, components, images, motion, Figma, HTML, or no-code prototypes.
- **Evidence**: research claims, path scores, and design decisions have sources, observations, or labeled assumptions.
- **Anti-generalization**: project-specific preferences are not turned into default rules for unrelated projects.
