# SDD Antigravity Template

A template for **Specification-Driven Development (SDD)** in Antigravity, inspired by [GitHub Spec Kit](https://github.com/github/spec-kit).

## What is SDD?

Specification-Driven Development (SDD) is a methodology that emphasizes creating detailed, natural language specifications before implementation. It treats the specification as the source of truth, ensuring alignment between intent and code.

The core workflow follows a loop:
1.  **Specify**: Define *what* needs to be built.
2.  **Clarify** (Optional): Identify ambiguity in the specification.
3.  **Plan**: Design *how* it will be implemented.
4.  **Task**: Break the plan into actionable steps.
5.  **Analyze** (Optional): Ensure consistency across artifacts.
6.  **Implement**: Execute the tasks.

## Features (Workflows)

This template leverages **Antigravity Workflows** (slash commands) to facilitate the SDD process.

| Workflow | Slash Command | Description |
| :--- | :--- | :--- |
| **Constitution** | `/speckit.constitution` | Establish project-wide principles and rules. |
| **Specify** | `/speckit.specify` | Create or update a detailed feature specification. |
| **Clarify** | `/speckit.clarify` | Identify ambiguity in specs and ask clarifying questions. |
| **Plan** | `/speckit.plan` | Generate a technical implementation plan from the spec. |
| **Checklist** | `/speckit.checklist` | Generate custom checklists for features. |
| **Tasks** | `/speckit.tasks` | Convert the plan into an actionable `tasks.md`. |
| **Implement** | `/speckit.implement` | Execute the implementation tasks. |
| **Analyze** | `/speckit.analyze` | Perform a quality consistency check across artifacts. |

## Getting Started

1.  **Initialize your Constitution**:
    Start by defining the core rules of your project. This ensures all future generation aligns with your standards.
    ```
    /speckit.constitution
    ```

2.  **Create a Feature Spec**:
    Describe your new feature in natural language, then run:
    ```
    /speckit.specify
    ```

3.  **Plan and Implement**:
    Follow the prompts to Plan (`/speckit.plan`), Task (`/speckit.tasks`), and Implement (`/speckit.implement`).

## Project Structure

*   `.specify/`: Contains templates and memory for the SDD process.
    *   `memory/`: Stores the project constitution and active context.
    *   `templates/`: Markdown templates for specs, plans, and tasks.
*   `.agent/workflows/`: Definitions for the SDD workflows (slash commands).