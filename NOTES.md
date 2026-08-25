# Git 速查笔记

## 日常操作
```bash
git status                  # 查看状态
git switch -c feat-x        # 新建并切换分支
git add -A && git commit -m "feat: xxx"
git push -u origin feat-x   # 推送新分支
```

## PR 流程
```bash
gh pr create --base main --head feat-x --title "feat: xxx" --body "描述"
gh pr merge --merge --delete-branch
```

## 常见翻车抢救
```bash
git restore <file>          # 撤销工作区改动
git reset --soft HEAD~1     # 撤销上次 commit，保留改动
git rebase -i HEAD~3        # 交互式整理最近 3 个提交
```
