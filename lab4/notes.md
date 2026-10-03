Here are clear, concise answers (2–3 sentences each) for your lab4/notes.md file based on the lab context:

Question 1: Meaning of --global in git config and omitting it
The --global flag applies the configuration settings across all Git repositories for your system user account. If you omit it, the configuration applies only to the current local repository you are working in.

Question 2: Contents of .git revealed by ls -a
Running ls -a reveals the hidden .git directory inside your project folder. This folder contains all of Git's underlying metadata, object databases, configuration settings, branch pointers, and historical commit logs for the repository.

Question 3: Approximate untracked file count and identifying untracked code
Git offers to track thousands of untracked files (around 2,000+ files). The code you did not write comes from the .venv/ directory, which contains Python's virtual environment dependencies and third-party library files.

Question 4: Difference in git status after creating .gitignore
After creating the .gitignore file, the thousands of files inside .venv/, __pycache__/, and other ignored rules disappeared from the untracked files list. Only .gitignore and your project files remain visible to Git.

Question 5: Why .gitignore itself should be committed rather than ignored
The .gitignore file must be committed so that its rules are tracked and shared across the entire team and repository. This ensures everyone collaborating on the project automatically ignores the exact same temporary and generated files.

Question 6: Movement of README.md across sections in git status (three-places model)
README.md moved from the "Untracked files" section to the "Changes to be committed" section. In the three-places model, running git add moved the file from your Working Directory into the Staging Area (Index).

Question 7: Output produced by git commit and count of changed files
Git outputs the root commit hash, branch name (main), commit message, and summary statistics about the commit. It shows that 1 file changed (or more depending on what you staged) with insertions for the file contents.

Question 8: Name and purpose of the first seven characters of a commit hash
The first seven characters are called the short commit hash (or short SHA-1 checksum). They act as a unique, abbreviated identifier for that specific commit snapshot in the repository's history.

Question 9: The 4 steps of the repetitive Git loop
Edit: Modify or create files in your working directory.

Status: Run git status to check modified and untracked files.

Stage: Run git add <file> to move changes to the staging area.

Commit: Run git commit -m "message" to save a snapshot to repository history.

Question 10: Special purpose and placement of README.md
README.md is placed in the root directory of a repository to serve as the main introduction and documentation for the project. Git platforms like GitHub automatically detect and render this file on the repository's main landing page for visitors to read.

Question 11: How gh auth login eliminates future password prompts
gh auth login authenticates your machine with GitHub via web browser OAuth or SSH/Personal Access Tokens and saves a secure credential token locally. Git uses this token automatically for future network operations like git push, eliminating the need for password entries.

Question 12: File rendered on GitHub's front page and the reason why
The README.md file in the root directory is rendered on the front page. GitHub is designed to automatically display root Markdown files named README to give users immediate context and documentation about the project.

Question 13: Effect of git push on local history
Running git push does not alter or modify your local commit history at all. It simply uploads your existing local commits and refs to the remote repository so both histories match.

Question 14: Distinction between a private repository vs. no repository on GitHub
A private repository exists on GitHub's servers with full version history, but access is restricted exclusively to the owner and explicitly added collaborators. A non-existent repository does not exist on GitHub at all, meaning no remote cloud backup or collaboration permissions exist anywhere online.
