# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a single-file browser game project. All code lives in standalone `.html` files — no build step, no dependencies, no package manager.

## Running the Game

Open any `.html` file directly in a browser. On Windows:

```bash
cmd.exe /c start "" "tictactoe.html"
```

## Architecture

Each project is a self-contained `.html` file with inline `<style>` and `<script>` blocks. There is no bundler, framework, or external dependency. JavaScript is vanilla ES6+.

## GitHub Workflow

Every new project gets its own GitHub repository. Standard workflow:

```bash
git init
git add <file>
git commit -m "Initial commit: <description>"
gh repo create <repo-name> --public --source=. --remote=origin --push
```

For subsequent changes:

```bash
git add <file>
git commit -m "<clean description of change>"
git push
```

GitHub account: `guysalm`
