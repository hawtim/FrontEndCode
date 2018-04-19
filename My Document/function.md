# 22.6 小结

JavaScript 中的函数非常强大，因为它们是第一类对象，使用闭包和函数环境切换，还可以有很多使用函数的强大方法，可以创建作用域安全的构造函数，确保在缺少new 操作符时调用构造函数不会改变错误的环境对象

- 可以使用惰性载入函数，将任何代码分支推迟到第一次调用函数的时候
- 函数绑定可以让你创建始终在指定环境中运行的函数，同时函数柯里化可以让你创建已经填了某些参数的函数
- 将绑定和柯里化组合起来，就能够给你一种在任意环境中以任意参数执行任意函数的方法

ES5 允许通过以下几种方式来创建防篡改对象

- 不可扩展对象，不允许添加新的属性或方法
- 密封的对象，是不可扩展对象，同事不允许删除已有的属性和方法
- 冻结的对象，也是密封的对象，不允许重写对象的成员

JavaScript 中可以使用 setTimeout() 和 setInterval() 如下创建定时器

- 定时器代码是放在一个等待区域，直到时间间隔到了之后。此时将代码添加到 JavaScript 的处理队列中，等待下一次 JavaScript 进程空闲时被执行
- 每次一段代码执行结束后，都会一小段空闲时间进行其他浏览器处理
- 这种行为意味着，可以使用定时器将长时间运行的脚本切分为一小块一小块可以在以后运行的代码段，有助于 web 应用对用户交互有更积极的响应

JavaScript 中经常以事件的形式应用观察者模式，虽然事件常常和 DOM 一起使用，但你可以通过实现自定义事件在自己的代码中应用，使用自定义事件有助于将不同的部分的代码相互之间解耦，让维护更加容易。


