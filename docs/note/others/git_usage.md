## Basic Usage
### Create Repositories
```shell
$ git init [project-name] 新建本地仓库
$ git clone [url] 将远程仓库克隆到本地仓库中
```
### Make Changes
```shell
$ git status 查看工作区待提交的已更改文件
$ git diff 比较暂存区和工作区文件的差异
$ git add [file] 将工作区文件至暂存区
$ git diff --staged 比较暂存区文件和上一文件版本的差异
$ git reset [file] 文件版本回退
$ git commit -m "[descriptive message]" 将暂存区文件添加至仓库中
```
### Group Changes
```shell
$ git branch 列出当前仓库的所有分支
$ git branch [branch-name] 新建分支
$ git checkout [branch-name] 跳转到指定分支
$ git checkout -b [branch-name] 新建分支并跳转到该分支
$ git merge [branch] 将特定分支合并到当前分支上
$ git branch -d [branch-name] 删除分支
```

### Refactor Filenames
```shell
$ git rm [file] 将文件从工作区和暂存区中删除
```

### Review History
```shell
$ git log 查看当前分支的版本历史
$ git log --follow [file] 查看文件版本历史（包括重命名）
$ git diff [first-branch] [second-branch] 比较两个分支的差异
$ git show [commit] 显示提交详情
```

### Redo Commits
```shell
$ git reset [--mixed | --soft | --hard] [commit]
--mixed或不带选项：移动HEAD指针，重置索引，不修改工作区，即工作区修改保留，撤销暂存和提交的更改
--soft：只移动HEAD指针，工作区和暂存区的修改都会保留，只撤销提交的更改
--hard：移动HEAD指针，重置索引，并修改工作区，工作区、暂存和提交的更改全部撤销
```

### Synchronize Changes
```shell
$ git fetch [bookmark] 将远程代码库下载到本地仓库中
$ git merge [bookmark]/[branch] 将更新合并到当前分支
$ git push [alias] [branch] 将本地分支的提交上传至GitHub
$ git pull 从远程仓库获取最新的提交记录，合并到当前的分支中，相当于git fetch + git merge
```

### Save Fragments
```shell
$ git stash 保存所有未提交的修改
$ git stash list 查看存储进度
$ git stash pop 恢复最近一次的保存
$ git stash drop 丢弃最近的存储
```

## Advanced Usage
**_TODO_**