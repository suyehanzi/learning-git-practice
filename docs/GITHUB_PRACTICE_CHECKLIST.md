# GitHub Practice Checklist

Use this file when you are ready to connect the local repository to GitHub.

## Before Connecting

- Make sure `git status` is clean or the changes are intentional.
- Keep the current branch on `main`.
- Confirm your GitHub account is ready.

## First Connection Steps

```powershell
git remote add origin <your-github-repo-url>
git remote -v
git push -u origin main
```

## Good Small Tests After Push

- Edit `README.md` and push again.
- Add one line to `docs/GITHUB_PRACTICE_CHECKLIST.md`.
- Make a small change in `scripts/hello.py`.
- Run `git log --oneline` before and after each push.

## Pull Practice Idea

After the repository is on GitHub:

1. Edit one file on GitHub.
2. Return to your local terminal.
3. Run `git pull`.
4. Check the updated file locally.
