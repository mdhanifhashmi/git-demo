
**💻 Git Workflow – Step-by-Step Guide (with Explanations)**

This is a friendly guide to walk through setting up a Git project, pushing it to GitHub, working with branches, and creating a pull request.

---

### ✅ Step 1: Link Local Project to GitHub

**Command:**
```bash
git remote add origin https://github.com/mdhanifhashmi/git-demo.git
```

**What it does:**  
This command connects your local project folder to a GitHub repository. Think of it as telling Git, “Here’s where I want to save my project online.”

---

### ✅ Step 2: Push Initial Code to GitHub

**Command:**
```bash
git push origin master
```

**What it does:**  
This uploads your current code to the `master` branch on GitHub. Now your project lives in the cloud too!

---

### ✅ Step 3: Create a `dev` Branch on GitHub

**How to do it:**
1. Go to your repository on GitHub.
2. Click on the branch dropdown (top left).
3. Type `dev` and hit Enter to create a new branch from `master`.

**Why:**  
It’s a good practice to keep your main (`master` or `main`) branch clean and use `dev` for ongoing development work.

---

### ✅ Step 4: Fetch Branch Info from GitHub

**Command:**
```bash
git fetch
```

**What it does:**  
This tells Git to check GitHub for any new branches or updates. It *doesn't* download the actual code, just the metadata.

---

### ✅ Step 5: Switch to the `dev` Branch Locally

**Command:**
```bash
git switch dev
```

**What it does:**  
Now you’re working on the `dev` branch in your local machine, matching the one on GitHub.

---

### ✅ Step 6: See All Local Branches

**Command:**
```bash
git branch
```

**What it does:**  
This lists all the branches that exist in your local repository. Useful to confirm that you’re on the right branch.

---

### ✅ Step 7: Create a New Feature Branch

**Command:**
```bash
git branch feature/user-registration
```

**What it does:**  
This creates a new branch where you can work on a specific feature — in this case, “user registration.” It's like a separate workbench.

---

### ✅ Step 8: Switch to the New Feature Branch

**Command:**
```bash
git switch feature/user-registration
```

**What it does:**  
Now you’re working inside your new branch. You’re free to make changes without affecting the `dev` or `master` branches.

---

### ✅ Step 9: Make Code Changes

Do your development work now — for example, create new files, write code, or make updates.

---

### ✅ Step 10: Save Your Changes (Commit)

**Command:**
```bash
git commit -am "Added user registration feature"
```

**What it does:**  
This saves all the changes with a commit message. Think of it as creating a restore point with a label.

---

### ✅ Step 11: Check Commit History

**Command:**
```bash
git log --oneline
```

**What it does:**  
This shows a quick list of all the commits you’ve made. Helpful to track your work.

---

### ✅ Step 12: Push Feature Branch to GitHub

**Command:**
```bash
git push origin feature/user-registration
```

**What it does:**  
Sends your new branch (with your code changes) to GitHub. Now your work is on the cloud, but not yet merged with the `dev` branch.

---

### ✅ Step 13: Create a Pull Request on GitHub

**How to do it:**
1. Go to your repository on GitHub.
2. Click the **Pull requests** tab.
3. Click the **New pull request** button.
4. Set the base branch to `dev` and the compare branch to `feature/user-registration`.
5. Add a title and description (what you changed, why).
6. Click **Create Pull Request**.

**Why:**  
This is how you request to merge your changes into the development branch. Others can review your code, or you can review it yourself before merging.
