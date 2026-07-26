# UE5 Fantastic Five & Cannaville Architecture 🎮

This repository contains the configuration and skills for an advanced, Agent-Driven Development (ADD) architecture tailored for Unreal Engine 5 C++ projects, specifically geared towards the **Cannaville** project.

These configurations (prompts and roles) are **ecosystem-agnostic** and can be loaded into Cursor (`.cursorrules`), Claude Projects, or any agentic workflow system to simulate a full indie studio.

## The Legacy Orchestration Setup: The Fantastic Five
At the core of this system is the **Fantastic Five**, a highly disciplined, enterprise-grade engineering pipeline. It implements a **Manager-Subordinate paradigm** and utilizes a local JSON-based memory system known as the **Memory Bank Protocol**. 

The legacy 5-agent engineering team consists of:
1. **Orchestrator**: The workflow router and project manager for engineering.
2. **Archivist**: The local RAG/Memory system maintainer.
3. **Lead Coder**: The C++ Architect that spawns subagents for implementation.
4. **Senior Reviewer**: The QA Manager that enforces SOLID principles, UE5 standards, and performance.
5. **Git Agent**: The version control expert that safely commits compiled code.

## The 3-Team Dynamic
For the Cannaville project, the architecture evolved into a comprehensive **3-Team Dynamic**, covering the entire game development lifecycle:

1. **Vision & Production Team**: Defines the game's soul, manages scope, and ensures player psychology is perfectly tuned.
2. **Engineering Team (Fantastic Five)**: Executes the C++ logic, maintains memory, and ensures architectural integrity.
3. **Engine & Integration Team**: Bridges the gap between the raw C++ code and the visual Unreal Engine 5 Editor (Blueprints, UMG).

## Agent Roles & Responsibilities

### 🎨 Lead Game Designer (`cannaville_gd`)
- **Focus**: Player psychology, the "cozy to panic" loop, Game Feel ("juice"), and Tactile UI.
- **Key Trait**: A strict "Anti-Yes-Man". Will aggressively push back on user ideas if they harm the game's psychological impact.

### 📊 Project Manager (`cannaville_pm`)
- **Focus**: Steam Next Fest deployment, scope management, and indie marketing strategies.
- **Key Trait**: The ultimate safeguard against "feature creep". Keeps the developer focused on the roadmap.

### 🎼 Orchestrator (`orchestrator_cannaville`)
- **Focus**: Big picture task routing and Memory Bank Protocol execution.
- **Key Trait**: Enforces the "Write Last" rule, ensuring all completed tasks are logged in memory before UI integration.

### 🛠️ UE5 Tech Director (`ue5_master`)
- **Focus**: Editor features, asset integration, and user mentorship.
- **Key Trait**: Strictly banned from writing C++ code. Acts purely as an editor guide and integration mentor.
