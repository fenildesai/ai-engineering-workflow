# AI Engineering Workflow for GitHub Copilot

Welcome to the AI Engineering Workflow repository! This project provides a production-ready, instruction-driven system that transforms GitHub Copilot into an intelligent orchestrator within VS Code.

## Features
- **Adaptive Execution**: Automatically detects if a task is simple (Fast Path) or complex (Deep Path).
- **Mode-Based Design**: Implicitly adopts personas (Analyst, Architect, Developer, Reviewer) based on the task phase.
- **Requirement Validation**: Strict checking of incoming JIRA tickets or tasks before writing code.
- **Token Efficient**: Relies on instructions and contextual awareness, saving developers from writing massive prompts.

## Getting Started
To use this setup in your own project:
1. Copy the `.github/` folder and `copilot-instructions.md` into your repository.
2. Ensure you have GitHub Copilot configured in VS Code.
3. Simply paste a JIRA ticket or requirement into Copilot Chat and let the orchestrator guide the workflow.

## Documentation
For a deep dive into the architecture, diagrams, and design principles, please read the [AI Engineering Pattern – Copilot Agentic Workflow](AI_Engineering_Pattern_Copilot_Workflow.md).

## Original Prompt
Curious how this repository was generated? Check out the [PROMPT.md](PROMPT.md) to see the exact instructions used to bootstrap this architecture.
