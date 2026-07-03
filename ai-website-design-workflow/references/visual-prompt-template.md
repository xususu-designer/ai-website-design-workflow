# Visual Prompt Template

Use this template to turn a design thesis into visual directions and reusable prompts.

## Inputs

- Design thesis:
- Brand keywords:
- Audience:
- Content priority:
- Public copy source:
- Must-have sections:
- Visual references:
- Constraints:

## Direction Diversity Rules

Generate directions that differ on at least three axes:

- Layout model: hero image, split system diagram, editorial portal, product UI, immersive scene
- Color mode: dark, light, photographic, brand-led, neutral editorial
- Visual metaphor: system map, real-world context, product interface, customer outcome, editorial narrative
- Trust strategy: proof-led, story-led, product-led, category-led, founder/brand-led
- Implementation format: HTML-first, image-first, Figma-first, component-system-first

If all directions share the same palette, layout, or metaphor, regenerate before choosing.

## Visual Direction Candidates

Generate 3-5 directions by default. Use more only when the user asks for broader divergence.

| Direction | Core Metaphor | Visual Keywords | Fit | Risk | Useful Elements |
| --- | --- | --- | --- | --- | --- |
| Direction 1 |  |  |  |  |  |
| Direction 2 |  |  |  |  |  |
| Direction 3 |  |  |  |  |  |
| Direction 4 |  |  |  |  |  |
| Direction 5 |  |  |  |  |  |

## Screening Criteria

| Criteria | Question |
| --- | --- |
| Brand fit | Does it match the company and audience? |
| Industry recognition | Does it signal the right domain? |
| Differentiation | Does it avoid generic site sameness? |
| Page feasibility | Can it become sections and components? |
| Extension | Can it support more than the hero? |
| Evidence | Is the direction grounded in brief, research, or a labeled assumption? |

## Chosen Direction

- Chosen route:
- Why:
- What to keep:
- What to reject:
- What to combine:

## Evidence Status

| Claim | Status | Source / Basis | Risk If Wrong | Next Verification |
| --- | --- | --- | --- | --- |
|  | Fact / Assumption / Design judgment / Unknown |  |  |  |

## Visual Constraint Package

- Layout:
- Color:
- Typography:
- Imagery:
- Icon / diagram style:
- Motion:
- Component style:
- Do not use:
- Copy boundary:

## Moodboard Search Terms

- Industry terms:
- Visual metaphor terms:
- Layout terms:
- Material / texture terms:
- Anti-reference terms:

## Reusable Generation Prompt

Use this structure:

```text
Create a [page type] for [company/product] in [industry].
Audience: [audience].
Goal: [goal].
Core message: [message].
Visual direction: [chosen route].
Information structure: [sections].
Style constraints: [layout, color, typography, imagery, component rules].
Public copy should come from [approved source / brief], not from style references.
Output should emphasize [priority] and avoid [negative rules].
```

## Negative Prompt

```text
Avoid generic AI gradients, meaningless glowing spheres, unrelated futuristic city backgrounds, stock-looking people, excessive dark sci-fi, vague slogans, fake metrics, copied brand identity, visible design-process notes, style-reference brand names as page copy, and layouts that hide the actual product or value.
```
