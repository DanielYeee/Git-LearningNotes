## Git-常用命令

> Git 是一个版本控制工具，通过版本迭代来进行内容的更新,
> 并且存储关于该内容的所有版本

***
##### 1.查看所有分支
（注：绿色字体为本地分支，红色字体为远程仓库的分支）
``` git branch -a ```
***
##### 2.创建本地分支
``` git branch local_branch```
***
##### 3.将分支push到远程仓库
```git push origin local_branch ```
***
##### 4.在本地拉取远程分支
``` git pull origin master```
***
##### 5.在本地删除对应的文件

```git rm filename ```
删除工作区的文件，但会将此次删除放进暂存区，待git commit后将版本库中的对应文件也删除

``` git rm -f filename ```
删除工作区和暂存区的内容，并放进暂存区，commit后删除版本库的文件

``` git rm --cache filename```
删除暂存区文件，但保留工作区的文件，并且将这次删除放入暂存区，commit后删除版本库的文件，此时只剩下工作区的文件

``` git restore filename ```
将在工作区而不在暂存区的文件撤销更改，（没有git add之前的文件）

``` git restore --staged filename ```
将在暂存区的文件撤出，但不会更改当前在工作区中的文件

***
##### 6.本地修改文件后保存版本并上传到远程仓库

``` git add filename ```
``` git commit -m '描述信息'```
``` git push origin master```



