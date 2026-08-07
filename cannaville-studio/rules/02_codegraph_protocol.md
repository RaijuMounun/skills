---
name: 02_codegraph_protocol
description: Enforces the use of CodeGraph for codebase navigation and clearly defines its limitations with UE5 Blueprints.
---
# The CodeGraph Protocol & Knowledge Boundary

CodeGraph is the primary semantic code intelligence engine for Cannaville Studio. It provides instant access to C++ architecture, call paths, and blast radius mapping.

## 1. Code Navigation Priority
Whenever any agent (especially `ue5_coder` or `cannaville_tech_director`) needs to understand existing code or architecture:
- YOU MUST prioritize `codegraph_explore` (via MCP) to get semantic graphs, call paths, and blast radius.
- `grep_search` and manual file reading (`view_file`) are STRICTLY FORBIDDEN unless CodeGraph fails or is completely unavailable.

## 2. The Blueprint Limitation (.uasset)
CodeGraph parses code using Tree-sitter, which means it **CANNOT read Binary Blueprint files (.uasset).**
- YOU MUST NEVER expect CodeGraph to find logic built entirely in Blueprints.
- For Blueprint modifications, agents MUST rely on manual Editor testing (as per the VBC Protocol's 'Manual Verification Plan') and coordinate with the `archivist` for Game Design Documents.

## 3. The Knowledge Boundary (Archivist)
- The `archivist` is the master of Game Design, Lore, Tasks, and Studio Rules.
- The `archivist` MUST NEVER attempt to manually index source code (C++, Blueprints, etc.). Source code indexing is handled automatically by the CodeGraph semantic engine.
- If technical agents need C++ context, they query CodeGraph. If they need Lore/GDD context, they query the Archivist.
