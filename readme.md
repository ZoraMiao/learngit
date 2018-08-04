### 将本地文件推送到Github远程仓库
1. 先在github上创建一个项目：例如 vue-demo
2. 在本地vue-demo 项目中使用 git init 把其变成git可以管理的仓库
git init
3. 若要忽略本地的文件或文件夹不被提交到github ，则需要在项目根目录下创建 .gitignore 文件
touch .gitignore
4. 打开文件，编辑内容，例如：
node_modules/ 
update.txt 
则可以忽略目录下node_modules 文件夹及updata.txt 文件.
5. 关联远程仓库 （第一次使用需要添加github公钥）
git remote add origin git@github.com:***/vue2.1-sell.git 或者 git remote add origin https://github.com/***/vue2.1-sell.git
6. 获取远程库与本地同步（远程仓库不为空需要这一步）
git pull --rebase origin master
7. 把本地内容推送到远程库 使用 git-push
git push -u origin master<br>
[相关文章](https://blog.csdn.net/chenzhijie101/article/details/79512336)
