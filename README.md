# mpvue-engineering

> --- 基于mpVue小程序工程化实践 ---

## 项目目录

``` bash
├─build  webpack构建目录
├─config  webpack配置目录
├─dist  打包目录
│  └─wx  环境目录
│      └─demo  项目目录
│         ├─common
│         ├─components
│         ├─pages
│         ├─projects
│         │  └─demo
│         │     ├─components
│         │     └─pages
│         └─static
│         └─app.js
│         └─app.json
│         └─app.wxss
├─src  开发目录
│  ├─apis  通用接口目录
│  ├─assets  通用静态文件目录
│  ├─components  通用组件目录
│  ├─config  通用配置目录
│  ├─global  全局目录
│  │  ├─css
│  │  └─js
│  ├─projects  项目总目录
│  │  └─demo  项目目录
│  │     ├─apis  项目接口目录
│  │     ├─components  项目组件目录
│  │     ├─config  项目配置目录
│  │     ├─mock  mock目录
│  │     ├─store  Vuex目录
│  │     ├─pages  项目页面目录
│  │     │  └─index  index页面目录
│  │     │     ├─index.vue
│  │     │     └─main.js
│  │     └─utils  项目工具目录
│  └─utils  通用工具目录
└─static  通用静态文件目录
```

## 使用模板

```
npm install -g @vue/cli-init
vue init lindingfeng/engineering#mpvue projectName

or

git clone https://github.com/lindingfeng/mpvue-engineering.git
```

## 开发

``` bash
# 安装依赖
yarn install

# 开发时构建
npm run dev demo

# 打包构建
npm run build demo

# 指定平台的开发时构建(微信、百度、头条、支付宝)
npm run dev:wx
npm run dev:swan
npm run dev:tt
npm run dev:my

# 指定平台的打包构建
npm run build:wx
npm run build:swan
npm run build:tt
npm run build:my

# 生成 bundle 分析报告
npm run build demo --report
```

## 微信小程序UI框架

### [Vant-Weapp](https://youzan.github.io/vant-weapp/#/intro) 
```JavaScript
--- main.json ---
// 引入Vant-Weapp组件
{
  "usingComponents": {
    "van-button": "/static/vant-weapp/dist/button/index"
  }
}

--- index.vue ---  
<template>
  <div class="index-page">
    <!-- 使用Vant-Weapp组件 -->
    <van-button type="primary">主要按钮</van-button>
  </div>
</template>
```
### Tip: 1、如果不希望使用UI框架，可以将static目录下的vant-weapp文件夹删除即可!
