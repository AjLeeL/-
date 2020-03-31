# 通用项目结构

!>``` 数据中心 ``` 和 ``` 数据市场 ``` 都是基于 vue-cli3.0脚手架构建，目录说明如下

```
├── *.config.js             配置
    ├── public/                 资源目录，第三方无需编译的资源
    ├── src/
    │   ├── assets/             资源目录，字体、图标、css、less等
    │   │     ├── css/
    │   │     │    ├── common   全局公用样式
    │   │     │    └── reset    样式重置
    │   │     ├── fonts/        iconfont 字体图标ui库
    │   │     ├── images/       图片类
    │   ├── components/         项目组件，项目内模块相关的组件
    │   │     ├── common        主框架ui公用组件 项目登录、导航相关
    │   │     └── dialog        主框架ui公用弹框组件入口
    │   ├── utils/              项目数据处理全局公用方法等...
    │   ├── views/              模块页面，包含各个模块独立路由配置及模块相关组件
    │   │     └──collectPlatform/   模块N...
    │   ├── router/            主路由配置
    │   │    |──collect        采集平台
    │   │    |──config         公用平台
    │   │    |──govern         质量平台
    │   │    |──share          共享平台
    │   │    |──system         系统设置
    │   └── store/             vuex相关
    ├── App.vue                 
    ├── main.js                 入口
    ├── common.js               全局公用接口公共方法（获取Echart数据配置）
    ├── global.js               全局挂载公共方法、下载等
    └──.env*                    环境配置
```