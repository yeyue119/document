## 方法

### close

> 销毁

```javascript
var navigator = weex.requireModule("navigator");
navigator.close({}, (event) => {
  console.log("callback: ", event);
});
```

### push

> 入栈

```javascript
var navigator = weex.requireModule("navigator");
navigator.push(
  {
    url: "http://dotwe.org/raw/dist/519962541fcf6acd911986357ad9c2ed.js",
    animated: "true",
  },
  (event) => {
    console.log("callback: ", event);
  }
);
```

### pop

> 出栈

```javascript
var navigator = weex.requireModule("navigator");
navigator.pop(
  {
    animated: "true",
  },
  (event) => {
    console.log("callback: ", event);
  }
);
```

### popPages

> 出栈(传参层级数目)

```javascript
var navigator = weex.requireModule("navigator");
navigator.popPages(
  2, // 后退2步
  (event) => {
    console.log("callback: ", event);
  }
);
```

### getPagesNumber

> 获取导航堆栈长度

```javascript
var navigator = weex.requireModule("navigator");
navigator.getPagesNumber(function (info) {
  // info = {
  //   message:"",
  //   content:`{"content":"2"}`,
  //   statusCode:"10001"
  // }
});
```
