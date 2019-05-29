# 远程仓库的使用

## 远程仓库克隆
> git clone https://github.com/schacon/ticgit

## 查看远程仓库
> git remote

你也可以指定选项 -v，会显示需要读写远程仓库使用的 Git 保存的简写与其对应的 URL。
> git remote -v

## 添加远程仓库
> git remote add pb https://github.com/paulboone/ticgit

## 从远程仓库中抓取与拉取
访问远程仓库，从中拉取所有你还没有的数据。 执行完成后，你将会拥有那个远程仓库中所有分支的引用，可以随时合并或查看。
$ git fetch [remote-name]

git pull 命令来自动的抓取然后合并远程分支到当前分支。 这对你来说可能是一个更简单或更舒服的工作流程；默认情况下，git clone 命令会自动设置本地 master 分支跟踪克隆的远程仓库的 master 分支（或不管是什么名字的默认分支）。 运行 git pull 通常会从最初克隆的服务器上抓取数据并自动尝试合并到当前所在的分支。

## 推送到远程仓库
git push [remote-name] [branch-name]
> git push origin master

## 查看远程仓库
> git remote show origin

## 远程仓库的移除与重命名
重命名
> git remote rename pb paul

移除
> git remote rm paul
