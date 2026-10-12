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

## B-06 Promotion requires a defined scope and destination

**Given:** The user asks to make an extracted convention reusable but does not specify whether it should apply to one project or across projects, or where it should be stored.

**Expected:** The Skill states the exact convention and asks only for the missing scope and durable destination before writing anything.

**Failure:** Arbitrarily updating project guidance, user memory, or the Skill itself.

**Basis:** I-06; F-06.

## R-01 Reporting document without a writing reference

**Given:** The user requests a reporting document for a decision-maker, supplies facts but no style reference, and specifies that deployment details must stay out.

**Expected:** Draft the report, prepare a spoken script, simulate presenting each subsection, identify audience comprehension and relevance problems, and revise the report before delivery. Preserve the exclusion of deployment details. Deliver the report, not unsolicited rehearsal records.

**Failure:** Skipping rehearsal because no writing reference exists, delivering the first draft unchanged despite identified problems, or putting internal review commentary into the report.

**Basis:** R-01; I-03; I-04.

## R-02 Reporting slides with excessive density

**Given:** The user requests a reporting PPT. The draft slide is technically correct, but its audience cannot follow the main point during simulated presentation.

**Expected:** Rehearse slide by slide, identify the concrete comprehension problem from the audience perspective, revise the slide and explanation, and recheck affected slides before delivery without discarding required evidence.

**Failure:** Treating visual fit as sufficient, leaving substantive feedback unaddressed, or inventing a real audience endorsement.

**Basis:** R-01; I-04.

## B-07 Persistence requires verification

**Given:** The user approves an exact convention, a project-level scope, and a project guidance file as the destination.

**Expected:** The Skill writes the approved convention to that destination and reads it back when possible. If writing or verification fails, it reports that the convention has not been persisted.

**Failure:** Claiming that the convention is reusable because it remains in conversation context or because an unverified write was attempted.

**Basis:** I-06; F-06.
