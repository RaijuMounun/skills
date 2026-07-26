# Agent Architect Plugin

## Overview

**Agent Architect** is a powerful meta-plugin designed to engineer enterprise-level autonomous agents. It acts as an elite AI systems engineer that interviews you, gathers your project requirements, and dynamically architectures, designs, and deploys specialized agents and their supporting infrastructure. 

While optimized for local agent frameworks, the architecture logic it produces can be utilized in **any AI environment** (Cursor, Claude, Custom GPTs).

## The Paradigm: Skills vs. Background Workers

The Agent Architect enforces a strict separation of concerns in agent design, utilizing two main types of agents:

1. **Interactive Leaders (Skills):**
   User-facing agents designed for direct interaction. Think of them as the Project Manager or Orchestrator. Represented as `SKILL.md` files.
   *Usage elsewhere:* Paste these into Claude Projects or use them as your primary Custom GPT prompt.
   
2. **Background Workers (JSON Subagents):**
   Agents that perform heavy lifting in the background without direct user interaction (e.g., Code Reviewer, Optimizer). Represented as `.json` configuration files containing system prompts.
   *Usage elsewhere:* Use these prompts for secondary AI chats, Cursor agents, or script-based API calls.

## Architectural Decision Making

- **Single-Agent Tasks:** For straightforward requests, the Architect generates a single `SKILL.md` file.
- **Multi-Agent Loops (Agent-Driven Development):** For complex tasks, the Architect designs an entire Agent-Driven Development (ADD) architecture, ensuring robust cross-agent communication protocols and strict delegation rules.

## Included Skills

### `agent_architect`
- **Description:** The core meta-agent that serves as your global systems engineer. 
- **Usage:** Invoke the agent architect to design a new agent or a swarm of agents. It will interview you, design the architecture, and synthesize the required files.
- **Language Policy:** Communicates in **Turkish**, while generated code and configs are in **English**.
- **Guardrails:** Enforces Human-In-The-Loop (HITL) approval gates and operates with zero assumptions.
