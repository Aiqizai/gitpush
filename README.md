how to check? open with index.html

#上传代码到github步骤

+ 首次配置仓库添加
  git config --global user.name "xiaoming"
  git config --global user.email "xm@sina.com"
+ 在项目目录右键打开 git bash, 创建(初始化)仓库 git init  
+ git add 命令把项目添加到仓库,（git add .把该目录下的所有文件添加到仓库，注意点是用空格隔开的）
+ git commit -m "first commit" 把项目提交到仓库(引号是提交的日志/这是对这次添加的东西的说明)
+ git remote add origin 复制的ssh地址, 与仓库建立连接 复制ssh地址,打开创建的仓库,复制仓库的ssh地址,
+ git push -u origin master, 把本地库的所有内容推送到远程仓库

#复制远程代码
+ git clone [url] 
+ url: 远程仓库的地址

#更新github上的代码
+ 项目目录右键打开 git bash
+ git pull 把已有的项目拉取下来
+ git status查看状态,可以查看是否有更新的地方
+ git add * --代表更新全部
+ git commit -m "更新说明"，commit只是提交到缓存区域
+ git pull(如果多人同时开发维护代码，得先拉取当前分支最新代码)
+ git push 推送代码
+ 回到github上刷新页面
