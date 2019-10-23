```shell
初始配置
配置命令: git config
配置所有用户: git config --system [选项]
配置文件位置: /etc/gitconfig

tarena@tarena:~$ sudo git config --system user.name Tedu
tarena@tarena:~$ cat /etc/gitconfig 
[user]
	name = Tedu

```

```shell
配置当前用户: git config --global [选项]
tarena@tarena:~$ git config --global user.email 1127026278@qq.com

配置文件位置: ~/.gitconfig
tarena@tarena:~$ cat ~/ .gitconfig 
cat: /home/tarena/: 是一个目录
[user]
	email = 1127026278@qq.com
初始化仓库
git init 意义:将某个项目目录变为git操作目录,生成git本地仓库。即该项目目录可以使用git管理

tarena@tarena:~$ cd '/home/tarena/桌面/Linux/day17' 
tarena@tarena:~/桌面/Linux/day17$ git init
已初始化空的 Git 仓库于 /home/tarena/桌面/Linux/day17/.git/
tarena@tarena:~/桌面/Linux/day17$ ls -a
.  ..  .git
配置编译器
tarena@tarena:~/桌面/Linux/day17$ git config core.edutor pycharm
tarena@tarena:~/桌面/Linux/day17$ cd .git/
tarena@tarena:~/桌面/Linux/day17/.git$ ls
branches  config  description  HEAD  hooks  info  objects  refs
tarena@tarena:~/桌面/Linux/day17/.git$ cat config 
[core]
	repositoryformatversion = 0
	filemode = true
	bare = false
	logallrefupdates = true
	edutor = pycharm
	
查看配置信息
tarena@tarena:~/桌面/Linux/day17/.git$ cd ..
tarena@tarena:~/桌面/Linux/day17$ git config --list
user.name=Tedu
user.email=1127026278@qq.com
core.repositoryformatversion=0
core.filemode=true
core.bare=false
core.logallrefupdates=true
core.edutor=pycharm


```
![](./0qp.jpg)
