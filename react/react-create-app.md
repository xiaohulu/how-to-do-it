# 如何使用 react-create-app 脚手架

react-create-app 是开发 react 时常用的脚手架，具有以下功能：
1. 新建 react 项目；
2. 搭建开发环境，自带开发服务器；
3. 搭建测试环境，自动化运行测试用例；
4. 生成生产环境下的部署文件。

## React 项目结构

以下为 React 约定的项目结构

```
my-app
├── README.md
├── node_modules
├── package.json
├── .gitignore
├── public
│   └── favicon.ico
│   └── index.html
│   └── manifest.json
└── src
    └── App.css
    └── App.js
    └── App.test.js
    └── index.css
    └── index.js
    └── logo.svg
    └── registerServiceWorker.js
```

## 如何安装 `create-react-app`

使用 npm 全局安装 `create-react-app` 和 `yarn`
```sh
npm install -g create-react-app yarn
```

## 如何创建 React 项目

使用 `create-react-app` 创建一个 React 项目
```sh
npx create-react-app my-react-app
```

## 如何启动开发服务器
1. 进入 `my-react-app` 项目根目录，并启动 web 服务器
    ```sh
    cd my-react-app
    yarn start # 或者 npm start
    ```
1. 然后会自动打开电脑默认浏览器访问 http://localhost:3000/ ，成功后会显示 `Welcome to React` 字样

## 创建支持 TypeScript 语言的 React 项目

```sh
create-react-app my-react-app --scripts-version=react-scripts-ts
```