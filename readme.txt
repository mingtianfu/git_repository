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