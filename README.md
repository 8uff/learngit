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

git init                                                  新建版本库  
git add  <file>                                           添加文件到仓库  
git commit -m "说明"                                      提交文件到仓库  
git status                                                查看版本库当前状态  
git diff                                                  查看改变/区别  
git log                                                   查看提交日志  
git log --pretty=oneline                                  简化查看提交日志  
git reflog                                                查看历史命令  
## 版本回退
git reset --hard HEAD(HEAD^,HEAD^^至HEAD~100,commit id)
## 放弃修改
git checkout -- filename                                  放弃修改工作区内容  
git reset HEAD  filename                                  放弃修改缓存区内容  
## 删除文件
git rm filename                                           删除文件  
