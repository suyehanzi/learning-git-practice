# Git 学习总结

## 已经练过的内容

- 初始化 Git 仓库
- 配置 `user.name` 和 `user.email`
- 在 PowerShell 中切换目录
- 用 `git status` 查看仓库状态
- 用 `git add` 把改动加入暂存区
- 用 `git commit -m` 创建提交
- 用 `git log --oneline` 查看历史
- 用 `git show` 查看某次提交的细节
- 用 `git restore` 撤回文件改动
- 创建、切换、合并、删除分支

## 核心命令

```powershell
git status
git add .
git commit -m "message"
git log --oneline
git show <commit-id>
git diff
git restore <file>
git restore --staged <file>
git branch
git switch -c <branch-name>
git switch main
git merge <branch-name>
git branch -d <branch-name>
```

## 命令含义

- `git status`：查看当前有哪些变化
- `git add .`：把当前改动放进暂存区
- `git commit -m "message"`：创建一次存档
- `git log --oneline`：查看提交历史
- `git show <commit-id>`：查看某次提交具体改了什么
- `git diff`：查看还没提交的改动
- `git restore <file>`：撤回工作区里某个文件的改动
- `git restore --staged <file>`：把某个文件从暂存区拿出来
- `git switch -c <branch-name>`：创建并切换到新分支
- `git merge <branch-name>`：把某个分支的改动合并回来
- `git branch -d <branch-name>`：删除已经合并的分支

## 日常常用流程

```powershell
git status
git diff
git add .
git commit -m "short description"
git log --oneline
```

## 安全习惯

- 完成一个小而清晰的步骤后就提交一次
- 重要命令前后都看一下 `git status`
- 只想提交部分改动时，用 `git add <file>`，不要直接用 `git add .`
- 做实验时优先开分支，不要直接改 `main`
- 临时分支合并后可以删除，保持仓库整洁

## 这次仓库里的实际体会

- `main` 适合保持稳定
- 分支适合练习和实验
- `git restore` 默认恢复到当前基准，指定旧版本时要用 `--source`
- 真正的存档点是每一次 `commit`

## 下一步可以学什么

- GitHub 远程仓库：`git remote`、`git push`、`git pull`
