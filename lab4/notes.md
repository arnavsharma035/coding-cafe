# Lab 4 Answers

1. `--global` applies settings to all repositories for the current system user. Leaving it out sets configuration only for the current repository.
2. The `.git` folder appeared. It contains all internal Git tracking data, history, hooks, and configuration files.
3. Git offers to track all untracked files in the directory. Files inside virtual environment directories like `.venv/` were not written by me.
4. The `.venv` directory and its contained files disappeared from untracked files after adding `.gitignore`.
5. `.gitignore` should be committed because it ensures everyone working on the repository ignores the same set of files.
6. `README.md` moved from "Untracked files" to "Changes to be committed". It was moved from the working directory to the staging area.
7. Git printed the commit hash and summary, stating 1 file changed (or similar count) with insertions.
8. The first 7 characters are a shortened SHA-1 hash used to uniquely identify that specific commit.
9. The 4-step loop is: Edit file, check status (`git status`), stage (`git add`), and commit (`git commit`).
10. `README.md` is special because GitHub automatically renders it on the repository home page as documentation.
11. `gh auth login` authenticates via OAuth/token, storing credentials securely so Git can authenticate automatically.
12. `README.md` is displayed on the front page because GitHub automatically searches for and renders the main README file.
13. `git push` uploads local commits to GitHub; it does not alter or rewrite local history.
14. A private repository exists online but restricts access to specified users; non-existent repositories do not exist anywhere on GitHub servers.
