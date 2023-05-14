# 项目启动

```bash
git clone
cd react_demo
npm i
npm start
```

# 项目变更

## 1. 调整项目结构

### 1.1 删除文件

使用 react-create-app 即 react 脚手架创建后的项目结构如下所示：

- react_demo
  - node_moudles
  - public
    - favicon.ico
    - index.html
    - logo192.png
    - logo512.png
    - manifest.json
    - robots.txt
  - src
    - App.css
    - App.js
    - App.test.js
    - index.css
    - index.js
    - logo.svg
    - reportWebVitals.js
    - setupTest.js
  - .gitignore
  - package.json
  - package-lock.json
  - README.md

删除一些文件精简为如下所示：

- react_demo
  - node_moudles
  - public
    - favicon.ico
    - index.html
  - src
    - App.js
  - .gitignore
  - package.json
  - package-lock.json
  - README.md

### 1.2 创建通用目录结构

项目目录结构可根据项目实际灵活制定，创建如下所示的通用目录结构：

- react_demo
  - node_moudles
  - public
    - favicon.ico         <-- 网页图标
    - index.html          <-- HTML页模板
  - src
    - common              <-- 全局公用目录
      - fonts             <-- 字体文件目录
      - images            <-- 图片文件目录
      - js                <-- 公用js文件目录
      - style             <-- 公用样式文件目录
        - frame.css       <-- 全局公用样式，import其它css
        - reset.css       <-- 清零样式
        - global.css      <-- 全局公用样式
    - components          <-- 公共模块组件目录
      - header            <-- 头部导航模块
        - index.js        <-- header主文件
        - header.css      <-- header样式文件
      - ......            <-- 其它模块
    - pages               <-- 页面组件目录
      - home              <-- home页目录
        - index.js        <-- home页主文件
        - home.css        <-- home页样式文件
      - login             <-- login页目录
        - index.js        <-- login页主文件
        - login.css       <-- login页样式文件
      - ......            <-- 其它页面
    - App.js              <-- 项目主模块
    - index.js            <-- 项目入口文件
  - .gitignore
  - package.json
  - package-lock.json
  - README.md
