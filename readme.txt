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
(.git目录默认是隐藏的，用ls -ah命令就可以看见)

4.把文件添加到车上：
$ git add xxx.txt

5.把运文件的车提交到仓库：
$ git commit -m "提交说明"

6.运行看结果：(工作区是否有修改没装车，车是否进仓库)
$ git status

7.查看修改记录：
$ git diff xxx.txt 

8.显示提交日志
$ git log
$ git log --pretty=oneline
(HEAD表示当前版本)
$ git reflog

9.返回上个版本(上一个版本：HEAD^；上上一个版本：HEAD^^；上100个版本：HEAD~100)
$ git reset --hard HEAD^

10.查看文件内容
$ cat xxx.txt

11.转到版本
$ git reset --hard xxxx

12.查看工作区和版本库里面最新版本的区别：
$ git diff HEAD -- readme.txt 

13.撤销一次操作：
	1.还没装车：工作区->仓库里文件的亚子；
	2.装车了还没进仓库：工作区->车上文件的亚子
$ git checkout -- readme.txt

14.把车上的文件返回工作区：
git reset HEAD <file>

15.删仓库文件，保存修改
$ git rm test.txt
$ git commit -m "remove test.txt"

16.丢弃工作区的修改，返回仓库里的版本
$ git checkout -- xxx.txt

17.创建SSH Key：
$ ssh-keygen -t rsa -C "1017465064@qq.com"

18.连接GitHub远程仓库
$ git remote add origin git@github.com:JohnZize/learngit.git

19.推送本地仓库到GitHub
$ git push -u origin master(第一次推送)
$ git push origin master