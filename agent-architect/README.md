# Agent Architect Plugin

## Overview

**Agent Architect** is a powerful meta-plugin designed to engineer enterprise-level autonomous agents. It acts as an elite AI systems engineer that interviews you, gathers your project requirements, and dynamically architectures, designs, and deploys specialized agents and their supporting infrastructure. 

It is tailored for complex agentic workflows, taking advantage of state-of-the-art multi-agent loop architectures.

## The New Paradigm: Skills vs. Background Workers

The Agent Architect enforces a strict separation of concerns in agent design, utilizing two main types of agents:

1. **Interactive Leaders (Skills):**
   These are user-facing agents designed for direct interaction. Think of them as the Project Manager, Orchestrator, or Lead Designer. They are created as `SKILL.md` files and invoked directly in the chat via `@mention`.
   
2. **Background Workers (JSON Subagents):**
   These agents perform the heavy lifting in the background without direct user interaction (e.g., Lead Coder, Senior Reviewer, Git Agent). They are created as `.json` configuration files and are spawned dynamically by the Interactive Leaders using the `invoke_subagent` tool.

## Architectural Decision Making

Depending on your request, the Agent Architect will design the appropriate system:

- **Single-Agent Tasks:** For straightforward and one-dimensional requests (like a specialized writer or a basic code analyzer), the Architect will generate a single `SKILL.md` file.
- **Multi-Agent Loops (Agent-Driven Development):** For complex tasks (such as building a complete application or a UE5 plugin), the Architect will design an entire Agent-Driven Development (ADD) architecture. This includes designing a "Chief / Orchestrator" skill and specialized background workers. It ensures robust cross-agent communication protocols and enforces loop breakers (pausing to ask for human help if needed).

## Included Skills

### `agent_architect`
- **Description:** The core meta-agent that serves as your global systems engineer. 
- **Usage:** Invoke the agent architect when you want to design a new agent or a swarm of agents. It will start by interviewing you to understand the scope and requirements of your project, then proceed to the architectural design, and finally synthesize and deploy the required `.md` and `.json` files to your workspace.
- **Language Policy:** The Agent Architect will communicate with you exclusively in **Turkish**, while all generated code, configs, and architectural files will be in **English**.
- **Guardrails:** It enforces Human-In-The-Loop (HITL) approval gates for high-stakes actions and operates with zero assumptions.

## How to Use

1. Mention the Agent Architect skill in your chat to begin the process.
2. The Architect will interview you (in Turkish) to gather your requirements. 
3. Based on your answers, it will design the architecture (either a single skill or a multi-agent system).
4. Upon your approval, the Architect will synthesize the necessary files and deploy them automatically.
