## 初始

1. 进入需要添加到github项目的目录下

   cd xxx

2. git init            //初始化库

3. git add -A       // 添加所有文件

   git add file

4. git commit -m "xxxxx"




提交
----------------------------------------------------------------------
	echo "# learngit" >> README.md
	git init
	git add README.md
	git commit -m "first commit"
	git remote add learngit https://github.com/LIJIEJIE519/learngit.git	// 本地库连接远程库
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

误删的文件恢复到最新版本
$ git checkout -- test.txt

git add -A
git commit -m "LJ commit"
git clone -b dev https://gitee.com/zll_programmer/qms.git		//克隆分支git clone -b +分支 + 地址