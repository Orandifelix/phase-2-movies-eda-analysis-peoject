# Contributing to Box Office Intelligence

Thank you for your interest in contributing! This document explains how to get involved, report issues, and submit changes.

---

## Table of Contents

1. [Who Can Contribute](#who-can-contribute)
2. [Getting Started](#getting-started)
3. [How to Contribute](#how-to-contribute)
4. [Commit Message Guidelines](#commit-message-guidelines)
5. [Pull Request Process](#pull-request-process)
6. [Reporting Issues](#reporting-issues)
7. [Code Style](#code-style)
8. [Current Contributors](#current-contributors)

---

## Who Can Contribute

Anyone is welcome to contribute — whether it's fixing a typo, improving a chart, adding a new analysis objective, or cleaning up documentation.

---

## Getting Started

### 1. Fork the repository

Click the **Fork** button at the top right of the repo page on GitHub.

### 2. Clone your fork

```bash
git clone https://github.com/Orandifelix/phase-2-movies-eda-analysis-peoject
cd phase-2-movies-eda-analysis-peoject
```

### 3. Create a virtual environment and install dependencies

```bash
python -m venv venv
source venv/bin/activate        # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```

### 4. Create a new branch

Always work on a dedicated branch — never commit directly to `main`.

```bash
git checkout -b feature/your-feature-name
```

---

## How to Contribute

### Areas open for contribution

| Area               | Examples                                                     |
| ------------------ | ------------------------------------------------------------ |
| **New analysis**   | Additional objectives, new datasets, extended EDA            |
| **Visualisations** | Improved charts, interactive plots, dashboard updates        |
| **Data cleaning**  | Better handling of missing values, more robust parsing       |
| **Documentation**  | Clearer explanations, better inline comments, README updates |
| **Bug fixes**      | Broken code, incorrect calculations, chart rendering issues  |

---

## Commit Message Guidelines

Use clear, descriptive commit messages in the imperative mood:

```
feat: add genre-level ROI breakdown chart
fix: correct budget tier bin labels
docs: update README with Objective 3 findings
refactor: simplify RT score band aggregation logic
data: add cleaned TMDB genre dataset
```

**Prefixes to use:**

- `feat:` — new feature or analysis
- `fix:` — bug fix
- `docs:` — documentation only
- `refactor:` — code restructuring without behaviour change
- `data:` — changes to datasets or data pipeline
- `style:` — formatting, whitespace, no logic change

---

## Pull Request Process

1. **Ensure your branch is up to date** with the latest `main`:

```bash
git fetch origin
git rebase origin/main
```

2. **Run the notebook end-to-end** to confirm no errors before submitting.

3. **Push your branch** to your fork:

```bash
git push origin feature/your-feature-name
```

4. **Open a Pull Request** against the `main` branch of this repository.

5. In your PR description, include:
   - What change you made and why
   - Any datasets or dependencies added
   - Screenshots of any new charts or outputs

6. At least **one existing contributor must review and approve** before merging.

7. Once approved, the PR will be squash-merged into `main`.

---

## Reporting Issues

Found a bug, a calculation error, or a broken chart? Please open a GitHub Issue:

1. Go to the **Issues** tab of this repository
2. Click **New Issue**
3. Use a clear title, e.g. `Bug: ROI calculation incorrect for zero-budget films`
4. Include:
   - Steps to reproduce
   - Expected vs. actual behaviour
   - Python version and relevant package versions

---

## Code Style

- Follow **PEP 8** for Python code
- Use **4-space indentation** (no tabs)
- Add **inline comments** for non-obvious logic
- Keep notebook cells focused — one task per cell
- Use the established **colour palette** for all new charts:

```python
NAVY   = '#0F172A'
BLUE   = '#3B82F6'
TEAL   = '#14B8A6'
CORAL  = '#F97316'
AMBER  = '#F59E0B'
PURPLE = '#8B5CF6'
GREEN  = '#22C55E'
MGRAY  = '#64748B'
BG     = '#F8FAFC'
```

---

## Current Contributors

| Contributor          | GitHub                                                               |
| -------------------- | -------------------------------------------------------------------- |
| **Chelimo Chebet**   | [@Chelimo-Chebet](https://github.com/Chelimo-Chebet)                 |
| **Orandi Felix**     | [@Orandifelix](https://github.com/Orandifelix)                       |
| **Richard Oketch**   | [@richardoketch32806-eng](https://github.com/richardoketch32806-eng) |
| **Shadrack Basweti** | [@symekah1999](https://github.com/symekah1999)                       |

---

_By contributing to this project, you agree that your contributions will be licensed under the [MIT License](LICENSE)._
