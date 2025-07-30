Shout-out to Ian Nuttall for his [video tutorial](https://www.youtube.com/watch?v=8dqqa0dLpGU).

---

## Quick Start: Enable Claude Code YOLO Mode Safely in 3 Steps

Want to let Claude Code work autonomously without constant permission requests? Here's how to set it up in just 3 steps:

### Step 1: Install Dev Containers Extension

Install the **Dev Containers** extension in VS Code:

- Open VS Code
- Go to Extensions
- Search for "Dev Containers"
- Install the extension by Anysphere (Note: If you install the Microsoft version, VS Code will prompt you to install the correct version when you open the dev container)

### Step 2: Copy the .devcontainer Configuration

1. Clone the repo [dev-container-for-claude-code-yolo](https://github.com/arealclimber/dev-container-for-claude-code-yolo?tab=readme-ov-file)

```bash
git clone https://github.com/arealclimber/dev-container-for-claude-code-yolo.git
```

2. Copy the appropriate `.devcontainer` folder for your framework:

   - `nextjs/` for Next.js projects
   - `python/` for Python projects

3. Place the `.devcontainer` folder in your project root
4. Open your project in VS Code
5. When prompted, click "Reopen in Container"

### Step 3: Run the Claude command

```bash
claude --dangerously-skip-permissions
```

**That's it!** Claude Code can now work in YOLO mode within the secure container environment.

Important: These configurations are templates. You should customize them based on your specific project needs, including:

1. Port forwarding for your development servers
2. Additional VS Code extensions
3. Environment variables
4. Package installations
5. Security firewall rules
