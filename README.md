# angular 入门

## angular 是什么?

angular是一个javascript框架, 可以用来构建SPA(single page applications 单页应用)


## 1. 表达式

表达式其实就是我们的各种运算, 加减乘除, 三元运算, 字符串相加等等

## 2. 指令

- ng-app 指令  
    `ng-app 指令启动一个AngularJS应用。它定义根元素。它会自动初始化或启动加载包含AngularJS应用程序的Web页面的应用程序。`
- ng-init 指令  
    `ng-init 指令初始化应用程序数据。`
- ng-model 指令  
    `ng-model 指令把元素值（比如输入域的值）绑定到应用程序。`
- ng-bind 指令
    `ng-bind 指令绑定一个变量`

更多指令 [点我](https://docs.angularjs.org/api/ng/directive)
    
## 3. 模块

通过angular.model我们可以创建一个模块, 这个模块可以依赖其他模块, 可以用来很好的组织代码结构  
通过模块, 我们可以在 AngularJS 应用中添加控制器，指令，过滤器等

## 4. 控制器

可以通过angular.controller创建一个控制器, 控制器主要用来控制程序中的应用数据(一般也就是模型).  


## 5. 服务

1. value `可以被修改`
2. constant `常量,不能被修改,可以在config的时候被注入`
3. factory `返回一个对象, 被注入服务的就是这个对象`
4. service `需要一个构造函数, 实际上factory和service是差不多的`
5. provider `返回一个对象, 对象必须要有一个$get方法, $get必须返回一个对象,这个对象就是被注入到服务的对象`

angular 内置服务
- $http
- $interval `相当于window.setInterval $interval.cancel 相当于clearInterval`
- $timeout `相当于window.setTimeout`

## 6. 过滤器

angular的过滤器一般用来转换数据.
内置的过滤器有`currency,date,filter,json,limitTo,lowercase,number,orderBy,uppercase`
当然,我们也可以自定义过滤器



[api文档地址](https://docs.angularjs.org/api)