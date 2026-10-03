1. The --global option makes the Git configuration apply to all repositories for my user account. Without --global, the configuration applies only to the current repository.

2. Running ls -a reveals the hidden .git directory, which does not appear with a normal ls command. The .git directory contains Git's internal data, configuration, and history for the repository.

3. Git offers roughly hundreds of files inside the .venv/ folder to track. Most of these files were created automatically by the Python virtual environment rather than written by me, so they should not be tracked by Git.

4. After creating .gitignore, the .venv/ files disappeared from the git status output. Git now shows only .gitignore as an untracked file because the .gitignore rules tell Git to ignore the virtual environment.

5. Yes, .gitignore should be committed because it contains the rules that tell Git which files and folders to ignore. Committing it ensures that other people working on the project use the same ignore rules.

6. README.md moved from the "Untracked files" section to "Changes to be committed." This demonstrates Git's three-place model: the file moved from the working directory into the staging area, ready to be included in the next commit.

7. Git printed the commit information, including the commit hash 6ca9ae2, the commit message "Lab work so far," and a summary showing that 2 files changed. It also showed that .gitignore and README.md were created.

8. The first seven characters of the commit hash, such as 6ca9ae2, are an abbreviated version of the commit's unique hash. They provide a convenient way to identify and refer to that specific commit.
