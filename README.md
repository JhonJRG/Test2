##### hello,这次是在练习如何把本地空文件夹变成仓库并推送到远程仓库 关键是以下这两句

 1. ```git init``` （获取.git文件）

 2. ```git remote add origin git@github.com:JhonJRG/Test2.git``` （推送给谁）
 
 3. ```git push origin master```（注意：origin指的就是```git@github.com:JhonJRG/Test2.git```这个地址，起了个名字而已）

  ps:github上新建空文件夹，本地新建空文件夹并推送至github，重要的语句是git init。注意git init是初始化.git信息，所以只适用于本地空文件夹推送至远程仓库，切勿在本地仓库内滥用，否则会删除掉以往操作信息及状态
  
  
  
  
  大发的说法安抚阿萨德
