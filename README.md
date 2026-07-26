# AI Agent Plugins & Skills Repository

Welcome to my custom **Plugins Repository**. This repository serves as the central hub for advanced AI Agent skills, subagents, and orchestrators. 

These configurations are designed to supercharge your AI assistants by equipping them with domain-specific knowledge, specialized workflows, and autonomous subagent architectures. **They are ecosystem-agnostic** and can be used in Cursor, Claude Projects, Antigravity, OpenAI Custom GPTs, or any other agentic framework.

## 🌌 Overview

This repository provides robust, enterprise-grade plugin bundles. Each plugin typically contains:
- **Skills (`SKILL.md`)**: Detailed instruction sets that teach an AI how to perform specific roles or tasks (Interactive Leaders).
- **Subagents (`.json`)**: System prompts and configurations for specialized background workers.
- **Orchestrators**: High-level manager agents that coordinate multiple subagents, manage data flow, and oversee complex, multi-step projects.

## 🚀 How to Use in Different Programs

Because these agents rely on text-based system prompts and instructions, you can easily adapt them to your favorite AI tool:

1. **Cursor / Windsurf**: 
   - Copy the contents of a `SKILL.md` or `.json` file into your `.cursorrules` or `.windsurfrules` file to give the IDE a specific persona (e.g., UE5 Tech Director).
2. **Claude (Projects)**: 
   - Upload the `SKILL.md` files as "Project Knowledge" and use the system prompts in the `.json` files as the custom instructions for the project.
3. **Custom GPTs (OpenAI)**: 
   - Paste the `system_prompt` from a `.json` or the instructions from a `SKILL.md` into the "Instructions" box of a new Custom GPT.
4. **Antigravity / Local Frameworks**: 
   - Drop the plugin folders directly into your configurations folder to utilize the dynamic `invoke_subagent` multi-agent loops natively.

## 🛠️ Utilization in Software Environments

These plugins excel in highly specialized contexts:
- **Specific Engine Environments (e.g., Unreal Engine 5)**: Plugins like `cannaville-studio` and `ue5-fantastic-five` provide agents with deep, context-aware knowledge of UE5 C++ and Blueprint conventions.
- **System Architecture**: Plugins like `agent-architect` can interview users and dynamically generate code or deploy scripts for complex enterprise architectures.

## 🎼 Orchestrating Complex Workflows

One of the most powerful features of these plugins is their ability to orchestrate complex workflows through **Multi-Agent Architectures**.
Instead of relying on a single agent to do everything, these plugins utilize a hierarchical structure:
1. **The Orchestrator (Project Manager/Director)**: Interfaces with the user, understands the high-level goal, and breaks it down into tasks.
2. **Specialized Subagents**: The Orchestrator delegates tasks to subagents (e.g., an Art Director, a QA Lead, or a Tech Director). 
3. **Data Flow Management**: The Orchestrator manages the communication and data flow between subagents.

## 📦 Included Plugins

### 1. `agent-architect`
A Meta-Agent designed for global systems engineering. It interviews the user, gathers requirements, and dynamically creates or updates Enterprise-Level agents, skills, and architectures.

### 2. `cannaville-studio`
A comprehensive suite of orchestrators designed for full-scale game development studio simulation (Art Direction, Game Design, Tech, QA). Uses a Zero-Assumption, Agent-Driven paradigm.

### 3. `ue5-fantastic-five`
A highly specialized legacy plugin focusing on the technical and production aspects of Unreal Engine 5 development and indie game publishing.
