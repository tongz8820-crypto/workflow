# Design Workflow

面向 Codex 的阶段化设计工作流 skill。它把方案设计、交付媒介选择、实施和审查拆成不同阶段，避免在产品目标尚未明确时过早进入 HTML 或视觉实现。

This repository contains a stage-aware design workflow skill for Codex. It separates design decisions, medium selection, implementation, and review so that medium-specific rules are loaded only when relevant.

## 主要能力

- 先识别当前处于设计、媒介选择、实施还是审查阶段。
- 在产品目标、用户、结构或交互仍未明确时，优先完成方案设计。
- 只在选择 HTML/Web 作为交付媒介后加载 HTML 实施规范。
- 将 PowerPoint、Figma、文档、PDF、原生应用和图片交给对应的专项工作流。
- 审查任务默认只输出有证据的发现，不静默修改用户文件。
- 从产品闭环、信息层级、交互状态、可访问性和实现质量多个维度进行检查。

## 安装

克隆仓库后，将 `design-workflow` 目录复制到 Codex skills 目录：

### Windows PowerShell

```powershell
git clone https://github.com/tongz8820-crypto/workflow.git
Copy-Item -Recurse -Force .\workflow\design-workflow "$env:USERPROFILE\.codex\skills\design-workflow"
```

### macOS / Linux

```bash
git clone https://github.com/tongz8820-crypto/workflow.git
cp -R workflow/design-workflow ~/.codex/skills/design-workflow
```

重新启动 Codex 或开启一个新任务，使 skill 被重新发现。

## 使用示例

- “先帮我梳理这个活动的产品方案，不要急着做页面。”
- “比较 H5、Figma 原型和 PPT，推荐合适的交付方式。”
- “方案已经确定，用 HTML 实现这个交互原型。”
- “审查这个 H5，区分产品闭环问题和视觉实现问题。”
- “优化这份设计，但保留已经确定的产品结构。”

## 仓库结构

```text
design-workflow/
  SKILL.md
  references/
    design-stage.md
    html-implementation.md
    implementation-routing.md
    quality-gates.md
evals/
  evals.json
LICENSE
SOURCE.md
```

运行时只需要安装 `design-workflow` 目录；`evals` 用于开发和回归评测。

## 来源与许可证

本 skill 是对 [Trystan-SA/claude-design-system-prompt](https://github.com/Trystan-SA/claude-design-system-prompt) 中部分设计流程的阶段化改造。详细来源、参考提交和改动范围见 [SOURCE.md](SOURCE.md)。

项目依据 [MIT License](LICENSE) 发布，并保留上游版权与许可声明。

