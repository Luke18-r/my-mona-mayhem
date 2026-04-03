🌐 [Português (Brasil)](README.pt_BR.md) | [Español](README.es.md)

# 🎮 Mona Mayhem

## ⚡ The Ultimate GitHub Copilot Hands-On Workshop

> **Turn your dev skills up to 11** with a retro arcade experience that teaches you **everything** about GitHub Copilot — from Chat Mode to Agent Mode to the blazing-fast CLI.

Build a **GitHub Contribution Battle Arena** — a retro arcade-themed app that pits your GitHub contributions against your friends'. This is your launchpad for mastering modern AI-assisted development.

![Mona Mayhem Screenshot](https://github.com/user-attachments/assets/5eca79e2-cb9f-4e93-aa0d-23666ebde3b7)
*Level up your Copilot skills by building this 👆*

### 🎯 What You'll Get

By the end of this workshop, you'll have:

- **✨ A deployed retro arcade web app** that fetches and displays real GitHub contribution graphs
- **🚀 Mastery of GitHub Copilot workflows** — Chat, Plan Mode, Agent Mode, and the CLI
- **🎨 Design-first development skills** — planning before coding
- **⚙️ Full-stack Astro experience** — API routes, server-side rendering, state management
- **🤝 Collaboration techniques** — parallel work, code reviews, and quality gates
- **🧠 AI-fluent mindset** — how to think about problems in an AI-assisted workflow

### 🔥 Why This Workshop?

- **Real-world stack** — Astro, TypeScript, Node.js (not a toy project)
- **Two learning paths** — choose VS Code or CLI, based on your style
- **Hands-on from start to finish** — you're building, not just watching
- **GitHub Copilot focused** — each step teaches a specific Copilot feature
- **~1 hour** — perfect for a lunch break or afternoon session

## 📚 Workshop

The workshop supports two tracks — follow the one that matches your preferred workflow:

- **VS Code track** — Chat, Plan Mode, Agent Mode, background agents, and editor-native review loops
- **CLI track** — `copilot`, `@file` context, `/plan`, autonomous edits, `/fleet`, `/delegate`, and `/review`

| Part | Title | Copilot Focus |
|------|-------|---------------|
| [00](workshop/00-overview.md) | Overview | Track selection and learning goals |
| [01](workshop/01-setup.md) | Setup & Context Engineering | Instructions, permissions, and environment setup |
| [02](workshop/02-plan-and-scaffold.md) | Plan & Scaffold | Planning the API and page architecture |
| [03](workshop/03-agent-mode.md) | Build the Game | Agentic implementation and iteration |
| [04](workshop/04-design-vibes.md) | Design-First Theming | Visual design planning and implementation |
| [05](workshop/05-polish.md) | Polish & Parallel Work | Parallelism, reviews, and quality passes |
| [06](workshop/06-bonus.md) | Bonus & Extensions | Open-ended feature ideas and extra Copilot experiments |

## 🚀 Quick Start

1. **Create your own repo first** by either:
   - clicking **Use this template** to create a new repo, or
   - forking this repository.
2. Choose your workshop path:
   - **VS Code:** clone your repo and open it in VS Code.
   - **GitHub Copilot CLI:** clone your repo locally, install `copilot`, and work from your terminal.
3. Follow the [workshop guide](workshop/00-overview.md)

## Prerequisites

### Shared

- GitHub Copilot (Pro, Business, or Enterprise)
- Git
- Node.js

### VS Code track

- VS Code v1.107+
- GitHub Copilot extension signed in

### CLI track

- GitHub Copilot CLI (`copilot`)
- Node.js 22+ if you plan to install the CLI via `npm install -g @github/copilot`
- Or Homebrew / WinGet if you prefer a native package manager install

## Technology Stack

- **Framework**: [Astro](https://astro.build/) v5
- **Runtime**: Node.js with [@astrojs/node](https://docs.astro.build/en/guides/integrations-guide/node/) adapter
- **Font**: Press Start 2P (retro gaming font)
- **API**: GitHub's contribution graph API

## License

MIT
