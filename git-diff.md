> 记录 git diff 用法

```
直接用 git diff 没有显示差异信息，
现在commit上去后在新增信息看看


```

EXAMPLES
       Various ways to check your working tree

               $ git diff            (1)
               $ git diff --cached   (2)
               $ git diff HEAD       (3)

           1. Changes in the working tree not yet staged for the next commit.
           2. Changes between the index and your last commit; what you would be committing if you run "git commit" without "-a" option.
           3. Changes in the working tree since your last commit; what you would be committing if you run "git commit -a"

       Comparing with arbitrary commits

               $ git diff test            (1)
               $ git diff HEAD -- ./test  (2)
               $ git diff HEAD^ HEAD      (3)

           1. Instead of using the tip of the current branch, compare with the tip of "test" branch.
           2. Instead of comparing with the tip of "test" branch, compare with the tip of the current branch, but limit the comparison to the file "test".
           3. Compare the version before the last commit and the last commit.
    
        Comparing branches
以前面的branch为基准，显示后面branch对比前面branch的差异
            $ git diff topic master    (1)
            $ git diff topic..master   (2)
            $ git diff topic...master  (3)

            1. Changes between the tips of the topic and the master branches.
            2. Same as above.
            3. Changes that occurred on the master branch since when the topic branch was started off it.