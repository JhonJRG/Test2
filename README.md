##### hello,这次是在练习如何把本地空文件夹变成仓库并推送到远程仓库 关键是以下这两句

 1. ```git init``` （获取.git文件）
 
 2. ```git push origin master```（注意：origin是远程主机名一般只有一个，指的就是```git@github.com:JhonJRG/Test2.git```这个地址，起了个名字而已）

 3. ```git push -u origin dev:dev```（远程分支的建立，就是这样做）
 
 ps：多嘴一句，clone仓库的远程分支可以直接这样做```git checkout -b dev origin/master```(切换到新建立的本地分支dev与远程分支origin/master对应)
 
  ps:github上新建空文件夹，本地新建空文件夹并推送至github，重要的语句是git init。注意git init是初始化.git信息，所以只适用于本地空文件夹推送至远程仓库，切勿在本地仓库内滥用，否则会删除掉以往操作信息及状态
  

######
  我们设置master对应远程仓库的master分支

  git branch --set-upstream master origin/master
  
  git branch -u origin/master dev
  
  git branch -vv(查看所有的本地远程分支映射关系)

  这样在我们每次想push或者pull的时候，只需要 输入git push 或者git pull即可。

  在此之前，我们必须要指定想要push或者pull的远程分支。

  git push origin master (git push origin master:master)

  git pull origin dev (git pull origin dev:dev)
######
