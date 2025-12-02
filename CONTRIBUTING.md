# 🤝 Contributing to stan-game-templates

Thank you for your interest in contributing to **Stan AI**! This repository is the core engine for Stan's knowledge, and your contributions ensure that Stan generates high-quality, up-to-date, and production-ready Unity code.

Before submitting a Pull Request, please take a moment to review this document.

## 📝 Code of Conduct

All contributors are expected to adhere to the [Code of Conduct](./CODE_OF_CONDUCT.md). We strive to maintain a welcoming, respectful, and constructive environment.

---

## 🎯 Contribution Types

We welcome three main types of contributions:

### 1. New Modular Core Projects (MCPs)

This involves adding a completely new game genre or technical template to the `/templates/` folder (e.g., a "Roguelike" or "Multiplayer Lobby" template).

* **Structure:** The new folder name should be snake\_case (e.g., `visual_novel`, `turn_based_combat`).
* **Requirements:**
    * Must be created using the latest [Unity LTS version](https://unity.com/releases/lts) supported by Stan.
    * Must use the **Unity Input System** package.
    * Must include a minimal, working C# script that demonstrates the core mechanic.
    * Must include the **`AI_PROMPT_DOC.md`** file (see Section 3).
    * Must be licensed under the MIT License.

### 2. Code Refinement and Fixes

Improving the existing C# scripts, optimizing performance, or fixing bugs in current MCPs.

* **Goal:** Ensure the existing scripts (like `FpsController.cs`) follow current Unity best practices and are highly readable.
* **Scope:** Focus changes on the specific script being fixed/improved. Do not refactor large portions of the template unless strictly necessary.

### 3. AI Instruction Refinements

This is arguably the most valuable contribution, as it directly teaches Stan how to be a better developer.

* **Target:** The `AI_PROMPT_DOC.md` file within each template folder.
* **Refinements include:**
    * Adding or updating `// STAN_ENTRY_POINT:` directives to guide the AI to the correct function for common feature requests (e.g., where to add a dash mechanic).
    * Providing new `// STAN_CONSTANTS:` to give the AI crucial context (e.g., "The Player object is tagged 'Player'").

---

## ⚙️ Submission Process

1.  **Fork** the `stan-game-templates` repository to your own GitHub account.
2.  **Clone** your forked repository locally.
3.  **Create a new branch** for your contribution:
    ```bash
    git checkout -b feature/new-rpg-template
    # OR
    git checkout -b fix/fps-input-bug
    ```
4.  **Implement** your changes. If you are adding a new MCP, ensure you test it locally in the Unity Editor.
5.  **Commit** your changes with a clear and descriptive commit message. (Please squash small, iterative commits if they clutter the history).
6.  **Push** the branch to your fork.
7.  **Open a Pull Request (PR)** against the `main` branch of the original `stan-game-templates` repository.

### Pull Request Guidelines

* **Title:** Use a clear, conventional prefix (e.g., `[FEAT]`, `[FIX]`, `[DOCS]`).
    * *Example:* `[FEAT] Add initial 2D Top-Down RPG template`
* **Description:**
    * Explain the problem your PR solves or the new feature it adds.
    * Reference any existing issues it closes (e.g., `Closes #15`).
    * If adding a new MCP, include a brief GIF or screenshot of the template working in the Unity Editor.

---

## 🛑 Project Conventions

To keep the templates consistent and easy for the AI to parse:

* **C# Standards:** Adhere to common Unity C# conventions (PascalCase for classes/methods, camelCase for local variables).
* **Unity Input System:** All templates must use the new Input System package.
* **No Binary Bloat:** Do not commit large binary assets, textures, or complex models. Templates should only contain essential scripts and minimal scene setups. **Commit all `.unitypackage` and binary files > 5MB to Git LFS.**

---

Thank you for helping us build the best AI co-pilot for Unity development!
