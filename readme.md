1、npm-node package manager
npm、cnpm、yarn

npm作用：自动下载东西；顺便下载依赖包；比较以前js开发，引入库，比如JQUERY等方式。

npm install 名字
npm uninstall 名字
比如：下载mysql包，npm install mysql
npm install 名字 --save 安装库，并保存在package.json中作为依赖库。

项目的package.json中配置依赖库，执行npm install命令，会根据依赖配置，自动下载依赖库。

npm -g install ... 
-g：表示全局安装，电脑上一次安装，以后都可以免重复安装。
没有-g是本地安装，只会在当前项目下。
？？-g的实验待验证

关于指定依赖库的版本号：
version 固定版本
>version 
>=version
<version
<=version 
~version 近似版本（一般版本号定义：主版本.次版本.build版本（天翻地覆.功能改进.小修补），近似版本一般时次版本不同，要保证主版本。）
^version 兼容版本
* 任何版本
a-b a->b之间版本
举例：
"1.0.0 - 3.999.999"
">=1.5.8 <2.0.0"
"3.x"
"latest"

npm version

npm上传自己的模块
需要先登陆一个账户；
创建一个自己的包。npm init，自动创建package。
npm publish上传包。更新后上传，需要升级版本号。

npm unpublish 名字 --force

npm adduser 注册一个账号。
npm login 登陆一个账号。
npm whoami，确认当前登陆的npm账号。

md文件

package.json文件中配置的script属性。
一般脚本的常用命令是start、stop、restart、test

package.json文件中配置的files属性。
本项目包还包含的文件。

淘宝镜像
cnpm
npm.taobao.org
npm install -g cnpm --registry=https://registry.npm.taobao.org
命令同npm，不能publish。

2、Vue2.0
关注视图层的前端框架，类似react，相比较Vue1.0引入虚拟Dom。

新建html文件的快捷键：!->TAB键

下载vue文件，通过npm install vue完成。