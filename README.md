# 🎮 stan-game-templates: Modular Core Projects (MCPs)

The official, community-driven library of **Modular Core Projects (MCPs)** and Starter Kits used by the **Stan AI** platform to accelerate Unity game development.

This repository is the **source of truth** for all foundational project structures, tested code templates, and configuration files that Stan uses for Retrieval-Augmented Generation (RAG).

---

## 🎯 Why This Repo Exists

Stan does not generate code from scratch. When a user requests a new feature or game, Stan pulls a corresponding, tested **Modular Core Project (MCP)** from this library and intelligently modifies it. This ensures:

* **Quality & Stability:** All generated code integrates with a clean, pre-configured Unity project setup.
* **Speed:** Drastically reduces generation time by referencing existing, high-quality C# scripts instead of generating boilerplate code.
* **Community Scaling:** Allows Unity experts to submit new game templates, expanding Stan's capabilities for every user.

---

## 📂 Repository Structure

The `templates/` directory is the core of this repository.

/
├── .github/                  # CI/CD and Contribution files <br>
├── docs/                     # Detailed documentation for contributors <br>
├── unity_base_project/       # ⬅️ Base Unity project settings (Input System, default folders) <br>
│ <br>
├── templates/ # ⬅️ Core Game Templates (Modular Core Projects) <br>
│   ├── fps_3d_shooter/ # Template for a 3D First-Person Shooter <br>
│   │   ├── Gameplay/         # Core scripts (e.g., FpsController.cs, GunSystem.cs) <br>
│   │   ├── Scenes/           # Minimal testing scene <br>
│   │   └── AI_PROMPT_DOC.md  # ⬅️ Instructions for the Stan AI <br>
│   │ <br>
│   ├── rpg_2d_topdown/ # Template for a 2D Top-Down RPG <br>
│   │   └── ...               # (Movement, InventorySystem, CombatManager) <br>
│   │ <br>
│   └── platformer_2d/ # Template for a simple 2D Platformer <br>
│       └── ... <br>
│ <br>
└── README.md

### 🧠 The `AI_PROMPT_DOC.md` (Crucial Component)

Each template folder contains an `AI_PROMPT_DOC.md` file. This file contains **meta-instructions** that Stan's LLM uses to correctly interact with the surrounding code:

| Section | Purpose | Example |
| :--- | :--- | :--- |
| `// STAN_ENTRY_POINT:` | Directs the AI to the specific function or class to modify for common user requests. | `FpsController.cs -> OnMovementInput()` |
| `// STAN_CONSTANTS:` | Provides key project constants (e.g., input bindings, variables) to maintain consistency. | `Gravity is applied in FpsController.cs, set to -9.81` |
| `// STAN_GENERATION_GUIDE:` | Explicitly tells Stan *how* to behave (e.g., to modify an existing script vs. create a new one). | "Do NOT create a new script for jump functionality; modify `FpsController.cs`." |

---

## 🤝 Contribution Guidelines

We actively encourage contributions from the Unity development community to make Stan smarter.

Before submitting a Pull Request, please read the full **[CONTRIBUTING.md](./docs/CONTRIBUTING.md)** document.

### Contribution Targets:

1.  **New MCPs:** Adding a new, well-structured game genre (e.g., Roguelike, Visual Novel).
2.  **Code Refinement:** Optimizing existing C# scripts for better performance, clean architecture, or adherence to the latest Unity best practices.
3.  **AI Instruction Refinement:** Improving the `AI_PROMPT_DOC.md` files to guide the AI toward more accurate and high-quality code generation.

### Installation (for Local Testing)

To test an MCP locally before contributing:

1.  Clone this repository: `git clone https://github.com/Stan-AI/stan-game-templates.git`
2.  Open the cloned project in the Unity Editor.
3.  Open the desired base scene from a template (e.g., `templates/fps_3d_shooter/Scenes/FPS_BaseScene.unity`).

---

## 📄 License

This project is licensed under the **MIT License**. See the [LICENSE](./LICENSE) file for details.
