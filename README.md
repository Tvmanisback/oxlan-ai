# Oxlan AI

Oxlan AI is a general-purpose AI assistant skill/plugin designed for programming, learning, Roblox Luau, game development, web development, secure software engineering, writing, planning, and troubleshooting.

This repository contains the plugin manifests and skill instructions needed to integrate Oxlan AI with compatible AI agent platforms.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Repository Structure](#repository-structure)
- [Installation](#installation)
- [Using Oxlan AI](#using-oxlan-ai)
- [Customization](#customization)
- [Security and Safety](#security-and-safety)
- [Limitations](#limitations)
- [Contributing](#contributing)
- [License](#license)
- [Support](#support)

## Overview

Oxlan AI helps users learn, build, debug, understand, and improve software.

Its instructions emphasize practical programming assistance, detailed explanations, beginner-friendly teaching, and secure software development.

Oxlan AI provides guidance for multiple programming languages and development environments, with particular attention to Roblox Studio and Luau.

The project is distributed as a collection of plugin manifests and Markdown-based skill instructions. It is not a standalone AI model or executable application.

Actual functionality depends on the AI platform loading the skill and providing the necessary capabilities.

## Features

### Programming Assistance
- Write complete programs and project files.
- Debug errors and investigate unexpected behavior.
- Explain code and programming concepts.
- Refactor and improve existing implementations.
- Design application architecture.
- Create documentation and tests.
- Help configure development environments and build pipelines.

### Programming Languages

Oxlan AI's instructions cover numerous languages and technologies, including:

- Python
- JavaScript and TypeScript
- HTML and CSS
- React and Node.js
- Lua and Roblox Luau
- C and C++
- C# and Java
- Kotlin and Swift
- Go and Rust
- SQL
- PHP
- Bash and PowerShell
- YAML, JSON, and XML

Support depends on the capabilities of the underlying AI platform.

### Roblox Development

Roblox development is a major focus of Oxlan AI.

Supported topics include:
- Scripts, LocalScripts, and ModuleScripts.
- User interfaces and menus.
- RemoteEvents and RemoteFunctions.
- Inventory and currency systems.
- Shops and purchases.
- DataStores and player progression.
- NPCs, dialogue, and gameplay mechanics.
- Multiplayer systems.
- Performance optimization.
- Server-side validation and anti-exploit protection.

Oxlan AI's instructions emphasize server-authoritative game architecture and secure handling of valuable gameplay actions.

### Game Development

Oxlan AI can assist with development concepts and code for:
- Roblox Studio.
- Unity and C#.
- Unreal Engine and C++.
- Godot and GDScript.
- Other programming-based game development workflows.

### Web and Application Development

The skill also covers:
- Responsive websites.
- Frontend and backend development.
- APIs and web services.
- Authentication systems.
- Application settings and interfaces.
- Databases and data processing.
- Configuration files.
- Build and deployment workflows.

### Secure Software Engineering

Oxlan AI encourages:
- Input validation.
- Secure authentication.
- Appropriate password hashing.
- Authorization checks.
- Least-privilege design.
- Safe error handling.
- Dependency review.
- Privacy protection.
- Defensive security testing.

### Teaching and Troubleshooting

Instructions encourage Oxlan AI to adapt explanations to the user's experience.

Beginners should receive clear explanations and practical steps. More experienced developers can receive deeper technical analysis, architecture guidance, and discussion of implementation tradeoffs.

Oxlan AI should also distinguish between code that has been generated, reviewed, and actually executed.

## Repository Structure

```text
oxlan-ai/
├── README.md
├── plugin.json
├── .codex-plugin/
│   └── plugin.json
└── skills/
    └── oxlan-chat/
        ├── SKILL.md
        └── RULES.md
```

### File Descriptions

| File | Description |
|---|---|
| `README.md` | Project overview and documentation. |
| `plugin.json` | General plugin manifest containing the name, version, and description. |
| `.codex-plugin/plugin.json` | Plugin descriptor for compatible Codex-style plugin loaders. |
| `skills/oxlan-chat/SKILL.md` | Main skill instructions, coding capabilities, behavior, and response style. |
| `skills/oxlan-chat/RULES.md` | Detailed safety, privacy, instruction-integrity, and security rules. |

## Installation

Installation depends on the AI agent platform you intend to use.

### 1. Download the Repository

Clone the repository:

```bash
git clone https://github.com/Tvmanisback/oxlan-ai.git
cd oxlan-ai
```

Alternatively, download the repository as a ZIP file from GitHub and extract it.

### 2. Load the Plugin

Use the installation method supported by your AI agent platform.

Depending on the platform, this may involve:

- Registering the repository as a plugin.
- Loading the plugin manifest.
- Importing the skill directory.
- Adding the skill instructions through the platform's supported configuration mechanism.

The repository includes two plugin manifests:

- `plugin.json`
- `.codex-plugin/plugin.json`

Use the manifest supported by your chosen platform.

### 3. Load the Skill Instructions

The main skill definition is located at:

```text
skills/oxlan-chat/SKILL.md
```

The detailed safety rules are located at:

```text
skills/oxlan-chat/RULES.md
```

Ensure that the host platform makes both files available when appropriate. The main skill explicitly refers to `RULES.md`.

**Important:** Cloning this repository does not automatically install Oxlan AI into every AI application. The target platform must support the relevant plugin or skill-loading mechanism.

## Using Oxlan AI

After loading the skill into a compatible platform, you can ask it for help with ordinary programming and development tasks.

Example prompts:

**Programming**
- "Explain this Python error and help me fix it."
- "Refactor this JavaScript function."
- "Help me organize this project into separate modules."

**Roblox**
- "Create a Roblox shop with server-validated purchases."
- "Help me debug this Luau script."
- "Design a secure inventory system."

**Game Development**
- "Help me implement a player movement system."
- "Explain how to structure a Unity project."
- "Help me optimize a game for lower-end hardware."

**Web Development**
- "Build a responsive website layout."
- "Help me debug an API request."
- "Review my authentication implementation."

**Learning**
- "Explain this code step by step."
- "Teach me how functions work in Python."
- "Help me understand this compiler error."

For troubleshooting, provide relevant source code, error messages, expected behavior, and software versions.

Never share real passwords, API keys, session tokens, or other private credentials when asking for help.

## Customization

You can modify Oxlan AI's skill instructions to suit your project.

### Main Skill

Edit:

```text
skills/oxlan-chat/SKILL.md
```

This file defines the assistant's identity, capabilities, coding guidance, teaching approach, and response style.

### Safety Rules

Edit:

```text
skills/oxlan-chat/RULES.md
```

This file contains detailed guidance covering instruction integrity, prompt injection, privacy, cybersecurity, Roblox development boundaries, and secure coding.

### Plugin Metadata

The plugin manifests define the plugin's name, version, and description.

If you rename the plugin or reorganize its files, update the relevant metadata and paths consistently.

### Testing Changes

After modifying the skill:

1. Test ordinary programming requests.
2. Test code explanations and debugging tasks.
3. Test Roblox development scenarios.
4. Check whether both skill files are loaded correctly.
5. Test relevant security and prompt-injection scenarios.
6. Verify that the assistant accurately describes its capabilities and limitations.

Changes to behavioral instructions alone cannot guarantee that an AI platform will follow every instruction.

## Security and Safety

Oxlan AI's instructions promote legitimate development, responsible security practices, and protection of private information.

The rules address:
- Prompt injection and attempts to override governing instructions.
- Credential theft and unauthorized account access.
- Malicious software and destructive actions.
- Secure authentication and authorization.
- Roblox exploit development and defensive alternatives.
- Privacy and secret management.
- Safe software engineering practices.

The project supports legitimate programming, defensive cybersecurity, authorized testing, and security education.

For the complete policy, see:

[`skills/oxlan-chat/RULES.md`](skills/oxlan-chat/RULES.md)

### Important Security Disclaimer

Oxlan AI's Markdown instructions are behavioral guidance, not an independent security-enforcement system.

Their effectiveness depends on whether the host platform loads and applies them.

They do not guarantee:
- Complete protection against prompt injection.
- Immunity to jailbreak attempts.
- Perfectly secure generated code.
- Error-free software.
- Detection of every harmful request.

Review and test generated code before using it in production.

## Limitations

- Oxlan AI is not a standalone AI model.
- Available tools depend on the host platform.
- Plugin compatibility varies between platforms.
- Installation procedures may change as platforms evolve.
- Generated code requires appropriate testing and review.
- The manifests do not independently provide model hosting or API credentials.
- Safety instructions cannot replace platform-level security controls.

## Contributing

Contributions, bug reports, and feature suggestions are welcome.

### Suggested Contribution Process

1. Review the existing README and skill instructions.
2. Identify the behavior or documentation that needs improvement.
3. Make focused changes.
4. Test your changes where practical.
5. Avoid including credentials, tokens, or private information.
6. Submit a pull request explaining the changes.

Contributions should preserve the project's emphasis on helpful programming assistance, accurate explanations, privacy, and secure development.

### Report Issues

Report bugs and suggest improvements through GitHub Issues:

https://github.com/Tvmanisback/oxlan-ai/issues

When reporting a problem, include relevant details and reproducible examples. Remove sensitive information from logs and screenshots.

## License

No `LICENSE` file was found in the repository when this README was prepared.

Until a license is added, do not assume the project is available for unrestricted copying, redistribution, or modification.

Contact the repository maintainer for clarification about reuse.

## Support

- **Repository:** https://github.com/Tvmanisback/oxlan-ai
- **Issues:** https://github.com/Tvmanisback/oxlan-ai/issues
- **Main skill:** [SKILL.md](skills/oxlan-chat/SKILL.md)
- **Safety rules:** [RULES.md](skills/oxlan-chat/RULES.md)

---

Made for developers, learners, and creators who want practical AI assistance.
