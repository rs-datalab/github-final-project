# Contributing to `github-final-project` (Simple Interest Calculator — Python)

First off, **thank you** for helping us build transparent, trustworthy financial tooling.  
This repo is part of a micro-finance initiative aimed at **empowering low-income individuals** with clear, accessible calculations.

We welcome contributions from beginners and experts alike—docs, tests, bug fixes, and improvements to the Python code are all valuable.

---

## Table of Contents
- [Code of Conduct](#code-of-conduct)
- [Ways to Contribute](#ways-to-contribute)
- [Before You Start](#before-you-start)
- [Local Development Setup](#local-development-setup)
- [Project Structure](#project-structure)
- [Quality: Lint, Format, Type, Test](#quality-lint-format-type-test)
- [Branching & Commit Messages](#branching--commit-messages)
- [Pull Request Process](#pull-request-process)
- [Reporting Bugs](#reporting-bugs)
- [Suggesting Enhancements](#suggesting-enhancements)
- [Developer Certificate of Origin (DCO)](#developer-certificate-of-origin-dco)
- [License](#license)

---

## Code of Conduct
Participation in this project is governed by our **[Code of Conduct](CODE_OF_CONDUCT.md)**.  
By contributing, you agree to uphold a respectful, inclusive environment.

---

## Ways to Contribute
- **Improve the code**: correctness, validation, error messages, CLI UX.
- **Add tests**: edge cases (zero/negative values), rounding, large inputs.
- **Documentation**: clarify the README, add examples, fix typos.
- **Tooling/CI**: ruff/black/isort/mypy config, GitHub Actions.
- **Issue triage**: reproduce bugs, write minimal repro steps.

If you’re new to Git/GitHub, improving docs or tests is a perfect first PR!

---

## Before You Start
1. **Search issues/PRs** to avoid duplicates.
2. **Open an issue** to discuss non-trivial changes or design decisions.
3. Aim for **clarity, simplicity, and transparency**—that’s our mission.

---

## Local Development Setup

### Prerequisites
- Python **3.10+**
- Git
- (Optional) `make`

### Create a virtual environment
```bash
git clone https://github.com/<your-username>/github-final-project.git
cd github-final-project

python -m venv .venv
# Windows: .venv\Scripts\activate
# macOS/Linux:
source .venv/bin/activate

python -m pip install --upgrade pip
pip install -r requirements.txt           # runtime deps (if any)
pip install -r requirements-dev.txt       # ruff, black, isort, mypy, pytest
````

### Quick run (CLI)

```bash
# Example:
python simple_interest.py --principal 1000 --rate 5 --years 2
# Expected:
# Simple Interest: 100.00
# Total Amount: 1100.00
```

---

## Project Structure

```
.
├─ simple_interest.py            # CLI entry / main function
├─ src/interest/                 # optional: library code (if you split it out)
│  ├─ __init__.py
│  └─ calculator.py              # pure functions for compute_interest(...)
├─ tests/
│  ├─ test_calculator.py
│  └─ test_cli.py
├─ requirements.txt
├─ requirements-dev.txt
├─ README.md
├─ CONTRIBUTING.md
├─ CODE_OF_CONDUCT.md
└─ LICENSE
```

> **Tip:** Keep business logic in pure functions (easy to test). Let the CLI handle I/O/arg parsing only.

---

## Quality: Lint, Format, Type, Test

We keep quality lightweight but consistent:

* **Format**: `black .`
* **Imports**: `isort .`
* **Lint**: `ruff .`
* **Typing**: `mypy .` (at least on new/changed code)
* **Tests**: `pytest -q`

Suggested workflow:

```bash
ruff . && black . && isort . && mypy . && pytest -q
```

### Testing Guidance

* Use **pytest** with clear, small tests.
* Cover:

  * correct formula: `SI = P * R * T / 100`
  * rounding/formatting to two decimals
  * invalid input (non-numeric, negative)
  * CLI argument parsing and exit codes

---

## Branching & Commit Messages

* Create a focused branch off `main`:

  ```bash
  git checkout -b feat/validate-inputs
  # or: fix/rounding-bug, docs/readme-examples, chore/ci
  ```
* Write clear commit messages (imperative mood). **Conventional Commits** encouraged:

  * `feat: add input validation for negative values`
  * `fix: correct rounding to two decimals`
  * `docs: expand README usage examples`
  * `test: add CLI error path tests`

---

## Pull Request Process

1. **Fork** the repo and **clone** your fork.
2. Create a feature branch and implement changes.
3. Run **ruff/black/isort/mypy/pytest** locally and ensure green.
4. Update **README** if behavior or usage changes.
5. Commit with clear messages and **sign-off** (see DCO).
6. Push and open a **Pull Request**:

   * Explain the problem and solution.
   * Add before/after output if relevant.
   * Note any trade-offs or follow-ups.

**PR checklist**

* [ ] Code runs locally (`python simple_interest.py …`)
* [ ] Tests added/updated and passing (`pytest -q`)
* [ ] Lint/format/type checks pass (ruff/black/isort/mypy)
* [ ] Docs updated (README / comments)
* [ ] **DCO sign-off** on each commit

---

## Reporting Bugs

Please include:

* **Exact command** you ran and full output/traceback
* **Expected vs actual** result
* Python version and OS
* Minimal repro (e.g., input arguments)

Open an issue and apply the `bug` label.

---

## Suggesting Enhancements

Open an issue and describe:

* **What** you propose (e.g., decimal support, currency formatting, JSON output)
* **Why** it helps users (accuracy, accessibility, transparency)
* **How** you’d approach it (brief plan)

We prioritize improvements that enhance **correctness**, **usability**, and **readability**.

---

## Developer Certificate of Origin (DCO)

We use the **DCO** to confirm you have the right to submit your contribution.

Sign your commits with:

```bash
git commit -s -m "feat: add --output json option"
```

If you forgot:

```bash
git commit --amend -s
git push --force-with-lease
```

---

## License

By contributing, you agree that your contributions are licensed under the **Apache License 2.0** (see [`LICENSE`](LICENSE)).

---

**Thank you** for contributing—every improvement helps make financial tools more accessible to the communities we serve. 💙

```ight away?
```
