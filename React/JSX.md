#### 基础知识

`JSX`： JavaScript and HTML（XML）把 `JS` 和 `HTML` 标签混合在一起。

```js
import React from 'react';  // React语法的核心
import ReactDOM from 'react-dom/client';  // 视图渲染的核心

import '@/index.less'

// 获取页面中id为root的容器，作为根容器
const root = ReactDOM.createRoot(document.getElementById('root'));

let text = 'Hello World!!!';
// 基于render方法渲染我们编写的视图，把渲染后的内容全部插入到页面root元素中
root.render(
  <div>{ text }</div>
);
```

在 HTML 中嵌入 JS 表达式，需要基于 `{}` 胡子语法。

每一个构建的视图，只能有一个根节点。出现多个根节点会报错，需要再用 `React` 提供的一个特殊的标签 `<></>` React.Fragment 空文档标记标签 包裹，且不会占据 `HTML` 的层级结构。

#### VSCode如何支持JSX语法

只需把文件后缀名改成 `.jxs` ，这样 `JS` 文件就能支持 `JSX` 语法了。

#### 具体应用

