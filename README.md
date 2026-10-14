# Oxlan AI

Oxlan AI is a general-purpose AI assistant focused on coding, learning, game and web development (notably Roblox Luau), writing, planning, and secure software engineering. This repository packages Oxlan AI as an agent plugin/skill set that can be loaded by compatible agent platforms.

## Table of contents
- [What is Oxlan AI](#what-is-oxlan-ai)
- [Features](#features)
- [Repository structure](#repository-structure)
- [Usage](#usage)
- [Developing / Extending](#developing--extending)
- [Security & Safety](#security--safety)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## What is Oxlan AI
Oxlan AI helps users learn, build, debug, and improve software and games. It provides practical programming assistance, detailed explanations, and secure-by-default guidance, with first-class support for Roblox Luau and game-development workflows.

## Features
- Programming help: design, implement, debug, refactor, and document code.
- Multi-language support (examples in-skill): Python, JavaScript/TypeScript, Lua/Luau, C#, C++, Go, Rust, and more.
- Game dev guidance: Roblox (Luau), Unity, Unreal, Godot patterns and recommendations.
- Secure coding recommendations and defensive engineering best practices.
- Teaching-oriented responses tailored to beginners and experienced developers.
- Safety and prompt-injection resistance rules for secure interactions.

## Repository structure
```text
plugin.json              # Plugin manifest (name, version, description)
.codex-plugin/plugin.json # Plugin descriptor used by some loaders
skills/                  # Skills provided by this plugin
  oxlan-chat/
    SKILL.md             # Main skill definition and behavior rules
    RULES.md             # Strict safety and security rules & policies
.github/                 # GitHub metadata (workflows, templates) — optional
