基于 express + mongodb 搭建的一个博客论坛系统

第三方包主要涉及 swig模版，cookies，mongoose 等

算是一个练手项目，扩展一下后台相关，例如cookie，模版引擎，数据库等知识

功能不定时添加

----

----

大致目录结构为：

```js
├── app.js          入口文件
├── db              数据库存储目录
├── models          数据库模型文件目录
│   ├── User.js
│   └── ...
├── routers         路由文件
│   ├── admin.js
│   ├── main.js
│   ├── api.js
│   └── ...
├── schemas         数据库视图文件目录
│   ├── user.js
│   └── ...
├── node_modules/
├── package.json
├── public          公共文件目录
│   ├── img
│   ├── css
│   ├── js
│   └── ...
└── views
    ├── user.html   模版目录
    ├── index.html
    └── ...
```

----

----

## Use

```js
npm install
```

然后开启 mongodb 服务

```js
mongod --dbpath "项目所在文件夹下的 ==> \db" --port 27018
```

mongodb 默认的为 27017 端口，可能会被占用，故选用 27018 端口

然后访问 ```localhost:3000```

----

----

2017.05.14

后台逻辑处理，添加文章列表后台管理功能（增删改查）


2017.05.13

后台逻辑处理，添加后台导航分类管理相关逻辑（增删改查）

前台获取导航分类数据用以展示

2017.05.12

添加用户登录注册，调用 cookie 保存登录状态

2017.05.11 

整体目录结构搭建，基本路由走通，即前端发送请求，后台响应处理




待续...



