>#**用`git add`命令把文件添加到暂存区 : 

`git add read.txt`

>**用`git commit`命令用把文件提交到仓库**

`git commit -m "message"`

>日志

`git log`

>**版本回退:**

使用命令`git reset`回退版本:

**说明:**

在Git中，用`HEAD`表示当前版本，也就是最新的提交`20b123....`，上一个版本就是`HEAD^`，上上一个版本就是`HEAD^^`，当然往上100个版本写100个`^`比较容易数不过来，所以写成`HEAD~100`

`git reset --hard HEAD^`

> 查看仓库当前的状态

命令`git status`查看仓库当前的状态，显示有变更的文件


>添加远程仓库

`git remote add origin __ADDR__`

>push

`git push -u origin master`

>genarate rsa key

`ssh-keygen -t rsa -C yourname@some.com`

注：成功的话会在 **~/** 下生成 **.ssh** 文件夹，进去，打开 **id_rsa.pub**，复制里面的 **key**

>配置用户信息

 `git config #查看本机是否配置了个人信息  
 `git config --global user.name "……" #定义全局的用户名  
 `git config --global user.email "……" #定义全局的邮件地址  
 `git config --list #查看配置信息`