#### Git与本地同步方法

##### 1.本地无项目，直接拉取远程

1. ```
   git clone https://github.com/CKTim/BlueTooth.git（https://github.com/CKTim/BlueTooth.git替换成你之前复制的地址） 
   ```

2. git add *    （注：别忘记后面的.，此操作是把Test文件夹下面的文件都添加进来）

   git commit  -m  "提交信息"  （注：“提交信息”里面换成你需要，如“first commit”）

   git push -u origin master   （注：此操作目的是把本地仓库push到github上面，此步骤需要你输入帐号和密码）

##### 2.本地有项目，连接远程项目进行合并

1. git init

2. git remote add origin https://github.com/guyibang/TEST2.git

3. git pull --rebase origin master (防止上传失败)

4. git push -u origin master 由于新建的远程仓库是空的，所以要加上-u这个参数，等远程仓库里面有了内容之后，下次再从本地库上传内容的时候只需下面这样就可以了： 

    git push origin master 

git pull origin master --allow-unrelated-histories 可以允许不相关历史提，强制合并 

git remote rm origin 删除远程链接

##### 生成密钥指令

```
ssh-keygen -t rsa -C "youremail@example.com" 注意ssh-keygen之间没有空格
```
#### 参考地址

https://cloud.tencent.com/developer/article/1504684#:~:text=%E6%80%BB%E7%BB%93%EF%BC%9A%E5%85%B6%E5%AE%9E%E5%8F%AA%E9%9C%80%E8%A6%81%E8%BF%9B%E8%A1%8C%E4%B8%8B%E9%9D%A2%E5%87%A0%E6%AD%A5%E5%B0%B1%E8%83%BD%E6%8A%8A%E6%9C%AC%E5%9C%B0%E9%A1%B9%E7%9B%AE%E4%B8%8A%E4%BC%A0%E5%88%B0Github%201%E3%80%81%E5%9C%A8%E6%9C%AC%E5%9C%B0%E5%88%9B%E5%BB%BA%E4%B8%80%E4%B8%AA%E7%89%88%E6%9C%AC%E5%BA%93%EF%BC%88%E5%8D%B3%E6%96%87%E4%BB%B6%E5%A4%B9%EF%BC%89%EF%BC%8C%E9%80%9A%E8%BF%87git%20init%E6%8A%8A%E5%AE%83%E5%8F%98%E6%88%90Git%E4%BB%93%E5%BA%93%EF%BC%9B%202%E3%80%81%E6%8A%8A%E9%A1%B9%E7%9B%AE%E5%A4%8D%E5%88%B6%E5%88%B0%E8%BF%99%E4%B8%AA%E6%96%87%E4%BB%B6%E5%A4%B9%E9%87%8C%E9%9D%A2%EF%BC%8C%E5%86%8D%E9%80%9A%E8%BF%87git%20add,.%E6%8A%8A%E9%A1%B9%E7%9B%AE%E6%B7%BB%E5%8A%A0%E5%88%B0%E4%BB%93%E5%BA%93%EF%BC%9B%203%E3%80%81%E5%86%8D%E9%80%9A%E8%BF%87git%20commit%20-m%20%22%E6%B3%A8%E9%87%8A%E5%86%85%E5%AE%B9%22%E6%8A%8A%E9%A1%B9%E7%9B%AE%E6%8F%90%E4%BA%A4%E5%88%B0%E4%BB%93%E5%BA%93%EF%BC%9B