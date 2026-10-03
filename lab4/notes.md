1. The --global option makes the Git configuration apply to all repositories for my user account. Without --global, the configuration applies only to the current repository.

2. Running ls -a reveals the hidden .git directory, which does not appear with a normal ls command. The .git directory contains Git's internal data, configuration, and history for the repository.

3. Git offers roughly hundreds of files inside the .venv/ folder to track. Most of these files were created automatically by the Python virtual environment rather than written by me, so they should not be tracked by Git.

4. After creating .gitignore, the .venv/ files disappeared from the git status output. Git now shows only .gitignore as an untracked file because the .gitignore rules tell Git to ignore the virtual environment.

5. Yes, .gitignore should be committed because it contains the rules that tell Git which files and folders to ignore. Committing it ensures that other people working on the project use the same ignore rules.

6. README.md moved from the "Untracked files" section to "Changes to be committed." This demonstrates Git's three-place model: the file moved from the working directory into the staging area, ready to be included in the next commit.

7. Git printed the commit information, including the commit hash 6ca9ae2, the commit message "Lab work so far," and a summary showing that 2 files changed. It also showed that .gitignore and README.md were created.

8. The first seven characters of the commit hash, such as 6ca9ae2, are an abbreviated version of the commit's unique hash. They provide a convenient way to identify and refer to that specific commit.

9. The four steps of the repetitive Git loop are edit, stage, commit, and repeat. In this lab, I edited lab4/notes.md, staged it with git add, committed it with git commit, and repeated the process when editing README.md.

10. README.md has a special purpose because GitHub automatically displays it on the repository's front page. It should be placed in the root directory of the repository so GitHub can find and render it automatically.

11. gh auth login authenticates my GitHub account and stores the credentials used by GitHub CLI. This allows Git operations such as git push to authenticate with GitHub without repeatedly asking for my password.

12. README.md is rendered on the front page of a GitHub repository. GitHub does this because README.md is conventionally used to provide an introduction and information about the project.

13. git push copies commits from the local repository to the remote GitHub repository. It does not change the commit history in the local repository.

14. A private GitHub repository is hosted on GitHub but can only be accessed by people who have been given permission. If there is no GitHub repository, the project is not hosted on GitHub and remains only in the local repository.
