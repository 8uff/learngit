Git学习笔记
======
git 由linus于2005年开发，2008年github上线。  
版本控制有以下两种：集中式（cvs、svn），分布式（Bitkeeper,Git,Mercurial,Bazaar)。  
Git安装。  
设置Git：git config --global user.name "your name"  
         git config --global user.email "your email"  
所有版本控制系统只能跟踪文本文件，无法跟踪二进制文件（图像，视频，word）。  
文本编码推荐“utf-8”。windows系统不要使用系统自带“记事本”。  
## 创建版本库（repository)
### 创建分支
`git init`  
### 添加文件到仓库  
`git add  <file> ` 
### 提交文件到仓库
`git commit -m "说明"`  
### 查看版本库当前状态 
`git status`   
### 查看改变/区别
`git diff`  
### 查看提交日志
`git log`  
### 简化查看提交日志
`git log --pretty=oneline`  
### 查看分支合并信息
`git log --graph --pretty=oneling --abbrev-comit`
### 查看历史命令
`git reflog`   
## 版本回退
`git reset --hard HEAD(HEAD^,HEAD^^至HEAD~100,commit id)`
## 放弃修改
### 放弃修改工作区内容
`git checkout -- <filename>`  
### 放弃修改缓存区内容
`git reset HEAD  <filename>`  
## 删除文件
### 删除文件
git rm <filename>  
## 分支
### 创建分支
`git branch <name>`  
### 切换分支
`git checkout <name>`  
### 创建并切换分支
`git checkout -b <name>`  
### 查看分支
`git branch`  
### 合并分支至当前分支
`git merge <name>`  
### no-ff方式合并分支至当前分支
`git merge --no-ff -m "说明" <name>  
### 删除分支
`git branch -d <name>`  
### 删除未合并分支
`git branch -D <name>`  
## 储藏
### 储藏现有工作
`git stash`  
### 恢复
`git stash apply`  
### 删除
`git stash drop`
### 恢复并删除
`git stash pop`
### 查看储藏信息
`git stash list`

