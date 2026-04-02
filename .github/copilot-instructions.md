# GitHub Copilot Instructions for holbertonschool-web-development

## 📌 Project overview
- Static HTML/CSS learning project with two main parts:
  - `html_advanced/`: HTML structure tasks and overall page layout
  - `css_advanced/` (not shown in this snapshot but implied): styling tasks for the same UI
- Primary anchor file: `html_advanced/index.html`
- Each task lives under `html_advanced/task_X/`, with task-specific guidelines in `README.md` in that folder.

## ✨ What AI agents should know first
- No backend code or JS runtime service exists; it's static paper website reconstruction.
- The goal is fidelity to a Figma design (see `html_advanced/readme.md` for the explicit design intent).
- The branch structure: top-level is flat with `html_advanced/`, assets under `html_advanced/assets/img/`, and tasks separated by `task_N` subdirectories.

## 🛠️ Common workflows in this repo
- Local preview: open `html_advanced/index.html` in browser.
- There is no explicit `npm`, `yarn`, or build pipeline in this repository.
- Markdown docs are the source of truth for requirements (`html_advanced/readme.md`, `html_advanced/task_0/README.md`).
- Keep updates within corresponding task folder (e.g., `html_advanced/task_0/`) and update its README to describe exactly what changed.

## 🧩 Style / architecture patterns
- Componentization is task-based; each task folder is treated as a block that can be integrated into the main page.
- SVG or image assets are in `html_advanced/assets/img/` and referenced by relative paths in HTML.
- Task names follow `task_N` and may contain a short explanation/README for expectations.

## 🔍 Issue triage for AI contributors
- If a change touches page layout, validate in browser and check the target instructions in `html_advanced/readme.md`.
- For HTML-only tasks, avoid adding extra scripting or frameworks.
- When generating HTML snippets, mimic existing class naming style (lowercase, hyphenated with semantic meaning if available).

## 📌 Example references (explicit from repo)
- `html_advanced/index.html` should contain final merged block outputs.
- `html_advanced/readme.md`: project mission, task boundaries, design source link.
- `html_advanced/task_0/README.md`: per-task instructions and grading expectations.

## 🧾 Merge instructions (for existing `.github/copilot-instructions.md` scenarios)
- Preserve existing guidance sections and update only project-specific areas above.
- If duplication exists, prefer the latest repository-specific details and keep bullet count concise (20-50 lines).

## 💬 Clarification needed
- Confirm whether `css_advanced/` folder exists in your active branch and whether style-related conventions should be added here.
- Indicate if tests or lints should be included after this baseline is validated.
