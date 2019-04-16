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
  **npm i browserify -g
  **browserify ./app.js -o ./built.js
  --app.js 模块化文件  --built.js 打包文件