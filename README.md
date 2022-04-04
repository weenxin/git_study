## git学习

**初始化**新建一个good.txt文件。

**git add** : 使 用`git add good.txt` 将文件加入到stage区
**git rm --cache** 将文件 从stage区中删除
**git status**修改good.txt文件,使用git status可以看到，文件状态变为modified
**git restore**，使用git restore good.txt，可以恢复good.txt文件
**git restore --stage good.txt**，恢复已经到staged的文件为未提交状态，与git rm --cache不同的是，git rm会在管理中删除文件
**git log --pretty=oneline**，可以查看版本日志
**git reflog**查看reflog
**增加多条提交日志，用于测试版本回滚**

### 查看提交日志
***git log***查看提交日志
***git log --online*** 每个提交日志一行显示
***git reflog*** 更优雅的显示日志

### 版本回滚
***git reset HEAD 098fac***， 回滚到指定版本
***git reset HEAD^*** 回滚的到上一个版本
***git reset HEAD^^*** 回滚到上两个版本
***git reset HEAD~3***回滚到上三个版本
***git reset --soft***只移动HEAD指针，不重制Stag区和Work区
***git reset --mix*** 移动HEAD指针，重制Stage区，但是不重制Work区
***git reset --hard*** 移动HEAD指针，重制Stage区，重制Work区

### 找回删除文件
***git reset --hard version_hash*** 直接reset到指定位置就好


### 比较不同
***git dif filename*** 查看文件修改内容

