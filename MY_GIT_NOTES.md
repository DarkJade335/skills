# 我的 Git 学习笔记

**作者：** DarkJade335
**日期：** 2026-05-15

## 今天学到了什么

- `git clone` —— 把远程仓库**完整下载**（含历史和所有分支）到本地
- `git status` —— 任何时候不知道"我在哪、改了啥"，先敲它
- `git branch -a` —— 看所有分支（本地 + 远程）
- `git log --oneline -10` —— 看最近 10 个 commit
- `git remote -v` —— 看远程地址别名
- `git checkout -b <name>` —— 创建并切换到新分支
- **Fork** vs **Clone**：
  - Fork 是在 **GitHub 服务器**上复制一份属于自己的仓库
  - Clone 是把**远程仓库下载到本地**

## 标准开源协作流程

```
原仓库 (upstream)  ← Fork →  我的副本 (origin)
                                  ↓ Clone
                              本地仓库
                                  ↓ 改动
                                  ↓ commit
                                  ↓ push
                              我的副本 (origin)
                                  ↓ 发起 Pull Request
                              原仓库 (upstream)
```

## 远程命名约定

- `origin` = 我自己的 fork
- `upstream` = 原仓库
