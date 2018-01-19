单文件组件

### 1. .vue文件
    .vue文件，称为单文件组件，是Vue.js自定义的一种文件格式，一个.vue文件就是一个单独的组件，在文件内封装了组件相关的代码：html、css、js

    .vue文件由三部分组成：<template>、<style>、<script>
        <template>
            html
        </template>

        <style>
            css
        </style>

        <script>
            js
        </script>

### 2. vue-loader  
    浏览器本身并不认为.vue文件，所以必须对.vue文件进行加载解析，此时需要vue-loader
    类似的loader还有许多，如：html-loader、css-loader、style-loader、babel-loader等
    需要注意的是vue-loader是基于webpack的     

### 3. webpack
    webpack是一个前端资源模板化加载器和打包工具，它能够把各种资源都作为模块来使用和处理
    实际上，webpack是通过不同的loader将这些资源加载后打包，然后输出打包后文件 
    简单来说，webpack就是一个模块加载器，所有资源都可以作为模块来加载，最后打包输出

    [官网](http://webpack.github.io/)     

    webpack版本：v1.x v2.x

    webpack有一个核心配置文件：webpack.config.js，必须放在项目根目录下

### 4. 示例，步骤：
    
#### 4.1 创建项目，目录结构 如下：
webpack-demo
    |-index.html
    |-main.js   入口文件       
    |-App.vue   vue文件
    |-package.json  工程文件
    |-webpack.config.js  webpack配置文件
    |-.babelrc   Babel配置文件

### 4.2 编写App.vue

### 4.3 安装相关模板    
    cnpm install vue -S

    cnpm install webpack -D
    cnpm install webpack-dev-server -D

    cnpm install vue-loader -D
    cnpm install vue-html-loader -D
    cnpm install css-loader -D
    cnpm install vue-style-loader -D
    cnpm install file-loader -D

    cnpm install babel-loader -D
    cnpm install babel-core -D
    cnpm install babel-preset-env -D  //根据配置的运行环境自动启用需要的babel插件
    cnpm install vue-template-compiler -D //预编译模板

    合并：cnpm install -D webpack webpack-dev-server vue-loader vue-html-loader css-loader vue-style-loader file-loader babel-loader babel-core babel-preset-env  vue-template-compiler

### 4.4 编写main.js    

### 4.5 编写webpack.config.js

### 4.6 编写.babelrc    

### 4.7 编写package.json

### 4.8 运行测试
    npm run dev    
