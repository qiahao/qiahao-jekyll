---
layout: post
title:  "Welcome to vue!"
date:   2017-12-20 09:24:16 +0800
categories: vue
<!-- permalink: page -->
---

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