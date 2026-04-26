# AGENTS.md

## Purpose

This document defines strict operational rules for AI agents contributing to the Nevo repository.
Agents must follow these rules to ensure safe, minimal, and correct code changes.

---

## Core Principles

### 1. Issue-Driven Work

* Every task is tied to a GitHub issue
* The issue defines:

  * Scope
  * Target folder
  * Expected outcome
* Do not infer or expand beyond the issue

---

## Folder Identification (MANDATORY)

Before making any changes, the agent must:

1. Identify which folder the issue belongs to:

   * `Frontend`
   * `Backend`
   * `Contract`

2. Restrict all actions to that folder only

> ❗ NEVER modify multiple folders in a single task

---

## Allowed Modifications

### Frontend (Next.js)

* Modify only:

  * The relevant page folder, OR
  * The corresponding `page.tsx`
* Ensure:

  * Build succeeds
  * UI remains responsive
  * Code formatting is consistent

---

### Backend (NestJS)

* Modify only:

  * Specific module, controller, or service tied to the issue
* Ensure:

  * Build succeeds
  * Formatting is correct

---

### Contract

* Modify only:

  * Main contract logic file/module
  * Relevant test files
* Ensure:

  * Contracts compile successfully
  * All tests pass
  * Formatting is correct

> ⚠️ Contract changes require strict minimalism and correctness

---

## Strict Constraints

### Minimal Scope Enforcement

* Do NOT:

  * Refactor unrelated code
  * Rename unrelated files
  * Introduce unrelated improvements
* Only implement what is explicitly required

### No Cross-Layer Changes

* NEVER combine:

  * Frontend + Backend
  * Backend + Contract
  * Frontend + Contract

---

## Build & Validation Requirements

Before completing a task, the agent must ensure:

* Relevant project builds successfully
* Tests pass (for contract work)
* No syntax or formatting errors exist

---

## Code Style

* Follow existing patterns in the repository
* Match formatting, naming, and structure
* Do not introduce new patterns unless required

---

## Safety Rules

* Do not modify sensitive logic unless explicitly required
* Avoid introducing breaking changes
* Preserve backward compatibility unless instructed otherwise

---

## Output Expectations

When completing a task, the agent should:

* Produce minimal diffs
* Clearly reflect issue requirements
* Avoid unnecessary verbosity in code changes

---

## Summary

AI agents must:

1. Identify the correct folder from the issue
2. Modify only necessary files within that folder
3. Ensure build/tests pass
4. Follow formatting and existing style
5. Avoid unrelated or cross-folder changes

Failure to follow these rules will result in rejection of the contribution.

---
