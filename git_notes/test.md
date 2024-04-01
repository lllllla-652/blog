### 创建版本仓库

1. 创建一个空目录
2. 创建一些文件(read.me)
3. `git init`(把这个目录变为仓库)
4. `git add <file>`
5. `git commit -m <message> `
6. `git status`(查看当前仓库的状态)
7. `git diff <file>`(查看文件修改内容)
8. `git log` `git log --prettyline`(显示提交日志)




### 版本回退
1. `HEAD`表示当前版本 `HEAD^`表示上一个版本 `HEAD^^`表示上上个版本
2. `git reset --hard HEAD^/HEAD^^` 回退到上一个版本/上上个版本
3. `git reset --hard <commit id>` 回到未来的某个commit id版本
4. `git reflog` 查看命令历史，以便确定回到未来的哪个版本
5. `git log` 查看提交历史，以便确定要回退到哪个版本

### 撤销修改
1. `git checkout -- file` 丢弃工作区的修改
2. `git reset HEAD <file>` 把暂存区的修改撤销掉，重新放回工作区

### 删除文件

1. `git rm file`从仓库中删除文件然后 `git commit`

### 添加远程仓库

```shell
git remote add origin https://github.com/lllllla-652/blog.git 
git branch -M main  修改分支名称
git push -u origin main
```

```
`git remote rm origin https://github.com/lllllla-652/blog.git` 删除与远程仓库的连接
```





### 初始化

1. 创建一个目录
2. 创建一些文件(read.me)
3. `git init`
4. `git add`
5. `git commit`
6. `git push -u origin main`
7. `git status` ,`git log`,`git branch -a`

### 舍弃git仓库

```
cd path/to/repo
rm -rf .git
```

### 本地分支推送到远程分支

```shell
git remote add origin https://github.com/lllllla-652/blog.git
git branch -M main
git push -u origin main
```

### clone别人的仓库然后再push到自己的github

```
git remote rm origin #把旧的绑定远程仓库删掉
git remote add origin https://github.com/lllllla-652/Moon.git  #添加新的远程仓库
git remote -v #查看远程连接
```


