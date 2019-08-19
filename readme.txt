Git is a distributed version control system.
Git is free software.

Study Git on https://www.liaoxuefeng.com/wiki/896043488029600

1.Setting user name and email:
$ git config --global user.name "Your Name"
$ git config --global user.email "email@example.com"

2.创建空目录:
$ mkdir learngit
$ cd learngit

3.把这个目录变成Git可以管理的仓库：
$ git init
（.git目录默认是隐藏的，用ls -ah命令就可以看见）

4.把文件添加到仓库：
$ git add xxx.txt

5.把文件提交到仓库：
$ git commit -m "提交说明"

6.运行看结果：
$ git status

7.查看修改记录：
$ git diff xxx.txt 

8.显示提交日志
$ git log
$ git log --pretty=oneline

9.