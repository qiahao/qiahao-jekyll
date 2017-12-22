---
layout: post
title:  "vue项目实战!"
date:   2017-12-20 09:24:16 +0800
categories: vue
#permalink: /:categories/:year/:month/:day/vue-practice
excerpt: 
---
vue项目实战，本篇文章根据近期参与的Vue项目做的整理。主要内容包括项目结构规划，实践过程中需要注意的事项。

项目介绍：单页面类型 vue + iview pc 管理系统。自动化构建使用vue官网提供的脚手架，使用iview作为项目UI，请求使用axios。同时希望你对以下技术有所了解：

* vue-router: 单页面应用需要前端构建路由
* vuex: 应用全局存储
* webpack: vue脚手架使用webpack构建
* es6: 使用es6可以使代码简洁
* jsx: 很多情况下使用jsx 比使用 createElement() 简便
* lodash: 一个方便的工具库


**项目结构**

```
--project
build	// 自动化构建文件
config	// 自动化构建配置
dist	// 打包生成的生产环境代码 -- 默认没有，在终端执行大包代码：npm run build  生成
node_modules	 //node 环境依赖包
src 	// 包含所有开发环境的代码，所有的业务逻辑在这里开发、维护
static	// 静态文件夹，默认会直接拷贝该文件夹到 dist (打包后的文件)
-.babelrc   // babel 配置
-package.json // 包描述文件
-index.html   // 用作应用html初始化模版
```

项目的基本结构是在脚手架里就有的，以下为Vue官网安装脚手架的步骤：也可以直接查看[官网](https://cn.vuejs.org/v2/guide/installation.html)


```
# 安装vue
npm install vue
# 安装vue-cli 命令行工具
npm install --global vue-cli
# 创建一个基于 webpack 模板的新项目
vue init webpack my-project
# 安装依赖，走你
cd my-project
npm install
npm run dev
```

* vue init webpack my-project 是创建项目文件，要注意终端现在所在位置。
* npm install 从package.json安装依赖包
* npm run dev 运行开发环境脚本 —— 开发完打包 npm run build


**src**

到此为止项目初始化完成，现在重点描述下src文件夹 —— 开发的所有代码都应该放在这里

```

```




**router/index.js**

```
import Router from 'vue-router'
import routes from './routes'
let router = new Router({routes})

router.beforeEach((to, from, next) => {
    
})

export default router;

```

**main.js**


```
import Vue from 'vue'
import router from 'router'

var app = new Vue({
	data () {
		return {}
	},
	router,
	mixins: [],
	methods: {},
	created (){},
	mounted (){},
})

```


> 恰好没文化



