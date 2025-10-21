# github-final-project — Simple Interest Calculator (Bash)
> 🧩 This repository was created as part of the IBM “Introduction to Git and GitHub” course on Coursera.  
> It demonstrates practical Git operations: creating a repo, adding supporting documents, branching, merging, and reverting changes via CLI.
> **Project context (Course Final Project)**
> - **Part 1 – GitHub UI:** Created public repo **github-final-project**, added `README.md`, `LICENSE` (Apache 2.0), `CODE_OF_CONDUCT.md` (Contributor Covenant), and `CONTRIBUTING.md` (based on provided resources). Added `simple-interest.sh`.
> - **Part 2 – Git CLI:** Forked the course repo, cloned locally, created `bug-fix-typo` to update README footer **2022 → 2023**, committed and pushed; merged into `main` locally; created `bug-fix-revert`, reverted the change back to **2022**, pushed branch and opened a PR from my fork to the upstream `main` (auto-closed per lab).



Empowering communities through transparent, accessible finance.

> I recently joined a micro-finance startup on a mission to **empower and provide opportunities to low-income individuals**.  
> This repository kicks off our migration from SVN to Git by hosting a small but essential example: a **Simple Interest Calculator**.  
> We’re using this project to model **open-source best practices**—clear docs, a welcoming community process, and a permissive license.

---

## Table of Contents
- [About](#about)
- [Why this matters](#why-this-matters)
- [What’s included](#whats-included)
- [Getting started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Run the calculator](#run-the-calculator)
  - [Examples](#examples)
- [Project structure](#project-structure)
- [Contributing](#contributing)
- [Code of Conduct](#code-of-conduct)
- [License](#license)
- [Grading checklist (Course Part 1)](#grading-checklist-course-part-1)

---

## About

This repository contains a **Bash script** that computes **simple interest**:

<p align="center"><b>Simple Interest = (P × R × T) / 100</b></p>


where:
- **P** = principal amount  
- **R** = annual rate of interest (in percent)  
- **T** = time period in years

The goal is twofold:
1. Provide a small, auditable utility our teams and partners can reuse.
2. Demonstrate healthy open-source practices (README, License, Code of Conduct, Contributing guidelines).

> **Note:** As stated in the script header, this is **sample code only** and **not for production** use.

---

## Why this matters

In micro-finance, clarity builds trust. By open-sourcing even a basic calculator, we:
- Show **transparent** logic behind cost calculations.
- Create a foundation for **community collaboration** and learning as we move from SVN to Git.
- Practice processes (issues, PRs, reviews) we’ll use on our core products.

---

## What’s included

- `simple-interest.sh` — Bash script to calculate simple interest (interactive; reads values from standard input).
- `README.md` — You’re reading it 😊
- [`LICENSE`](LICENSE) — **Apache License 2.0** to encourage broad use.
- [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md) — Sets expectations for respectful collaboration.
- [`CONTRIBUTING.md`](CONTRIBUTING.md) — How to propose changes, open issues, and submit PRs.

---

## Getting started

### Prerequisites
- A POSIX-compatible shell (Linux/macOS/WSL).
- `bash` installed (usually available by default).
- Make the script executable if needed.

### Run the calculator

```bash
# Clone your repo (example)
git clone https://github.com/<your-username>/github-final-project.git
cd github-final-project

# Ensure the script is executable
chmod +x simple-interest.sh

# Run (the script will prompt for values)
./simple-interest.sh
````

### Examples

**Interactive session (matches the script behavior):**

```text
$ ./simple-interest.sh
Enter the principal:
1000
Enter rate of interest per year:
5
Enter time period in years:
2
The simple interest is:
100
```

> **Notes**
>
> * Inputs must be numeric.
> * Rate is in **percent** (e.g., `7.5` for 7.5%).
> * Time is in **years**.

---

## Project structure

```
github-final-project/
├─ simple-interest.sh          # The calculator script (interactive)
├─ README.md                   # Project overview & usage
├─ LICENSE                     # Apache 2.0 license
├─ CODE_OF_CONDUCT.md          # Community standards (Contributor Covenant)
└─ CONTRIBUTING.md             # How to propose changes
```

---

## Contributing

We welcome issues, suggestions, and pull requests—especially from learners adopting Git for the first time.

* Read our guidelines: [`CONTRIBUTING.md`](CONTRIBUTING.md)
* Open an issue to discuss ideas or report a bug.
* Keep changes focused and documented.

Together we can make financial tools **more understandable** and **more available**.

---

## Code of Conduct

Please review and uphold our community standards in [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md).
We’re committed to fostering an open and inclusive environment for contributors of all backgrounds.

---

## License

This project is licensed under the **Apache License 2.0**.
See [`LICENSE`](LICENSE) for details.

---
