[![test](https://github.com/cisco/ChezScheme/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/cisco/ChezScheme/actions/workflows/test.yml)

简介

源：https://github.com/cisco/ChezScheme

啬赛美(Chez Scheme，法语音 Chez Schème)既是一种编程语言，也是该语言的一种实现，带有支持工具和文档。

作为“关于算法语言方案的修订版<sup>6</sup>报告”([Revised<sup>6</sup> Report on the Algorithmic Language Scheme](http://www.r6rs.org)
，R6RS) 中描述的语言的超集，啬赛美支持赛美(Scheme，法语音 Schème)的所有标准特性，包括一流的过程、尾调用的正确处理、延续、用户定义的记录、库、异常和纯净宏扩展。

啬赛美还包括对与 C 和其他语言接口的广泛支持、对可能在多核上运行的多线程的支持、非阻塞 I/O 以及许多其他功能。

啬赛美实现由编译器、运行时系统和编程环境组成。尽管可以使用解释器，但默认情况下会编译所有代码。当从源文件加载或通过 shell 输入时，源代码会即时编译。源文件也可以预编译为存储的二进制形式，并在其依赖项发生变化时自动重新编译。无论是动态编译还是预编译，编译器都会生成优化的机器代码，并在单独编译的库边界上进行一些优化。还可以指示编译器执行整个程序编译，它进行完整的跨库优化，并将程序及其依赖的库减少到单个二进制文件。

运行时系统与操作系统接口并支持二进制和文本(Unicode)I/O、自动存储管理(动态内存分配和分代垃圾收集)、库管理和异常处理等。默认情况下，编译器包含在运行时系统中，允许在运行时生成和编译程序，动态编译代码的存储，就像任何其他动态分配的存储一样，由垃圾收集器自动回收。

编程环境包括源代码级调试器、在编译期间启用分析时生成分析计数和程序“热点”的 HTML 显示的机制、用于检查内存使用情况的工具和交互式 shell 界面(表达式编辑器，或简称“exeditor”)，支持多行表达式编辑。
啬赛美语言的 R6RS 核心在[“Scheme编程语言”(The Scheme Programming Language)](http://www.scheme.com/tspl4/) 中进行了描述，其中还包括对赛美的介绍和一组示例程序。啬赛美的附加语言、运行时系统和编程环境功能在[啬赛美用户指南](http://cisco.github.io/ChezScheme/csug9.5/csug.html/) 中进行了描述。后者包括一个共享索引和一个共享的表格摘要，在适合前者的地方带有链接，因此它通常是最好的起点。

通过构建啬赛美开始使用[啬赛美](BUILDING)。

有关更多信息，请参阅[啬赛美项目页面](https://cisco.github.io/ChezScheme/)。

================================================================================

[![Build Status](https://travis-ci.org/cisco/ChezScheme.svg?branch=master)](https://travis-ci.org/cisco/ChezScheme)

Chez Scheme is both a programming language and an implementation
of that language, with supporting tools and documentation.

As a superset of the language described in the
[Revised<sup>6</sup> Report on the Algorithmic Language Scheme](http://www.r6rs.org)
(R6RS), Chez Scheme supports all standard features of Scheme,
including first-class procedures, proper treatment of tail calls,
continuations, user-defined records, libraries, exceptions, and
hygienic macro expansion.

Chez Scheme also includes extensive support for interfacing with C
and other languages, support for multiple threads possibly running
on multiple cores, non-blocking I/O, and many other features.

The Chez Scheme implementation consists of a compiler, run-time
system, and programming environment.
Although an interpreter is available, all code is compiled by
default.
Source code is compiled on-the-fly when loaded from a source file
or entered via the shell.
A source file can also be precompiled into a stored binary form and
automatically recompiled when its dependencies change.
Whether compiling on the fly or precompiling, the compiler produces
optimized machine code, with some optimization across separately
compiled library boundaries.
The compiler can also be directed to perform whole-program compilation,
which does full cross-library optimization and also reduces a
program and the libraries upon which it depends to a single binary.

The run-time system interfaces with the operating system and supports,
among other things, binary and textual (Unicode) I/O, automatic
storage management (dynamic memory allocation and generational
garbage collection), library management, and exception handling.
By default, the compiler is included in the run-time system, allowing
programs to be generated and compiled at run time, and storage for
dynamically compiled code, just like any other dynamically allocated
storage, is automatically reclaimed by the garbage collector.

The programming environment includes a source-level debugger, a
mechanism for producing HTML displays of profile counts and program
"hot spots" when profiling is enabled during compilation, tools for
inspecting memory usage, and an interactive shell interface (the
expression editor, or "expeditor" for short) that supports multi-line
expression editing.

The R6RS core of the Chez Scheme language is described in
[The Scheme Programming Language](http://www.scheme.com/tspl4/),
which also includes an introduction to Scheme and a set of example programs.
Chez Scheme's additional language, run-time system, and
programming environment features are described in the
[Chez Scheme User's Guide](http://cisco.github.io/ChezScheme/csug9.5/csug.html).
The latter includes a shared index and a shared summary of forms,
with links where appropriate to the former, so it is often the best
starting point.

Get started with Chez Scheme by [Building Chez Scheme](BUILDING).

For more information see the [Chez Scheme Project Page](https://cisco.github.io/ChezScheme/).

