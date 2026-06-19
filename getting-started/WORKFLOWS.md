# Getting Started with Workflows

> "There's not much you can do without a CPU." — Mr. Robot

This document covers the tools, configurations, and conventions you'll need to set up before your first sprint. Work through each section in order and flag anything that doesn't work to your mentor or the team's IT contact.

---

## Hardware

We support the following operating systems:

- **macOS** — Preferred for most development roles. Apple Silicon (M-series) and Intel both supported.
- **Linux** — Any modern Debian/Ubuntu-based or Arch-based distribution works well.
- **Windows** — Supported via WSL2 (Windows Subsystem for Linux). Set up WSL2 with Ubuntu 22.04 before proceeding.

If you're unsure whether your hardware meets requirements, ask before you start installing things.

---

## Software

### Browser

We require **Chrome** or a Chromium-based browser. Extensions used across the team:

- [axe DevTools](https://www.deque.com/axe/devtools/) — Accessibility testing
- [React Developer Tools](https://react.dev/learn/react-developer-tools) — Component inspection
- [JSON Viewer](https://chromewebstore.google.com/detail/json-viewer/gbmdgpbipfallnflgajpaliibnhdgobh) — Readable API responses

---

### Integrated Development Environment (IDE)

**Recommended:** VS Code or VSCodium

Install the following extensions as a baseline:

```
ESLint
Prettier - Code formatter
GitLens
Docker
REST Client
EditorConfig for VS Code
```

**Also supported:** JetBrains IDEs (WebStorm, IntelliJ IDEA). The team maintains a shared `.editorconfig` and linting config that works with both.

Configure your editor to:
- Format on save
- Use 2-space indentation (project `.editorconfig` will enforce this)
- Show trailing whitespace

---

### Version Control

We use **Git** and **GitHub**.

**Setup checklist:**

1. Install git: `brew install git` (macOS) or `sudo apt install git` (Linux/WSL)
2. Configure your identity:
   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "you@company.com"
   ```
3. Generate an SSH key and add it to GitHub:
   ```bash
   ssh-keygen -t ed25519 -C "you@company.com"
   cat ~/.ssh/id_ed25519.pub
   # Paste into GitHub → Settings → SSH and GPG Keys
   ```
4. Set your default branch name:
   ```bash
   git config --global init.defaultBranch main
   ```

---

### Node.js / Runtime

We use **Node.js** for most frontend and tooling work.

Install via [nvm](https://github.com/nvm-sh/nvm) (Node Version Manager) so you can switch versions per project:

```bash
# Install nvm
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash

# Install the LTS version
nvm install --lts
nvm use --lts
```

The project's `.nvmrc` file will specify the correct version. Run `nvm use` at the project root to switch automatically.

---

### Package Management

- **npm** — default, always available with Node
- **pnpm** — preferred for monorepos: `npm install -g pnpm`
- **bun** — used in select projects: follow the [bun docs](https://bun.sh/docs/installation)

Check the project's `README.md` for which one it uses.

---

### Docker

We containerize services for local development. Install [Docker Desktop](https://www.docker.com/products/docker-desktop/) (macOS/Windows) or Docker Engine + Docker Compose (Linux).

Verify your install:

```bash
docker --version
docker compose version
```

---

## Conventions

### Branch Naming

```
feature/short-description
fix/short-description
chore/short-description
docs/short-description
```

### Commit Messages

We follow [Conventional Commits](https://www.conventionalcommits.org/):

```
feat: add user authentication
fix: resolve null pointer in payment flow
docs: update onboarding README
chore: upgrade eslint to v9
```

### Pull Requests

- Keep PRs small and focused (one concern per PR)
- Link the relevant GitHub issue in the PR description
- Request at least one reviewer before merging
- Do not merge your own PR unless explicitly allowed

---

## Communication Tools

- **Slack** — Primary async communication
- **GitHub** — Code reviews, issues, project boards
- **Google Meet / Zoom** — Standups and ceremonies
- **Notion / Confluence** — Documentation and decision records

Check your welcome email for workspace invite links.
