git init
git add 文件    如果不加点则仅提交该文件
git remote add git-learn https://github.com/even-lq/git-learn.git
git push git-learn
git push --set-upstream git-learn master 设置master分支，并把git-learn放到该分支


点击vscode左下角创建新的分支
git branch 查看本地分支

### 新的方法

拉取仓库 git clone https://github.com/even-lq/git-learn.git
切换分支，如果没有就创建并切换到该分支 git checkout -b dev
git add readme.md
测试分支 git commit -m 'branch test'
切换分支 git checkout main
查看分支 git branch
合并分支 git merge dev 在当前分支下合并dev分支
删除分支 git branch -d dev



### 冲突处理
git checkout -b future1
git branch
发生冲突