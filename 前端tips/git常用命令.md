//从git下载代码到本地文件夹

```
git clone ssh://git@....
```
//切换train分支
```
git checkout train
```
//从当前分支拉取代码
```
git pull
```
```
git status //查看当前状态
git add 文件名 //添加至暂存区
git commit -m "" //提交至工作区
git push //上传至git仓库
```
###git常用命令
```
ssh keygen -t rsa -C "xxx@qq.com"
git config --global user.name ""
git config --global user.email ""
git init
git log 
git reflog
git reset --hard HEAD^ //回退到上个版本
git reset --hard HEAD^^ //回退到上上个版本
git reset --hard XXXX //回退到指定版本
git checkout -- test.txt // 撤销修改
```
推送现有文件夹
```
cd 
git init
git remote add origin ssh://git@...
git add .
git commit -m ""
git push -u origin master
```
推送现有的git仓
```
cd 
git remote rename origin  old-origin
git remote add origin ssh://git@...
git push -u origin -all
git push -u origin --tags
```
```
git checkout -b dev //创建分支
git merge dev //合并分支
git merge -no-ff -m "" dev //快速合并
git branch -d dev //删除分支
```

