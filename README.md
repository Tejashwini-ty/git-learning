# git-learning
# 📘 Git – What I Learned Today

# 🔹 What is Git?
Git is a distributed version control system used to track changes in source code.

# 🔹 Git Commands I Learned
- `git init` – Initialize a git repository
- `git status` – Check file status
- `git add` – Stage changes
- `git commit` – Save changes
- `git log` – View commit history

# 🔹 Key Learnings
- Git tracks changes locally
- Files must be staged before commit
- Commits represent snapshots of code

📅 Date: 18 Jan 2026

Date 8 Sept 2026
GIT & GITHUB
Definitions, Essential Commands & Interview Questions
1. Git
Git: Git is a version control system (VCS) that tracks changes in code, allowing multiple developers to work together without overwriting each other's work.
Distributed Version Control System (DVCS): A version control system in which every developer has a full copy of the repository, including its history.
Version Control: A system that tracks changes in files over time and allows previous versions to be recalled.
Repository: A project location that stores files and their Git version history.
Commit: A snapshot of the changes made to the code, with a unique ID (hash).
Branch: A separate line of development that allows developers to work on features without affecting the main project.
Merge: The process of combining changes from one branch into another.
2. Version Control Concepts
Version Control System (VCS): Software that manages and records changes to files over time.
Local Version Control: A system that saves different versions on the same computer.
Centralized Version Control (CVCS): A system in which one central server stores all versions and users fetch changes from it. Examples: SVN and Perforce.
Distributed Version Control (DVCS): A system in which every user has a full copy of the repository, making it faster and more reliable. Examples: Git and Mercurial.
Why Version Control is used: To track changes, identify who made changes, restore older versions, collaborate with multiple developers, and work on different features separately.
3. History of Git
History of Git: Git was created by Linus Torvalds in 2005 to manage the Linux kernel source code. It was designed for speed, distributed development, non-linear development through branching and merging, and security/integrity.
•	Before Git, Linux development used BitKeeper.
•	Git was created after the free BitKeeper arrangement for Linux developers ended.
•	Git is open-source and distributed.
•	GitHub is a platform built to host Git repositories and provide collaboration features.
4. Why Git?
Collaboration: Multiple developers can work on the same project.
History: Git records changes so developers can track what changed and when.
Rollback: Previous versions can be restored when required.
Branching: Developers can work on separate features without directly changing the main branch.
Offline work: Most Git operations can be performed locally without an internet connection.
Data integrity: Git uses cryptographic hashing to help detect changes or corruption in repository data.
5. GitHub
GitHub: GitHub is a web-based/cloud platform for hosting Git repositories and providing collaboration features such as pull requests, code review, issues, and GitHub Actions.
Git vs GitHub: Git is the version control tool; GitHub is a platform that hosts Git repositories and adds collaboration features.
Pull Request (PR): A formal request to review and merge changes from one branch or fork into another branch.
Fork: A personal copy of another user's repository under your own GitHub account.
Code Review: The practice of having developers examine proposed changes before they are merged into the main codebase.
GitHub Actions: A GitHub automation feature used to run workflows such as testing, building, and deployment.
6. Essential Git Commands
Command	Definition / Purpose	Syntax
git --version	Checks the installed Git version.	git --version
git config	Sets Git user information used for commits.	git config --global user.name "Your Name"
git init	Initializes a new Git repository and creates the hidden .git directory.	git init
git clone	Creates a copy of a remote repository on the local system, including its history.	git clone <repository_url>
git status	Shows the current state of the working directory and staging area.	git status
git add	Stages changes so they can be included in the next commit.	git add .
git commit	Saves the staged changes as a snapshot in Git history.	git commit -m "message"
git log	Displays commit history.	git log
git branch	Lists, creates, or manages branches.	git branch feature-1
git switch	Switches to another branch.	git switch feature-1
git checkout	Switches to an existing branch; it can also create and switch to a branch.	git checkout feature-1
git merge	Combines changes from one branch into another.	git merge feature-1
git remote -v	Shows configured remote repositories and their URLs.	git remote -v
git push	Uploads local commits to a remote repository.	git push origin main
git pull	Downloads changes from a remote repository and merges them into the current branch.	git pull origin main
git fetch	Downloads remote commits/history without automatically merging them.	git fetch origin
git revert	Creates a new commit that reverses the effect of an earlier commit.	git revert <commit_id>
7. Important Command Workflows
7.1 New Local Project
mkdir my_project
cd my_project
git init
git add .
git commit -m "Initial commit"
7.2 Clone Existing Project
git clone <repository_url>
cd <repository_name>
git status
7.3 Create and Work on a Feature Branch
git switch -c feature-1
git add .
git commit -m "Added feature"
7.4 Push Changes
git remote -v
git push origin feature-1
7.5 Merge Feature into Main
git switch main
git merge feature-1
7.6 Merge Conflict
Merge Conflict: A situation that occurs when two branches modify the same part of a file and Git cannot automatically determine which change to keep.
git status
# Fix the conflicted file
git add <conflicted-file>
git commit -m "Resolved merge conflict"
8. Command-Specific Interview Definitions
git init: Initializes a new Git repository and starts version control in the project directory.
git clone: Creates a local copy of a remote repository, including project files and Git history.
git add: Moves changes to the staging area so they can be included in a commit.
git commit: Creates a snapshot of staged changes and records it in Git history.
git push: Uploads local commits to a remote repository.
git pull: Fetches changes from a remote repository and merges them into the current local branch.
git fetch: Downloads changes from a remote repository without merging them.
git branch: Creates, lists, or manages branches.
git merge: Combines changes from one branch into another.
git revert: Creates a new commit that reverses the changes introduced by an earlier commit.
git reset: Moves the current branch pointer to another commit and can change the staging area and working tree depending on the option used.

 9. Git & GitHub Interview Questions with Short Answers
1. What is Git?
Git is a distributed version control system used to track changes in code and collaborate with multiple developers.
2. Why do we use Git?
To track changes, maintain history, collaborate, create branches, and restore previous versions.
3. What is version control?
Version control is a system that tracks changes in files over time and allows previous versions to be recalled.
4. Why is Git called a distributed VCS?
Because every developer has a full copy of the repository and its history.
5. What is a Git repository?
A repository is the project location containing files and Git version history.
6. What is GitHub?
GitHub is a cloud/web platform used to host Git repositories and support collaboration.
7. What is the difference between Git and GitHub?
Git is the version control tool; GitHub is a platform for hosting Git repositories and collaboration.
8. What does git init do?
It initializes a new Git repository and creates the .git directory.
9. What does git clone do?
It creates a local copy of a remote repository, including its history.
10. What is the difference between git clone and git pull?
git clone creates the repository copy for the first time; git pull gets the latest changes for an already cloned repository.
11. What is git add?
It stages changes for the next commit.
12. What is git commit?
It saves staged changes as a snapshot in Git history.
13. What is the difference between git add and git commit?
git add stages changes; git commit records those staged changes in Git history.
14. What is git push?
It uploads local commits to a remote repository.
15. What is git pull?
It downloads remote changes and merges them into the current branch.
16. What is git fetch?
It downloads remote commits/history without automatically merging them.
17. Difference between git pull and git fetch?
git fetch downloads changes without merging; git pull downloads and merges the changes.
18. What is a branch?
A branch is a separate line of development used to work on changes independently.
19. What does git branch do?
It lists, creates, or manages branches.
20. Does git branch feature-1 switch to the new branch?
No. It creates the branch but does not switch to it.
21. How do you create and switch to a branch in one command?
Use git switch -c feature-1 or git checkout -b feature-1.
22. What is git merge?
It combines changes from one branch into another.
23. How do you merge a feature branch into main?
Switch to main using git switch main, then run git merge feature-1.
24. What is a merge conflict?
It occurs when Git cannot automatically combine changes, commonly because two branches changed the same part of a file.
25. How do you resolve a merge conflict?
Check the conflicted files with git status, manually resolve the file, run git add, and then commit the resolved merge.
26. What is a fast-forward merge?
It occurs when the main branch has no new commits and Git can simply move the branch pointer forward to the feature branch commit.
27. What is a merge commit?
A commit created during a merge that records the merge operation.
28. What is a Pull Request?
A formal request to review and merge changes from one branch or fork into another branch.
29. What is a fork?
A personal copy of another user's repository under your GitHub account.
30. What is code review?
The process of examining proposed code changes before merging them into the main codebase.
31. What is the difference between merge and rebase?
git merge combines branches and preserves their history; rebase replays commits from one branch onto another.
32. How do you check commit history?
Use git log or git log --oneline --graph.
33. How do you undo the latest commit while keeping changes?
Use git reset --soft HEAD~1.
34. How do you undo the latest commit and remove the changes?
Use git reset --hard HEAD~1.
35. How do you safely undo a pushed commit?
Use git revert <commit_id>, which creates a new commit that reverses the earlier commit.
36. What is origin in Git?
origin is the common default name given to the remote repository.
37. How do you check the remote repository?
Use git remote -v.
38. What is .git?
It is the hidden directory that stores Git repository metadata and version-control history.
39. What is .gitignore?
It specifies files and folders that Git should intentionally not track.
40. What is README.md?
It is the repository's main documentation file, normally displayed on the repository's main page.
10. Practical / Scenario Interview Questions
You made code changes locally. What steps do you follow to upload them to GitHub?
git status → git add . → git commit -m "message" → git push origin <branch>.
A developer asks you to work on a new feature without affecting main. What do you do?
Create a separate feature branch, switch to it, make and commit the changes, then push the branch and create a Pull Request.
Your push is rejected because the remote branch has new changes. What do you do?
Fetch or pull the latest remote changes, resolve any conflicts if required, commit the resolution, and push again.
Two developers changed the same lines and a merge conflict occurs. What do you do?
Run git status, open the conflicted file, resolve the conflict, stage the file with git add, and complete the merge with a commit.
You want to review remote changes before merging them. Which command do you use?
git fetch.
You want to get the latest changes and merge them into your current branch. Which command do you use?
git pull.
You accidentally committed a change and want to undo it without rewriting shared history. What do you use?
git revert <commit_id>.
You want to create and immediately switch to a feature branch. What command do you use?
git switch -c feature-1 or git checkout -b feature-1.
A feature is completed and needs to be added to main. What is the basic process?
Switch to main, run git merge <feature-branch>, resolve conflicts if any, and complete the merge.
What is a common GitHub workflow for team development?
Clone or fork → create feature branch → make changes → git add → git commit → git push → Pull Request → code review → merge.
11. One-Minute Revision
•	Git = Version control tool
•	GitHub = Cloud platform for Git repositories
•	init = Start a new Git repository
•	clone = Copy a remote repository locally
•	add = Stage changes
•	commit = Save staged changes in Git history
•	branch = Separate line of development
•	switch/checkout = Move between branches
•	merge = Combine branches
•	fetch = Download remote changes only
•	pull = Download + merge remote changes
•	push = Upload local commits
•	revert = Reverse a commit with a new commit
•	PR = Request review and merge
•	fork = Personal copy of a repository
•	origin = Default remote name
•	.git = Git metadata/history directory
•	.gitignore = Files Git should not track
