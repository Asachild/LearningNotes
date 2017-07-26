学习中遇到的问题-小雪雪的学习笔记

### 一、初学Github

#### 1.用命令行上传本地项目
  * 第一步：要把当前的目录生成git可以管理的仓库（这个仓库是本地仓库，会出现有一个.git的文件夹）<br>
    ```
    git init
    ``` 
    
  * 第二步：这一步要添加文件到本地仓库啦，这一步不是直接到仓库哦，可以说先添加到暂存区，添加到暂存区有三种情况<br>
    ```
    git add 文件名  //添加单个文件
    ```
    ```
    git add *  //git会自动将当前目录里面所有修改过的文件进行添加，不是检索全部哦
    ```
    ```
    git add .  //git会递归地将执行命令时所在的目录中的所有文件添加上去
    ```
    
  * 第三步：这一步就是提交到本地仓库啦<br>
    ```
    git commit -m '这里面填说明'  //说明可以是简单描述对这个文件，以后看历史记录方便查找，它是可以提交多个文件的
    ```
    
  * 第四步：要关联远程仓库，当然你要先在Github上创建自己的仓库<br>
          （一般就是本地仓库名，我觉得不管是远程仓库还是本地仓库都用项目名最好啦）
    ```
    git remote add origin https://github.com/用户名/仓库名.git  //这个是仓库的链接
    ```
    
  * 第五步：将代码由本地仓库上传到Github远程仓库<br>
    <b>注意</b>:本地代码目录中如果没有github仓库中的`README.md`文件，要执行以下命令，进行代码合并
    ```
    git pull --rebase origin master
    ```
    接下来就能push到我们的远程仓库啦
    ```
    git push -u origin master
    ```
