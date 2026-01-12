# Git Large File Storage (LFS)

This project is designed to teach you how to handle large files in Git without bloating your repository size or slowing down your workflow. Suppose you have a file that exceeds 100mb. In this case your file will get slower or may not be pushed into git repo. As a solution we have Git LfS for this problem.

---

## 🧠 What is Git LFS?

Standard Git stores the entire history of every file. If you change a 100MB video ten times, your repo becomes 1GB. **Git LFS** solves this by:
1.  Replacing the large file in Git with a tiny **Pointer File**.
2.  Storing the actual data in a dedicated **LFS Cache** on the server.
3.  Downloading the real file only when you "check out" that specific version.



---
### 1. Installation
Before you can interact with LFS files, you must install the extension locally:
* **Install:** `git lfs install` (Run this once per machine).

### 2. Tracking Files (The "Teaching" Part)
To tell Git which files should be handled by LFS, use the `track` command. This creates/updates a `.gitattributes` file.

```bash
# Track all .psd files
git lfs track "*.psd"

# Track a specific large video
git lfs track "assets/intro_video.mp4"
````
# The Workflow
````bash
Once tracked, you use Git exactly as you normally would:

    git add .gitattributes (Crucial: Always commit this!)

    git add my_large_file.psd

    git commit -m "Add design assets"

    git push origin main
````

# ⚠️ Common Pitfalls to Avoid
 - Forgetting to commit .gitattributes: If you don't commit this file, your teammates will download the large files as "raw" Git objects, potentially breaking the repo.
 
 - Tracking files too late: If you commit a 500MB file to regular Git first and then try to track it with LFS, that 500MB stays in your Git history forever. 
 
 - You would need to use git lfs migrate to fix the history.
 Bandwidth Limits: Remember that GitHub/GitLab often have "Bandwidth Quotas" for LFS downloads.

 Now after this you will be able to work with large files too .
 
 [<<Back to Previous Page](./SpecialGithubFiles.md)