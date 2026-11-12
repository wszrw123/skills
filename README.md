# Image-Led UI Design

**Image-led UI/UX design and interaction simplification for AI coding agents.**

A lightweight Agent Skill for turning existing interfaces into more expressive, coherent, and easier-to-use products. It combines image-driven visual direction, reusable visual assets, preservation of approved design language, and practical interaction-cost reduction.

[中文说明](#中文介绍) · [Installation](#installation) · [Usage](#usage)

## What it helps with

- **Image-led redesign** — use visual references and image generation to establish a clear design direction, not just tweak CSS values.
- **Preserve what already works** — identify user-approved colors, typography, imagery, components, and layout patterns; extend them instead of redesigning everything.
- **Cohesive visual assets** — choose photography, illustrations, icon sets, and decorative assets by purpose; keep a consistent visual language.
- **Simpler workflows** — reduce unnecessary fields, repeated input, clicks, waiting, and decision burden without hiding important functionality.
- **Mobile-aware experience** — pay attention to touch targets, keyboard obstruction, safe areas, narrow layouts, and complete task flows.
- **Business-safe implementation** — preserve existing business rules, permissions, user choices, and recovery paths.

## Design principles

1. Visual richness and operational simplicity are designed separately and evaluated together.
2. Images should explain, guide, or reinforce the product—not fill every empty space.
3. Reuse suitable assets first. When image generation is unavailable, state the limitation instead of pretending an asset was generated.
4. Never replace real user content with generated examples.
5. Fewer clicks are not automatically better: discoverability, user control, correctness, and safety come first.
6. Do not impose a fixed aesthetic, framework, component library, or full-site rewrite.

## Workflow

Understand the requested scope → inspect the existing interface and task → extract approved visual language → define the image-led direction → simplify the user journey → implement within the authorized scope → verify both visual quality and task completion.

## Installation

Clone the repository:

```bash
git clone https://github.com/wszrw123/skills.git
```

Copy the skill folder into your user-level Agent Skills directory:

```bash
mkdir -p ~/.agents/skills
cp -R skills/image-led-ui-design ~/.agents/skills/
```

On Windows PowerShell:

```powershell
gh repo clone wszrw123/skills "$HOME\Downloads\wszrw123-skills"
New-Item -ItemType Directory -Force "$HOME\.agents\skills" | Out-Null
Copy-Item "$HOME\Downloads\wszrw123-skills\skills\image-led-ui-design" "$HOME\.agents\skills\image-led-ui-design" -Recurse
```

Restart or refresh the agent client if the skill does not appear immediately.

## Usage

In a compatible Agent Skills client, invoke:

```text
$image-led-ui-design
```

Example request:

```text
$image-led-ui-design

Review the current interface and the user's approved visual references.
Use image generation for a high-fidelity visual direction where available.
Preserve working business behavior, improve the visual language, reduce
unnecessary input and interaction steps, then verify the complete task flow.
```

## Requirements and limitations

- The skill provides instructions and workflow guidance; it does not itself install image-generation, browser, or coding tools.
- Image generation depends on the capabilities available in the host agent environment. If unavailable, the skill must state the limitation and use suitable existing assets without claiming generation took place.
- Browser and business-flow verification depend on the project's available runtime, credentials, and test environment.

## License

No license file is currently included in this repository. Public visibility does not by itself grant permission to reuse, redistribute, or commercially use the contents. Contact the repository owner for permission.

---

## 中文介绍

**图片驱动的 UI 设计与操作减负 Skill**，面向 Codex 和兼容 Agent Skills 的 AI 编程助手。

它不只是让页面“更好看”，而是帮助 AI：

- 从用户认可的页面中提取并延伸视觉语言，避免每次改造都推翻重做；
- 通过 Image 参考与生成建立更有辨识度的界面视觉；
- 按职责规划摄影图、插画、图标和背景素材，保持成套资产风格一致；
- 梳理真实用户任务，减少重复填写、不必要点击、等待和决策；
- 在减少操作的同时保留功能可发现性、用户控制权、权限和业务安全；
- 在授权范围内实施，并检查完整任务流程，而不只是看静态截图。

**适用场景：** 现有 Web/H5 页面视觉升级、移动端体验优化、功能入口和插画设计、表单减负、重复操作简化，以及局部产品体验改造。

**核心理念：视觉丰富与操作简单分别设计、一起验收。**
