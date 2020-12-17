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
git add readme.md
git commit -m "新增future1分支"
git checkout main 切换到main，不会把future1的更改更新到main中
切换到main后，在main中随便加入一段代码
git merge future1
发生冲突：main和future1各自有新提交的代码
提示错误：在main分支之前future分支提交了
手动解决冲突
再git add，git commit，git push完成操作


git log 查看每次commit情况

### 分支管理
git checkout -b dev
再次创建