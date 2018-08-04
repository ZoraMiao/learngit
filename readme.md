### 将本地文件推送到Github远程仓库
1. 先在github上创建一个项目：例如 vue-demo<br>
2. 在本地vue-demo 项目中使用 git init 把其变成git可以管理的仓库<br>
git init<br>
3. 若要忽略本地的文件或文件夹不被提交到github ，则需要在项目根目录下创建 .gitignore 文件<br>
touch .gitignore<br>
4. 打开文件，编辑内容，例如：<br>
node_modules/ <br>
update.txt <br>
则可以忽略目录下node_modules 文件夹及updata.txt 文件.<br>
5. 关联远程仓库 （第一次使用需要添加github公钥）<br>
git remote add origin git@github.com:***/vue2.1-sell.git <br>
或者 git remote add origin https://github.com/***/vue2.1-sell.git<br>
6. 获取远程库与本地同步（远程仓库不为空需要这一步）<br>
git pull --rebase origin master<br>
7. 把本地内容推送到远程库 使用 git-push<br>
git push -u origin master<br>
[相关文章](https://blog.csdn.net/chenzhijie101/article/details/79512336)
