# JSX

是一种语法扩展，可以允许我们直接在js中写html代码。

```js
ReactDOM.render(
    <p>Hello React</p>,
    document.getElementById(element)
)

const title = <h1>React Learning</h1>
// html:<div id="box"></div>


// 将JSX元素渲染成DOM的方法
ReactDOM.render(title,document.getElementById('box'))
```

- JSX属性：

JSX的标签同样可以拥有自己的属性：

```js
const title = <h1 id='wrapper'>React Learning</h1>
const title = <h1 className='wrapper'>React Learning</h1>
```

- JSX嵌套

JSX的标签也可以像HTML一样互相嵌套，一般有嵌套解构的JSX元素在外面
我们习惯于为它加上一个小括号

```js
const title = (
    <div>
        <h1 className='head'>React Learning</h1>
        <p>Let's learn JSX</p>
    </div>
)
```

- JSX表达式

在JSX元素中，我们同样可以使用JavaScript表达式，

```js
function sayhi(name){
    return 'Hi,'+name;
}
const title = (
    <div>
        <h1 className='head'>React Learning</h1>
        <p>Let's learn JSX.<span>{sayhi('xin')}</span></p>
    </div>
)
```