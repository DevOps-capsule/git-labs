
# Git Hands-On Lab for Beginners

This beginner-friendly lab introduces the basics of Git: initialization, commits, branches, merges, and pushing to remote repositories. It's designed for self-paced learning with step-by-step instructions.

----------

## Prerequisites

-   Git installed on your system ([Install Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git))
    
-   GitHub or GitLab account (optional but recommended)
    
-   Basic terminal/command line knowledge
----------

## Lab Setup

### Step 1: Create a Project Directory

```bash
mkdir git-lab
cd git-lab
```

### Step 2: Initialize a Git Repository

```bash
git init
```
You now have an empty Git repository.

----------

## Stage 1: Working with Commits

### Step 1: Create a File

```bash
echo "Hello, Git!" > hello.txt
```

### Step 2: Add and Commit the File

```bash
git add hello.txt
git commit -m "Add hello.txt with welcome message"
```

### Step 3: Check History

```bash
git log
```

----------

## Stage 2: Branching and Merging

### Step 1: Create a New Branch

```bash
git checkout -b feature/greet-user
```

### Step 2: Modify the File

```bash
echo "Welcome, user!" >> hello.txt
```

### Step 3: Commit the Changes

```bash
git add hello.txt
git commit -m "Append user greeting to hello.txt"

```

### Step 4: Merge the Branch into Main

```bash
git checkout main
git merge feature/greet-user
```

----------

## Stage 3: Viewing Changes

### Step 1: See Changes Over Time

```bash
git log --oneline --graph
```
----------

## Stage 4: Connecting to a Remote Repository

### Step 1: Create a Repository on GitHub/GitLab

-   Go to GitHub.com or GitLab.com
-   Click "New Repository"
-   Name it `git-lab`
    
### Step 2: Add the Remote URL

```bash
git remote add origin https://github.com/<your-username>/git-lab.git
```

### Step 3: Push Your Code

```bash
git push -u origin main
```

----------

## Stage 5: Cleanup

### Delete Feature Branch (optional)

```bash
git branch -d feature/greet-user
```

----------

## Summary

You’ve just:

-   Initialized a repository
-   Made commits and viewed history
-   Created and merged branches
-   Connected to a remote repo and pushed your code

🎉 Congratulations on completing your first hands-on Git lab!