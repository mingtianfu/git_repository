Git is a version control system.
Git is free software.

第一步，用命令git add告诉Git，把文件添加到仓库：
git add readme.txt
git add file2.txt file3.txt
可以一次添加多个文件
第二步，用命令git commit告诉Git，把文件提交到仓库：
git commit -m "wrote a readme file"
简单解释一下git commit命令，-m后面输入的是本次提交的说明

git status命令可以让我们时刻掌握仓库当前的状态
git diff readme.txt 查看文件具体修改了什么内容

git log 查看提交日志
git log --pretty=oneline 查看提交日志，简化版

git reset --hard HEAD^ 回退到上一个版本，上一个版本就是HEAD^，上上一个版本就是HEAD^^，当然往上100个版本写100个^比较容易数不过来，所以写成HEAD~100。
git reflog 用来记录你的每一次命令

cat readme.txt 查看文件

修改了文件 git add只会把当前的修改添加到暂存区，之后修改的每次修改都要git add，git commit才会提交每次修改的 

git checkout -- readme.txt意思就是，把readme.txt文件在工作区的修改全部撤销，这里有两种情况：

一种是readme.txt自修改后还没有被放到暂存区，现在，撤销修改就回到和版本库一模一样的状态；

一种是readme.txt已经添加到暂存区后，又作了修改，现在，撤销修改就回到添加到暂存区后的状态。

总之，就是让这个文件回到最近一次git commit或git add时的状态。


git rm readme.txt用于删除一个文件。如果一个文件已经被提交到版本库，那么你永远不用担心误删，但是要小心，你只能 git checkout -- readme.txt 恢复文件到最新版本，你会丢失最近一次提交后你修改的内容。


Creating a new branch is quick.

Git鼓励大量使用分支：

查看分支：git branch

创建分支：git branch <name>

切换分支：git checkout <name>

创建+切换分支：git checkout -b <name>

合并某分支到当前分支：git merge <name>

删除分支：git branch -d <name>


git merge --no-ff -m "merge with no-ff" dev  合并分支时，加上--no-ff参数就可以用普通模式合并，合并后的历史有分支，能看出来曾经做过合并，而fast forward合并就看不出来曾经做过合并。

