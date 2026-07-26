# Antigravity Plugins Repository

Welcome to the **Antigravity Plugins Repository**. This repository serves as the central hub for advanced AI Agent skills, subagents, and orchestrators designed for the Google Antigravity ecosystem.

These plugins supercharge your AI assistants by equipping them with domain-specific knowledge, specialized workflows, and autonomous subagent architectures. 

## 🌌 Overview

The Antigravity ecosystem empowers users to build and interact with specialized AI agents. This repository extends those capabilities by providing robust, enterprise-grade plugin bundles. Each plugin can contain:
- **Skills**: Detailed markdown-based instruction sets (`SKILL.md`) that teach an agent how to perform specific roles or tasks, along with helper scripts and reference materials.
- **Subagents**: Specialized autonomous agents that can be dynamically invoked to handle distinct parts of a larger workflow.
- **Orchestrators**: High-level manager agents that coordinate multiple subagents, manage data flow, and oversee complex, multi-step projects.

## 🛠️ Utilization in Software Environments

These plugins are designed to be environment-agnostic while excelling in highly specialized contexts (like Game Development, Enterprise Architecture, or Project Management). 

- **Local IDEs & File Systems**: Agents can read, analyze, and modify your local codebase directly, guided by the specialized skills within these plugins.
- **Specific Engine Environments (e.g., Unreal Engine 5)**: Plugins like `cannaville-studio` and `ue5-fantastic-five` provide agents with deep, context-aware knowledge of specific software architectures (like UE5 C++ and Blueprint conventions), allowing them to act as technical directors or game designers.
- **System Architecture & Cloud**: Plugins like `agent-architect` can interview users and dynamically generate code or deploy scripts for complex enterprise architectures.

## 🎼 Orchestrating Complex Workflows

One of the most powerful features of these plugins is their ability to orchestrate complex workflows through **Multi-Agent Architectures**.

Instead of relying on a single agent to do everything, these plugins utilize a hierarchical structure:
1. **The Orchestrator (Project Manager/Director)**: Interfaces with the user, understands the high-level goal, breaks it down into tasks, and maintains the overarching context (e.g., executing the Memory Bank protocol).
2. **Specialized Subagents**: The Orchestrator delegates tasks to subagents (e.g., an Art Director, a QA Lead, or a Tech Director). Each subagent operates with a hyper-focused prompt and toolset.
3. **Data Flow Management**: The Orchestrator manages the communication and data flow between subagents, synthesizing their outputs and presenting cohesive results back to the user.

## 📦 Included Plugins

### 1. `agent-architect`
The **Agent Architect** plugin provides a Meta-Agent designed for global systems engineering.
- **Role**: A master architect that interviews the user, gathers extensive requirements, and dynamically creates or updates Enterprise-Level agents, skills, and architectures.
- **Key Features**: Automates the creation of *new* AI agents and skills, essentially allowing the Antigravity ecosystem to expand and self-organize based on your project's unique needs.

### 2. `cannaville-studio`
A comprehensive suite of orchestrators designed for full-scale game development studio simulation.
- **Role**: Provides a complete studio hierarchy to manage the development of the "Cannaville" project.
- **Key Agents/Skills**:
  - **Art Director**: Orchestrates visuals, lighting, and UI.
  - **Lead Game Designer**: Orchestrates game design, features, and player experience.
  - **UE5 Technical Director**: Orchestrates engineering tasks, C++ architecture, and technical implementation.
  - **QA & Release Manager**: Manages testing, optimization tracking, and release pipelines.

### 3. `ue5-fantastic-five`
A highly specialized plugin focusing on the technical and production aspects of Unreal Engine 5 development and indie game publishing.
- **Role**: A tactical team of experts for UE5 project execution and deployment.
- **Key Agents/Skills**:
  - **Project Manager (Orchestrator)**: Sees the big picture, breaks down tasks, and manages data flow between the Fantastic Five.
  - **Senior UE5 Technical Director**: A master of UE5 editor features and asset integration. Guides users through technical hurdles with perfect understanding of C++ architecture.
  - **Lead Game Designer (Director)**: Hyper-focused on player psychology, "Game Feel," and Tactile UI.
  - **Project Manager & Steam Deploy Master**: Specializes in scope management for milestones (like Steam Next Fest) and designing indie marketing strategies.

---
*Note: To utilize a skill or agent from this repository in your Antigravity workflow, reference its specific path or invoke the relevant subagent by name as defined in your environment configuration.*
