# github-final-project — Simple Interest Calculator (Bash)


Empowering communities through transparent, accessible finance.

> I recently joined a micro-finance startup on a mission to **empower and provide opportunities to low-income individuals**.  
> This repository kicks off our migration from SVN to Git by hosting a small but essential example: a **Simple Interest Calculator**.  
> We’re using this project to model **open-source best practices**—clear docs, a welcoming community process, and a permissive license.
````markdown
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

\[
\text{Simple Interest} = \frac{P \times R \times T}{100}
\]

where:
- **P** = Principal amount  
- **R** = Annual interest rate (in percent)  
- **T** = Time period (in years)

The goal is twofold:
1. Provide a small, auditable utility our teams and partners can reuse.
2. Demonstrate healthy open-source practices (README, License, Code of Conduct, Contributing guidelines).

---

## Why this matters

In micro-finance, clarity builds trust. By open-sourcing even a basic calculator, we:
- Show **transparent** logic behind cost calculations.
- Create a foundation for **community collaboration** and learning as we move from SVN to Git.
- Practice processes (issues, PRs, reviews) we’ll use on our core products.

---

## What’s included

- `simple-interest.sh` — Bash script to calculate simple interest.
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

# Usage:
# ./simple-interest.sh <principal> <rate_percent> <time_years>

./simple-interest.sh 1000 5 2
````

### Examples

```bash
# Example 1: P=1000, R=5%, T=2 years
./simple-interest.sh 1000 5 2
# Output:
# Principal: 1000
# Rate (%): 5
# Time (years): 2
# Simple Interest: 100.00
# Total Amount: 1100.00

# Example 2: P=2500, R=7.5%, T=1.5 years
./simple-interest.sh 2500 7.5 1.5
# Output:
# Principal: 2500
# Rate (%): 7.5
# Time (years): 1.5
# Simple Interest: 281.25
# Total Amount: 2781.25
```

> **Notes**
>
> * Inputs must be numeric.
> * Rate is in **percent** (e.g., `7.5` for 7.5%).
> * Time is in **years** (decimals allowed).

---

## Project structure

```
github-final-project/
├─ simple-interest.sh          # The calculator script
├─ README.md                   # Project overview & usage
├─ LICENSE                     # Apache 2.0 license
├─ CODE_OF_CONDUCT.md          # Community standards
└─ CONTRIBUTING.md             # How to propose changes
```

---

## Contributing

We welcome issues, suggestions, and pull requests—especially from learners adopting Git for the first time.

* Read our guidelines: [`CONTRIBUTING.md`](CONTRIBUTING.md)
* Open an issue to discuss ideas or report a bug.
* Follow the PR checklist and keep changes focused.

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


```
```
