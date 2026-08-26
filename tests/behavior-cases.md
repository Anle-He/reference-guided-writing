# Behavior Acceptance Cases

These cases test decisions and outcomes rather than exact wording.

## A-01 Activation boundary

**Given:** The user provides a document only as a factual source and does not ask to follow its writing style.

**Expected:** The Skill does not activate merely because a document is present.

**Failure:** Treating every supplied source as a writing exemplar.

**Basis:** Scope; Non-Goals.

## B-01 Content isolation

**Given:** A medical report is designated only as a writing reference for a target document about urban planning.

**Expected:** The target may follow supported structural or stylistic conventions, but it does not import medical facts, claims, conclusions, or terminology.

**Failure:** Reusing the reference document's subject matter as target content.

**Basis:** I-01; F-01.

## B-02 Temporary conventions

**Given:** One reference in the current session uses a distinctive local convention, and the user has not requested reusable guidance.

**Expected:** The convention remains local to the current task or session.

**Failure:** Saving or presenting it as a general rule for future unrelated tasks.

**Basis:** I-02; F-02.

## B-03 No invented preferences

**Given:** The references do not establish a preference about paragraph length.

**Expected:** The Skill does not claim that paragraphs should be short or long as a reference-derived rule.

**Failure:** Adding an unsupported default because it seems like better writing practice.

**Basis:** I-03; F-03.

## B-04 Task requirements take priority

**Given:** The user requires a specified section, while the writing reference omits that kind of section.

**Expected:** The required section remains; applicable conventions may shape how it is written.

**Failure:** Removing or weakening the section to resemble the reference.

**Basis:** I-04; F-04.

## B-05 Unresolved reference conflict

**Given:** Two equally ranked references use materially conflicting organization, and the user gives no priority or resolving criterion.

**Expected:** The Skill does not silently merge or generalize the conflict. It asks for direction only if the choice materially affects the result.

**Failure:** Arbitrarily selecting one convention or presenting a blend as a shared rule.

**Basis:** I-05; F-05.
