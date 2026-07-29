# Prototype QA Checklist

Use this template when checking an HTML prototype, Figma-to-code output, Cursor/Codex output, no-code preview, screenshot, or implementation preview.

## Inputs

- Design reference:
- Prototype URL or files:
- Target viewport:
- Expected interactions:
- Known constraints:

## Required Verification Evidence

Do not mark prototype QA complete without at least one visual capture or an explicit reason why capture is unavailable.

- Desktop screenshot:
- Mobile screenshot:
- Full-page screenshot:
- Console/runtime issues:
- Broken assets:
- Text overflow:
- Public website copy:
- CTA click behavior:
- Reduced motion:
- Keyboard focus:

## Viewports

| Viewport | Purpose | Result |
| --- | --- | --- |
| 1440 desktop | Primary desktop review |  |
| 1024 tablet | Mid-size reflow |  |
| 390 mobile | Narrow mobile usability |  |

## Visual Restoration

| Check | Pass / Issue | Notes | Priority |
| --- | --- | --- | --- |
| Layout proportions match the design |  |  |  |
| Typography scale and weight match |  |  |  |
| Color and contrast match |  |  |  |
| Spacing rhythm is consistent |  |  |  |
| Images / diagrams render correctly |  |  |  |
| Components keep intended hierarchy |  |  |  |

## Responsive Behavior

| Viewport | Check | Notes |
| --- | --- | --- |
| Desktop | No overlap, cropped text, broken hero, or blank areas |  |
| Tablet | Sections reflow predictably |  |
| Mobile | Text remains readable and CTAs remain usable |  |

## Motion And Interaction

| Check | Notes |
| --- | --- |
| Motion supports the message rather than distracting |  |
| Hover / scroll / reveal effects are smooth enough for prototype review |  |
| Reduced-motion fallback is considered when needed |  |
| Important content is not hidden behind animation |  |

## Accessibility And Readability

| Check | Notes |
| --- | --- |
| Text contrast is readable |  |
| Focus states are visible |  |
| Buttons and links are identifiable |  |
| Images have useful alt text when needed |  |
| Text does not depend on background image legibility alone |  |

## Public Content Integrity

Use this for marketing sites, official websites, campaign pages, and product homepages.

| Check | Pass / Issue | Notes |
| --- | --- | --- |
| Hero states company/product, offer, audience outcome, and CTA |  |  |
| Page copy describes real capabilities, solutions, services, and benefits |  |  |
| No design-process wording appears in public page text |  |  |
| No style-reference brands appear as visible copy unless legally/publicly intended |  |  |
| Required names and product terms are consistent |  |  |
| Unsupported metrics, fake customers, or placeholder proof are removed or marked outside the public page |  |  |
| Metadata, alt text, SVG text, and accessibility labels do not contain stale names or internal notes |  |  |

## Handoff Boundary

State clearly:

- This prototype validates:
- This prototype does not validate:
- Frontend still needs to check:

## Fix Priorities

1. Critical:
2. Important:
3. Nice to have:
