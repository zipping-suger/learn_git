# Learning Git

## 绑定用户

```git
git config --global user.name "Your Name" // User name
git config --global user.email "your_email@example.com" // e-mail

```

## 为 Github 账户设置 SSH key

#### 检查密钥

```
cd ~/.ssh
```

如果没有，利用一下代码生成

```
ssh-keygen -t rsa -C "your_email@example.com"
```

生成成功后，去对应目录 `C:\Users\Administator\.ssh` （Administator为电脑用户名，每个人不同）用记事本打开 id_rsa.pub，得到 ssh key公钥

将 id_rsa.pub 文件中 key 粘贴到此，最后 Add SSH key 生成密钥。

##  Command Line Cheat Sheet

```git
touch // create new doc
git init // 把这个目录变成Git可以管理的仓库
git add README.md // 文件添加到仓库
git add . // 不但可以跟单一文件，还可以跟通配符，更可以跟目录。一个点就把当前目录下所有未追踪的文件全部add了 
git commit -m "first commit" // 把文件提交到仓库
git remote add origin git@github.com:wangjiax9/practice.git // 关联远程仓库
git push -u origin master // 把本地库的所有内容推送到远程库上 
git clone ssh://xxx.git // 克隆库
git help //联机帮助
git log --oneline --left-right origin/master...<本地分支名称>
```



