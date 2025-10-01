# COMAP MPhys Project 2025/2026 — Git/GitHub Instructions

**This repository contains code and documentation for the COMAP MPhys project.**

⚠️ **Do not store data files here** — only code, scripts, and documentation.

---

## 1. Install Git
- **Linux and WSL (Ubuntu/Debian):**
  ```bash
  sudo apt update
  sudo apt install git
  ```
- **Mac (Homebrew):**
  ```bash
  brew install git
  ```
- **Windows (not WSL):**
  Download and install from [git-scm.com](git-scm.com)
  Use Git Bash (install with Git).

  Check installation:
  ```bash
  git --version
  ```

## 2. Configure Git
Log in to Harrier. Run these commands once (replace with your own details):
  ```bash
  git config --global user.name "username"
  git config --global user.email "your_email@example.com"
  ```

## 3. Authenticate with GitHub
To push code, you need to connect your computer to GitHub.

1. On GitHub: Settings → Developer settings → Personal access tokens.
2. Generate a Fine-grained token with repo access.
3. Don't forget that you need to generate a token that gives you read and write power.
4. Save the token because you won't be able to see it again.

## 4. Clone the Project (first time only)
Navigate to the folder where you want to keep your MPhys work (e.g. `~/phd/mphys`):
```bash
cd ~/phd/mphys/
git clone https://github.com/gabrielhoerning/comap_mphys_2526.git
```

This creates the folder:
```bash
~/phd/mphys/comap_mphys_2526/
```

## 5. Daily Workflow
0) When you try to pull or push for the first time after a modification, you will need to use your personal token like this:
```bash
git pull https://gabrielhoerning:<TOKEN>@github.com/gabrielhoerning/comap_mphys_2526.git
```
And after that, you can use this command so your local Git should, in principl,e save your credentials so you don't need to use your token every time (but who knows) 
```bash
git config --global credential.helper store
```

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

## 6. Example Session
```bash
cd ~/phd/mphys/comap_mphys_2526
git pull
vi analysis.py    # edit file
git add analysis.py
git commit -m "Added first draft of analysis script"
git push
```

## 7. Good Practices
- Always `git pull` before starting new work.
- Never commit large data files - only code, configs and documentation.
- If unsure, ask before using `git push --force`.

---

## Happy coding! 🚀
