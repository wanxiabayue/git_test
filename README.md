### this is the git_test demo

#### 状态

1. git log 提交日志  
   q 退出日志状态
2. git status 查看本地文件更改状态

#### 创建版本库（本地）

1. git init 初始化 git 本地仓库，生成一个.git 隐藏文件夹
2. git config --global user.name ‘zet’ 初始话就要配置仓库：配置用户名
3. git config --global user.email ‘834997495@qq.com’ 配置用户邮箱
4. 添加到版本库（暂存区）
   - git add. 添加全部更改
   - git add user/index.html 添加更改文件
   - git add src / \*.html 批量添加更改文件
5. git commit -m '注释内容' 提交到版本库

#### 忽略文件

1. 添加 .gitignore 文件，输入忽略类型：

   \*.txt 文件
   ./ignore 文件夹

#### 创建分支、合并分支（默认主分支为 master）

1. git branch login 创建分支 login
2. git checkout login 切换到分支 login
3. git checkout master 切换回主线 master
4. git merge login 合并分支（注意：必须在 master 主线下，才能合并分支）

#### 建立远程仓库（协同管理代码），与本地仓库连接 github(gitlab)

1. git remote 检查远程是否有这个仓库
2. git remote add origin https://github.com/wanxiabayue/git_test.git github 新建一个 git_test 仓库，与本地仓库关联
3. git pull origin master 上传代码前，建议拉取一下（空仓库不用）
4. git push -u origin master 第一次推送 master 分支的所有内容
5. git push origin master 每次本地更改后，都可以上传（也可以 git push）
   - git pull 多人协同管理，上传前需要先拉取
