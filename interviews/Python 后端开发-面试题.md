### 《Python 后端开发》面试题

---

1. **你了解过哪些 Python 的 Web 框架？**

    &emsp;&emsp;答：我用过最多的是 Django 框架，它相比于其它的 Python Web 框架来说，功能较全且强大，而且它自带完善的后台管理，所以对于博客系统的开发来说是特别方便的。且对于数据库操作来说，只需要使用其提供的 ORM，就可以完成。<br>
    &emsp;&emsp;除了 Django 外，Python 还有 Flask、Tornado 我也了解且用过。Flask 是一个使用 Python 编写的轻量级 Web 应用框架，同样基于 WSGI 工具箱和 Jinja2 模板引擎，但是相比 Django，它自带的功能并不是很完善，功能模块也是在需要使用时单独引用。<br>
    &emsp;&emsp;Tornado 采用的是单进程单线程异步 IO 的网络模型，可以编写异步非阻塞的程序。因为它非阻塞的方式和对 epoll 的运用，可以每秒处理数以千计的连接。它是实时 Web 服务的一个理想框架。
    &emsp;&emsp;至于其他的 Web 框架，因为 Python 开源的特性，所以其实还有很多，但是我也没基本了解过了。

1. **什么是 WSGI 工具箱？**

    &emsp;&emsp;答：WSGI 全称 The Web Server Gateway Interface，就是 Web 服务器网关接口。它是 Python Web 开发中的一个标准，规定了服务端开发中的服务器程序和应用程序双方各自需要实现什么接口、提供什么功能，以便二者能够配合使用。

1. **什么是 Jinja2 模板引擎？**

    &emsp;&emsp;答：Jinja2 是基于 Python 的模板引擎，它的设计思想来源于 Django 的模板引擎，并扩展了其语法和一系列强大的的功能。模板引擎是为了使用户 UI 界面与业务逻辑数据分离而产生的，在 Python Web 开发中，这部分文档放在 templates 文件夹下，并且在 render 渲染时转换为 html 文档。

