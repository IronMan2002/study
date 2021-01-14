# Git的用法

## 1.github仓库和账号创建完毕

## 2.git版本控制

操作说明：

### 1.创建

```
git init 初始化仓库
git clone 拷贝仓库到本地
```

此时应在本地创建一个文件夹

### 2.提交

```
git add 把文件添加到仓库
git commit 提交文件
git rm 删除文件
```

git commit后加-m <xxx>表示提交说明

## 3.远程操作

### 以ssh协议将GitHub与本地仓库关联

```
ssh-keygen -t rsa -C "关联电子邮件"
创建ssh key命令
```

然后在GitHub中关联id_rsa.pub中的公钥

```
$ git remote add origin git@github.com:IronMan2002/learngit.git
```

关联仓库

### 远程推送命令***git push***

```
git remote 操作远程库
```

将文件添加到本地库后

```
$ git push origin master 推送master分支到GitHub
```

推送到GitHub

## 4.分支管理

`master`是主分支，`HEAD`指向的是当前分支。

可使用`git branch (名称)`创建新分支。