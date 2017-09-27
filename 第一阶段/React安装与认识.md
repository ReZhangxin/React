# React认识与安装

## 环境安装

在终端输入 `npm install -g create-react-app`

然后执行   `create-react-app my-app`

进入项目中 `cd my-app`

执行       `npm start`

## 初次见面，よろしく

React 是一个采用声明式，高效而且灵活的用来构建用户界面的框架。

五大核心概念：

- 组件
- JSX
- Props & State
- 组件API
- 组件类型

### 什么是组件

组件就是能够像原生HTML一样输出特定的界面元素，而且还能包括一些元素相关逻辑功能的代码。

```js

class MyComponent extends React.Component {
    render(){
        return <p>Hello React</p>;
    }
}
```