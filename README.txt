new file
ubuntu(for git)
安装git：
  sudo apt-get install git 
配置名字和邮箱：
  git config --global user.name <name>
  git config --global user.email <email>
配置公钥：
  ssh-keygen -C <email> -t rsa
查看公钥然后复制出来：
  cd ~/.ssh
  cat id_rsa.pub
然后登录Github把复制的公钥添加进去就好了

现在来到本地就可以对仓库进行处理
初始化仓库：
git init
将文件添加到暂存区：
git add <file>
将文件从暂存区添加到版本库中：
git commit -m "some decription"
然后将本地仓库和远程仓库关联：
git remote add origin git@<url>
可以推送到远程仓库了：
git push <-u> origin master
也可以拉取远程仓库：
git pull origin master
克隆远程仓库:
git clone git@<url>

