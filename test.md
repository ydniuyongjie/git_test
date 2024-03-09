# 一份简单的GIT教程

>[!TIP] 首先明白在GIT中有几个概念：工作区---暂存区---版本库以及远程库
![Alt text](image-1.png)
* git add test.c &nbsp;&nbsp;&nbsp;&nbsp;工作区创建text.c文件，并**添加**到暂存区
* git commit &nbsp;&nbsp;&nbsp;&nbsp; 将文件从暂存区提交到版本库
* git reset --hard HEAD^ &nbsp;&nbsp;&nbsp;&nbsp; 回退到上一个版本
* git reflog&nbsp;&nbsp;&nbsp;&nbsp;用来记录你的每一次命令

---
## 管理修改

* git restore --staged test.md可以将文件test.md从暂存区撤销
* git reset HEAD test.md**也**可以将文件test.md从暂存区撤销，是从**版本库**将文件恢复，
*  现在我在项目里添加了一个文件叫test.c文件，
而且我已经提交给版本库，现在我手工把test.c文件从工作区删掉了。存在两种情况：
    
    1. 我删除错了，需要恢复，git checkout -- test.c :从版本库中将文件恢复到工作区。
    2. 这个文件的确需要删除，那用git rm test.c 从版本库中将test.c文件删除，然后使用git commit -m “删除文件”进行确认，否则文件没有真的被删除。
*  fsfsdfs
*  fsad
*  
