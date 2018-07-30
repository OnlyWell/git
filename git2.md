#### 版本修改
#### git版本操作
>>>> - git status //查看当前状态
>>>> - git diff readme.txt 查看修改内容
>>>> - git log //显示从最近到最远的提交日志,如果输入信息太多,可以加上 --pretty=oneline
>>>> - git reset --hard HEAD^ 回退到上一个版本
>>>> - cat read.txt 查看当前文件
>>>> - git reflog 查看历史提交版本，包含commitId
>>>> - git reset --hard commit_id
>>>> - git的版本库中存了很多东西,其中最重要的是称为stage(或index)的东西,需要提交的东西都在暂存区,一次性提交暂存区的所有修改
>>>> - git diff HEAD -- read.txt 查看工作区和版本库里面最新版本的区别
>>>> - git checkout -- read.txt  把在read.txt文件在工作区的修改全部撤销.有两种情况，一是read.txt自修改后还没有被放到暂存区,现在撤销修改就回到和版本库一模一样的状态;
一种是read.txt已经添加到暂存区后,又做了修改,现在,撤销修改就回到添加到暂存区后的状态.
>>>> - git checkout -- read.txt 也可以用来恢复删除的文件, git checkout 其实是用版本库里的版本替换工作区的版本,无论工作区是修改还是删除,都可以"一键还原"
>>>> -从版本库删文件 git rm test.txt 并进行 git commit -m " delete a file"