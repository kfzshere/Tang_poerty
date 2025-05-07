# Tang Poetry
This is my study record of Tang poetry  

2025.5.7  

提交指令：  
git add .  
git commit -m "update"  
git push

  
如果是第一次：  
设置远程仓库地址为 SSH（如果你还没设置过）  
git remote set-url origin git@github.com:你的用户名/你的仓库.git  
git remote -v  # 应该看到 ssh 开头的地址  


每次提交需打开SSH agent进程：  
Start-Service ssh-agent  

ssh-add C:\Users\13017\.ssh\id_rsa
