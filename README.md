# git-practice
练习git命令

fix: 修改

## 练习命令
> 后面生成todo选项
---
### git diff
- 工作区 和 index 的差异
- index 和 版本库 的差异
- working tree 和 版本库 的差异
- 两个提交中某个文件的差异
- 某分支与主分支的差异（从主分支切出去后）

### git merge
- 新建分支，然后将该分支合并到主分支，保留合并历史
- 新建分支，在同一文件上，主分支和新分支都做处理，然后尝试合并策略进行合并
- 中止合并


### git switch
- 新建分支
- 切换分支
- 基于 commit 创建分支
- 仅查看某 commit 的内容

### git restore
- 恢复 working tree
- 恢复 index
- 恢复 working tree + index
- 从 commit 恢复 文件

### git reset
> commit 未提交
- 回退 HEAD^2，保留commit到index
- 回退 HEAD^2，保留commit到working tree
- 回退 HEAD^2，不保留

### git revert
> 一般用于commit 已经 push到远程
- 撤销单个提交
- 撤销多个提交
- 撤销合并提交

### git chery-pick
> 用于pick一个或多个提交
- pick单个提交，
- pick多个提交，(] []，
- 参数 --no-commit, --edit, --signoff, --continue, --abort, --x

