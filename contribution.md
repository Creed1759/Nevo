# CONTRIBUTING.md

## Introduction

Thank you for your interest in contributing to **Nevo**!
We welcome contributions from developers of all backgrounds. This document outlines the process and rules to ensure a smooth and consistent contribution workflow.

---

## Getting Started

### 1. Fork the Repository

Fork the repository to your GitHub account:

```
https://github.com/Web3Novalabs/Nevo
```

### 2. Clone Your Fork

```bash
git clone https://github.com/YOUR-USERNAME/Nevo.git
cd Nevo
```

### 3. Create a Branch

```bash
git checkout -b feature/issue-<issue-number>
```

---

## Project Structure

The repository is organized into three main folders:

* **Frontend** → Next.js application
* **Backend** → NestJS API
* **Contract** → Smart contract code

Each GitHub issue will clearly belong to **one and only one** of these folders.

---

## Contribution Rules

### Issue-Based Work

* Every contribution **must be tied to a GitHub issue**
* Issues are created and scoped by maintainers
* Follow the issue description carefully

### Single-Folder Rule (IMPORTANT)

* Only modify **one** of the following per PR:

  * Frontend
  * Backend
  * Contract
* Do NOT mix changes across multiple folders in a single PR

### Minimal Changes

* Only modify files necessary to solve the issue
* Avoid touching unrelated code
* Keep PRs focused and clean

---

## Frontend Contributions (Next.js)

When working in the `Frontend` folder:

* Ensure the project builds successfully
* Ensure UI is responsive across screen sizes
* Follow consistent formatting and styling
* Limit changes to:

  * The new page folder being implemented, or
  * The relevant `page.tsx` (or main page file)

---

## Backend Contributions (NestJS)

When working in the `Backend` folder:

* Ensure the backend builds successfully
* Follow proper code formatting
* Only modify:

  * The specific module
  * Controller
  * Service related to the issue

---

## Contract Contributions

When working in the `Contract` folder:

* Ensure contracts compile/build successfully
* Ensure **all tests pass**
* Follow strict formatting rules
* Only modify:

  * The main contract file/module being updated
  * Relevant test files

> ⚠️ Contract contributions are stricter due to security and immutability concerns.

---

## Code Quality

* Follow the existing code style
* Keep code clean and readable
* Write meaningful commit messages
* Ensure no build errors before submitting PR

---

## Submitting a Pull Request

1. Push your branch:

```bash
git push origin feature/issue-<issue-number>
```

2. Open a Pull Request against the main repository

3. In your PR:

* Reference the issue (`Closes #<issue-number>`)
* Clearly describe what was changed
* Confirm:

  * Build passes
  * Tests pass (if applicable)
  * Scope is limited to one folder

---

## Review Process

* Maintainers will review your PR
* Feedback may require changes before merging
* Once approved, your PR will be merged

---

## Final Notes

* Respect the project structure and rules
* Keep contributions focused and minimal
* When in doubt, ask for clarification in the issue

---

Thank you for contributing to Nevo 🚀
