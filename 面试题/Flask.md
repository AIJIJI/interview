# Base

## 简单

1. before_request, after_request, teardown_request 三个方法是做什么的
    
    before_request() : It is called before a request and requires no arguments.
    after_request() : It is called after a request and pass the response that will be sent to the client
    teardown_request(): It is used when exception is raised and response are not guaranteed. It is called after the response and not allowed to modify the request or their values.


## 进阶

1. app.errorhandler 方法是做什么的

    装饰器，将函数注册为错误处理函数

    app.errorhandler(code or Exception)(_handle_function)