#### 1.下载安装

- windows： [Git (git-scm.com)](https://git-scm.com/)

- ubuntu：apt-get install git
- centOs：yum install git

#### 2.简单配置

```bash
git config --global user.name "melanchozy"
git config --global user.email "wbszzy@qq.com"

git config --list
```

#### 3.简单操作

`git config <key>`： 来检查 Git 的某一项配置

```bash
git config user.name
melanchozy
```

#### 4.github使用

1. 创建密钥

   本地 Git Bash

   ```sh
   ssh-keygen -t ed25519 -C "wbszzy@.com"
   ```

   密钥对位于 `C:\Users\zy\.ssh`.

2. github配置 

   setting 

   ​	Access 

   ​		SSH and GPG keys

   ​			New SSH key

   复制公钥内容粘贴。

3. 测试

   ```sh
   ssh -T git@github.com
   ```

4. 本地建立仓库

   ```sh
   git init
   ```

5. 连接远程仓库

   ```sh
   git remote add origin https://github.com/melanchozy/leetcode_daily.git
   ```

6. 提交

   ```sh
   git add *
   git commit -m "first commit"
   git push -u origin master
   ```

#### *tips

1. 修改仓库指向

   ```bash
   git remote set-url origin git@github.com:melanchozy/git-notes.git
   ```

