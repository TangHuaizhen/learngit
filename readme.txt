nodeJs 
Beyond Compare 版本 3及以上
sublime text3 or Visual Studio Code
FSCapture截图工具
（ chrome浏览器 ）
SVN or Git

Git is a version control system.
Git is free software.

Git is a distributed version control system.
Git is free software.

Git is a distributed version control system.
Git is free software distributed under the GPL.
Git has a mutable index called stage.
在Windows上使用Git，使用从Git官网上直接下载安装程序，（网速慢的同学请移步国内镜像），然后按默认选项安装即可。
安装完成后，在开始菜单里找到“Git”->“Git Bush”，蹦出一个类似命令窗口的东西，就说明Git安装成功！
安装完成后还需要最后一步设置，在命令行输入：
git config --global user.name "Your Name"
git config --global user.email "email@example.com"


mkdir learngit
cd learngit
pwd
最好不要出现中文字符

git init
.git 文件目录 没事千万不要手动修改这个目录里面的文件，不然改乱了，就把Git仓库给破坏了。
ls -ah 可以看到默认隐藏的.git目录

git add readme.txt
git commit -m "worte a readme file"
git status 告诉有没有修改
git diff 修改了什么
git log 日志
git log --pretty=oneline
git reset --hard HEAD
git reset --hard HEAD~3
cat readme.txt 查看文件内容
git reflog
HEAD指向的版本就是当前版本，因此，Git允许我们在版本的历史之间穿梭，使用命令git reset --hard commit_id
穿梭前，用git log 可以查看提交历史，以便确定要回退到哪个版本
要重返未来，用git reflog 查看命令历史，以便确定要回到未来的哪个版本
