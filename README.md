# Reference-Guided Writing

[中文](#中文) · [English](#english)

## 中文

`reference-guided-writing` 是一个 Codex Skill，用于从一个或多个参考文档中提取可迁移的写作规范，并将其应用于当前文档写作或修订任务。

它将参考文档的写作方式与领域内容分开处理，遵循当前任务要求，并将单次任务中提取的规范默认保留在当前任务或会话内。

### 核心行为

- 识别输入文档是写作参考、内容来源，还是同时承担两种角色。
- 只提取有明确依据的可迁移写作规范。
- 保持参考文档的领域事实、观点、结论和术语与目标内容隔离。
- 保留当前任务的内容、范围和交付要求。
- 在多份参考文档发生冲突时，遵循用户指定的优先级；缺乏依据时保留冲突。
- 仅在用户明确要求或确认后，将临时规范提升为长期复用规范。

### 仓库内容

- [`SKILL.md`](SKILL.md)：Skill 的运行与维护规则。
- [`SPEC.md`](SPEC.md)：不可违反的行为规范和变更审查基准。
- [`tests/behavior-cases.md`](tests/behavior-cases.md)：基于 SPEC 的行为验收案例。

### 安装

可以让 Codex 从 [本 GitHub 仓库](https://github.com/Anle-He/reference-guided-writing) 安装该 Skill。

也可以将本仓库复制到：

```text
~/.codex/skills/reference-guided-writing
```

如果设置了 `CODEX_HOME`，则安装到：

```text
<CODEX_HOME>/skills/reference-guided-writing
```

安装完成后，该 Skill 会在后续对话轮次中可用。

### 使用

向 Codex 提供一个或多个写作参考文档，并说明目标文档的内容要求。例如：

> 请参考这些文档的写作规范，起草一份关于新主题的报告。参考文档仅用于指导写作方式。

### 维护

修改 `SKILL.md` 前必须完整阅读 `SPEC.md`。每项重要行为变更都应能够追溯到某个 Invariant、Failure Mode 或明确记录的新需求，并通过相应的行为验收案例检查。

## English

`reference-guided-writing` is a Codex Skill that extracts transferable writing conventions from one or more reference documents and applies them to the current drafting or revision task.

It keeps the references' writing conventions separate from their domain content, preserves the current task requirements, and treats conventions extracted from a single task as local to that task or session by default.

### Core behavior

- Identify whether each input is a writing reference, a content source, or both.
- Extract only transferable writing conventions with a clear basis.
- Keep domain facts, claims, conclusions, and terminology from writing-only references separate from target content.
- Preserve the current task's content, scope, and delivery requirements.
- Follow user-defined priority when references conflict; preserve unresolved conflicts when no basis determines a choice.
- Promote temporary conventions to reusable guidance only when the user explicitly requests or confirms it.

### Repository contents

- [`SKILL.md`](SKILL.md): Runtime and maintenance instructions for the Skill.
- [`SPEC.md`](SPEC.md): Behavioral invariants and the change-review baseline.
- [`tests/behavior-cases.md`](tests/behavior-cases.md): Behavior acceptance cases derived from the SPEC.

### Installation

Ask Codex to install the Skill from [this GitHub repository](https://github.com/Anle-He/reference-guided-writing).

Alternatively, copy this repository to:

```text
~/.codex/skills/reference-guided-writing
```

If `CODEX_HOME` is set, install it under:

```text
<CODEX_HOME>/skills/reference-guided-writing
```

The Skill becomes available in subsequent conversation turns after installation.

### Usage

Give Codex one or more writing reference documents and specify the target document's content requirements. For example:

> Follow the writing conventions in these references to draft a report on a new topic. Use the references only to guide how the report is written.

### Maintenance

Read `SPEC.md` in full before changing `SKILL.md`. Every material behavior change should trace to an Invariant, Failure Mode, or explicitly recorded new requirement and should be checked against the corresponding behavior acceptance cases.
