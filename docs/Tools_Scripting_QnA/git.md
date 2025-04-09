# 📚 GIT 

### 🚗💻 **Git – What, When, Where, Why, How, and Benefits**
<a class="back-sidebar-btn" href="javascript:history.back()">⬅️ Back</a>

---

### 🔍 **What is Git?**
Git is a **distributed version control system** used to track changes in source code during software development.  
It helps teams collaborate, manage versions, and keep history of code changes.

---

### 🕒 **When do we use Git?**
- During **development of software/code/models**  
- While working in **collaborative teams**
- When maintaining **multiple versions/branches** of a project  
- While reviewing or rolling back to previous states  
- In **CI/CD pipelines**, testing and release cycles

---

### 🌍 **Where is Git used?**
- Across **software and automotive domains**  
- In **Model-Based Development (MBD)** to version models, scripts, and configs  
- Inside **Simulink/Embedded C projects**  
- Integrated with **GitHub, GitLab, Bitbucket** and other repositories  
- In **DevOps pipelines**, Jenkins, Azure, etc.

---

### ❓ **Why do we use Git?**
- To **track every code/model change**
- To enable **team collaboration without conflict**
- To **manage different versions** and branches (e.g., dev, test, release)
- To **revert mistakes**, compare differences
- For **safe and traceable delivery pipelines**

---

### ⚙️ **How do we use Git? (Common Commands)**
- `git init` – Start a new Git repo  
- `git clone <repo-url>` – Copy a remote repo  
- `git status` – See changes made  
- `git add <file>` – Stage changes  
- `git commit -m "message"` – Commit changes  
- `git push` – Upload to remote repo  
- `git pull` – Download latest changes  
- `git branch` – View or create branches  
- `git merge` – Merge branches  
- `git log` – View commit history  

---

### ✨ **Benefits of Git**
- ✅ Full history and traceability  
- ✅ Safe experimentation with branches  
- ✅ Collaborative development with conflict resolution  
- ✅ Easy rollback to previous versions  
- ✅ Integrates with **JIRA**, **CI/CD**, and **Quality Gates**  
- ✅ Supports **automotive V-model workflows** and traceable deliveries  
- ✅ Powerful when integrated with versioning tools in **MagicDraw**, **Preevision**, or **Simulink Projects**

---

### **Git Interview Questions and Answers**

---

**1. What is Git?**  
   Git is a distributed version control system used for tracking changes in code and collaborating across teams.

**2. What is the difference between Git and GitHub?**  
   Git is the tool (VCS), GitHub is a web-based platform for hosting Git repositories.

**3. What does `git init` do?**  
   Initializes a new Git repository in your project folder.

**4. What is `git clone`?**  
   Copies a remote repository to your local machine.

**5. What is the use of `git add`?**  
   Stages changes to be included in the next commit.

**6. What does `git commit` do?**  
   Saves the staged changes with a message to the local repo.

**7. What is `git push`?**  
   Uploads local commits to a remote repository.

**8. What is `git pull`?**  
   Fetches and merges changes from remote to local branch.

**9. What is a Git branch?**  
   A parallel version of the repository used to develop features independently.

**10. How do you create a new branch?**  
    `git branch feature_name`

**11. How do you switch branches?**  
    `git checkout feature_name`

**12. How to merge branches?**  
    Switch to the target branch and use `git merge source_branch`.

**13. What is a conflict in Git?**  
    A conflict occurs when two changes affect the same line in a file during merge.

**14. How do you resolve merge conflicts?**  
    Manually edit the files, then `git add` and `git commit`.

**15. What is `git status`?**  
    Shows current branch, staged/unstaged changes, and untracked files.

**16. What is `git log`?**  
    Displays commit history.

**17. What is `git stash`?**  
    Temporarily stores uncommitted changes to revert to a clean working state.

**18. What is `git rebase`?**  
    Moves or combines commits to a new base commit (linear history).

**19. Difference between `merge` and `rebase`?**  
    `merge` keeps history with a new merge commit; `rebase` rewrites commit history linearly.

**20. What is `HEAD` in Git?**  
    Refers to the current commit your branch is pointing to.

**21. What is a remote repository?**  
    A shared Git repository typically hosted on GitHub/GitLab for collaboration.

**22. How do you remove a file from Git?**  
    `git rm file_name` and then commit.

**23. How to undo the last commit?**  
    `git reset --soft HEAD~1` (keeps changes),  
    `git reset --hard HEAD~1` (discards changes).

**24. What is `.gitignore`?**  
    A file listing paths Git should ignore (e.g., build folders, logs).

**25. What is `git fetch`?**  
    Downloads changes from remote without merging.

**26. Difference between `git fetch` and `git pull`?**  
    `fetch` only downloads, `pull` downloads + merges.

**27. How to delete a branch?**  
    `git branch -d branch_name` (local),  
    `git push origin --delete branch_name` (remote).

**28. What is a tag in Git?**  
    A marker for a specific commit (often used for releases).

**29. How to create a tag?**  
    `git tag v1.0`

**30. How to push a tag?**  
    `git push origin v1.0`

**31. How do you see differences between commits?**  
    `git diff commit1 commit2`

**32. What is `git cherry-pick`?**  
    Apply a specific commit from one branch to another.

**33. How can Git be used in the automotive industry?**  
    For versioning models, code, configuration files, and traceability in ASPICE/SOTIF pipelines.

**34. What are hooks in Git?**  
    Scripts triggered by Git actions like commit or push.

**35. How to recover a deleted commit?**  
    Use `git reflog` to find and reset to the commit.

**36. How do you track a file in Git?**  
    Use `git add` followed by a commit.

**37. What is a detached HEAD?**  
    You’re not on a branch, but a specific commit.

**38. How to create a Git alias?**  
    `git config --global alias.co checkout`

**39. What is `origin` in Git?**  
    Default name for a remote repo when you clone.

**40. How to see the commit author history?**  
    `git log --pretty=format:"%h %an %s"`

**41. How do you use Git with JIRA?**  
    By linking commits with JIRA ticket IDs in messages.

**42. How do you ensure quality in Git commits?**  
    Follow commit message conventions and code reviews.

**43. What are submodules in Git?**  
    Repositories embedded in another Git repo.

**44. How to revert a commit?**  
    `git revert commit_id` — creates a new commit undoing the change.

**45. What is Git flow?**  
    A branching model with main, develop, feature, release, and hotfix branches.

**46. How to squash commits?**  
    Use interactive rebase: `git rebase -i HEAD~n`

**47. Why is Git important in team projects?**  
    Enables parallel development, traceability, and safe collaboration.

**48. How do you test before pushing?**  
    Use `git stash` and run tests, or use Git hooks for pre-push validation.

**49. What is `git clean`?**  
    Deletes untracked files: `git clean -f`

**50. How do you create a patch file?**  
    `git format-patch -1` creates a patch for the last commit.