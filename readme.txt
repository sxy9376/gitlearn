 github 学习笔记
 第一步，建立git仓库，使用git init指令
第二部，加入git仓库，使用 git add和git commet指令
第三部，尝试反复提交add 和commit
第四部，查看当前仓库状态，git status ；查看文件更改历史，git diff
版本回退和版本回复：
需要使用git log指令来查看每次提交版本的id号，选择回退到哪一个版本中，使用git reset --hard HEAD^（上一个版本）或者
git reset --hard HEAD~100(上100个版本)，又或者git reset --hard 版本号，选择回到某个特定版本。
回退后，可以在任何时间使用git reset --hard 版本号，再前滚到最新的版本，使用git reflog，可以查看每次操作的版本号。

git跟踪每次文件的修改，如果不适用git add将修改提交到暂存区，commit将不会把修改提交到版本库

使用git restore <file>指令可以将工作区已经保存的文件的修改退回到暂存区或者仓库的版本
