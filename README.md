学习中遇到的问题-小雪雪的学习笔记

## 一、初学Github

#### 1.命令行上传本地项目

  * 第一步：要把当前的目录生成git可以管理的仓库（会出现有一个.git的文件夹）<br>
    命令：`git init`
    
  * 第二步：这一步要添加文件啦，有三种情况<br>
    命令：`git add 文件名`//添加单个文件<br>
         `git add *`//git会自动将当前目录里面所有修改过的文件进行添加，不是检索全部哦<br>
         `git add .`//git会递归地将执行命令时所在的目录中的*所有文件*添加上去<br>

