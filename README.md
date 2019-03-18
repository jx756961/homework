##### 1.下载安装及配置
1. [官方下载地址](https://git-scm.com/)
2. 直接下一步安装git后面自行改动,不改动直接下一步
3. 安装结束 *win+r*  打开*cmd*窗口运行,==git --version== 查看版本正常查看证明安装成功
4. 右键项目找到 ==Git Bash Here== 点击运行后会弹出一个类似于cmd形式的窗口这里就能运行git的命令。
5. 如果有需要忽略上传的文件在 ==.gitignore== 文件中写上后就可以 例如：文件 ==bak.css== 或者 文件夹 ==/.idea==
##### 2.基础命令行操作
序号 | 使用命令   | 含义
-------- |-------- | -----
1|git init | 初始化本地git仓库 |
2|git add  < file > | 添加文件（file文件名）|
3|git status | 查看状态 |
4|git commit | 提交  -m备注 |
4|git checkout| 切换分支和主线 |
4|git reset|  回退到历史的某个版本|
5|git push | 推送到仓库 |
6|git pull | 远程仓库拉取数据 |
7|git clone | 远程仓库拷贝数据 |

#####  3.操作分支和主线
1. 新建分支==login==
```cmd
	git branch login
```
2. 切换工作空间到==login==
```cmd
	-这时就可以直接在你自己的空间编写你要的模块,在你没有合并主线之前这里的代码不会污染到主线
	-如果你要保存分支的内容你要commit你的文件
	git checkout login
	git commit -m '我所更新的内容'
```
3. 切换工作空间到主线 ==master==
```cmd
	-开发测试结束,合并分支到主线内容 git merge (你所要合并的分支模块名称)
	git merge login
```
4. 提交到远程仓库
	1. 登陆github
	2.
```cmd

	git init
	git add README.md
	git commit -m "first commit"
	git remote add origin https://github.com/账号/项目.git
	git push -u origin master

	…or
	git remote add origin https://github.com/账号/项目.git
	git push -u origin master

 ```
