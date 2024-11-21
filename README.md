# Lua

# Lua 源码阅读学习计划

## 第一周：环境搭建与 Lua 基础回顾

搭建 Lua 源码阅读环境，熟悉 Lua 语言的基本特性和语法，为深入阅读源码奠定基础。

1. 从 Lua 官方网站（https://www.lua.org/）下载 Lua 源码，并解压到本地开发目录。
2. 安装 C 语言开发环境（如果尚未安装），如 MinGW（Windows 环境）或 GCC（Linux 环境）。确保可以在命令行中正常编译和运行 C 语言程序。
3. 阅读 Lua 官方参考手册的前几章，重点回顾 Lua 的数据类型（如数字、字符串、表、函数等）、变量定义、控制流语句（if-else、while、for 等）以及函数的定义和调用方式。

## 第二周：深入 Lua 核心数据结构

理解 Lua 核心数据结构的设计与实现，包括 `TValue`、`Table`、`lua_State` 等，以及它们在 Lua 运行时的作用。

## 第三周：探索 Lua 语法解析与虚拟机执行

掌握 Lua 语法解析的过程和虚拟机的执行机制，包括词法分析、语法分析以及操作码的执行逻辑。

## 第四周：综合学习与实践应用

对之前学习的 Lua 源码知识进行综合运用，深入理解一些高级特性和应用场景，尝试对 Lua 源码进行简单的修改和扩展。

# lua-users wiki: Tutorial Directory

[lua-users wiki: Tutorial Directory](https://lua-users.org/wiki/TutorialDirectory)

| 优先级 | Content                |                                                              |                                                  |
| ------ | ---------------------- | ------------------------------------------------------------ | ------------------------------------------------ |
|        | LuaTypes               | A gentle introduction to variable types used in Lua.         |                                                  |
|        | Assignment             | More on setting variable values.                             |                                                  |
|        | Numbers                | The Lua number type and related functions.                   |                                                  |
|        | Strings                | String (text) usage and related functions.                   |                                                  |
|        | Operators              | Using arithmetic and logical operators.                      |                                                  |
|        | Control Structure      | Keywords if, while, repeat, for, break.                      |                                                  |
| 01     | Tables                 | Lua tables and related functions.                            |                                                  |
|        | Functions              | Introduction to functions.                                   |                                                  |
|        | Scope                  | Introduction to local variables and closures.                |                                                  |
| 02     | Metamethods            | Lua's powerful extension mechanism.                          |                                                  |
|        | Environments           | Lua's global namespace mechanism.                            |                                                  |
| 03     | Modules                | Modules, grouping related code.                              |                                                  |
| 04     | Object Orientation     | An introduction to simulating classes.                       |                                                  |
|        | Patterns               | String searching.                                            |                                                  |
| 06     | Coroutines             | Functions that can return part way through and then resume later. |                                                  |
|        | Iterators              | Writing custom for iterators.                                |                                                  |
| 05     | Garbage Collection     | What happens to deleted objects?                             |                                                  |
| 07     | Weak Tables            | Special table mode where elements are weak references.       |                                                  |
|        | Lua standard libraries |                                                              | Brief explanation and examples of usage of each. |
|        |                        | Core Functions                                               | Basic functions e.g. dofile, assert, error, etc. |
|        |                        | Math Library                                                 | Mathematical functions                           |
|        |                        | String Library                                               | String manipulation                              |
|        |                        | Table Library                                                | Table (or array) manipulation                    |
|        |                        | Os Library                                                   | Operating system facilities                      |
|        |                        | Io Library                                                   | Input/Output facilities                          |
|        |                        | Module Library                                               | Module facilities                                |
|        |                        | Debug Library                                                | Debugging facilities                             |
|        |                        | Coroutine Library                                            | Coroutine manipulation                           |
|        | For                    | Detail on the for statement.                                 |                                                  |
| 09     | Threads                | Using Lua in a pre-emptive threading environment.            |                                                  |
| 10     | Optimisation           | Getting good performance from Lua. See OptimisationTips.     |                                                  |
| 08     | Inheritance            | A technique for implementing OO inheritance in Lua.          |                                                  |

# 学习路线

学习 Lua 编程语言可以从以下几个步骤开始：

## 1. **理解基础概念**

- **编程基础**：确保你有一些编程基础知识，例如变量、条件语句、循环和函数等。
- **Lua 简介**：了解 Lua 是什么，它的应用领域，以及它与其他编程语言的区别和优势。

## 2. **安装和设置开发环境**

- **安装 Lua**：从 [Lua 官方网站](https://www.lua.org/) 下载并安装 Lua。
- **选择编辑器**：选择一个适合编写 Lua 代码的文本编辑器或 IDE，比如 Visual Studio Code、Sublime Text 或 Notepad++。

## 3. **学习基础语法**

- **变量和数据类型**：了解如何声明变量以及常用的数据类型（如字符串、数字、表等）。
- **运算符**：学习算术运算符、关系运算符和逻辑运算符。
- **控制结构**：熟悉 if-else 语句、for 循环和 while 循环等控制结构。
- **函数**：学习如何定义和调用函数。

## 4. **实践基础示例**

- **简单示例**：编写一些简单的 Lua 脚本，比如打印 “Hello, World!”、计算两个数的和等。
- **项目练习**：根据实际需求，尝试一些小项目，比如简单的计算器、猜数字游戏等。

## 5. **深入学习和进阶**

- **表（Tables）**：深入学习 Lua 的核心数据结构——表，包括如何创建、访问和操作表。
- **元表和元方法**：学习元表和元方法，了解如何通过它们扩展 Lua 的功能。
- **模块和包**：了解如何创建和使用模块，以组织和重用代码。
- **面向对象编程**：学习如何在 Lua 中实现面向对象编程。

## 6. **参考资料和社区资源**

- **官方文档**：Lua 官方文档是学习 Lua 最权威的资源，可以在 [Lua 官方网站](https://www.lua.org/docs.html) 查阅。
- **在线教程**：如 [Lua Users Wiki](https://lua-users.org/wiki/TutorialDirectory) 。
- **书籍**：推荐书籍包括《Programming in Lua》（由 Lua 创始人 Roberto Ierusalimschy 编写）。
- **社区和论坛**：加入 Lua 社区，比如 [Lua Users Forum](https://lua-users.org/lists/lua-l/)，与其他学习者和专家交流。

## 7. **项目实战**

- **实践项目**：参与一些开源项目或尝试自己开发一些小工具和应用，积累实际编程经验。
- **代码审查**：与他人分享代码并接受反馈，以不断提高自己的编程能力。

通过以上步骤，逐步学习和掌握 Lua 编程语言，最终能够独立编写和调试 Lua 代码。
