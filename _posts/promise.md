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
回调函数是一段可执行的代码段，它以「参数」的形式传递给其他代码，在其合适的时间执行这段（回调函数）的代码。

**三、为什么使用promise**
上面有提到其实用回调函数可以解决异步，那为什么还要使用promise。对于咱们来说，使用回调函数，当层级较深的时候会很容易陷入回调地狱。在我们使用promise的时候，可以多重链式调用，避免层层嵌套回调。除此之外，为了我们的代码更加具有可读性和可维护性，我们需要将数据请求与数据处理明确的区分开来。

**promise基本使用简单介绍**
一般情况下我们都会使用 new Promise() 来创建promise对象，但是除此之外我们也可以使用其他方法。
在这里，我们将会学习如何使用 Promise.resolve 和 Promise.reject这两个方法。
静态方法Promise.resolve(value) 可以认为是 new Promise() 方法的快捷方式。

例子：
new Promise(function(resolve){
    resolve(1);
});

 