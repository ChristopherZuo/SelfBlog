# 异步调用与http请求

## Async/Await

Async/Await 模式被认为是最优雅的异步操作模式，其实质是异步调用的一种语法糖。

### 使用方式
#### async
async是一个修饰function的关键字，其作用是确保function永远返回一个Promise，其更大的作用是在function内部启用await关键字。
```javascript
async function aFunction() {
    return 1;
}

async function aFunction() {
    return Promise.resove(1);
}
```
上述两种写法效果相同。
async function调用结果可以直接作为Promise使用:
```javascript
aFunction().then(alert);
```
