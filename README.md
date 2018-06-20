# GitTest

### 基本操作

+ git init：初始化仓库
+ git status：查看仓库的状态
+ git add：向暂存区添加文件
+ git commit：保存仓库的历史纪录
  + 记述简单提交信息
    + -m “提交信息”
  + 记述详细提交信息
    + 第一行：用一行文字简述提交的根本更改内容
    + 第二行：空行
    + 第三行以后：记述更改的原因和详细内容
  + 修改提交信息
    + git commit --amend
+ git log：查看提交日志
  + --pretty=short：只显示提交信息的第一行
  + -p：显示文件的改动
+ git diff：查看更改前后的差别
  + git diff HEAD：查看工作树和最新提交的差别
+ git branch：显示分支一览表
+ git checkout -b：创建、切换分支
  + git checkout -b feature-A
+ git merge：合并分支
  + git merge --no-ff：创建合并提交
+ git reflog：查看操作日志
+ git reset：回溯历史版本
  + git reset --hard 目标时间点的哈希值
+ git rebase：更改历史

#### 推送至远程仓库

+ git remote add origin git@github.com:QiuYe/xxxx.git
+ git push -u origin master
+ git checkout -b feature-A
+ git push -u origin feature-A

#### 从远程仓库获取

+ git clone git@github.com:QiuYe/xxxx.git
+ git branch -a
+ git checkout -b feature-A origin/feature-A
+ git diff
+ git commint -am "Add feature-A"
+ git push
+ git pull origin feature-A
+ 