# Contributing to `github-final-project` (Simple Interest Calculator — Bash)

Thank you for helping us build transparent, trustworthy financial tooling.  
This repo is part of a micro-finance initiative aimed at **empowering low-income individuals** with clear, accessible calculations.

All **contributions, bug reports, bug fixes, documentation improvements, enhancements, and ideas are welcome.**

---

## Table of Contents
- [Code of Conduct](#code-of-conduct)
- [Ways to Contribute](#ways-to-contribute)
- [Before You Start](#before-you-start)
- [Local Development Setup](#local-development-setup)
- [Project Structure](#project-structure)
- [Quality (Optional)](#quality-optional)
- [Branching & Commit Messages](#branching--commit-messages)
- [Pull Request Process](#pull-request-process)
- [Reporting Bugs](#reporting-bugs)
- [Suggesting Enhancements](#suggesting-enhancements)
- [License](#license)

---

## Code of Conduct
Participation in this project is governed by our **[Code of Conduct](CODE_OF_CONDUCT.md)**.  
By contributing, you agree to uphold a respectful, inclusive environment.

---

## Ways to Contribute
- Improve the Bash script (correctness, validation, clearer prompts).
- Documentation: clarify README, fix typos, add usage notes.
- File housekeeping (comments, header metadata).
- Issue triage: reproduce bugs, provide minimal repro steps.

If you’re new to Git/GitHub, improving docs is a perfect first PR!

---

## Before You Start
1. **Search issues/PRs** to avoid duplicates.
2. **Open an issue** to discuss non-trivial changes.
3. Keep changes **small and focused**.

---

## Local Development Setup

**Requirements**
- POSIX-compatible shell (Linux/macOS/WSL)
- `bash`

**Run**
```bash
git clone https://github.com/<your-username>/github-final-project.git
cd github-final-project
chmod +x simple-interest.sh
./simple-interest.sh
````

The script is **interactive** and will prompt for principal, rate (%), and time (years).

---

## Project Structure

```
.
├─ simple-interest.sh          # interactive calculator
├─ README.md                   # project overview & usage
├─ LICENSE                     # Apache 2.0 license
├─ CODE_OF_CONDUCT.md          # Contributor Covenant
└─ CONTRIBUTING.md             # this file
```

---

## Quality (Optional)

This is a simple Bash project—quality checks are optional but appreciated:

* Lint with [`shellcheck`](https://www.shellcheck.net/) if available:

  ```bash
  shellcheck simple-interest.sh
  ```

---

## Branching & Commit Messages

* Create a short-lived branch from `main`:

  ```bash
  git checkout -b docs/readme-example
  # or: fix/validate-inputs, chore/comments
  ```
* Write clear, concise commit messages (imperative mood).

  * `fix: validate numeric input for rate`
  * `docs: clarify interactive example in README`

---

## Pull Request Process

1. **Fork** the repo and **clone** your fork.
2. Create a branch and implement your changes.
3. Run the script locally to verify behavior.
4. Update **README** if usage or messaging changes.
5. Push and open a **Pull Request** with a short description of the *problem* and *solution*.
6. Be ready to iterate on maintainer feedback.

**PR checklist**

* [ ] Script runs interactively without errors
* [ ] Docs updated if behavior changed
* [ ] Changes are focused and clearly described

---

## Reporting Bugs

Please include:

* **Exact steps/inputs** (copy/paste the interactive session if possible)
* **Expected vs actual** result
* OS/shell details

Open an issue and label it `bug`.

---

## Suggesting Enhancements

Open an issue and describe:

* **What** you propose (e.g., input validation, decimal handling, output formatting)
* **Why** it helps users (clarity, accessibility)
* **How** you’d approach it (brief plan)

---

## License

By contributing, you agree that your contributions are licensed under the **Apache License 2.0** (see [`LICENSE`](LICENSE)).

---

**Thank you** for contributing—every improvement helps make financial tools more accessible to the communities we serve. 💙


