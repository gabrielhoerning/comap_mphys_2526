# COMAP MPhys Project 2025/2026 — Git/GitHub Instructions

This repository contains code and documentation for the COMAP MPhys project.  
⚠️ **Do not store data files here** — only code, scripts, and documentation.

---

## 1. Install Git
- **Linux (Ubuntu/Debian):**
  ```bash
  sudo apt update
  sudo apt install git
  ```
- **Mac (Homebrew):**
  ```bash
  brew install git
  ```
- **Windows:**
  Download and install from git-scm.com
  Use Git Bash (install with Git).

  Check installation:
  ```bash
  git --version
  ```

## 2. Configure Git
Run these commands once (replace with your own details):
  ```bash
  git config --global user.name "Your Name"
  git config --global user.email "your_email@example.com"
  ```

## 3. Authenticate with GitHub
To push code, you need to connect your computer to GitHub.

1. On GitHub: Settings → Developer settings → Personal access tokens.
2. Generate a Fine-grained token with repo access.
3. When Git asks for a password after git push, paste the token.

## 4. Clone the Project (first time only)
Navigate to the folder where you want to keep your MPhys work, e.g.,
```bash
cd ~/phd/mphys/
git clone https://github.com/gabrielhoerning/comap_mphys_2526.git
```

This creates the folder:
```bash
~/phd/mphys/comap_mphys_2526/
```

## 5. Daily Workflow
a) Update your local copy
```bash
cd ~/phd/mphys/comap_mphys_2526
git pull
```

b) Add or edit files
Work on your scripts, notes, or code.

c) See what changed
```bash
git status
```

d) Stage files
```bash
git add my_code.py
# or all files
git add .
```

e) Commit changes
```bash
git commit -m "Short description of changes"
```

f) Push to GitHub
```bash
git push
```
