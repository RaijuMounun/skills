# UE5 Fantastic Five & Cannaville Architecture 🎮

This repository contains the configuration and skills for an advanced, Agent-Driven Development (ADD) architecture tailored for Unreal Engine 5 C++ projects, specifically geared towards the **Cannaville** project.

## The Legacy Orchestration Setup: The Fantastic Five
At the core of this system is the **Fantastic Five**, a highly disciplined, enterprise-grade engineering pipeline. It moves beyond simple LLM code generation by implementing a **Manager-Subordinate paradigm** and utilizing a local JSON-based memory system known as the **Memory Bank Protocol**. 

The legacy 5-agent engineering team consists of:
1. **Orchestrator**: The workflow router and project manager for engineering.
2. **Archivist**: The local RAG/Memory system maintainer.
3. **Lead Coder**: The C++ Architect that spawns subagents for implementation.
4. **Senior Reviewer**: The QA Manager that enforces SOLID principles, UE5 standards, and performance.
5. **Git Agent**: The version control expert that safely commits compiled code.

## The 3-Team Dynamic
For the Cannaville project, the architecture has evolved beyond pure C++ engineering into a comprehensive **3-Team Dynamic**, covering the entire game development lifecycle:

1. **Vision & Production Team**: Responsible for the "what" and the "why". They define the game's soul, manage the scope for Steam Next Fest, and ensure the player psychology is perfectly tuned.
2. **Engineering Team (Fantastic Five)**: Responsible for the "how" (in code). They execute the C++ logic, maintain the Memory Bank, and ensure architectural integrity.
3. **Engine & Integration Team**: Responsible for the "where". They bridge the gap between the raw C++ code and the visual Unreal Engine 5 Editor (Blueprints, UMG, Animations).

## Agent Roles & Responsibilities

### 🎨 Lead Game Designer (`cannaville_gd`)
- **Role**: Creative Director & Game Feel Expert.
- **Focus**: Player psychology, the "cozy to panic" loop, Game Feel ("juice"), and Tactile UI.
- **Workflow**: Proposes bold ideas without fear of scope creep (leaving that to the PM). Provides detailed, non-technical "director" descriptions of how things should look and feel. 
- **Key Trait**: A strict "Anti-Yes-Man". Will aggressively push back on user ideas if they harm the game's psychological impact or lack "juice".

### 📊 Project Manager (`cannaville_pm`)
- **Role**: Executive Producer & Steam Deploy Master.
- **Focus**: Steam Next Fest deployment, scope management, and indie marketing strategies.
- **Workflow**: Analyzes Obsidian GDDs, prioritizes features for the demo, and designs capsule/trailer strategies. 
- **Key Trait**: The ultimate safeguard against "feature creep". Keeps the project on track and the developer focused on the roadmap.

### 🎼 Orchestrator (`orchestrator_cannaville`)
- **Role**: Engineering Project Manager.
- **Focus**: Big picture task routing and Memory Bank Protocol execution.
- **Workflow**: Enforces a strict "Design-First" rule. Reads context via the Archivist before allowing any coding. Delegates to the Lead Coder and manages the QA loop (preventing infinite "Redjection" loops).
- **Key Trait**: Enforces the "Write Last" rule, ensuring all completed tasks are logged in the project's state memory before handing off UI/Blueprint integration to the Tech Director.

### 🛠️ UE5 Tech Director (`ue5_master`)
- **Role**: Senior Unreal Engine 5 Technical Director.
- **Focus**: Editor features, asset integration, and user mentorship.
- **Workflow**: Takes over after the Engineering team commits C++ code. Guides the user step-by-step (using precise English UE5 UI terminology) on how to bind C++ classes to UMG Widgets, AnimBPs, and other engine assets.
- **Key Trait**: Strictly banned from writing C++ code or suggesting gameplay logic in Blueprints. Acts purely as an editor guide and integration mentor.
