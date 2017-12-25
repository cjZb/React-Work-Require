# React.js 前端开发预备知识
## React.js 来源
### 声明式
React 可以非常轻松地创建用户交互界面。为你应用的每一个状态设计简洁的视图，在数据改变时 React 也可以高效地更新渲染界面。

以声明式编写UI，可以让你的代码更加可靠，且方便调试。
###组件化
创建好拥有各自状态的组件，再由组件构成更加复杂的界面。

无需再用模版代码，通过使用JavaScript编写的组件你可以更好地传递数据，将应用状态和DOM拆分开来。
###一次学习，随处编写
无论你现在正在使用什么技术栈，你都可以随时引入 React 开发新特性。

React 也可以用作开发原生应用的框架 React Native.

## 环境搭建
### macOS

Homebrew

[Homebrew](https://brew.sh/), Mac系统的包管理器，用于安装NodeJS和一些其他必需的工具软件。
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Node

Homebrew 安装 [Node](https://nodejs.org)

```
brew install node
```

更换npm 镜像 (mac windows版)
```
npm config set registry https://registry.npm.taobao.org --global
npm config set disturl https://npm.taobao.org/dist --global
```

### Windows
Nodejs

win7  64位下载链接：http://download.csdn.net/detail/vichou_fa/9731294


1、安装node.js 安装路径 D:/nodejs
2、安装cnpm npm install -g cnpm registry=https://registry.npm.taobao.org
3、安装yarn npm install -g yarn
4、安装dva，npm install -g dva-cli
5、修改系统环境变量 
我的电脑 》 右键 》 属性》高级系统设置 》环境变量
PATH 值 修改为 D:/nodejs/node_global
重启电脑
6、检测是否安装成功
npm : npm -v
cnpm : cnpm -v
yarn: yarn -v
dva: dva -v
7、node安装过程中出现的错误解决办法
socket 错误
需要重置系统网络通信
netsh winsock reset
8、使用dva 创建项目
dva new 项目名称 例如 dva new myProject
创建项目过程中出现错误，进入到该项目的文件夹下面，把node_modules文件夹删除然后在cmd中进入到该项目的目录下执行 yarn install
9、创建成功以后 进入该项目文件夹下面 安装依赖
yarn install
10、启动 service 服务 查看项目页面
yarn start

/*yarn 和 npm 的区别*/
1、npm安装包的速度不够快，拉取的packages可能版本不同
2、 yarn 有一个锁定文件（yarn.lock）记录了被确切安装上的模块的版本号，每次只要增加一个模块，yarn就会创建（更新）yarn.lock这个文件，保证了每一次拉取一个项目依赖时用的是一样的模块版本
3、yarn 会优先安装yarn,lock中记录的依赖模块，没有这样的锁定文件时才会去安装packages.json中的依赖模块

/*修改npm 镜像文件地址*/
在node JS 根文件夹下面node_modules文件夹下面的npm 下面的npmrc文件里面修改成为
prefix=${APPDATA}\npm
registry =https://registry.npm.taobao.org

## require install software

[SourceTree](https://www.sourcetreeapp.com/)
[bearychat](https://bearychat.com/) [邀请链接](https://ylyj.bearychat.com/apply)
[webstorm](https://www.jetbrains.com/webstorm/)

[H5项目邀请链接](http://gitee.com/josin/YLYJ-YDB-H5/invite?invite_id=1514170385&inviter=josin&level=developer&secret_key=2a1a88019214533cb417442a5fc59fd5)






