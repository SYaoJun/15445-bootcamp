# 15-445/645 C++ 训练营
这个编程训练营旨在为现代C++编程提供基本入门。C++语言的特性非常广泛和深远，无法在一个训练营中全面涵盖，而且坦白地说，最好通过实际经验来学习。工作人员确信，参加15-445课程将使您成为更自信的C++程序员！然而，在完成编程作业时，我们确实会涵盖一些必须了解的C++主题。本教程不涵盖基本的C/C++语法，主要关注C++编程特性，特别是那些在C语言中不存在的概念。

这是15-445/645课程的C++编程训练营的第一版，欢迎提供反馈！

## Format
这个训练营包括位于`src/`目录中的C++代码文件，旨在深入阅读。每个文件都可以编译成同名的可执行文件。请使用CMake来构建这些可执行文件。以下一组命令可以构建所有的可执行文件。在运行这些命令之后，这些可执行文件应该会位于`build`目录中。
```console
$ mkdir build
$ cd build
$ cmake ..
$ make -j8
```
例如，`src/references.cpp`文件会编译成名为`references`的可执行文件，位于`./build`目录中。对于源目录中的每个文件也是如此。

## 文件
`src/`目录中有十五个文件，每个文件涵盖不同的概念。它们应该按照以下顺序阅读，因为每个文件都是在前一个文件的基础上构建的。然而，如果您了解一些现代C++的概念，并且想要刷新您的知识，从阅读您不熟悉的概念文件开始可能是可以的。

### 引用和移动语义
- `references.cpp`：介绍了C++引用的概念。
- `move_semantics.cpp`：介绍了C++移动语义的概念。
- `move_constructors.cpp`：介绍了C++类的移动构造函数和移动赋值运算符的概念。

### C++ 模版
- `templated_functions.cpp`：介绍了C++模板函数的概念。
- `templated_classes.cpp`：介绍了C++模板类的概念。

### 杂类
- `wrapper_class.cpp`：介绍了C++封装类的概念。
- `iterator.cpp`：介绍了实现基本C++风格迭代器的概念。
- `namespaces.cpp`：介绍了C++命名空间的概念。

### C++标准库（STL）容器
- `vectors.cpp`：介绍了`std::vector`。
- `set.cpp`：介绍了`std::set`。
- `unordered_map.cpp`：介绍了`std::unordered_map`。
- `auto.cpp`：介绍了C++关键字`auto`的用法，包括在C++ STL容器中使用`auto`进行迭代。

### C++标准库（STL）内存
- `unique_ptr.cpp`：介绍了`std::unique_ptr`。
- `shared_ptr.cpp`：介绍了`std::shared_ptr`。

### C++标准库（STL）同步原语
- `mutex.cpp`：介绍了`std::mutex`。
- `scoped_lock.cpp`：介绍了`std::scoped_lock`。
- `condition_variable.cpp`：介绍了`std::condition_variable`。
- `rwlock.cpp`：介绍了使用多个C++ STL同步原语库（`std::shared_mutex`，`std::shared_lock`，`std::unique_lock`）来创建读写锁实现。

## 其他资源
在熟悉C++的过程中，还有许多其他有用的资源。我在这里列出了一些！
- [https://en.cppreference.com/w/](https://en.cppreference.com/w/)：这是官方的C++文档。
- [https://cplusplus.com/](https://cplusplus.com/)：包含C++语言[教程](https://cplusplus.com/doc/tutorial/)和C++库[参考](https://cplusplus.com/reference/)。
- [现代C++教程](https://github.com/changkun/modern-cpp-tutorial)。这个GitHub存储库包含了一些有用的信息和练习！

## 附录：官方C++文档（涵盖训练营中的主题）
这些文档可能对您有用！它非常全面（比这个训练营更全面），但可读性可能不如此训练营。总的来说，我认为在项目上工作时，阅读和理解这些文档仍然是一个好主意。尽管训练营尽可能全面，但仍然只涵盖了使用现代C++的基础知识。

- [References](https://en.cppreference.com/w/cpp/language/reference)
- [std::move](https://en.cppreference.com/w/cpp/utility/move)
- [Move Constructors](https://en.cppreference.com/w/cpp/language/move_constructor) and [Move Assignment Operators](https://en.cppreference.com/w/cpp/language/move_assignment)
- [Templated Functions](https://en.cppreference.com/w/cpp/language/function_template)
- [Templated Classes](https://en.cppreference.com/w/cpp/language/class_template)
- [Iterators](https://en.cppreference.com/w/cpp/iterator)
- [Namespaces](https://en.cppreference.com/w/cpp/language/namespace)
- [std::vector](https://en.cppreference.com/w/cpp/container/vector)
- [std::set](https://en.cppreference.com/w/cpp/container/set)
- [std::unordered_map](https://en.cppreference.com/w/cpp/container/unordered_map)
- [auto](https://en.cppreference.com/w/cpp/language/auto)
- [std::unique_ptr](https://en.cppreference.com/w/cpp/memory/unique_ptr)
- [std::shared_ptr](https://en.cppreference.com/w/cpp/memory/shared_ptr)
- [std::mutex](https://en.cppreference.com/w/cpp/thread/mutex)
- [std::scoped_lock](https://en.cppreference.com/w/cpp/thread/scoped_lock)
- [std::condition_variable](https://en.cppreference.com/w/cpp/thread/condition_variable)
- [std::shared_mutex](https://en.cppreference.com/w/cpp/thread/shared_mutex)
- [std::shared_lock](https://en.cppreference.com/w/cpp/thread/shared_lock)
- [std::unique_lock](https://en.cppreference.com/w/cpp/thread/unique_lock)