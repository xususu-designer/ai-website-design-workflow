[README.md](https://github.com/user-attachments/files/30502329/README.md)
# AI Website Design Workflow

一个用于 Codex 的协作式官网设计 Skill。它不会在收到模糊需求后直接生成完整网站，而是通过多轮问答、可检查的竞品与视觉方案，以及必须由人确认的决策闸门，把不完整输入逐步推进为官网 Brief、设计方向、原型和交付物。

## Core Idea

> AI expands breadth; the designer makes depth judgments and final decisions.

AI 负责整理信息、补充研究、扩展方案和生成辅助；设计师负责校准事实、判断方向、确认取舍并控制最终质量。

## Key Features

- 每轮只提出 1–3 个真正影响下一步的高价值问题
- 持续区分 `Confirmed / Assumed / Unknown / Next questions`
- 提供可检查的竞品网站、截图、视觉备选与取舍依据
- 默认采用 Collaborative Mode，不静默替用户完成关键决策
- 在 Brief、竞品、视觉、页面架构、实现路径和最终交付处设置人工决策闸门
- 支持从模糊需求推进到 Figma 深化、HTML 原型、交付与 QA

## Human Decision Gates

```text
Brief Calibration
→ Competitor Preference
→ Visual Direction
→ Architecture and Public Content
→ Implementation Path
→ Final Handoff
```

在每个闸门中，Skill 会提供：

1. What we learned
2. Options you can inspect
3. My recommendation and why
4. Decision needed from you

## Workflow

1. Guided intake and task triage
2. Website Brief
3. Research and design thesis
4. Visual exploration and direction selection
5. AI output sampling and implementation-path validation
6. Public website content pass
7. Designer and Figma deepening handoff
8. Figma-to-web implementation
9. Prototype QA
10. Workflow retrospective

## Repository Structure

```text
.
├── README.md
├── LICENSE
├── .gitignore
└── ai-website-design-workflow/
    ├── SKILL.md
    ├── agents/
    │   └── openai.yaml
    └── references/
        ├── guided-intake-qa.md
        ├── human-decision-gates.md
        ├── input-triage-template.md
        ├── brief-template.md
        ├── research-to-design-thesis.md
        ├── visual-prompt-template.md
        ├── ai-output-sampling-template.md
        ├── ai-path-validation-matrix.md
        ├── design-deepening-template.md
        ├── designer-deepening-handoff.md
        ├── figma-to-web-implementation.md
        ├── public-website-content-pass.md
        ├── prototype-qa-checklist.md
        └── workflow-retrospective-template.md
```

## Installation

Copy only the inner Skill folder into the Codex skills directory:

```bash
mkdir -p ~/.codex/skills
ditto ai-website-design-workflow ~/.codex/skills/ai-website-design-workflow
```

Restart or refresh Codex after installation.

## Example Prompt

```text
Use $ai-website-design-workflow in collaborative mode.

I only have rough product materials and do not yet know the primary audience,
homepage structure, or visual direction. Guide me through several short
decision rounds, show me competitor and visual alternatives, and wait for my
choices before continuing.
```

## Expected Behavior

For incomplete inputs, the first response should:

- use `Confirmed / Assumed / Unknown / Next questions`
- ask no more than three questions
- avoid immediately producing a complete website plan

During later stages, the Skill should present evidence and alternatives, then stop at the relevant human decision gate before continuing.

## Updating

Replace the existing Skill directory with the latest inner folder, then restart Codex:

```bash
ditto ai-website-design-workflow ~/.codex/skills/ai-website-design-workflow
```

When updating the GitHub repository, commit the complete repository structure shown above. Do not place `README.md` inside the installable Skill folder.

## Boundary

- This is a collaborative design-process Skill, not a one-click website generator.
- AI-generated samples are direction evidence, not automatically final design.
- Generated HTML is a validation prototype unless production implementation is explicitly requested.
- Final business claims, visual decisions, implementation choices, and quality approval remain human responsibilities.
