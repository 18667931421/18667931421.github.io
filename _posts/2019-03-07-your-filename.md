---
published: false
---
 Promise深入浅出
 
**一、什么是Promise**
 The Promise object is used for asynchronous computations. A Promise represents a single asynchronous operation that hasn't completed yet, but is expected in the future.
译文：Promise对象用于异步操作，它表示一个尚未完成且预计在未来完成的异步操作。

我的理解是 Promise本意是承诺，在程序中的意思就是承诺我过一段时间后会给你一个结果。 什么时候会用到过一段时间？答案是异步操作，异步是指可能比较长时间才有结果的才做，例如网络请求、读取本地文件等。

**二、同步异步**
1、同步
同步模式，即单线程模式，一次只能执行一个任务，函数调用后需等到函数执行结束，返回执行的结果，才能进行下一个任务。如果这个任务执行的时间较长，就会导致「线程阻塞」。
2、异步
异步模式，即与同步模式相反，可以一起执行多个任务，函数调用后不会立即返回执行的结果，如果任务A需要等待，可先执行任务B，等到任务A结果返回后再继续回调。 
3、回调函数
提起异步，就不得不谈谈回调函数了。可以简单理解为：（执行完）回（来）调（用）的函数。
 