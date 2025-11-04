# Git 学习仓库

这是一个用于学习和练习 Git 版本控制的仓库。

## 仓库信息

- **仓库名称**: learngit
- **远程仓库**: git@github.com:286010056/learngit.git
- **默认分支**: main

## Git 学习指南

### 1. Git 基础概念

Git 是一个分布式版本控制系统，用于跟踪文件的变化。主要概念包括：

- **仓库 (Repository)**: 存储项目文件和版本历史的地方
- **提交 (Commit)**: 对文件变化的快照
- **分支 (Branch)**: 独立的工作线
- **远程仓库 (Remote)**: 存储在服务器上的仓库副本

### 2. 常用 Git 命令

#### 初始化与配置
```bash
# 初始化新仓库
git init

# 配置用户信息
git config --global user.name "你的名字"
git config --global user.email "你的邮箱"

# 查看配置
git config --list
```

#### 基本操作
```bash
# 查看仓库状态
git status

# 添加文件到暂存区
git add <文件名>
git add .  # 添加所有文件

# 提交更改
git commit -m "提交信息"

# 查看提交历史
git log
git log --oneline  # 简洁显示
```

#### 分支管理
```bash
# 创建新分支
git branch <分支名>

# 切换分支
git checkout <分支名>
git switch <分支名>  # Git 2.23+ 新命令

# 创建并切换分支
git checkout -b <分支名>
git switch -c <分支名>

# 合并分支
git merge <分支名>

# 删除分支
git branch -d <分支名>
```

#### 远程操作
```bash
# 克隆远程仓库
git clone <仓库地址>

# 添加远程仓库
git remote add origin <仓库地址>

# 推送更改
git push origin <分支名>

# 拉取更新
git pull origin <分支名>

# 查看远程仓库
git remote -v
```

### 3. 学习路径建议

#### 第一阶段：基础操作
1. 创建和提交文件
2. 查看提交历史
3. 理解工作区、暂存区和版本库

#### 第二阶段：分支管理
1. 创建和切换分支
2. 分支合并
3. 解决合并冲突

#### 第三阶段：远程协作
1. 与远程仓库同步
2. 推送和拉取代码
3. 团队协作流程

### 4. 实践练习

在这个仓库中，你可以尝试以下练习：

1. **基础提交练习**
   - 创建新文件并提交
   - 修改文件并查看差异
   - 回滚到之前的版本

2. **分支管理练习**
   - 创建功能分支开发新功能
   - 合并分支到主分支
   - 处理合并冲突

3. **远程操作练习**
   - 推送本地提交到远程仓库
   - 从远程仓库拉取更新
   - 协作开发流程

### 5. 常见问题解决

#### 撤销更改
```bash
# 撤销工作区的修改
git checkout -- <文件名>

# 撤销暂存区的修改
git reset HEAD <文件名>

# 撤销提交（谨慎使用）
git reset --soft HEAD~1  # 保留更改到暂存区
git reset --hard HEAD~1  # 完全撤销提交
```

#### 解决冲突
当合并出现冲突时：
1. 编辑冲突文件，解决冲突标记
2. 添加解决后的文件：`git add <文件名>`
3. 完成合并：`git commit`

### 6. 最佳实践

1. **提交信息规范**
   - 使用清晰的提交信息
   - 遵循约定式提交规范
   - 每次提交只完成一个明确的任务

2. **分支策略**
   - 主分支保持稳定
   - 功能分支独立开发
   - 定期同步远程仓库

3. **工作流程**
   - 频繁提交，小步快跑
   - 定期拉取远程更新
   - 及时解决冲突

## 资源推荐

- [Pro Git 书籍](https://git-scm.com/book/zh/v2) - 官方Git教程
- [Git 官方文档](https://git-scm.com/doc) - 完整的命令参考
- [GitHub Learning Lab](https://lab.github.com/) - 互动式学习

## 注意事项

- 在练习时，可以随意创建和删除分支
- 重要文件请做好备份
- 遇到问题可以查看Git的help文档：`git help <命令>`

---

*Happy Coding! 享受Git学习之旅！*
