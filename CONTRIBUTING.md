# Contributing to Our NLP Projects

Welcome to the team! We're excited to have you contribute. This document provides a set of guidelines to ensure our collaboration is smooth, consistent, and effective. Following these rules helps us maintain high-quality code and a clear project history.

## Code of Conduct

All members are expected to adhere to our [Code of Conduct](CODE_OF_CONDUCT.md). Please take a moment to read it. We are committed to fostering an open and welcoming environment.

## The Core Workflow: Branch, Commit, Pull Request

All work must be done on a separate branch and submitted via a Pull Request (PR). **Direct pushes to the `main` branch are disabled.**

### 1. Create a Branch

Before writing any code, create a new branch from the `main` branch.

*   **Make sure your `main` branch is up-to-date:**
    ```
    git checkout main
    git pull origin main
    ```
*   **Create and switch to your new branch:**
    ```
    git checkout -b <branch-name>
    ```

**Branch Naming Convention:**
Please use the following prefixes for your branch names to keep them organized:
*   `feature/`: For new features (e.g., `feature/add-rag-pipeline`)
*   `bugfix/`: For fixing bugs (e.g., `bugfix/fix-tokenization-error`)
*   `docs/`: For documentation changes (e.g., `docs/update-readme`)
*   `experiment/`: For experimental code that may not be merged

### 2. Make and Commit Your Changes

Write your code on your new branch. As you work, make small, logical commits.

**Commit Message Format:**
We use the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) standard. This helps us create a clear history. Each message should be in the format `type: description`.

*   **`feat`**: A new feature for the user.
*   **`fix`**: A bug fix for the user.
*   **`docs`**: Documentation only changes.
*   **`style`**: Code style changes (formatting, etc.) that don't change logic.
*   **`refactor`**: Rewriting code without changing its external behavior.
*   **`test`**: Adding or correcting tests.
*   **`chore`**: Build process or tooling changes.

**Example Commit:**
```
git add .
git commit -m "feat: add initial tokenizer for Marathi language"
```

### 3. Push and Create a Pull Request

Once your work is ready for review, push your branch to GitHub and open a Pull Request.

*   **Push your branch:**
    ```
    git push origin <branch-name>
    ```
*   **Open a Pull Request:** Go to the repository on GitHub. You will see a prompt to create a Pull Request from your branch.
    *   Use a clear title and provide a brief description of the changes.
    *   If your PR addresses an existing issue, link it by writing `Closes #issue-number` in the description.
    *   Assign at least one other team member to review your code.

### 4. Code Review

Your PR will be reviewed by team members. Be prepared to discuss your work and make additional changes based on feedback. Once approved, the PR will be merged into the `main` branch.

## Style Guides

*   **Python**: All Python code must follow the **PEP 8** style guide. Using an auto-formatter like `black` is highly encouraged.
*   **Jupyter Notebooks**: **Crucial Rule**: Before committing any notebook (`.ipynb` file), you must **clear all cell outputs**. This keeps our repository clean and avoids merge conflicts.

---

Thank you for your contribution! Let's build amazing things together.
