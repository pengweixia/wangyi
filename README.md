## 基于react+mobx实现的web音乐app

接口地址：[网易云音乐 API](https://github.com/Binaryify/NeteaseCloudMusicApi)
<hr/>
前端React+后端NodeJS（网易云音乐的官方接口）



### 技术栈

 - react 
 - react-router
 - mobx（基于flux架构的思想的一个实现的机制，跟redux是一样的，解决state的问题，关于数据的问题）
 - fetch（用来访问后端的API接口的）
 - antd-mobile （ant是一个react的UI界面库，是阿里蚂蚁金服这个团队编写的）
 - better-scroll（组件）
 - ES6（必须的）
 - less（样式编译器）

项目由`create-react-app`脚手架搭建，并用`react-app-rewired`进行扩展了配置（`react-app-rewired`高版本的配置方法会改变，所以我用的是`react-app-rewired@2.0.2-next.0`）

<br/>
### 实现的功能
- [x] 歌单页、推荐页、歌手页、排行榜
- [x] 搜索功能
- [x] 播放器（前进、后退、暂停、播放、喜欢）
- [x] 歌词功能
- [x] 视频播放功能
- [x] 上拉加载更多功能
 ...
<br/>

### 目录结构（src）

```javascript
├── assets                                     # 资源文件，包括icon、less公共文件                    
├── components                                 # 自定义组件
├── home                                       # 首页、包括侧边栏和主页面
├── pages                                      # 路由跳转的页面
├── store                                      # 全局store
├── utils                                      # 工具函数                   
```

<br/>

### 运行本项目



1. 先运行后端的项目，进入项目并安装依赖

```shell
cd NeteaseCloudMusicApi
cnpm install 
node app.js
```

​	接口项目以8000端口启动(可在app.js中修改启动端口)

2. 进入项目并安装依赖然后运行项目

```shell
cd react-music-master
npm install -g yarn  #如果你没有装yarn命令，需要安装一下，否则会报错
yarn install 
yarn start
```










