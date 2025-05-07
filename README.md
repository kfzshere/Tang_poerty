# Tang Poetry
This is my study record of Tang poetry 
2025.5.7  

### **vscode远程ssh连接github注意事项**
#### **首次连接**
本地仓库首次连接 GitHub 远程仓库时
假设你已经在 GitHub 上新建了一个仓库，比如 https://github.com/用户名/仓库名.git
1. 初始化本地仓库
2. 添加远程仓库地址
3. 添加文件、提交
4. 推送到 GitHub（首次推送要指定分支，比如 main）
```sh
git init
git remote add origin git@github.com:yourusername/yourrepo.git
git add .
git commit -m "first commit"
git push -u origin main
```

#### **后续提交**
**1. 使用命令行**
```
git add .  
git commit -m "update"  
git push
```
**2. 使用拓展**
每次提交需打开SSH agent进程：  
```
Start-Service ssh-agent  
ssh-add C:\Users\13017\.ssh\id_rsa
```