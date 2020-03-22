**# react 脚手架**

**## 创建项目并启动**

\1. 首先基于 npm 在全局安装 create-react-app

\- npm install -g create-react-app

  \2. 在指定目录中创建一个 react 项目工程

\- create-react-app my-app

  \3. 进入到指定的项目文件，启动项目

\- cd my-app

\- npm start 或者 \$ yarn start 启动(前提是在全局安装了 yarn)

**## 脚手架生产的结构目录介绍**

\- my-app

\- |--build //构建目录，遵循发布系统规范

\- | |-- index.html //静态页面

\- | |-- static //资源文件

\- |

\- |-- node_modules //项目组件文件夹：所有安装的组件都在这

\- |

\- |--src //源码目录

\- | |--index.js //入口文件(还生成了其它的文件，但是没啥用，我们可以直接的删除掉)

\- |

\- |--public //静态页面目录

\- | |--index.html //主页面(还生成了其它的文件，但是没啥用，我们可以直接的删除掉)

\- |

\- |-- .gitignore //git 提交的忽略文件，我们一般还需要再手动增加.idea(通过 webstorm 编辑工具进行开发，生成的文件)

\- |--package.json //项目依赖项及项目基础信息

\- |--README.md //项目描述

\- |-- ......

\- ├─ config

\- | ├─ paths.js 包含 n 个本地文件/目录绝对路径

\- | ├─ webpack.config.js 生产/开发环境下 webpack 主要配置文件

\- | └─ webpack.devServer.js devServer 的配置

\- ├─ package-lock.json

\- ├─ package.json

\- ├─ public

\- | └─ index.html

\- ├─ scripts

\- | ├─ build.js 运行 yarn build 指令实际启动的文件

\- | └─ start.js 运行 yarn start 指令实际启动的文件

\- └─ src

\- ├─ App.css

\- ├─ App.jsx

\- └─ index.js

**### 生成的 package.json**

**### 可执行脚本注释:**

\- npm run start 启动服务，自动编译项目，可以实现边开发，边自动编译刷新，看到最新开发的效果

\-

\- npm run build 把项目整体进行编译，最后再 build 目录中生成项目编译后的文件，我们上传服务器的就是这些文件

\-

\- npm run test 使用 Jest 作为测试运行程序（不常用）

\-

\- npm run eject 下文具体介绍使用

\-

\- 当然以上操作也可以基于 yarn 来完成

```
$yarn eject或者npm run eject 此命令执行完成不可逆转(慎重使用)
```