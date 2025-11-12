# Step-by-Step Guide: Upload Project to GitHub

## Prerequisites
- GitHub account (create one at https://github.com if you don't have it)
- Git installed on your computer (check with `git --version`)

## Step 1: Initialize Git Repository (if not already done)
```bash
git init
```

## Step 2: Add All Files to Git
```bash
git add .
```

## Step 3: Create Initial Commit
```bash
git commit -m "Initial commit"
```

## Step 4: Create a New Repository on GitHub
1. Go to https://github.com and sign in
2. Click the "+" icon in the top right corner
3. Select "New repository"
4. Choose a repository name (e.g., "finalecom")
5. Choose public or private
6. **DO NOT** initialize with README, .gitignore, or license (since we already have these)
7. Click "Create repository"

## Step 5: Connect Local Repository to GitHub

**Where to run these commands:**
- Open your terminal/command prompt
- Navigate to your project directory: `/Users/daniela/Documents/Appdev1/Appdev2/finalecom`
- Or if you're in VS Code, open the integrated terminal (Terminal → New Terminal)
- Make sure you're in the project folder

After creating the repository, GitHub will show you commands. Use these:
```bash
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
git branch -M main
git push -u origin main
```

**Important:** Replace `YOUR_USERNAME` and `YOUR_REPO_NAME` with your actual GitHub username and repository name.

**Example:** If your username is `daniela123` and repository name is `finalecom`, the command would be:
```bash
git remote add origin https://github.com/daniela123/finalecom.git
```

## Step 6: Push Your Code
```bash
git push -u origin main
```

## Authentication
- If prompted for username/password, use a Personal Access Token (not your GitHub password)
- To create a token: GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic) → Generate new token
- Give it "repo" permissions
- Copy the token and use it as your password when pushing

---

## Quick Command Summary
```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
git branch -M main
git push -u origin main
```

