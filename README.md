# Front-end
前端面试题整理
## 一、HTML
## 二、JavaScript
### Vue
### React
### Webpack
### JavaScript
-------
1、下面执行的函数输出是多少？

```javascript
function Foo() {
	getName = function () { alert(1) };
	return this;
};
Foo.getName = function () { alert(2) };
Foo.prototype.getName = function () { alert(3) };
var getName = function () { alert(4) };
function getName() { alert(5) };

Foo.getName(); //2
getName(); //4
Foo().getName(); //1
getName(); //1
new Foo.getName(); //2
new Foo().getName(); //3
new new Foo().getName(); //3
```
[详细介绍](http://www.jb51.net/article/79461.htm)

2、下面执行的函数输出是多少？

```javascript
function outerFun() {
	var a = 0;
	function innerFun() {
		a++;
		alert(a);
	}
	return innerFun;
}

var obj = outerFun();
obj(); //1
obj(); //2
var obj2 = outerFun();
obj2(); //1
obj2(); //2
```
[详细介绍](http://www.jb51.net/article/24101.htm)
## 三、CSS


