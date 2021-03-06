# 使用[Webpack DllPlugin](https://webpack.js.org/plugins/dll-plugin/)打包出来的dll 基本上等于talent-libs

目前包含进去的库有：

* react
* react-dom
* prop-types
* react-router-dom
* redux
* react-redux
* react-transition-group
* immutable

使用dll方式引入基础库到项目中可以极大的增加项目打包的速度，也能很好的利用浏览器的缓存机制， 减少页面的渲染时间

# 发版

本项目已经接入标准的ci流程，在master分支push后会出发自动构建和发版，将构建后的文件同步到服务器

流程：

更改依赖版本号，删除node_modules 重新install，更改版本号，完善changeLog ,npm publish

push到beisen远程服务器 触发ci，将文件同步到线上服务器

# 引入

本dll的线上服务器地址是：http://stnew03.beisen.com/ux/upaas/@talentui/dll-react/release/dist/dll-react-{版本号}.min.js 

# changeLog:

# 16.1.3

在react16.1.0版本的基础上去掉`immutable`依赖

[远程文件地址](http://stnew03.beisen.com/ux/upaas/@talentui/dll-react/release/dist/dll-react-16.1.3.min.js)

本次版本的依赖有：
* react
* react-dom
* prop-types
* react-router-dom
* redux
* react-redux
* react-transition-group


# 16.1.2

修改项目内的依赖关系，将依赖放到devDependencies 以及 peerDependencies，项目内的库及其版本都未改动

[远程文件地址](http://stnew03.beisen.com/ux/upaas/@talentui/dll-react/release/dist/dll-react-16.1.1.min.js)

本次版本的依赖有：
* react
* react-dom
* prop-types
* react-router-dom
* redux
* react-redux
* react-transition-group
* immutable

## 16.1.1[![依赖有问题 停用](http://badges.github.io/stability-badges/dist/deprecated.svg)](http://github.com/badges/stability-badges)
在react16.1.0版本上加上immutable依赖

**依赖有问题，停用**

本次版本的依赖有：
* react
* react-dom
* prop-types
* react-router-dom
* redux
* react-redux
* react-transition-group
* immutable

## 16.1.0[![依赖有问题 停用](http://badges.github.io/stability-badges/dist/deprecated.svg)](http://github.com/badges/stability-badges)

**依赖有问题，停用**

升级react 和 react-dom到16.1.0， 删除immutable依赖

本次版本的依赖有：
* react
* react-dom
* prop-types
* react-router-dom
* redux
* react-redux
* react-transition-group

## 15.6.1

打包react 15版本的dll , 并处理package.json内的依赖关系

[远程文件地址](http://stnew03.beisen.com/ux/upaas/@talentui/dll-react/release/dist/dll-react-15.6.1.min.js)

本次版本的依赖有：
* react
* react-dom
* prop-types
* react-router-dom
* redux
* react-redux
* react-transition-group
* immutable