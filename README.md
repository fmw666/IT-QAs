## IT知识储备库
> *愿我能早日成为一名大佬！*

---

[Q:](#welcome) 什么是 jdk(JDK)，什么又是 jre(JRE)？

[A:](#welcome) jdk 全称 Java Development Kit，即 Java 语言的软件开发工具（SDK，Software Development Kit），没有 jdk 的话无法编译 Java 源程序。jdk 是整个 Java 开发的核心，它包含了 Java 的运行环境 jre（JVM + Java 系统类库）和 JAVA 工具。<br>&emsp; jre 全称 Java Runtime Environment，即 Java 运行环境，是一个软件，可以让计算机系统运行 Java 应用程序（Java Application）。jre 内部有一个虚拟机（JVM，Java Virtual Machine）以及一些标准的类别函数库（Class Library），没有 jre 的话无法运行 Java 程序（class 或 jar 或其他归档文件）。

---

[Q:](#welcome) 什么是 api(API)？

[A:](#welcome) api 全称 Application Programming Interface，即应用程序接口，是一些预先定义的函数，或指软件系统不同组成部分衔接的约定。目的是提供应用程序与开发人员基于某软件或硬件得以访问一组例程的能力，而又无需访问原码，或理解内部工作机制的细节。

---

[Q:](#welcome) 什么是 例程？

[A:](#welcome) 例程的作用类似于函数，但含义更为丰富一些。例程是某个系统对外提供的功能接口或服务的集合。比如操作系统的 API、服务等就是例程；Delphi 或C++Builder 提供的标准函数和库函数等也是例程。我们编写一个 DLL 的时候，里面的输出函数就是这个 DLL 的例程。<br>&emsp; 可以这么简单地来理解：把一段相对独立的代码写成单独的一个模块就是函数的概念。我们可以在自己的程序中编写很多个函数，从而实现模块化编程。但这些模块或者说函数并不一定向外输出（即提供给别的程序使用），只用于当前这个程序里面。此时这些函数就仅仅具有独立函数的意义，但不是例程。
