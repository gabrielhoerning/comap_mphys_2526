# COMAP MPhys Project 2025/2026 — Git/GitHub Instructions

This repository contains code and documentation for the COMAP MPhys project.  
⚠️ **Do not store data files here** — only code, scripts, and documentation.

---

## 1. Install Git
- **Linux (Ubuntu/Debian):**
  ```bash
  sudo apt update
  sudo apt install git
- **Mac (Homebrew):**
  ```bash
  brew install git
- **Windows:**
  Download and install from git-scm.com
  Use Git Bash (install with Git).

  Check installation:
  ```bash
  git --version

## 2. Configure Git
Run these commands once (replace with your own details):
```bash
git config --global user.name "Your Name"
git config --global user.email "your_email@example.com"

## 3. Authenticate with GitHub
You need to connect your computer to GitHub to push code.

Option A: HTTPS + Personal Access Token
On GitHub: Settings → Developer settings → Personal access tokens.
Generate a Fine-grained token with repo access.
When Git asks for a password after git push, paste the token.

