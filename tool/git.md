#GIT工具的快速使用

##安装 请到官网 [git-scm.com](http://git-scm.com/) 或国内的下载站，下载安装包。

###创建项目有两种情况

1、本地无项目

克隆远程库的文件到本地 例如在github或oscgit上已有的项目，可以将其拉取到本地上
```text
    git clone  https://github.com/angular/quickstart  my-projName
    cd my-projName
```
**注意：**上面的`git clone`命令需要传入第一个参数是远端git库的地址，第二个参数是本地的项目名字（也就是本地的文件夹名称）

2、本地有项目

合并远程库的文件到本地 例如我本地开发好一个程序应用，并且在`github`或`oscgit`上创建好一个空的库，需要把代码上传到该库

首先,你需要执行下面两条命令,作为git的基础配置,作用是告诉git你是谁,你输入的信息将出现在你创建的提交中.
```text
    git config --global user.name "你的名字或昵称"
    git config --global user.email "你的邮箱"
```
那我们第一步可以初始化本地库先
```text
    //进入到本地程序所在根目录
    git init                //git的初始化
```
把本地库文件和远程库文件进行合并
```text
    git pull origin master
```
添加文件到本地库
```text
    git add .                            //添加本地队列
    git commit -m "第一次提交"            //把队列中的文件提交到本地库
```
合并后提交代码  
```text
    git push origin master            //把本地库的文件推送到远程库的master主线
```
>**如果需要账号密码的话就输入账号密码，这样就完成了一次提交。**

设置操作的默认库和分支
```text
    git branch --set-upstream-to=origin/master
```
###常用的提交操作
修改或添加好自己的文件后，需要把文件添加到git队列中
```text
    git add .        //把当前所有改动后的文件添加到git队列中    
```
把队列中的文件提交到本地库
```text
    git commit -m "提交说明"
```
> **注意**参数-m ,是必须的，表示提交时的说明文字
