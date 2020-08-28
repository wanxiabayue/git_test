### this is the git_test demo

> 状态

1. git log 提交日志  
   q 退出日志状态
2. git status 查看本地文件更改状态

> 创建版本库（本地）

1. git init 初始化 git 本地仓库，生成一个.git 隐藏文件夹
2. git config --global user.name ‘zet’ 初始话就要配置仓库：配置用户名
3. git config --global user.email ‘834997495@qq.com’ 配置用户邮箱
4. 添加到版本库（暂存区）
   - git add. 添加全部更改
   - git add user/index.html 添加更改文件
   - git add src / \*.html 批量添加更改文件
5. git commit -m '注释内容' 提交到版本库

> 忽略文件

1. 添加 .gitignore 文件，输入忽略类型：

   \*.txt 文件
   ./ignore 文件夹

> 建立远程仓库（协同管理代码），与本地仓库连接 github(gitlab)

1. git remote 检查远程是否有这个仓库
2. git remote add origin https://github.com/wanxiabayue/git_test.git github 新建一个 git_test 仓库，与本地仓库关联
3. git pull origin master 上传代码前，建议拉取一下（空仓库不用）
4. git push -u origin master 第一次推送 master 分支的所有内容
5. git push origin master 每次本地更改后，都可以上传（也可以 git push）
   - git pull 多人协同管理，上传前需要先拉取

> 创建分支、合并分支（默认主分支为 master）

1. git branch 检查本地分支，当前分支前面有'\*'号
2. git branch dev 创建分支 dev
3. git checkout dev 切换到分支 dev
4. git checkout master 切换回主线 master
5. git merge dev 合并分支（注意：必须在 master 主线下，才能合并分支）
6. git branch -d dev 删除分支

> 开发中分支管理

1. 分支可以在 github 上建，也可以在本地建
2. 在本地分支开发，结束后，提交到远程分支仓库；然后本地切换到 master，merge 分支
3. 在本地 master 上 push 到远程 master

##### Git 鼓励你使用分支完成某个任务，合并后再删掉分支，这和直接在 master 分支上工作效果是一样的，但过程更安全
