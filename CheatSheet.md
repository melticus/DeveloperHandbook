# Cheat Sheets Appendix

## Git & GitHub Cheat Sheet

| Task | CLI Command | VS Code GUI |
|--------|---------|---------|
| Status | `git status` | Source Control |
| Add All | `git add .` | Stage All Changes |
| Commit | `git commit -m "msg"` | Commit ✓ |
| Push | `git push` | Sync Changes |
| Pull | `git pull` | Pull |
| Diff | `git diff` | Open changed file |
| Create Branch | `git switch -c branch` | Create New Branch |
| Switch Branch | `git switch branch` | Select Branch |
| Merge | `git merge branch` | Merge Branch |

---

## Python venv Cheat Sheet

| Task | CLI Command | VS Code GUI |
|--------|---------|---------|
| Create | `python3 -m venv .venv` | Python: Create Environment |
| Activate | `source .venv/bin/activate` | Select Interpreter |
| Deactivate | `deactivate` | Change Interpreter |
| Install | `pip install package` | Terminal |
| List | `pip list` | Python Environment Panel |
| Save Requirements | `pip freeze > requirements.txt` | Terminal |
| Restore | `pip install -r requirements.txt` | Terminal |

---

## Linux & WSL Cheat Sheet

| Task | Command | Description |
|--------|---------|---------|
| Current Directory | `pwd` | Show current path |
| List Files | `ls -la` | List all files |
| Change Directory | `cd folder` | Navigate |
| Create Directory | `mkdir dir` | Create folder |
| Copy | `cp source dest` | Copy file |
| Move/Rename | `mv old new` | Move or rename |
| Delete File | `rm file` | Remove file |
| Delete Folder | `rm -rf dir` | Remove directory tree |
| Find Files | `find . -name "*.py"` | Locate files |
| Open VS Code | `code .` | Open current folder |
| WSL Version | `wsl --version` | Check WSL |
| Restart WSL | `wsl --shutdown` | Restart WSL |

---

## Docker Cheat Sheet

| Task | Command | Purpose |
|--------|---------|---------|
| Version | `docker --version` | Verify install |
| Images | `docker images` | List images |
| Containers | `docker ps -a` | List containers |
| Run | `docker run image` | Start container |
| Interactive Shell | `docker run -it ubuntu bash` | Shell access |
| Stop | `docker stop ID` | Stop container |
| Remove Container | `docker rm ID` | Delete container |
| Remove Image | `docker rmi IMAGE` | Delete image |
| Build | `docker build -t myapp .` | Build image |
| Logs | `docker logs ID` | View output |
| Exec | `docker exec -it ID bash` | Enter container |
| Compose Up | `docker compose up -d` | Start stack |
| Compose Down | `docker compose down` | Stop stack |

### Key Concept

```text
Image = Template

Container = Running instance of the image
```

---

## VS Code Shortcuts & Productivity

| Task | Shortcut | Purpose |
|--------|---------|---------|
| Command Palette | `Ctrl+Shift+P` | Access commands |
| Quick Open | `Ctrl+P` | Open files |
| Integrated Terminal | `Ctrl+\`` | Toggle terminal |
| Find in File | `Ctrl+F` | Search current file |
| Replace | `Ctrl+H` | Replace text |
| Global Search | `Ctrl+Shift+F` | Search workspace |
| Source Control | `Ctrl+Shift+G` | Open Git panel |
| Extensions | `Ctrl+Shift+X` | Manage extensions |
| Explorer | `Ctrl+Shift+E` | File explorer |
| Run & Debug | `F5` | Start debugging |
| Multi Cursor | `Alt+Click` | Edit multiple locations |
| Comment Line | `Ctrl+/` | Toggle comment |
| Format Document | `Shift+Alt+F` | Auto format |
| Open WSL Folder | `code .` | Open WSL project |

---

## Edge AI Developer Stack

```text
Linux / WSL
    ↓
Git + GitHub
    ↓
Python + venv
    ↓
Docker
    ↓
VS Code
    ↓
CUDA / PyTorch
    ↓
Edge AI / TinyML
```
``