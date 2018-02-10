webpack

Webpack的工作方式：把你的项目当做一个整体，通过一个给定的主文件（如：index.js），Webpack将从这个文件开始找到你的项目的所有依赖文件，使用loaders处理它们，最后打包为一个（或多个）浏览器可识别的JavaScript文件。


### 全局安装webpack

    npm install -g webpack
    

### 安装Webpack作为依赖包

    npm install --save-dev webpack


### 使用webpack构建本地服务器

    npm install --save-dev webpack-dev-server

### Babel

Babel其实是一个编译JavaScript的平台，它可以编译代码帮你达到以下目的：
让你能使用最新的JavaScript代码（ES6，ES7...），而不用管新标准是否被当前使用的浏览器完全支持；
让你能使用基于JavaScript进行了拓展的语言，比如React的JSX；

    npm install --save-dev babel-core babel-loader babel-preset-env babel-preset-react


### 安装 React 和 React-DOM

    npm install --save react react-dom

### 安装css loader

    npm install --save-dev style-loader css-loader

### CSS预处理器
允许使用类似于variables, nesting, mixins, inheritance等不存在于CSS中的特性来写CSS，
CSS预处理器可以将其转化为浏览器可识别的CSS语句常用的CSS 处理loaders:
Less Loader、Sass Loader、Stylus Loader
PostCSS为CSS代码自动添加适应不同浏览器的CSS前缀

    npm install --save-dev postcss-loader autoprefixer

### 插件（Plugins）
build文件夹下面生成了bundle.js和index.html
    npm install --save-dev html-webpack-plugin

Hot Module Replacement
允许你在修改组件代码后，自动刷新实时预览修改后的效果

    npm install --save-dev babel-plugin-react-transform react-transform-hmr


UglifyJsPlugin：压缩JS代码；
ExtractTextPlugin：分离CSS和JS文件
OccurenceOrder 和 UglifyJS plugins 都是内置插件，你需要做的只是安装其它非内置插件

    npm install --save-dev extract-text-webpack-plugin


改变文件内容后重新打包时，文件名不同而内容越来越多，去除build文件中的残余文件

    npm install clean-webpack-plugin --save-dev


### 启动项目：

	1、`npm start` 对项目进行打包
	2、`npm run server`启用本地的8080端服务器


cantact：ximelly@163.com