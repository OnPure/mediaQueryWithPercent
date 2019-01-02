### 本项目是最常用的媒体查询方案在react框架中的实践，因为本人使用react较多。媒体查询方案因为其搭建方便，并且可实用性强，所以得到了非常普遍的应用，此项目仅作为模板和他人学习使用。

> 项目模仿**苏宁易购**的移动端页面，它本身就是基于media query的。

> 在此项目中使用**flex布局**，**media query**定义font-size，细节采用**百分比**的形式来实现各分辨率的兼容。


## 项目结构
> 本项目是基于create-react-app框架自己一步步搭建出来的，踩了很多坑，最多的就是版本不一致导致的编译错误，还找不到原因，mmp......

![普通进度条](https://github.com/OnPure/react-with-flexible/blob/master/static/images/structor.png)
> assets————存放字体<br/>
> build————webpack.base.conf.js、webpack.dev.conf.js、webpack.prod.conf.js<br/>
> dist————编译输出目录<br/>
> App.test.js————测试文件<br/>
> index.html————定义最重要的id：root，但是不要<meta name="viewport" content="width=device-width, initial-scale=1.0"> <br/>
> index.js————最重要的渲染js<br/>
> serviceWorker.js————create-react-app自带，默认关闭，我手贱开启了......<br/>
> src<br/>
>> component————组件<br/>
>> pages————页面<br/>
>> store————用于整合redux<br/>


## 技术栈

* React

> 1.classnames————合并class名，此处因为使用cssModules，所以为了合并local和普通css类名<br/>

> 2.支持ES6语法，支持箭头函数<br/>

> 3.px2rem————使用atom插件px2rem-plus对750px设计图进行px->rem的转换，如果你使用的不是atom，可以网上搜搜如何使用，sublime插件名叫px2rem<br/>

> 4.支持less和sass预编译css语言，使用cssModules对类名修饰<br/><br/><br/>



* webpack

> 1.使用webpack@3.11.0版本,webpack-dev-server@2.9.7，webpack-dev-server如果是3.x编译就会出错mmp......<br/>


> 2.HtmlWebpackPlugin————用于生产html入口文件，只要用webpack都会用这个插件吧......<br/>


> 3.支持热更新————HotModuleReplacementPlugin()<br/>


>> dev指令————package.json文件中webpack-dev-server --inline --progress --hot --config build/webpack.dev.conf.js<br/><br/><br/>


* swiper@4.4.6————最新版本<br/><br/><br/>



* iconfont————把阿里字体引入，使用unicode字符，支持修改颜色，给我这种不想自己ps图标的前端工程师开了一条捷径......<br/><br/><br/>

## 使用方法

* npm i

* npm run build

* npm run dev

* 大功告成

> 最终说一下，这篇文章都是我一个一个字打出来的，如果你路过觉得我写的不错，或者使用了我的项目结构，留个star吧！！！
> 
