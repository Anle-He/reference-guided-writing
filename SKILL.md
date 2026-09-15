---
name: reference-guided-writing
description: Extract and apply transferable writing conventions from documents designated as style references. Use when the user asks to draft or revise a document by following one or more reference documents; do not use when those documents are only factual sources.
---

# Reference-Guided Writing

Use reference documents to guide how the target document is written without treating their subject matter as target content.

## Establish the inputs

- Identify the current task's content, scope, and delivery requirements before applying writing conventions.
- Determine whether each input is a writing reference, a content source, or both. Keep those roles distinct throughout the task.

## Extract conventions

- Extract only conventions supported by the designated writing references, the user's explicit instructions, or already-applicable general rules. Do not invent a new default preference. [I-03]
- Separate transferable writing conventions from domain facts, claims, conclusions, and terminology. [I-01]
- Treat conventions inferred from a single task, session, or limited sample as local to that context. [I-02]

## Resolve priorities and conflicts

- Preserve the current task's content, scope, and delivery requirements; writing conventions do not override them. [I-04]
- Follow any priority among references stated by the user.
- When references conflict and no priority or other basis resolves the conflict, do not arbitrarily merge, generalize, or select among the conflicting conventions. Ask the user only when the unresolved choice materially affects the result. [I-05]

## Apply conventions

- Apply the supported conventions within the current task.
- Do not import subject matter from a document designated only as a writing reference. A document may supply content only when the user also designates it as a content source. [I-01]
- Do not expand, remove, or alter required content merely to resemble a reference. [I-04]

## Co-design writing mode

Use this mode when the user explicitly asks to develop a scheme, method, or design while drafting the corresponding section of an existing report or structured document.

- Preserve the existing document structure as the writing scaffold, but design the scheme and the report text together instead of treating the scheme as a completed black box.
- For any design step that will be reported externally, examine the theory, source evidence, and overall logic before drafting the corresponding prose.
- Do not merely translate code, workflow steps, or implementation comments into report text. Distinguish theory-supported claims, project-specific inferences, and implementation details.
- When theory or source support is missing, mark the point as tentative, internal, or out of scope instead of forcing it into the report narrative. [I-03] [I-04]

## Persistence

- Keep extracted conventions in the active task or session by default and make no durable write. Do not present conversation context alone as reusable guidance. [I-02]
- Before any promotion, ensure the user has explicitly approved the exact convention, intended reuse scope, and durable destination. Ask only for choices that remain materially unspecified. [I-06]
- Match the destination to the approved scope: use project guidance or a project-scoped Skill for project reuse; use user-level guidance, memory, or a personal Skill for cross-project reuse; modify this Skill only when the approved requirement changes its behavior and passes the Maintenance review below. [I-03] [I-06]
- After writing, read back the destination when possible. Claim persistence only after successful verification; otherwise report that the convention has not been persisted. [I-06]

## Maintenance

Before changing this Skill, read `SPEC.md` in full. Check every material behavior against its Invariants, Failure Modes, and Change Review Criteria. Make the smallest sufficient change, and do not retain a rule that lacks the traceability required by the SPEC.
