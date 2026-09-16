# Developer Handbook

## Overview

This handbook is my personal developer reference.

Goals:

- Learn modern software development workflows
- Become proficient with Linux and WSL
- Master Git and GitHub
- Build Python and AI applications
- Create good markdown files
- Learn Docker and containers
- Develop Edge AI and TinyML systems
- Create reusable reference material

---

# Part 1 - Development Environment

## Linux / WSL

### Common Commands

| Task | Command | Description |
|--------|---------|-------------|
| Current Directory | `pwd` | Show current path |
| List Files | `ls -la` | List files |
| Change Directory | `cd folder` | Navigate |
| Create Directory | `mkdir dir` | Create folder |
| Delete Directory | `rm -rf dir` | Remove folder tree |
| Open VS Code | `code .` | Open current folder |

### Useful WSL Commands

```bash
wsl --version
wsl --shutdown
```

### Notes

- WSL gives a full Linux environment inside Windows.
- Most AI tooling works best in WSL.

---

## VS Code

### Essential Shortcuts

| Task | Shortcut |
|--------|----------|
| Command Palette | Ctrl+Shift+P |
| Quick Open | Ctrl+P |
| Terminal | Ctrl+` |
| Source Control | Ctrl+Shift+G |
| Extensions | Ctrl+Shift+X |
| Explorer | Ctrl+Shift+E |
| Debug | F5 |

### Notes

- VS Code is the primary development environment.
- Use Remote WSL whenever possible.

---

# Part 2 - Git & GitHub

## Daily Workflow

```bash
git pull

git status

git add .

git commit -m "Description"

git push
```

## Essential Commands

```bash
git status

git add .

git commit -m "message"

git push

git pull

git diff

git log --oneline

git branch

git switch -c branch-name

git merge branch-name
```

## Branch Workflow

Create:

```bash
git switch -c feature-name
```

Switch:

```bash
git switch master
```

Merge:

```bash
git merge feature-name
```

## Notes

- `master` = local branch
- `origin/master` = GitHub branch

---

# Part 3 - Python

## Virtual Environments

### Create

```bash
python3 -m venv .venv
```

### Activate

```bash
source .venv/bin/activate
```

### Deactivate

```bash
deactivate
```

## Package Management

Install:

```bash
pip install package-name
```

List:

```bash
pip list
```

Save dependencies:

```bash
pip freeze > requirements.txt
```

Restore dependencies:

```bash
pip install -r requirements.txt
```

## Notes

- Every project gets its own `.venv`
- Never commit `.venv`

---

## requirements.txt

Generate:

```bash
pip freeze > requirements.txt
```

Install:

```bash
pip install -r requirements.txt
```

Example:

```text
numpy==2.3.3
pandas==2.3.2
matplotlib==3.10.6
```
---

## Markdown Document Creation

Markdown is the standard documentation format used by:

- GitHub
- README files
- Project documentation
- Developer handbooks
- AI project notes
- GitHub Wikis

### Create a Markdown File

Create an empty file:

```bash
touch notes.md
```

Create and open in VS Code:

```bash
code notes.md
```

Create and edit with nano:

```bash
nano notes.md
```

---

### Common Markdown Files

| File | Purpose |
|--------|---------|
| `README.md` | Project documentation |
| `handbook.md` | Personal knowledge base |
| `cheatsheets.md` | Quick reference material |
| `CHANGELOG.md` | Release history |
| `CONTRIBUTING.md` | Contribution guidelines |
| `NOTES.md` | General notes |

---

### Headings

```markdown
# Heading 1

## Heading 2

### Heading 3

#### Heading 4
```

---

### Bold and Italics

```markdown
**Bold**

*Italic*

***Bold Italic***
```

---

### Lists

Unordered list:

```markdown
- Item 1
- Item 2
- Item 3
```

Ordered list:

```markdown
1. First
2. Second
3. Third
```

---

### Task Lists

Useful for learning plans:

```markdown
- [x] Git
- [x] Python
- [ ] Docker Compose
- [ ] CUDA
- [ ] Kubernetes
```

---

### Code Blocks

Inline code:

```markdown
Use `git status`
```

Multi-line code:

````markdown
```bash
git status
git add .
git commit -m "update"
```
---

# Part 4 - Docker

## Core Concept

```text
Image = Template

Container = Running instance
```

## Essential Commands

Check Docker:

```bash
docker --version
```

Images:

```bash
docker images
```

Containers:

```bash
docker ps -a
```

Run:

```bash
docker run image
```

Interactive shell:

```bash
docker run -it ubuntu bash
```

Build:

```bash
docker build -t myapp .
```

Logs:

```bash
docker logs ID
```

Enter container:

```bash
docker exec -it ID bash
```

---

# Part 5 - AI Development

## CUDA

### Notes

(To be added)

---

## PyTorch

### Notes

(To be added)

---

## Ollama

### Notes

(To be added)

---

# Part 6 - Edge AI

## Raspberry Pi

### Notes

(To be added)

---

## TinyML

### Notes

(To be added)

---

## TensorRT

### Notes

(To be added)

---

# Project Templates

## Python Project

```text
project/
│
├── .venv/
├── requirements.txt
├── README.md
├── main.py
├── .gitignore
└── tests/
```

## AI Project

```text
project/
│
├── data/
├── models/
├── notebooks/
├── src/
├── requirements.txt
└── README.md
```

---

# Learning Log

## Topics Learned

- [x] Git basics
- [x] Git branches
- [x] GitHub repositories
- [x] Python virtual environments
- [x] Requirements files
- [x] Docker basics
- [x] VS Code Source Control

## Topics To Learn

- [ ] GitHub Pull Requests
- [ ] Docker Compose
- [ ] CUDA
- [ ] PyTorch
- [ ] Ollama
- [ ] TensorRT
- [ ] TinyML
- [ ] Kubernetes