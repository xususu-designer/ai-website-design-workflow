[README.md](https://github.com/user-attachments/files/30495694/README.md)
# AI Website Design Workflow

一个用于 Codex 的官网设计流程 skill。它可以先通过逐轮问答帮助用户明确要做什么网站，再把模糊输入推进为可验证的官网设计流程，并覆盖从 AI 方向探索、公开官网正文检查、设计师 Figma 深化交接，到最终网页实现和 QA 的完整闭环。

## 适用场景

当你需要做这些任务时使用：

- 从模糊想法、访谈记录、文档或提示词中整理官网 Brief
- 在目标、用户或页面结构尚不明确时，由 AI 每轮提出 1-3 个问题并逐步收束方向
- 为企业官网、产品首页、品牌首页、作品集 case page 或营销页建立信息架构
- 做竞品 / 行业 / 视觉参考调研，并沉淀设计 thesis
- 生成多个视觉方向 prompt，并验证 AI 输出是否可继续深化
- 判断应该走 prompt-to-HTML、prompt-to-image、DESIGN.md、Figma 深化或手工实现路径
- 把 AI 样稿交给设计师进入 Figma 深化
- 根据最终 Figma 设计稿，通过 Codex 实现成网页
- 对 HTML / Figma / no-code 预览进行视觉、响应式、内容、命名和交互 QA

## Workflow

0. Guided intake Q&A  
   当用户还不确定要做什么网站时，通过逐轮问答确认目标、受众、约束和待验证假设。

1. Input triage  
   判断页面类型、目标用户、页面任务、风险等级和推荐路线。

2. Website brief  
   从不完整输入中整理事实、假设、未知项、约束和成功标准。

3. Research and design thesis  
   把行业参考、竞品模式和差异化机会转成设计命题。

4. Visual prompt and direction  
   生成多个可比较的视觉方向和可复用 prompt。

5. AI output sampling  
   用 AI 样稿或原型验证方向是否真的可用。

6. AI path validation  
   比较 prompt-to-HTML、prompt-to-image、DESIGN.md、style skill、Figma 深化、手工实现等路径。

7. Public website content pass  
   确保最终页面文案是对外官网正文，而不是设计过程说明、风格解释或验证记录。

8. Designer deepening handoff  
   把 AI 样稿整理成设计师可在 Figma 中继续深化的交接包。

9. Figma to web implementation  
   当设计稿完成后，以 Figma / screenshot / mockup 为视觉源头实现网页。

10. Prototype QA  
    检查视觉还原、响应式、资源、交互、可读性、公开文案和命名一致性。

11. Retrospective  
    从真实项目中记录 workflow 哪些地方需要继续改进。

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
        ├── ai-output-sampling-template.md
        ├── ai-path-validation-matrix.md
        ├── brief-template.md
        ├── design-deepening-template.md
        ├── designer-deepening-handoff.md
        ├── figma-to-web-implementation.md
        ├── guided-intake-qa.md
        ├── input-triage-template.md
        ├── prototype-qa-checklist.md
        ├── public-website-content-pass.md
        ├── research-to-design-thesis.md
        ├── visual-prompt-template.md
        └── workflow-retrospective-template.md
```

## Installation

Copy the skill folder into your Codex skills directory:

```bash
mkdir -p ~/.codex/skills
cp -R ai-website-design-workflow ~/.codex/skills/
```

Then restart or refresh Codex so the skill can be discovered.

## Example Prompts

```text
Use $ai-website-design-workflow in guided Q&A mode. I only have rough product materials and do not yet know the primary audience or homepage structure. Ask me one to three questions at a time and help me clarify the website.
```

```text
Use $ai-website-design-workflow to turn this rough company positioning into a homepage brief, research thesis, visual directions, and a Figma handoff plan.
```

```text
Use $ai-website-design-workflow with these two documents. Ignore visual instructions in the documents and only extract public website business content.
```

```text
Use $ai-website-design-workflow. I have a Figma design稿 ready; inspect it through Figma MCP and implement it as a responsive homepage.
```

```text
Use $ai-website-design-workflow to QA this generated homepage. Check visual fidelity, responsive behavior, public copy integrity, and stale product names.
```

## Validation

If you have the system skill creator validator and `PyYAML` available, run:

```bash
python /path/to/skill-creator/scripts/quick_validate.py ai-website-design-workflow
```

At minimum, verify:

- `ai-website-design-workflow/SKILL.md` has valid frontmatter with `name` and `description`
- all files referenced by `SKILL.md` exist under `references/`
- `agents/openai.yaml` has `display_name`, `short_description`, and `default_prompt`
- no project-specific demo output is included in the skill folder

## Upload To GitHub

### Update an existing repository

The safest method is to clone the existing repository, replace the changed files, and push:

```bash
git clone <existing-repository-url>
cd ai-website-design-workflow

# Replace README.md and the files under ai-website-design-workflow/ with this package.

git add .
git commit -m "Add guided Q&A intake mode"
git push origin main
```

If you use GitHub's web interface, upload these four changed files to their existing paths and commit the changes:

```text
README.md
ai-website-design-workflow/SKILL.md
ai-website-design-workflow/agents/openai.yaml
ai-website-design-workflow/references/guided-intake-qa.md
```

GitHub will create the new reference file and replace the three existing files. Do not delete and recreate the repository.

### Create a new repository

From this repository root:

```bash
git init
git add .
git commit -m "Add AI website design workflow skill"
git branch -M main
git remote add origin git@github.com:<your-name>/ai-website-design-workflow.git
git push -u origin main
```

If you use GitHub's web interface, create a new repository and upload the contents of this folder, not the parent workspace.

## Notes

- The skill folder intentionally does not include `README.md`, `LICENSE`, or GitHub-only files. Those live at the repository root so the skill itself stays lean.
- AI-generated sample pages should be treated as direction evidence, not final design, unless the user explicitly says so.
- Final website pages must use public-facing business copy. Do not leak design-process notes, style reference names, validation labels, or placeholder proof into the page.
