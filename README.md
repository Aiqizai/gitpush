## 上传代码到github步骤

+ 首次配置仓库添加
  1.git config --global user.name "xiaoming" /
  2.git config --global user.email "xm@sina.com"
+ 在项目目录右键打开 git bash, 创建(初始化)仓库 git init  
+ git add 命令把项目添加到仓库,（git add .把该目录下的所有文件添加到仓库，注意点是用空格隔开的）
+ git commit -m "first commit" 把项目提交到仓库(引号是提交的日志/这是对这次添加的东西的说明)
+ git remote add origin 复制的ssh地址, 与仓库建立连接 复制ssh地址,打开创建的仓库,复制仓库的ssh地址,
+ git push -u origin master, 把本地库的所有内容推送到远程仓库

#如果想把这个项目要上传到其他仓库
+ git remote rm origin // 先移除本地关联仓库
+ git remote add origin git@github.com/example.git // 添加线上仓库
+ git push -u origin master // 注意：更改后，第一次上传需要指定 origin


## 复制远程代码
+ 新建文件夹存放克隆的项目
+ 在文件夹内部右键打开 git bash
+ git clone [url] 
+ url: 远程仓库的地址

## 更新github上的代码
+ 项目目录右键打开 git bash
+ git clone 把已有的项目克隆下来 
+ git status查看状态,可以查看是否有更新的地方
+ git add * --代表更新全部
+ git commit -m "更新说明"，commit只是提交到缓存区域
+ git pull(如果多人同时开发维护代码，得先拉取当前分支最新代码)
+ git push 推送代码
+ 回到github上刷新页面

## 更改远程仓库地址
+ git remote -v   //查看fetch和push路径
+ git remote set-url origin "https://github.com/xxx/xxx.git"  //修改远程路径

## 个人操作
- 在项目文件夹右键打开 git bash
- git pull
- git status查看状态,可以查看是否有更新的地方
- git add * --代表更新全部
- git commit -m "更新说明"，commit只是提交到缓存区域
- git push
