# Tang Poetry
This is my study record of Tang poetry 
2025.5.7  

### **vscode远程ssh连接github注意事项**
#### **1. 首次连接**
本地仓库首次连接 GitHub 远程仓库时
假设你已经在 GitHub 上新建了一个仓库，比如 https://github.com/用户名/仓库名.git
1. 初始化本地仓库
2. 添加远程仓库地址
3. 添加文件、提交
4. 推送到 GitHub（首次推送要指定分支，比如 main）
```powershell
git init
git remote add origin git@github.com:yourusername/yourrepo.git
git add .
git commit -m "first commit"
git push -u origin main
```
#### **2. 后续提交**
**- 使用命令行**
```
git add .  
git commit -m "update"  
git push
```
**- 使用拓展**  
每次提交需打开SSH agent进程：  
```
Start-Service ssh-agent  
ssh-add C:\Users\13017\.ssh\id_rsa
```

#### Tips:推送(Push)与同步(Sync)  
**推送**：把本地仓库的提交上传到远程仓库，commit只会保存在本地
**同步**：是**拉取+推送**的组合。先拉到本地，再把本地未提交的推送到远程。