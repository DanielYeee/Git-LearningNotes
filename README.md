# Git-学习笔记
这是一篇Git工具的基础入门笔记

常用git命令
***

一.用git在远程仓库创建分支

1.查看所有分支
（注：绿色字体为本地分支，红色字体为远程仓库的分支）
>git branch -a

2.创建本地分支
>git branch local_branch

3.将分支push到远程仓库
>git push origin local_branch

***

二.git删除远程仓库的文件

1.在本地拉取远程分支
>git pull origin master

2.在本地产出对应的文件
*同时在缓存和物理存储中删除文件，慎用！
>git rm filename
*只在缓存中删除对应的文件
>git rm --cache filename

3.上传到远程仓库
>git commit -m '删除某个文件'
>git push origin master

***

三.git中出现 '>' 符号怎么办
*解析：表示输入没有闭合，比如，双引号或单引号只输入了一个
>crtl + d

***




