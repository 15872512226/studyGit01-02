#学习git 版本管理软件 

github 代码托管

xxxxxxxx

xxxxxxxx


 第一步 本地文件夹内 点击右键 打开 Git Bash Here 
    再打开的小黑框 写： git init （初始化仓库）
    #--会出现一个隐藏的.git文件夹，不要动它

 第二步 文件夹里面创建文件再看敲代码****

    git add .      //存放到暂存区域
    git commit -m"描述提交的代码"   //提交

 ***(第一次提交会出现要设置邮箱和用户名)  建议与GitHub一致
    
    git status  查看提交
    git log 查看提交日志

 第三部：推送远程仓库

    git push   //推送


 git版本穿梭(回滚)：

 git reset --hard 版本号  //版本回滚的命令
 git  log --oneline          //查看一行类型的日志,包括版本号
 git  reflog     //查看所有的日志,包括回滚的日志

 git reset --hard HEAD^   //回滚到上一行版本
 git reset --hard HEAD^^   //回滚到上上个版本


 设置邮箱和用户名
    查看用户名邮箱

    git  config  user.email
    git  config  user.name

    一：直接设置  会覆盖

        git config --global user.email "you@example.com"
        git config --global user.name "Your Name" 
    二：退出再登录
    
    git  config  --global   --unset  user.email
    git  config  --global   --unset  user.name


   ***************

   分支学习：

   查看分支：

   git branch

   新建分支：

   git branch 分支名

   切换分支：

   git checkout 分支名

   合并分支：

   git merge 分支名
      回到要合并的分支哪里

   删除分支：

   git branch -d 分支名
   











