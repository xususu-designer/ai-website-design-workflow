# Figma To Web Implementation

Use this when the designer has refined the page in Figma and the user asks Codex to implement it as a webpage.

If Figma MCP tools are available and the user provides a Figma file, frame, link, or node, use the relevant Figma skill/tool instructions before reading or manipulating the design. If only screenshots or exports are provided, inspect those files visually and implement from the visible design.

## Inputs

- Figma file / frame / node / screenshot:
- Target technology:
- Output path:
- Required breakpoints:
- Existing codebase:
- Public copy source:
- Assets source:

## Design Inspection

Capture the design before coding.

| Area | Notes |
| --- | --- |
| Frame sizes |  |
| Layout grid |  |
| Typography |  |
| Color roles |  |
| Image / media assets |  |
| Icons / diagrams |  |
| Components |  |
| Motion / interactions |  |
| Responsive behavior |  |

## Implementation Boundary

State what is being implemented.

- Page(s):
- Technology:
- Static or interactive:
- Assets to reuse:
- Assets to recreate:
- Out of scope:

## Section And Component Mapping

| Figma Section / Node | Web Section / Component | Content Source | Asset Handling | Responsive Rule |
| --- | --- | --- | --- | --- |
|  |  |  |  |  |

## Fidelity Rules

- Preserve visible hierarchy, spacing rhythm, image treatment, and component proportions.
- Use the Figma design as the visual source of truth once the user says the design稿 is ready.
- Keep public website copy from the approved content source unless the Figma text is clearly newer or the user confirms it.
- Do not reintroduce exploratory style labels, reference-brand names, or validation notes into the webpage.
- If exact fonts or assets are unavailable, choose the closest local/web-safe substitute and record the gap.
- Implement responsive behavior intentionally; do not rely on accidental browser shrinkage.

## Verification

Before delivery:

- Check generated page at desktop and mobile widths when possible.
- Compare hero, key sections, typography scale, colors, and spacing against Figma or screenshot.
- Verify images/assets load.
- Verify public copy has no stale names or internal process language.
- Report fidelity gaps, unavailable assets, and any unverified interactions.

## Handoff Output

- Files changed:
- Preview URL or file:
- Verification performed:
- Fidelity gaps:
- Next fixes:
