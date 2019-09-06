### this is the git_test demo
#### 状态
1.	git log 提交日志
2.	git status 查看本地文件更改状态 

### 添加
1.	git init 初始化git本地仓库
2.	git config --global user.name ‘zet’ 初始话就要配置仓库：配置用户名
   git config --global user,email ‘834997495@qq.com’ 配置用户邮箱
3.	git add .  \  git add index.html \ git add *.html 添加本地缓存，队列，仓库 (全部，文件名，一类)
4.	git rm --cached index.html 取消添加文件

### 忽略文件
1.	添加 .gitignore文件，输入忽略类型：

    *.txt   文件
    ./ignore 文件夹

### 提交
1.	git commit -m ‘first change’ 添加提交注释
2. git push

### 创建分支、合并分支（默认主线为master）
1.	git branch login 创建分支login
2.	git checkout login 切换到分支login
3.	git checkout master 切换回主线master
4.	git merge login 合并分支（注意：必须在master主线下，才能合并分支）

### 提交本地仓库到远程仓库github
1.	git remote 检查远程是否有这个仓库
2.	git remote add origin https://github.com/wanxiabayue/git_test.git github新建一个git_test仓库，与本地仓库链接
3.	git push -u origin master 本地仓库连上远程仓库

