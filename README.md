# git-practice
练习git命令

fix: 修改

feat: 练习的时候总结命令的用法和使用范围，还有相近的操作有哪些
feat: 先确定练习的命令会有什么结果，对比加深印象

## 练习命令
> 后面生成todo选项
---

### git 基础命令
- 日志查看，自定义alias的三种
- 查看所有branch(本地，远程，本地+远程，本地与远程关系)
- 追加commit
- 删除文件
- 存储工作区
- 推送并指定本地与远程分支的跟踪关系


### git diff
- 工作区 和 index 的差异
- index 和 版本库 的差异
- working tree 和 版本库 的差异
- 两个提交中某个文件的差异
- 某分支与主分支的差异（从主分支切出去后）
- 分析两个提交上某个文件的区别 git diff commit1:file commit2:file


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

### git reflog
- 查找被删掉的commit
- 查找被删掉的branch
- 回到rebase前
- 回到两天前

### git rebase
- 将branchA的代码合并到branchB
- 整理提交记录，保持线性，在非主线、非公共分支上执行

