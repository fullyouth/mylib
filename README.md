# [mylib](https://github.com/fullyouth/mylib)
[![](https://img.shields.io/badge/Powered%20by-jslib%20base-brightgreen.svg)](https://github.com/yanhaijing/jslib-base)
[![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/fullyouth/mylib/blob/master/LICENSE)
[![CI](https://github.com/fullyouth/mylib/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/fullyouth/mylib/actions/workflows/ci.yml)
[![npm](https://img.shields.io/badge/npm-0.1.0-orange.svg)](https://www.npmjs.com/package/mylib)
[![NPM downloads](http://img.shields.io/npm/dm/mylib.svg?style=flat-square)](http://www.npmtrends.com/mylib)
[![Percentage of issues still open](http://isitmaintained.com/badge/open/fullyouth/mylib.svg)](http://isitmaintained.com/project/fullyouth/mylib "Percentage of issues still open")

最好用的 `JS|TS` 第三方库脚手架

## :star: 特性

- 支持ES6+或TypeScript编写源码，编译生成生产代码
- 多环境支持（支持浏览器原生，支持AMD，CMD，支持Webpack，Rollup，fis等，支持Node）
- 集成[jsmini](https://github.com/jsmini)

> 注意: 如果不同时使用 `export` 与 `export default` 可打开 `legacy模式`，`legacy模式` 下的模块系统可以兼容 `ie6-8`，见rollup配置文件

## :pill: 兼容性
单元测试保证支持如下环境：

| IE   | CH   | FF   | SF   | OP   | IOS  | Android   | Node  |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- | ----- |
| 11+   | 100+ | 100+  | 16+   | 100+  | 10.3+   | 4.1+   | 14+ |

**注意：编译代码依赖ES5环境，对于ie6-8需要引入[es5-shim](http://github.com/es-shims/es5-shim/)才可以兼容，可以查看[demo/demo-global.html](./demo/demo-global.html)中的例子**

## :open_file_folder: 目录介绍

```
.
├── demo 使用demo
├── dist 编译产出代码
├── doc 项目文档
├── src 源代码目录
├── test 单元测试
├── CHANGELOG.md 变更日志
└── TODO.md 计划功能
```

## :rocket: 使用者指南

通过npm下载安装代码

```bash
$ npm install --save mylib
```

如果你是node环境

```js
const mylib = require('mylib');
```

如果你是webpack等环境

```js
import mylib from 'mylib';
```

如果你是浏览器环境

```html
<script src="node_modules/mylib/dist/index.aio.js"></script>
```

## :bookmark_tabs: 文档
[API](./doc/api.md)

## :kissing_heart: 贡献者指南
首次运行需要先安装依赖

```bash
$ npm install
```

一键打包生成生产代码

```bash
$ npm run build
```

运行单元测试:

```bash
$ npm test
```

> 注意：浏览器环境需要手动测试，位于`test/browser`

修改 package.json 中的版本号，修改 README.md 中的版本号，修改 CHANGELOG.md，然后发布新版

```bash
$ npm run release
```

将新版本发布到npm

```bash
$ npm publish
```

## 贡献者列表

[contributors](https://github.com/fullyouth/mylib/graphs/contributors)

## :gear: 更新日志
[CHANGELOG.md](./CHANGELOG.md)

## :airplane: 计划列表
[TODO.md](./TODO.md)