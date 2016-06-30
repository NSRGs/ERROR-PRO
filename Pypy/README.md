pypy
====

PyPy是Armin Rigo开发的，Python语言的动态编译器，是Psyco的后继项目。PyPy的目的是，做到Psyco没有做到的动态编译。

PyPy开始只是研究性质的项目。但是开发非常成熟，在2007年中旬发布了1.0 Release版本后，大家关注的焦点是，能否在2008年出现可供生产环境使用的版本。

可以运行在Linux的32位和64位、MacOSX和Windows的32位平台中，但是基于arm平台的正在开发中。

它支持Python语言的所有核心部分以及大多数的Python语言标准库函数模块，并且通过了Python语言的test suite。

与CPython的区别可以去看它的兼容性页面.

PyPy还提供了JIT编译器和沙盒功能，因此运行速度比CPython要快，以及可以安全的运行一些不被信任的代码。

PyPy还有一个单独的支持微线程的版本。

另外，PyPy 也有 每夜构建 版本供开发者测试。

