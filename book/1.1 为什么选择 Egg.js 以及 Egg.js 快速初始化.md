## 为什么选择 Egg.js

- ~~因为懒~~

- Egg 2.x 底层基于 Koa 2.x，异步解决方案基于 async function，**可有效避免[callback hell](http://callbackhell.com) 和 [release zalgo](https://oren.github.io/blog/zalgo.html)**

- 性能优异，框架稳定

- [部署简单](https://eggjs.org/zh-cn/core/deployment.html#部署)

- [官方文档](https://eggjs.org/zh-cn/intro/quickstart.html)完善，**基础功能丰富**

- **安全问题**：对于像我这种初学者而言，非常容易忽视或者难以防范安全威胁。**Egg 内置了对于常见安全风险的解决方案，并且有十分友好的[文档说明](https://eggjs.org/zh-cn/core/security.html)**


## 快速初始化

直接使用脚手架，只需几条简单指令，即可快速生成项目:

```shell
$ npm i egg-init -g
$ egg-init egg-example --type=simple
$ cd egg-example
$ npm i
```

其中egg-example为项目名称  
在初始化过程中，会询问cookie security keys，详情请参考[Cookie 秘钥](https://eggjs.org/zh-cn/core/cookie-and-session.html#cookie-秘钥)  
以下是脚手架目录结构

```shell
.
├── README.md
├── README.zh-CN.md
├── app
│   ├── controller
│   │   └── home.js
│   └── router.js
├── config
│   ├── config.default.js
│   └── plugin.js
├── package.json
└── test
    └── app
        └── controller
            └── home.test.js
```

使用 `npm run dev` 启动项目  
访问 localhost:7001 看到 hi, egg 表示初始化成功
