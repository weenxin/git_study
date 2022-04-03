## git学习

**初始化**新建一个good.txt文件。

**git add** : 使 用`git add good.txt` 将文件加入到stage区
**git rm --cache** 将文件 从stage区中删除
**git status**修改good.txt文件,使用git status可以看到，文件状态变为modified
**git restore**，使用git restore good.txt，可以恢复good.txt文件
**git restore --stage good.txt**，恢复已经到staged的文件为未提交状态，与git rm --cache不同的是，git rm会在管理中删除文件
**git log --pretty=oneline**，可以查看版本日志
**增加多条提交日志，用于测试版本回滚**



