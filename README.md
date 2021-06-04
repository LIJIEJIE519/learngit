## 初始

1. 进入需要添加到github项目的目录下

   cd xxx

2. git init            //初始化库

3. git add -A       // 添加所有文件

   git add file

4. git commit -m "xxxxx"

## 添加

```
git add xxx 	// 指定文件
git add xxx/	//指定文件夹
git add -A		// 添加所以变化
```




提交
----------------------------------------------------------------------
	echo "# learngit" >> README.md
	git init
	git add README.md
	git commit -m "first commit"
	git remote add learngit https://github.com/LIJIEJIE519/learngit.git	// 本地库连接远程库
	git branch -M main
	git push -u learngit master


​	


克隆
---------------------------------
$ git clone git@github.com:michaelliao/gitskills.git


删除
-----------------------------
1. git rm xxxx   

2. git commit -m "xxxx"

3. git push 

   ### 删除远程库文件夹

   1. git pull origin master   //将远程仓库里面的项目拉下来
   2. git rm -r --cached target  //删除target文件夹
   3. git commit -m "xxx"
   4. git push -u origin master

误删的文件恢复到最新版本
$ git checkout -- test.txt

git add -A
git commit -m "LJ commit"
git clone -b dev https://gitee.com/zll_programmer/qms.git		//克隆分支git clone -b +分支 + 地址





# Github创建新分支

### 一、clone Repository

https://www.jianshu.com/p/4b95058088c2

clone Github 上的Repository，如下：

```
git clone https://github.com/siskinc/siskinc.github.io
```

### 二、管理分支

1、查看分支

#### 1、查看本地分支

使用 git branch命令，如下：

```
$ git branch
git status
```

* master

*标识的是你当前所在的分支。

#### 2、查看远程分支

命令如下：

```
git branch -r
```

#### 3、查看所有分支

命令如下：

```
git branch -a
```

#### 2、本地创建新的分支

命令如下：

```
git branch [branch name]

例如：
git branch save
```

#### 3、切换到新的分支

```
命令如下：
git checkout [branch name]

例如：
$ git checkout save
```



#### 4、创建+切换分支

创建分支的同时切换到该分支上，命令如下：

```
git checkout -b [branch name]

git checkout -b [branch name] 的效果相当于以下两步操作：
git branch [branch name]
git checkout [branch name]
```



#### 5、将新分支推送到github

命令如下：

```
git push origin [branch name]

例如：
git push origin save
```



#### 6、删除本地分支

命令如下：

```
git branch -d [branch name]

例如：
git branch -d save
```



#### 7、删除github远程分支

命令如下：

```
git push origin :[branch name]
```



分支名前的冒号代表删除。
例如：

```
git push origin :save
```

### 设置上游分支
```
git push --set-upstream origin wangxiao
```


