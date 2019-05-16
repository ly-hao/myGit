# git管理仓库
## 1、本地仓库管理
* 建立忽略文件
  * .gitignore
  * 一定要在add之前
* git init
* git add ./*/-A
* git commit -m 'xxx'

## 2、远程仓库管理
* 新建远程仓库

## 3、本地和远程的使用
* 本地仓库和远程仓库关联
  * git remote add origin xxxx
* 本地仓库提交代码到远程仓库去
  * git push origin master
* 本地仓库更新远程仓库最新的代码
  * git pull origin master
* 本地仓库需要拉取远程仓库的dev分支内容
  * 注意：默认clone下来是master分支
  * git fetch origin dev1:dev2  拉取远程仓库dev1分支的内容到本地的dev2分支上

* git插件（Chrome插件）
  * octotree

##webstorm的配置node路径
  file --> setting  --> 搜索node

## 通过某个工具将commonjs模块化语法编译成浏览器能识别的js语法
 使用browserify插件解决html不认模块化代码
  #npm i browserify -g
  #browserify ./app.js -o ./built.js
  #app.js 模块化文件  --built.js 打包

##一、常用命令：

    mkdir XX：创建一个空目录 XX指目录名
    pwd：显示当前目录的路经
    cat xx：查看xx文件内容
    git init：把当前的目录变成可以管理的git仓库，生成隐藏的.git文件夹
    git add xx：把xx文件添加到暂存区
    git commit -m “xx”：提交文件 -m后面的是注释
    git status：查看仓库状态
    git log：查看历史记录
    git reset --hard HEAD^：往上回退一个版本
    git reflog：查看历史记录的版本号id
    git checkout -- xx：把xx文件在工作区的修改全部撤销
    git rm xx：删除xx文件 之后要commit
    git remote add origin https://github.com/xxxxx/a.git 关联一个远程库
    git push -u（第一次要用-u，以后不用）origin master：把当前master分支              推送到远程库
    git clone https://github.com/xxxxx   从远程库中克隆
    git checkout -b dev：创建dev分支 并切换到dev分支上
    git branch：查看当前所有的分支
    git checkout master：切换回master分支
    git merge dev：在当前分支合并dev分支
    git branch -d dev：删除dev分支
    git branch xxx：创建分支xxx
    git remote：查看远程库信息
    git remote -v查看远程库的详细信息
    git pull origin master 将远程库的更新拉取到本地来
    git push origin master：git会把master分支推送到远程库对应的分支上
