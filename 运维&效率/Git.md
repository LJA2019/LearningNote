```
// 配置用户信息，应用于所有本地仓库
git config --global "user.name"
git config --global "user.email" // 仅用作标识用户

// 生成SSH Key
ssh-keygen -t rsa -C "user.email"  // 会提示生成的ssh key存储的地址


// 初始化仓库
git init

// 或者克隆远程仓库
git clone <远程仓库名>

// 手动建立分支追踪
git branch --set-upstream-to=origin/<远程分支名> <本地分支名>

// 查看本地分支与远程分支的追踪关系:   * main   abc1234 [origin/main] 最新提交描述
git branch -vv


// 添加文件到暂存区
git add .

// 添加单个文件
git add <文件名>

// 查看暂存状态
git status

// 提交暂存区内容到本地仓库
git commit -m "提交描述"

// 跳过暂存直接提交   -a参数直接将工作区修改提交到本地仓库（无需git add）
git commit -a -m "提交描述"
```

