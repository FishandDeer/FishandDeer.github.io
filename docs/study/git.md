## 简述
Git 是一个开源的分布式版本控制系统，主要用于软件开发中对源代码进行版本管理。  
在团队协同开发中，项目的版本管理很重要。在个人开发中，通过git上传仓库，记录开发版本也很重要。   

- 实现跨区域多人协同开发
- 追踪和记载一个或者多个文件的历史记录
- 组织和保护你的源代码和文档
- 统计工作量
- 并行开发、提高开发效率
- 追踪记录整个软件的开发过程
- 减轻开发人员的负担、节省时间、同时降低人为错误

## 安装
这个网上教程非常多

## 使用方法
**1.初始化本地仓库**  
如果你是项目的创建者，进入项目目录从零开始创建一个本地仓库  
```bash
git init
```
---

**2.克隆远程仓库**  
如何是开发一个已经存在的项目，或者你已经在github或gitee上完成了仓库的创建，需要从远程仓库克隆项目到本地。  
```bash
git clone [远程仓库的url]
```
---

**3.创建分支**  
为避免所修改的代码对于源代码（主分支）产生影响，即隔离环境，需要创建分支，并在分支上进行开发。  
```bash
git checkout -b [分支名称]  #在当前分支的基础上创建一个新分支，并切换到该分支
```

```bash
git checkout [分支名称]  #切换分支
```

```bash
git branch  #查看全部分支，当前分支显示*号
```
**4.添加到暂存区**  
临时区域，用于暂存即将提交的内容，内容尚未被永久保存到本地仓库
```bash
git add [文件]
```
```bash
git add .  #提交全部代码
```
---

**5.提交到本地仓库**
将暂存区的内容永久保存到本地仓库
```bash
git commit -m "注释"
```
---

**6.合并分支**
开发完毕后，可以将分支的更改合并到主分支
```bash
git checkout main  # 切换回主分支
git merge [分支名称]  # 将其他分支的更改合并到主分支
```
---

**7.与远程仓库同步**
在开发的过程中，需要将本地的代码推送到远程，或者拉取远程的最新代码
```bash
git push origin [分支]  #将本地代码推送到远程仓库
git pull origin [分支]  #从远程仓库拉取最新的更改

