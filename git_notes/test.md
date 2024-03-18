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



