# CHATGPT / GPT-4 和 Python3 数据可视化

> 原文：[Python 3 data visualization using chatgpt / GPT-4 ](https://annas-archive.org/md5/0b427d0e4a9314354e391f46d15209a3)
> 
> 译者：[飞龙](https://github.com/wizardforcel)
> 
> 协议：[CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)


![封面：使用 CHATGPT / GPT-4 进行 Python 3 数据可视化](img/python-3-data-visualization-using-chatgpt-9781501522321.jpg)

## **前言**

### **本书的主要价值主张是什么？**

这本书旨在向读者展示 Python 3 编程的概念和数据可视化的艺术。第一章介绍了 Python 的基础知识，涵盖了从基本数据类型、循环和函数到更高级的结构如字典、集合和矩阵等众多主题。在第二章中，重点转向 NumPy 及其强大的数组操作，进而引入使用 Matplotlib 等突出库进行数据可视化的世界。第六章包含了 Seaborn 丰富的可视化工具，为 Iris 和 Titanic 等数据集提供了洞察。此外，本书还涵盖了其他可视化工具和技术，包括 SVG 图形、D3 动态可视化等。第七章涵盖了 ChatGPT 和 GPT-4 的主要功能以及一些竞争对手的信息。第八章包含了使用 ChatGPT 进行数据可视化的示例，例如基于数据集（例如 Titanic 数据集）的图表和图形。从 Python 的基础概念到数据可视化的复杂性，本书为初学者和资深专业人士提供了一个全面的学习资源。

### **目标受众**

本书主要面向那些使用过 Python 并且对学习 Python 库中的图形效果感兴趣的人。本书还旨在吸引具有高度多样化背景的国际读者群体，涵盖各个年龄段。因此，本书使用标准英语而不是可能让读者感到困惑的口语表达。本书为预期读者提供了一个舒适而有意义的的学习体验。

### **为什么代码示例主要使用 Python？**

大多数代码示例都很短（通常不到一页，有时甚至不到半页），如果需要，你可以轻松快速地将代码复制/粘贴到新的 Jupyter 笔记本中。对于引用 CSV 文件的 Python 代码示例，你不需要在相应的 Jupyter 笔记本中添加任何额外的代码来访问 CSV 文件。此外，代码示例执行速度快，因此你不需要使用 Google Colaboratory 提供的免费 GPU。

如果你决定使用 Google Colaboratory，你可以轻松地将 Python 代码复制/粘贴到笔记本中，并使用上传功能上传现有的 Jupyter 笔记本。请注意以下要点：如果 Python 代码引用了 CSV 文件，请确保包含适当的代码片段（详细信息可在网上找到）以在 Google Colaboratory 中访问相应的 Jupyter 笔记本中的 CSV 文件。

### **为什么本书包含 SKLEARN 材料？**

首先，请记住，这本书中的 Sklearn 材料是简约的，因为这本书不是关于机器学习的。其次，Sklearn 材料位于第六章，在那里你将了解一些 Sklearn 内置数据集。如果你决定深入研究机器学习，你将已经接触到 Sklearn 的一些方面。

### **如何充分利用这本书？**

一些程序员擅长从文本中学习，而另一些程序员擅长从示例代码（以及大量的代码）中学习，这意味着没有一种单一的风格可以适用于所有人。

此外，一些程序员希望先运行代码，看看它做了什么，然后再回到代码中去深入了解细节（而其他人则采用相反的方法）。

因此，这本书中有各种类型的代码示例：有些很短，有些很长，还有一些代码示例是从早期的代码示例“构建”出来的。

### **我需要了解这本书的哪些内容？**

对于 Python 3.x 的当前知识是最有帮助的技能。了解其他编程语言（如 Java）的知识也可能有所帮助，因为这样可以接触到编程概念和结构。你拥有的技术知识越少，为了理解所涵盖的各种主题，就越需要勤奋。

至于非技术技能，重要的是要有强烈的了解数据可视化的愿望，以及阅读和理解代码示例的动机和纪律。

### **配套文件是否可以替代这本书？**

配套文件包含了所有代码示例，以节省你手动将代码输入文本文件的时间和精力。此外，可能存在你无法轻松访问配套光盘的情况。此外，书中的代码示例提供了配套文件中不可用的解释。

### **这本书是否包含生产级别的代码示例？**

这本书中代码示例的主要目的是向你展示基于 Python 的数据可视化库。清晰度比编写更紧凑但更难理解的代码（并且可能更容易出现错误）更重要。如果你决定在生产网站上使用这本书中的任何代码，你应该将那段代码提交与你代码库的其他部分相同的严格分析。

### **我该如何设置命令行？**

如果你是一名 Mac 用户，有三种方法可以做到。第一种方法是使用 Finder 导航到应用程序 > 工具，然后双击工具应用程序。接下来，如果你已经有了可用的命令行，你可以通过输入以下命令来启动一个新的命令行：

```py
 open /Applications/Utilities/Terminal.app 
```

对于 Mac 用户来说，第二种方法是直接在可见的命令行中点击 command+n 来打开一个新的命令行，这样你的 Mac 就会启动另一个命令行。

如果你使用的是 PC，你可以安装 Cygwin（开源 *https://cygwin.com/*），它模拟 bash 命令，或者使用其他工具包，如 MKS（一个商业产品）。请阅读在线文档，该文档描述了下载和安装过程。请注意，如果自定义别名定义在除主启动文件（如 .bash_login）之外的其他文件中，则不会自动设置。

### **配套文件**

本书中的所有代码示例和图表都可以通过给出版商写信至 *info@merclearning.com* 获取。

### **完成这本书后的“下一步是什么”？**

这个问题的答案差异很大，主要是因为答案很大程度上取决于你的目标。如果你主要对自然语言处理（NLP）感兴趣，那么你可以学习更高级的概念，如注意力、转换器以及与 BERT 相关的模型。

如果你主要对机器学习感兴趣，那么机器学习的一些子领域，如深度学习、强化学习（以及深度强化学习）可能对你有吸引力。幸运的是，有许多资源可供选择，你可以通过互联网搜索这些资源。另一个要点：你需要学习的机器学习方面取决于你自己的身份：机器学习工程师、数据科学家、经理、学生或软件开发者的需求都是不同的。

**O. Campesato**

**2023 年 12 月**

## **第一章**

## *Python 简介*

本章包含 Python 介绍，包括有关安装模块的有用工具、基本结构和如何处理某些数据类型的信息。

本章的第一部分介绍了如何安装 Python、一些环境变量以及如何使用解释器。你将看到代码示例，以及如何将代码保存到文本文件中，这些文件可以从命令行启动。本章的第二部分展示了如何处理简单数据类型，如数字、分数和字符串。本章的最后一部分讨论了异常以及如何在脚本中使用它们。

**注意** *本书中的 Python 文件适用于 Python 3.x.*

### **Python 工具**

可在 *[`continuum.io/downloads`](http://continuum.io/downloads)* 下载适用于 Windows、Linux 和 Mac 的 Anaconda Python 发行版。

Anaconda 非常适合 numpy 和 scipy 等模块，如果你是 Windows 用户，Anaconda 看起来是一个更好的替代方案。

#### **easy_install 和 pip**

当你需要安装 Python 模块时，easy_install 和 pip 都很容易使用。无论何时你需要安装一个模块（本书中有许多），都可以使用以下语法中的 easy_install 或 pip：

```py
 easy_install <module-name>
pip install <module-name> 
```

**注意** *基于 Python 的模块更容易安装，而用 C 语言编写的模块通常运行更快，但在安装方面更困难。*

#### **virtualenv**

virtualenv 工具允许您创建独立的 Python 环境，其主页在*[`www.virtualenv.org/en/latest/virtualenv.html`](http://www.virtualenv.org/en/latest/virtualenv.html)*。

virtualenv 解决了为不同应用程序保留正确依赖项和版本（以及间接权限）的问题。如果您是 Python 新手，您可能现在不需要 virtualenv，但请记住这个工具。

#### **IPython**

另一个非常好的工具是 IPython（它赢得了 Jolt 奖），其主页在*[`ipython.org/install.html`](http://ipython.org/install.html)*。IPython 的两个非常不错的特性是 Tab 补全和“？”（文本帮助）。Tab 补全的一个例子如下：

```py
 python
Python 3.9.1 (v3.9.1:1e5d33e9b9, Dec  7 2020, 12:44:01)
[Clang 12.0.0 (clang-1200.0.32.27)] on darwin
Type "help", "copyright", "credits" or "license" for more information. IPython 0.13.2 -- An enhanced Interactive Python. ? -> Introduction and overview of IPython's features. %quickref -> Quick reference. help      -> Python's own help system. object? -> Details about 'object', use 'object??' for extra details. In [1]: di
%dirs   dict    dir     divmod 
```

在前面的会话中，如果您输入字符 di，IPython 会响应以下包含所有以字母 di 开头的函数的行：

```py
 %dirs   dict    dir     divmod 
```

如果您输入一个问号（“？”），IPython 会提供文本帮助，其中第一部分如下：

```py
 IPython -- An enhanced Interactive Python
=========================================

IPython offers a combination of convenient shell features,
special commands and a history mechanism for both input
(command history) and output (results caching, similar
to Mathematica). It is intended to be a fully compatible
replacement for the standard Python interpreter, while
offering vastly improved functionality and flexibility. 
```

下一个部分将向您展示如何检查您的机器上是否已安装 Python，以及您可以从哪里下载 Python。

### **PYTHON 安装**

在下载任何内容之前，请通过在命令提示符中输入以下命令来检查您的机器上是否已安装 Python（如果您有一台 MacBook 或 Linux 机器，则很可能已安装）：

```py
 python -V 
```

本书所使用的 MacBook 的输出如下：

```py
 Python 3.9.1 
```

**注意** *请在您的机器上安装 Python 3.9（或尽可能接近这个版本），以便您将拥有与本书中测试 Python 文件相同的 Python 版本。*

如果您需要在您的机器上安装 Python，请导航到 Python 主页并选择下载链接，或直接导航到该网站：

*[`www.python.org/download/`](http://www.python.org/download/)*

此外，PythonWin 适用于 Windows，其主页如下：

*[`www.cgl.ucsf.edu/Outreach/pc204/pythonwin.html`](http://www.cgl.ucsf.edu/Outreach/pc204/pythonwin.html)*

使用任何可以创建、编辑和保存 Python 脚本并保存为纯文本文件的文本编辑器（不要使用 Microsoft Word）。在您的机器上安装并配置 Python 之后，您就可以开始使用本书中的 Python 脚本了。

### **设置路径环境变量（仅限 Windows）**

PATH 环境变量指定了一个目录列表，每当您在命令行中指定一个可执行程序时，都会搜索这些目录。以下 URL 提供了一个有用的指南，说明如何设置环境，以便 Python 可执行文件始终在所有命令提示符中可用：

*[`www.blog.pythonlibrary.org/2011/11/24/python-101-setting-up-python-on-windows/`](http://www.blog.pythonlibrary.org/2011/11/24/python-101-setting-up-python-on-windows/)*

### **在您的机器上启动 PYTHON**

有三种不同的方式来启动 Python：

+   使用 Python 交互式解释器。

+   从命令行启动 Python 脚本。

+   使用集成开发环境（IDE）。

下一节将向您展示如何从命令行启动 Python 解释器，在本章的后面部分，您将学习如何从命令行启动脚本以及 IDE 的相关知识。

**注意** *本书的重点是介绍如何从命令行启动 Python 脚本或输入 Python 解释器中的代码。*

#### **Python 交互式解释器**

通过打开命令壳并输入以下命令从命令行启动交互式解释器：

```py
 python 
```

您将看到以下提示（或类似提示）：

```py
 Python 3.9.1 (v3.9.1:1e5d33e9b9, Dec  7 2020, 12:44:01)
[Clang 12.0.0 (clang-1200.0.32.27)] on darwin
Type "help", "copyright", "credits" or "license" for more information. >>> 
```

现在在提示符下输入表达式 2 + 7：

```py
 >>> 2 + 7 
```

Python 显示以下结果：

```py
 9
>>> 
```

按 ctrl-d 退出 Python 壳。

您可以从命令行启动任何 Python 脚本，只需在脚本前加上“python”这个词。例如，如果您有一个包含命令的脚本 myscript.py，启动脚本的方式如下：

```py
 python myscript.py 
```

作为简单的说明，假设脚本 myscript.py 包含以下代码：

```py
 print('Hello World from Python')
print('2 + 7 = ', 2+7) 
```

当您启动前面的脚本时，您将看到以下输出：

```py
 Hello World from Python
2 + 7 =  9 
```

### **PYTHON 标识符**

*标识符*是变量、函数、类、模块或其他 Python 对象的名称，有效的标识符符合以下规则：

+   以字母 A 到 Z 或 a 到 z 或下划线 (_) 开头

+   零个或多个字母、下划线和数字（0 到 9）

**注意** *Python 标识符不能包含如 @、$ 和 % 这样的字符。*

Python 是区分大小写的语言，所以 Abc 和 abc 在 Python 中是不同的标识符。此外，Python 还有以下命名约定：

+   类名以大写字母开头，所有其他标识符以小写字母开头

+   初始下划线用于私有标识符。

+   两个初始下划线用于强私有标识符。

Python 中以两个初始下划线和两个尾随下划线字符开头的标识符表示语言定义的特殊名称。

### **行、缩进和多行注释**

与其他编程语言（如 Java 或 Objective-C）不同，Python 使用缩进来代替花括号作为代码块。代码块中的缩进必须一致，如下所示：

```py
 if True:
    print("ABC")
    print("DEF")
else:
    print("ABC")
    print("DEF") 
```

Python 中的多行语句可以用新行或反斜杠（“\”）字符结束，如下所示：

```py
 total = x1 + \
        x2 + \
        x3 
```

显然，您可以将 x1、x2 和 x3 放在同一行上，因此没有必要使用三行；然而，如果您需要添加一组不适合单行的变量，此功能是可用的。

您可以使用分号（“;”）分隔每个语句，在单行中指定多个语句，如下所示：

```py
 a=10; b=5; print(a); print(a+b) 
```

上述代码片段的输出如下：

```py
 10
15 
```

**注意** *在 Python 中不建议使用分号和续行符。*

### **Python 中的引号和注释**

Python 允许使用单引号（'）、双引号（"）和三引号（''' 或 """）作为字符串字面量，前提是它们与字符串的开始和结束相匹配。你可以使用三引号来表示跨越多行的字符串。以下示例是合法的 Python 字符串：

```py
 word = 'word'
line = "This is a sentence." para = """This is a paragraph. This paragraph contains
more than one sentence.""" 
```

以字母“r”（代表“raw”）开头的字符串字面量将把所有内容视为字面字符，并“转义”元字符的含义，如下所示：

```py
 a1 = r'\n'
a2 = r'\r'
a3 = r'\t'
print('a1:',a1,'a2:',a2,'a3:',a3) 
```

前一个代码块的结果如下：

```py
 a1: \n a2: \r a3: \t 
```

你可以在一对双引号中嵌入一个单引号（反之亦然）来显示单引号或双引号。另一种实现相同结果的方法是在单引号或双引号前加上一个反斜杠（“\”）字符。以下代码块展示了这些技术：

```py
 b1 = "'"
b2 = '"'
b3 = '\''
b4 = "\""
print('b1:',b1,'b2:',b2)
print('b3:',b3,'b4:',b4) 
```

前一个代码块的结果如下：

```py
 b1: ' b2: "
b3: ' b4: " 
```

一个不在字符串字面量内的井号（#）是表示注释开始的字符。此外，# 之后直到物理行结束的所有字符都是注释的一部分（并由 Python 解释器忽略）。考虑以下代码块：

```py
 #!/usr/bin/python
# First comment
print("Hello, Python!")  # second comment 
```

这将产生以下结果：

```py
 Hello, Python! 
```

注释可以紧跟在语句或表达式的同一行之后：

```py
 name = "Tom Jones" # This is also comment 
```

你可以这样注释多行：

```py
 # This is comment one
# This is comment two
# This is comment three 
```

Python 中的一个空白行是只包含空白、注释或两者的行。

### **在模块中保存你的代码**

之前你看到了如何从命令行启动 Python 解释器，然后输入命令。然而，你在 Python 解释器中输入的每一行代码只对当前会话有效：如果你退出解释器然后再次启动解释器，你之前的定义就不再有效。幸运的是，Python 允许你将代码存储在文本文件中，如下一节所述。

Python 中的 *模块* 是一个包含 Python 语句的文本文件。在前一节中，你看到了解释器如何使你能够测试当前会话中定义有效的代码片段。如果你想保留代码片段和其他定义，将它们放置在一个文本文件中，这样你就可以在解释器外执行该代码。

当模块首次导入时，Python 程序的外部语句会从上到下执行，这将设置其变量和函数。

Python 模块可以直接从命令行运行，如下所示：

```py
 python first.py 
```

举例来说，将以下两个语句放置在一个名为 first.py 的文本文件中：

```py
 x = 3
print(x) 
```

现在输入以下命令：

```py
 python first.py 
```

前一个命令的输出是 3，这与在解释器中执行前面的代码相同。

当模块直接运行时，特殊变量 __name__ 被设置为 __main__。你经常会在模块中看到以下类型的代码：

```py
 if __name__ == '__main__':
    # do something here
    print('Running directly') 
```

前面的代码片段使 Python 能够确定模块是从命令行启动还是被导入到另一个模块中。

### **Python 中的标准模块**

Python 标准库提供了许多模块，可以简化你的脚本。标准库模块的列表在 *[`www.python.org/doc/`](http://www.python.org/doc/)*。

最重要的模块包括 cgi、math、os、pickle、random、re、socket、sys、time 和 urllib。

本书中的代码示例使用了 math、os、random、re、socket、sys、time 和 urllib 模块。你需要导入这些模块才能在代码中使用它们。例如，以下代码块显示了如何导入 4 个标准 Python 模块：

```py
 import datetime
import re
import sys
import time 
```

本书中的代码示例导入了一个或多个上述模块，以及其他 Python 模块。

### **help() 和 dir() 函数**

对 Python 相关主题的互联网搜索通常会返回包含有用信息的多个链接。或者，你可以检查官方 Python 文档网站：*[docs.python.org](http://docs.python.org)*。

此外，Python 提供了从解释器可访问的 help() 和 dir() 函数。help() 函数显示文档字符串，而 dir() 函数显示定义的符号。

例如，如果你输入 help(sys)，你将看到 sys 模块的文档，而 dir(sys) 则显示定义的符号列表。

在解释器中输入以下命令以显示 Python 中的字符串相关方法：

```py
 >>> dir(str) 
```

前一个命令生成了以下输出：

```py
 ['__add__', '__class__', '__contains__', '__delattr__',
'__doc__', '__eq__', '__format__', '__ge__', '__
getattribute__', '__getitem__', '__getnewargs__', '__
getslice__', '__gt__', '__hash__', '__init__', '__le__',
'__len__', '__lt__', '__mod__', '__mul__', '__ne__',
'__new__', '__reduce__', '__reduce_ex__', '__repr__',
'__rmod__', '__rmul__', '__setattr__', '__sizeof__',
'__str__', '__subclasshook__', '_formatter_field_name_
split', '_formatter_parser', 'capitalize', 'center',
'count', 'decode', 'encode', 'endswith', 'expandtabs',
'find', 'format', 'index', 'isalnum', 'isalpha', 'isdigit',
'islower', 'isspace', 'istitle', 'isupper', 'join',
'ljust', 'lower', 'lstrip', 'partition', 'replace',
'rfind', 'rindex', 'rjust', 'rpartition', 'rsplit',
'rstrip', 'split', 'splitlines', 'startswith', 'strip',
'swapcase', 'title', 'translate', 'upper', 'zfill'] 
```

上述列表提供了一个内置函数的汇总“输出”（包括本章后面讨论的一些函数）。尽管 max() 函数显然返回其参数的最大值，但 filter() 或 map() 等其他函数的目的并不立即明显（除非你在其他编程语言中使用过它们）。上述列表提供了了解本章未讨论的各种 Python 内置函数的起点。

注意，虽然 dir() 不列出内置函数和变量的名称，但你可以从自动导入的名为 __builtin__ 的标准模块中获取这些信息：

```py
 >>> dir(__builtins__) 
```

下面的命令显示了如何获取有关函数的更多信息：

```py
 help(str.lower) 
```

前一个命令的输出如下：

```py
 Help on method_descriptor:

lower(...)
    S.lower() -> string

    Return a copy of the string S converted to lowercase. (END) 
```

检查在线文档，并在需要有关特定函数或模块的附加信息时，尝试使用 help() 和 dir()。

### **编译时和运行时代码检查**

Python 执行一些编译时检查，但大多数检查（包括类型、名称等）都推迟到代码执行。因此，如果你的 Python 代码引用了一个不存在的用户定义函数，代码将成功编译。实际上，代码只有在代码执行路径引用了该不存在的函数时才会失败，并抛出异常。

作为简单的示例，考虑以下函数 myFunc，它引用了一个不存在的名为 DoesNotExist 的函数：

```py
 def myFunc(x):
    if x == 3:
        print(DoesNotExist(x))
    else:
        print('x: ',x) 
```

如果 myFunc 函数传递了值 3，则前面的代码将失败，之后 Python 会引发错误。

在 第二章 中，你将学习如何定义和调用用户自定义函数，以及解释 Python 中局部变量和全局变量的区别。

现在你已经理解了一些基本概念（例如如何使用 Python 解释器）以及如何启动自定义模块，下一节将讨论原始数据类型。

### **简单数据类型**

Python 支持原始数据类型，例如数字（整数、浮点数和指数数）、字符串和日期。Python 还支持更复杂的数据类型，如列表（或数组）、元组和字典，这些内容将在 第三章 中讨论。接下来的几节将讨论一些 Python 原始数据类型，以及一些代码片段，展示如何对这些数据类型执行各种操作。

### **处理数字**

Python 提供了与其他编程语言类似的直观算术运算来操作数字。以下示例涉及整数上的算术运算：

```py
 >>> 2+2
4
>>> 4/3
1
>>> 3*8
24 
```

以下示例将数字赋给两个变量并计算它们的乘积：

```py
 >>> x = 4
>>> y = 7
>>> x * y
28 
```

以下示例演示了涉及整数的算术运算：

```py
 >>> 2+2
4
>>> 4/3
1
>>> 3*8
24 
```

注意，两个整数之间的除法（“/”）实际上是截断，只保留整数结果。以下示例将浮点数转换为指数形式：

```py
 >>> fnum = 0.00012345689000007
>>> "%.14e"%fnum
'1.23456890000070e-04' 
```

你可以使用 int() 函数和 float() 函数将字符串转换为数字：

```py
 word1 = "123"
word2 = "456.78"
var1 = int(word1)
var2 = float(word2)
print("var1: ",var1," var2: ",var2) 
```

上述代码块输出的结果如下：

```py
 var1:  123  var2:  456.78 
```

或者，你可以使用 eval() 函数：

```py
 word1 = "123"
word2 = "456.78"
var1 = eval(word1)
var2 = eval(word2)
print("var1: ",var1," var2: ",var2) 
```

如果你尝试将一个既不是有效整数也不是浮点数的字符串进行转换，Python 会引发异常，因此建议将你的代码放在 try/except 块中。

#### **处理其他进制**

Python 中的数字是以十进制（默认）为基础的，但你可以轻松地将数字转换为其他进制。例如，以下代码块将变量 x 初始化为 1234，然后以 2、8 和 16 进制显示该数字：

```py
 >>> x = 1234
>>> bin(x) '0b10011010010'
>>> oct(x) '0o2322'
>>> hex(x) '0x4d2' >>> 
```

如果你想要抑制 0b、0o 或 0x 前缀，可以使用 format() 函数，如下所示：

```py
 >>> format(x, 'b') '10011010010'
>>> format(x, 'o') '2322'
>>> format(x, 'x') '4d2' 
```

负整数会显示为负号：

```py
 >>> x = -1234
>>> format(x, 'b') '-10011010010'
>>> format(x, 'x') '-4d2' 
```

#### **chr() 函数**

chr() 函数接受一个正整数作为参数，并将其转换为相应的字母值（如果存在）。大写字母 A 到 Z 的十进制表示为 65 到 91（对应十六进制 41 到 5b），小写字母 a 到 z 的十进制表示为 97 到 122（十六进制 61 到 7b）。

以下是一个使用 chr() 函数打印大写字母 A 的示例：

```py
 >>> x=chr(65)
>>> x
'A' 
```

以下代码块打印了一系列整数的 ASCII 值：

```py
 result = ""
for x in range(65,91):
  print(x, chr(x))
  result = result+chr(x)+' '
print("result: ",result) 
```

**注意** *Python 2 使用 ASCII 字符串，而 Python 3 使用 Unicode。*

你可以使用以下行表示字符范围：

```py
 for x in range(65,91): 
```

然而，以下等效的代码片段更直观：

```py
 for x in range(ord('A'), ord('Z')): 
```

如果你想显示小写字母的结果，将前面的范围从（65，91）更改为以下任一语句：

```py
 for x in range(65,91):
for x in range(ord('a'), ord('z')): 
```

#### **round()函数**

round()函数允许你将十进制值四舍五入到最近的精度：

```py
>>> round(1.23, 1)
1.2
>>> round(-3.42,1)
-3.4 
```

#### **数字格式化**

Python 允许你指定打印十进制数字时使用的精度位数，如下所示：

```py
 >>> x = 1.23456
>>> format(x, '0.2f')
'1.23'
>>> format(x, '0.3f')
'1.235'
>>> 'value is {:0.3f}'.format(x) 'value is 1.235'
>>> from decimal import Decimal
>>> a = Decimal('4.2')
>>> b = Decimal('2.1')
>>> a + b
Decimal('6.3')
>>> print(a + b)
6.3
>>> (a + b) == Decimal('6.3')
True
>>> x = 1234.56789
>>> # Two decimal places of accuracy
>>> format(x, '0.2f')
'1234.57'
>>> # Right justified in 10 chars, one-digit accuracy
>>> format(x, '>10.1f')
' 1234.6'
>>> # Left justified
>>> format(x, '<10.1f') '1234.6 '
>>> # Centered
>>> format(x, '¹⁰.1f') ' 1234.6 '
>>> # Inclusion of thousands separator
>>> format(x, ',')
'1,234.56789'
>>> format(x, '0,.1f')
'1,234.6' 
```

### **分数操作**

Python 支持 Fraction()函数（在 fractions 模块中定义），它接受两个整数，分别代表分数的分子和分母（分母必须非零）。以下展示了定义和操作分数的几个示例：

```py
 >>> from fractions import Fraction
>>> a = Fraction(5, 4)
>>> b = Fraction(7, 16)
>>> print(a + b)
27/16
>>> print(a * b) 35/64
>>> # Getting numerator/denominator
>>> c = a * b >>> c.numerator
35
>>> c.denominator 64
>>> # Converting to a float >>> float(c)
0.546875
>>> # Limiting the denominator of a value
>>> print(c.limit_denominator(8))
4
>>> # Converting a float to a fraction >>> x = 3.75
>>> y = Fraction(*x.as_integer_ratio())
>>> y
Fraction(15, 4) 
```

在深入探讨与字符串一起工作的代码示例之前，下一节简要讨论 Unicode 和 UTF-8，它们都是字符编码。

### **UNICODE 和 UTF-8**

Unicode 字符串由一系列介于 0 和 0x10ffff 之间的数字组成，其中每个数字代表一组字节。*编码*是将 Unicode 字符串转换为一系列字节的方式。在各种编码中，UTF-8（“Unicode 转换格式”）可能是最常用的，它也是许多系统的默认编码。UTF-8 中的数字 8 表示编码使用 8 位数字，而 UTF-16 使用 16 位数字（但这种编码较少见）。

ASCII 字符集是 UTF-8 的子集，因此有效的 ASCII 字符串可以作为一个 UTF-8 字符串读取，无需重新编码。此外，Unicode 字符串可以转换为 UTF-8 字符串。

### **UNICODE 和 UTF-8**

Python 支持 Unicode，这意味着你可以渲染不同语言的字符。Unicode 数据可以像字符串一样存储和处理。可以通过在前面添加字母 u 来创建一个 Unicode 字符串，如下所示：

```py
 >>> u'Hello from Python!' u'Hello from Python!' 
```

可以通过指定其 Unicode 值来在字符串中包含特殊字符。例如，以下 Unicode 字符串在字符串中嵌入了一个空格（其 Unicode 值为 0x0020）：

```py
 >>> u'Hello\u0020from Python!' u'Hello from Python!' 
```

列表 1.1 显示了 unicode1.py 的内容，该内容演示了如何显示一个日文字符串和另一个中文（普通话）字符串：

***列表 1.1：unicode1.py***

```py
 chinese1 = u'\u5c07\u63a2\u8a0e HTML5 \u53ca\u5176\u4ed6'
hiragana = u'D3 \u306F \u304B\u3063\u3053\u3043\u3043 \u3067\u3059!' print('Chinese:',chinese1)
print('Hiragana:',hiragana) 
```

列表 1.2 的输出如下：

```py
 Chinese: 將探討 HTML5 及其他
Hiragana: D3 は かっこぃぃ です! 
```

本章的下一部分将向你展示如何使用内置的 Python 函数“切片和切块”文本字符串。

### **字符串操作**

你可以使用“+”运算符连接两个字符串。以下示例首先打印一个字符串，然后连接两个单字母字符串：

```py
 >>> 'abc'
'abc'
>>> 'a' + 'b'
'ab' 
```

你可以使用“+”或“*”来连接相同的字符串，如下所示：

```py
 >>> 'a' + 'a' + 'a'
'aaa'
>>> 'a' * 3
'aaa' 
```

你可以将字符串分配给变量，并使用 print()命令打印它们：

```py
 >>> print('abc')
abc
>>> x = 'abc'
>>> print(x)
abc
>>> y = 'def'
>>> print(x + y)
abcdef 
```

你可以将字符串的字母“解包”并分配给变量，如下所示：

```py
 >>> str = "World"
>>> x1,x2,x3,x4,x5 = str
>>> x1 'W'
>>> x2
'o'
>>> x3
'r'
>>> x4
'l'
>>> x5
'd' 
```

前面的代码片段展示了提取文本字符串中的字母是多么容易，而在第三章中，你将学习如何“解包”其他数据结构。

你可以像以下示例那样提取字符串的子串：

```py
 >>> x = "abcdef"
>>> x[0]
'a'
>>> x[-1]
'f'
>>> x[1:3]
'bc'
>>> x[0:2] + x[5:]
'abf' 
```

然而，如果你尝试“减去”两个字符串，将会引发错误：

```py
 >>> 'a' - 'b'
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: unsupported operand type(s) for -: 'str' and 'str' 
```

try/except 构造允许你优雅地处理前面类型的中断。

#### **字符串比较**

你可以使用 lower() 和 upper() 方法将字符串分别转换为小写和大写，如下所示：

```py
 >>> 'Python'.lower()
'python'
>>> 'Python'.upper()
'PYTHON'
>>> 
```

lower() 和 upper() 方法对于执行两个 ASCII 字符串的不区分大小写的比较非常有用。列表 1.2 展示了使用 lower() 函数比较两个 ASCII 字符串的 compare.py 内容。

***列表 1.2：compare.py***

```py
 x = 'Abc'
y = 'abc'

if(x == y):
  print('x and y: identical')
elif (x.lower() == y.lower()):
  print('x and y: case insensitive match')
else:
  print('x and y: different') 
```

由于 x 包含混合大小写的字母，而 y 包含小写字母，列表 1.2 显示了以下输出：

```py
 x and y: different 
```

#### **字符串格式化**

Python 提供了 string.lstring()、string.rstring() 和 string.center() 函数，用于定位文本字符串，使其分别左对齐、右对齐和居中对齐。正如你在前面的章节中看到的，Python 还提供了 format() 方法来实现高级插值功能。

现在在解释器中输入以下命令：

```py
 import string

str1 = 'this is a string'
print(string.ljust(str1, 10))
print(string.rjust(str1, 40))
print(string.center(str1,40)) 
```

输出如下所示：

```py
 this is a string
                        this is a string
            this is a string 
```

本章的下一部分将向你展示如何使用内置函数“切片和切块”文本字符串。

### **字符串切片和拼接**

Python 允许你使用数组表示法提取字符串的子串（称为“切片”）。切片表示法是 start:stop:step，其中 start、stop 和 step 的值分别是整数，分别指定起始值、结束值和增量值。Python 切片的一个有趣之处在于你可以使用 -1 的值，它从字符串的右侧而不是左侧开始操作。

这里有一些字符串切片的示例：

```py
 text1 = "this is a string"
print('First 7 characters:',text1[0:7])
print('Characters 2-4:',text1[2:4])
print('Right-most character:',text1[-1])
print('Right-most 2 characters:',text1[-3:-1]) 
```

前一个代码块输出的内容如下：

```py
 First 7 characters: this is
Characters 2-4: is
Right-most character: g
Right-most 2 characters: in 
```

在本章的后面部分，你将看到如何将一个字符串插入到另一个字符串的中间。

#### **测试数字和字母字符**

Python 允许你检查字符串中的每个字符，然后测试该字符是否为真正的数字或字母字符。本节为第四章中讨论的正则表达式提供了一个先导。

列表 1.3 展示了 char_types.py 的内容，说明了如何确定一个字符串是否包含数字或字符。如果你对 列表 1.3 中的条件“if”语句不熟悉，更详细的信息可以在第二章中找到。

***列表 1.3：char_types.py***

```py
 str1 = "4"
str2 = "4234"
str3 = "b"
str4 = "abc"
str5 = "a1b2c3"

if(str1.isdigit()):
  print("this is a digit:",str1)

if(str2.isdigit()):
  print("this is a digit:",str2)

if(str3.isalpha()):
  print("this is alphabetic:",str3)

if(str4.isalpha()):
  print("this is alphabetic:",str4)

if(not str5.isalpha()):
  print("this is not pure alphabetic:",str5)

print("capitalized first letter:",str5.title()) 
```

列表 1.3 初始化了一些变量，然后进行了 2 个条件测试，使用 isdigit() 函数检查 str1 和 str2 是否为数字。列表 1.3 的下一部分使用 isalpha() 函数检查 str3、str4 和 str5 是否为字母字符串。列表 1.3 的输出如下：

```py
 this is a digit: 4
this is a digit: 4234
this is alphabetic: b
this is alphabetic: abc
this is not pure alphabetic: a1b2c3
capitalized first letter: A1B2C3 
```

### **在其他字符串中搜索和替换字符串**

Python 提供了在第二个文本字符串中搜索和替换字符串的方法。列表 1.4 展示了 find_pos1.py 的内容，展示了如何使用 find 函数在另一个字符串中搜索一个字符串的出现。

***列表 1.4：find_pos1.py***

```py
 item1 = 'abc'
item2 = 'Abc'
text = 'This is a text string with abc'

pos1 = text.find(item1)
pos2 = text.find(item2)

print('pos1=',pos1)
print('pos2=',pos2) 
```

列表 1.4 初始化了变量 item1、item2 和 text，然后在字符串 text 中搜索 item1 和 item2 的内容索引。find() 函数返回第一个成功匹配的列号；如果没有成功匹配，则 find() 函数返回 -1。

启动 列表 1.4 的输出如下：

```py
 pos1= 27
pos2= -1 
```

除了 find() 方法外，当你想要测试元素是否存在时，还可以使用 in 操作符，如下所示：

```py
 >>> lst = [1,2,3]
>>> 1 in lst
True 
```

列表 1.5 展示了 replace1.py 的内容，展示了如何用另一个字符串替换一个字符串。

***列表 1.5：replace1.py***

```py
 text = 'This is a text string with abc'
print('text:',text)
text = text.replace('is a', 'was a')
print('text:',text) 
```

列表 1.5 首先初始化变量 text 并打印其内容。然后 列表 1.5 将字符串 text 中的“is a”替换为“was a”，然后打印修改后的字符串。启动 列表 1.5 的输出如下：

```py
 text: This is a text string with abc
text: This was a text string with abc 
```

### **移除前导和尾随字符**

Python 提供了 strip()、lstrip() 和 rstrip() 函数来移除文本字符串中的字符。列表 1.6 展示了 remove1.py 的内容，展示了如何搜索字符串。

***列表 1.6：remove1.py***

```py
 text = '   leading and trailing white space   '
print('text1:','x',text,'y')

text = text.lstrip()
print('text2:','x',text,'y')

text = text.rstrip()
print('text3:','x',text,'y') 
```

列表 1.6 首先将字母 x 和变量 text 的内容连接起来，然后打印结果。列表 1.6 的第二部分移除了字符串 text 中的前导空白字符，然后将结果连接到字母 x 上。列表 1.6 的第三部分移除了字符串 text 中的尾随空白字符（注意，前导空白字符已经被移除），然后将结果连接到字母 x 上。

启动 列表 1.6 的输出如下：

```py
 text1: x    leading and trailing white space    y
text2: x leading and trailing white space    y
text3: x leading and trailing white space y 
```

如果你想在文本字符串内部移除多余的空白字符，请使用前面章节中讨论的 replace() 函数。以下示例说明了如何实现这一点，同时也包含 re 模块作为对你在 第四章 中将要学习内容的“预览”：

```py
 import re
text = 'a    b' a = text.replace(' ', '')
b = re.sub('\s+', ' ', text)

print(a)
print(b) 
```

结果如下：

```py
 ab
a b 
```

第二章 展示了如何使用 join() 函数在文本字符串中移除多余的空白字符。

### **不使用换行符打印文本**

如果你需要抑制使用多个 print()语句输出对象之间的空白和换行符，你可以使用连接或 write()函数。

第一种技术是在打印结果之前，使用 str()函数连接每个对象的字符串表示形式。例如，在 Python 中运行以下语句：

```py
 x = str(9)+str(0xff)+str(-3.1)
print('x: ',x) 
```

输出如下所示：

```py
 x:  9255-3.1 
```

前一行包含数字 9 和 255（这是十六进制数 0xff 的十进制值）以及-3.1 的连接。

顺便提一下，你可以使用 str()函数与模块和用户定义的类一起使用。以下是一个涉及 Python 内置模块 sys 的示例：

```py
 >>> import sys
>>> print(str(sys))
<module 'sys' (built-in)> 
```

以下代码片段说明了如何使用 write()函数显示一个字符串：

```py
 import sys
write = sys.stdout.write
write('123')
write('123456789') 
```

输出如下所示：

```py
 123123456789 
```

### **文本对齐**

Python 提供了 ljust()、rjust()和 center()方法用于对齐文本。ljust()和 rjust()函数分别左对齐和右对齐文本字符串，而 center()函数将字符串居中。以下代码块中有一个示例：

```py
 text = 'Hello World'
text.ljust(20)
'Hello World '
>>> text.rjust(20)
' Hello World'
>>> text.center(20)
' Hello World ' 
```

你可以使用 format()函数对文本进行对齐。使用<, >或^字符，以及所需的宽度，分别以右对齐、左对齐和居中对齐文本。以下示例说明了如何指定文本对齐方式：

```py
 >>> format(text, '>20')
'         Hello World'
>>>
>>> format(text, '<20')
'Hello World         '
>>>
>>> format(text, '²⁰')
'    Hello World     '
>>> 
```

### **处理日期**

Python 提供了一组丰富的日期相关函数。列表 1.7 显示了脚本 date_time2.py 的内容，该脚本显示各种日期相关值，例如当前日期和时间；星期几、月份和年份；以及自纪元以来的时间（以秒为单位）。

***列表 1.7：date_time2.py***

```py
 import time
import datetime

print("Time in seconds since the epoch: %s" %time.time())
print("Current date and time: " , datetime.datetime.now())
print("Or like this: " ,datetime.datetime.now().strftime("%y-%m-%d-%H-%M"))

print("Current year: ", datetime.date.today().strftime("%Y"))
print("Month of year: ", datetime.date.today().strftime("%B")) print("Week number of the year: ", datetime.date.today().strftime("%W"))
print("Weekday of the week: ", datetime.date.today().strftime("%w"))
print("Day of year: ", datetime.date.today().strftime("%j"))
print("Day of the month : ", datetime.date.today().strftime("%d"))
print("Day of week: ", datetime.date.today().strftime("%A")) 
```

列表 1.8 显示了运行列表 1.7 中的代码生成的输出。

***列表 1.8 datetime2.out***

```py
 Time in seconds since the epoch: 1375144195.66
Current date and time:  2013-07-29 17:29:55.664164
Or like this:  13-07-29-17-29
Current year:  2013
Month of year:  July
Week number of the year:  30
Weekday of the week:  1
Day of year:  210
Day of the month :  29
Day of week:  Monday 
```

Python 允许你使用日期相关值进行算术计算，以下代码块中有一个示例：

```py
 >>> from datetime import timedelta
>>> a = timedelta(days=2, hours=6)
>>> b = timedelta(hours=4.5)
>>> c = a + b
>>> c.days
2
>>> c.seconds
37800
>>> c.seconds / 3600
10.5
>>> c.total_seconds() / 3600
58.5 
```

#### **将字符串转换为日期**

列表 1.9 显示了 string2date.py 的内容，该内容说明了如何将字符串转换为日期，以及如何计算两个日期之间的差异。

***列表 1.9：string2date.py***

```py
 from datetime import datetime

text = '2014-08-13'
y = datetime.strptime(text, '%Y-%m-%d') z = datetime.now()
diff = z - y
print('Date difference:',diff) 
```

列表 1.9 的输出如下所示：

```py
 Date difference: -210 days, 18:58:40.197130 
```

### **Python 中的异常处理**

与 JavaScript 不同，在 Python 中你不能将数字和字符串相加。然而，你可以使用 Python 中的 try/except 结构检测非法操作，这与 JavaScript 和 Java 等语言中的 try/catch 结构类似。

以下是一个 try/except 块的示例：

```py
 try:
  x = 4
  y = 'abc'
  z = x + y
except:
  print('cannot add incompatible types:', x, y) 
```

当你运行前面的代码时，except 代码块中的 print()语句会被执行，因为变量 x 和 y 具有不兼容的类型。

在本章的早期部分，你也看到了减去两个字符串会抛出异常：

```py
 >>> 'a' - 'b'
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: unsupported operand type(s) for -: 'str' and 'str' 
```

处理这种情况的一个简单方法是使用 try/except 块：

```py
 >>> try:
... print('a' - 'b')
... except TypeError:
... print('TypeError exception while trying to subtract two strings')
... except:
... print('Exception while trying to subtract two strings')
... 
```

前面代码块的输出如下所示：

```py
 TypeError exception while trying to subtract two strings 
```

如您所见，前面的代码块指定了更细粒度的异常 TypeError，然后是一个通用的 except 代码块来处理在执行您的 Python 代码过程中可能发生的所有其他异常。这种风格类似于 Java 代码中的异常处理。

Listing 1.10 展示了 exception1.py 的内容，该程序说明了如何处理各种类型的异常。

***LISTING 1.10: exception1.py***

```py
 import sys

try:
    f = open('myfile.txt')
    s = f.readline()
    i = int(s.strip())
except IOError as err:
    print("I/O error: {0}".format(err))
except ValueError:
    print("Could not convert data to an integer.")
except:
    print("Unexpected error:", sys.exc_info()[0])
    raise 
```

Listing 1.10 包含一个 try 块后跟三个 except 语句。如果在 try 块中发生错误，第一个 except 语句将与发生的异常类型进行比较。如果匹配，则执行随后的 print() 语句，程序终止。如果不匹配，则对第二个 except 语句执行类似的测试。如果两个 except 语句都不匹配异常，第三个 except 语句将处理异常，这涉及到打印一条消息然后“抛出”一个异常。请注意，您也可以在单个语句中指定多个异常类型，如下所示：

```py
 except (NameError, RuntimeError, TypeError):
    print('One of three error types occurred') 
```

上述代码块更为紧凑，但您不知道三种错误类型中的哪一种发生了。Python 允许您定义自定义异常，但这个主题超出了本书的范围。

### **处理用户输入**

Python 允许您通过 input() 函数或 raw_input() 函数从命令行读取用户输入。Listing 1.11 展示了 user_input1.py 的内容，该程序提示用户输入他们的名字，然后使用插值显示响应。

***LISTING 1.11: user_input1.py***

```py
 userInput = input("Enter your name: ")
print ("Hello %s, my name is Python" % userInput) 
```

Listing 1.11 的输出如下（假设用户输入了单词 Dave）：

```py
 Hello Dave, my name is Python 
```

Listing 1.11 中的 print() 语句使用 %s 进行字符串插值，它将 % 符号后面的变量的值替换进去。当您需要在运行时确定某些内容时，这种功能显然很有用。

用户输入可能会引发异常（取决于您的代码执行的操作），因此包含异常处理代码很重要。

Listing 1.12 展示了 user_input2.py 的内容，该程序提示用户输入一个字符串，并尝试在 try/except 块中将字符串转换为数字。

***LISTING 1.12: user_input2.py***

```py
 userInput = input("Enter something: ")

try:
  x = 0 + eval(userInput)
  print('you entered the number:',userInput)
except:
  print(userInput,'is a string') 
```

Listing 1.12 在将用户输入转换为数字的结果中添加了数字 0。如果转换成功，将显示包含用户输入的消息。如果转换失败，except 代码块包含一个 print() 语句，显示一条消息。

**注意** *此代码示例使用 eval() 函数，应避免使用，以免您的代码评估任意（可能具有破坏性的）命令。*

列表 1.13 显示了 user_input3.py 的内容，提示用户输入两个数字，并尝试在 try/except 块中计算它们的和。

***列表 1.13: user_input3.py***

```py
 sum = 0

msg = 'Enter a number:'
val1 = input(msg) try:
  sum = sum + eval(val1)
except:
  print(val1,'is a string')

msg = 'Enter a number:'
val2 = input(msg)

try:
  sum = sum + eval(val2)
except:
  print(val2,'is a string')

print('The sum of',val1,'and',val2,'is',sum) 
```

列表 1.13 包含两个 try 块，每个 try 块后面都跟着一个 except 语句。第一个 try 块尝试将第一个用户提供的数字添加到变量 sum 中，第二个 try 块尝试将第二个用户提供的数字添加到之前输入的数字上。如果任一输入字符串不是有效的数字，将发生错误消息；如果两个都是有效数字，将显示包含输入数字及其总和的消息。务必阅读本章前面提到的有关 eval() 函数的注意事项。

### **命令行参数**

Python 提供了一个 getopt 模块来解析命令行选项和参数，sys 模块通过 sys.argv 提供了对任何命令行参数的访问。这有两个作用：

1.  sys.argv 是命令行参数的列表。

1.  len(sys.argv) 是命令行参数的数量。

在这里，sys.argv[0] 是程序名称，因此如果程序被命名为 test.py，它将匹配 sys.argv[0] 的值。

现在，您可以在命令行上为 Python 程序提供输入值，而不是通过提示用户输入来提供输入值。

例如，考虑以下所示的脚本 test.py：

```py
 #!/usr/bin/python
import sys
print('Number of arguments:',len(sys.argv),'arguments')
print('Argument List:', str(sys.argv)) 
```

现在按照以下方式运行上述脚本：

```py
 python test.py arg1 arg2 arg3 
```

这将产生以下结果：

```py
 Number of arguments: 4 arguments. Argument List: ['test.py', 'arg1', 'arg2', 'arg3'] 
```

从命令行指定输入值的功能非常有用。例如，假设您有一个包含 add 和 subtract 方法的自定义 Python 类，用于添加和减去一对数字。

您可以使用命令行参数指定对一对数字执行哪个方法，如下所示：

```py
 python MyClass add 3 5
python MyClass subtract 3 5 
```

这种功能非常有用，因为您可以在 Python 类中程序化地执行不同的方法，这意味着您可以为您自己的代码编写单元测试。阅读第八章了解如何创建自定义类。

列表 1.14 显示了 hello.py 的内容，展示了如何使用 sys.argv 检查命令行参数的数量。

***列表 1.14: hello.py***

```py
 import sys

def main():
  if len(sys.argv) >= 2:
    name = sys.argv[1]
  else:
    name = 'World'
  print('Hello', name)

# Standard boilerplate to invoke the main() function
if __name__ == '__main__':
  main() 
```

列表 1.14 定义了 main() 函数，该函数检查命令行参数的数量：如果此值至少为 2，则变量 name 被分配第二个参数的值（第一个参数是 hello.py），否则 name 被分配值 Hello。然后 print() 语句打印变量 name 的值。

列表 1.14 的最后部分使用条件逻辑来确定是否执行 main() 函数。

### **总结**

本章向您展示了如何处理数字并在数字上执行算术运算，然后您学习了如何处理字符串并使用字符串操作。您还学习了如何使用 try/except 结构来处理 Python 代码中可能发生的异常。下一章将向您展示如何处理条件语句、循环和用户定义的函数。

## 第二章

## *NUMPY 简介*

本章快速介绍了 Python NumPy 包，它提供了非常实用的功能，不仅适用于“常规”Python 脚本，也适用于基于 TensorFlow 的 Python 脚本。例如，您将看到包含循环、数组和列表的 NumPy 代码示例。您还将了解点积、reshape() 方法（非常有用！）、如何使用 Matplotlib 绘图（在第四章中详细讨论），以及线性回归的示例。

本章的第一部分简要介绍了 NumPy 以及其一些有用的特性。第二部分包含了 NumPy 中工作数组的示例，并对比了列表与数组相同 API 的使用。此外，您还将看到计算数组中元素指数相关值（平方、立方等）是多么简单。

本章的第二部分介绍了子范围的概念，这在机器学习任务中提取数据集的部分时非常有用（并且经常使用）。特别是，您将看到处理向量和数组中负（-1）子范围的代码示例，因为它们在向量和数组中的解释方式不同。

本章的第三部分深入探讨了其他 NumPy 方法，包括 reshape() 方法，这在处理图像文件时非常有用（并且非常常见）：一些 TensorFlow API 需要将 (R,G,B) 值的二维数组转换为相应的一维向量。

本章的第四部分深入探讨了线性回归、均方误差（MSE）以及如何使用 NumPy linspace() API 计算 MSE。

### **什么是 NumPy？**

NumPy 是一个 Python 库，提供了许多方便的方法和改进的代码性能。NumPy 包含了 Python 中的科学计算核心库，具有高性能的多维数组和向量化数学函数，以及线性代数和随机数支持。

NumPy 是基于 MatLab 构建的，支持列表、数组等。NumPy 比 MatLab 更易于使用，并且在 TensorFlow 代码以及 Python 代码中都非常常见。

#### **有用的 NumPy 特性**

NumPy 包含了 *ndarray* 对象，它封装了同构数据类型的 *多* 维数组。许多 ndarray 操作都是通过编译代码来执行的，以提高性能。

NumPy 数组与标准 Python 序列之间存在重要差异。首先，NumPy 数组具有固定大小，而 Python 列表可以动态扩展。其次，NumPy 数组是同质的，这意味着 NumPy 数组中的元素必须具有相同的数据类型。第三，NumPy 数组支持更高效的执行（并且需要更少的代码）来处理大量数据的各种操作。

现在您对 NumPy 有了一个大致的了解，让我们深入研究一些示例，这些示例说明了如何使用 NumPy 数组，这是下一节的主题。

### **什么是 NumPy 数组？**

*数组* 是一组连续的内存位置，用于存储数据。数组中的每个项目称为 *元素*。数组中的元素数量称为数组的 *维度*。一个典型的数组声明如下：

```py
 arr1 = np.array([1,2,3,4,5]) 
```

上述代码片段将 arr1 声明为一个包含五个元素的数组，您可以通过 arr1[0] 到 arr1[4] 访问这些元素。请注意，第一个元素的索引值为 0，第二个元素的索引值为 1，依此类推。因此，如果您声明一个包含 100 个元素的数组，那么第 100 个元素的索引值为 99。

**注意** *NumPy 数组中的第一个位置具有索引“0。”*

NumPy 将数组视为向量。数学运算按元素逐个执行。请记住以下区别：“加倍”数组会将每个元素乘以 2，而“加倍”列表会将列表添加到自身。

列表 2.1 展示了 nparray1.py 的内容，该文件说明了在 NumPy 数组上执行的一些操作。

***列表 2.1：nparray1.py***

```py
 import numpy as np

list1 = [1,2,3,4,5]
print(list1) arr1  = np.array([1,2,3,4,5])
print(arr1)

list2 = [(1,2,3),(4,5,6)]
print(list2)

arr2  = np.array([(1,2,3),(4,5,6)])
print(arr2) 
```

列表 2.1 定义了变量 list1 和 list2（它们是 Python 列表），以及变量 arr1 和 arr2（它们是数组），并打印了它们的值。启动 列表 2.1 的输出如下：

```py
 [1, 2, 3, 4, 5]
[1 2 3 4 5]
[(1, 2, 3), (4, 5, 6)]
[[1 2 3]
 [4 5 6]] 
```

如您所见，Python 列表和数组很容易定义。现在，我们准备查看一些列表和数组的循环操作。

### **使用循环**

列表 2.2 展示了 loop1.py 的内容，该文件说明了如何遍历 NumPy 数组和 Python 列表中的元素。

***列表 2.2：loop1.py***

```py
 import numpy as np

list = [1,2,3]
arr1 = np.array([1,2,3])

for e in list:
  print(e)

for e in arr1:
  print(e) 
```

列表 2.2 初始化了变量 list，它是一个 Python 列表，以及变量 arr1，它是一个 NumPy 数组。列表 2.2 的下一部分包含两个循环，每个循环遍历 list 和 arr1 中的元素。如您所见，两个循环的语法相同。启动 列表 2.2 的输出如下：

```py
 1
2
3
1
2
3 
```

### **向数组中添加元素（1）**

列表 2.3 展示了 append1.py 的内容，该文件说明了如何向 NumPy 数组和 Python 列表中添加元素。

***列表 2.3：append1.py***

```py
 import numpy as np

arr1 = np.array([1,2,3])

# these do not work:
#arr1.append(4)
#arr1 = arr1 + [5]

arr1 = np.append(arr1,4)
arr1 = np.append(arr1,[5])

for e in arr1:
  print(e)

arr2 = arr1 + arr1

for e in arr2:
  print(e) 
```

列表 2.3 初始化了变量 arr1，它是一个 NumPy 数组，并初始化了 arr2，它是一个另一个 NumPy 数组。启动 列表 2.3 的输出如下：

```py
 1
2
3
4
5
2
4
6
8
10 
```

### **向数组中添加元素（2）**

列表 2.4 展示了 append2.py 的内容，该内容说明了如何向 NumPy 数组和 Python 列表中追加元素。

***列表 2.4: append2.py***

```py
 import numpy as np

arr1 = np.array([1,2,3])
arr1 = np.append(arr1,4) for e in arr1:
  print(e)

arr1 = np.array([1,2,3])
arr1 = np.append(arr1,4)

arr2 = arr1 + arr1

for e in arr2:
  print(e) 
```

列表 2.4 初始化了变量 arr1，它是一个 NumPy 数组。请注意，NumPy 数组没有“追加”方法：这个方法通过 NumPy 本身提供。Python 列表和 NumPy 数组之间的重要区别之一是，“+” 运算符连接 Python 列表，而此运算符加倍 NumPy 数组中的元素。启动 列表 2.4 的输出如下：

```py
 1
2
3
4
2
4
6
8 
```

### **列表和数组相乘**

列表 2.5 展示了 multiply1.py 的内容，该内容说明了如何乘以 Python 列表和 NumPy 数组中的元素。

***列表 2.5: multiply1.py***

```py
 import numpy as np

list1 = [1,2,3]
arr1  = np.array([1,2,3])
print('list:  ',list1)
print('arr1:  ',arr1)
print('2*list:',2*list)
print('2*arr1:',2*arr1) 
```

列表 2.5 包含一个名为 list 的 Python 列表和一个名为 arr1 的 NumPy 数组。print() 语句显示了 list1 和 arr1 的内容，以及将 list1 和 arr1 加倍的结果。回想一下，“加倍”一个 Python 列表与加倍一个 Python 数组是不同的，这可以从启动 列表 2.5 的输出中看到：

```py
 ('list:  ', [1, 2, 3])
('arr1:  ', array([1, 2, 3]))
('2*list:', [1, 2, 3, 1, 2, 3])
('2*arr1:', array([2, 4, 6])) 
```

### **列表中元素的加倍**

列表 2.6 展示了 double_list1.py 的内容，该内容说明了如何加倍 Python 列表中的元素。

***列表 2.6: double_list1.py***

```py
 import numpy as np

list1 = [1,2,3]
list2 = []

for e in list1:
  list2.append(2*e)

print('list1:',list1)
print('list2:',list2) 
```

列表 2.6 包含一个名为 list1 的 Python 列表和一个空白的 Python 列表名为 list2。接下来的代码片段遍历 list1 中的元素，并将它们追加到变量 list2 中。一对 print() 语句显示了 list1 和 list2 的内容，以显示它们是相同的。启动 列表 2.6 的输出如下：

```py
 ('list: ', [1, 2, 3])
('list2:', [2, 4, 6]) 
```

### **列表和指数**

列表 2.7 展示了 exponent_list1.py 的内容，该内容说明了如何计算 Python 列表中元素的指数。

***列表 2.7: exponent_list1.py***

```py
 import numpy as np

list1 = [1,2,3]
list2 = []

for e in list1:
  list2.append(e*e) # e*e = squared

print('list1:',list1)
print('list2:',list2) 
```

列表 2.7 包含一个名为 list1 的 Python 列表和一个空白的 Python 列表名为 list2。接下来的代码片段遍历 list1 中的元素，并将每个元素的平方追加到变量 list2 中。一对 print() 语句显示了 list1 和 list2 的内容。启动 列表 2.7 的输出如下：

```py
 ('list1:', [1, 2, 3])
('list2:', [1, 4, 9]) 
```

### **数组和指数**

列表 2.8 展示了 exponent_array1.py 的内容，该内容说明了如何计算 NumPy 数组中元素的指数。

***列表 2.8: exponent_array1.py***

```py
 import numpy as np

arr1 = np.array([1,2,3])
arr2 = arr1**2
arr3 = arr1**3

print('arr1:',arr1)
print('arr2:',arr2)
print('arr3:',arr3) 
```

列表 2.8 包含一个名为 arr1 的 NumPy 数组，后面跟着两个名为 arr2 和 arr3 的 NumPy 数组。请注意，NumPy 的 arr2 以 arr1 中元素的平方初始化，然后是 NumPy 数组 arr3 以 arr1 中元素的立方初始化。三个 print() 语句显示了 arr1、arr2 和 arr3 的内容。启动 列表 2.8 的输出如下：

```py
 ('arr1:', array([1, 2, 3]))
('arr2:', array([1, 4, 9]))
('arr3:', array([ 1,  8, 27])) 
```

### **数学运算和数组**

列表 2.9 展示了 mathops_array1.py 的内容，该内容说明了如何计算 NumPy 数组中元素的指数。

***列表 2.9: mathops_array1.py***

```py
 import numpy as np

arr1 = np.array([1,2,3])
sqrt = np.sqrt(arr1)
log1 = np.log(arr1)
exp1 = np.exp(arr1)

print('sqrt:',sqrt)
print('log1:',log1)
print('exp1:',exp1) 
```

列表 2.9 包含一个名为 arr1 的 NumPy 数组，后面跟着三个名为 sqrt、log1 和 exp1 的 NumPy 数组，分别初始化为 arr1 中元素的平方根、对数和指数值。三个 print() 语句显示了 sqrt、log1 和 exp1 的内容。启动 列表 2.9 的输出如下：

```py
 ('sqrt:', array([1\. , 1.41421356, 1.73205081]))
('log1:', array([0\. , 0.69314718, 1.09861229]))
('exp1:', array([2.71828183, 7.3890561,  20.08553692])) 
```

### **使用向量处理“–1”子范围**

列表 2.10 展示了 npsubarray2.py 的内容，该内容说明了如何计算 NumPy 数组中元素的指数。

***列表 2.10: npsubarray2.py***

```py
 import numpy as np

# -1 => "all *except* the last element in …" (row or col)

arr1  = np.array([1,2,3,4,5])
print('arr1:',arr1)
print('arr1[0:-1]:',arr1[0:-1])
print('arr1[1:-1]:',arr1[1:-1])
print('arr1[::-1]:', arr1[::-1]) # reverse! 
```

列表 2.10 包含一个名为 arr1 的 NumPy 数组，后面跟着四个 print() 语句，每个语句都显示了 arr1 中不同范围的值。启动 列表 2.10 的输出如下：

```py
 ('arr1:',       array([1, 2, 3, 4, 5]))
('arr1[0:-1]:', array([1, 2, 3, 4]))
('arr1[1:-1]:', array([2, 3, 4]))
('arr1[::-1]:', array([5, 4, 3, 2, 1])) 
```

### **使用数组处理“–1”子范围**

列表 2.11 展示了 np2darray2.py 的内容，该内容说明了如何计算 NumPy 数组中元素的指数。

***列表 2.11: np2darray2.py***

```py
 import numpy as np

# -1 => "the *last* element in …" (row or col)

arr1  = np.array([(1,2,3),(4,5,6),(7,8,9),(10,11,12)])
print('arr1:',        arr1)
print('arr1[-1,:]:',  arr1[-1,:])
print('arr1[:,-1]:',  arr1[:,-1])
print('arr1[-1:,-1]:',arr1[-1:,-1]) 
```

列表 2.11 包含一个名为 arr1 的 NumPy 数组，后面跟着四个 print() 语句，每个语句都显示了 arr1 中不同范围的值。启动 列表 2.11 的输出如下：

```py
 (arr1:', array([[1,  2,  3],
                [4,  5,  6],
                [7,  8,  9],
                [10, 11, 12]]))
(arr1[-1,:]]',   array([10, 11, 12]))
(arr1[:,-1]:',   array([3,  6,  9, 12]))
(arr1[-1:,-1]]', array([12])) 
```

### **其他有用的 NumPy 方法**

除了本节之前代码示例中看到的 NumPy 方法之外，以下 NumPy 方法也非常有用。

+   np.zeros() 方法使用 0 值初始化一个数组。

+   np.ones() 方法使用 1 值初始化一个数组。

+   np.empty() 方法使用 0 值初始化一个数组。

+   np.arange() 方法提供了一系列数字。

+   np.shape() 方法显示了一个对象的大小。

+   np.reshape() 方法 <= *非常有用！*

+   np.linspace() 方法 <= *非常有用，用于回归*

+   np.mean() 方法计算一组数字的平均值。

+   np.std() 方法计算一组数字的标准差。

虽然 np.zeros() 和 np.empty() 都使用 0 初始化一个二维数组，但 np.zeros() 需要更少的执行时间。您还可以使用 np.full(size, 0)，但这是三种方法中最慢的一种。

reshape() 方法以及 linspace() 方法非常有用，分别用于改变数组的维度和生成一系列数值。reshape() 方法常出现在 TensorFlow 代码中，而 linspace() 方法对于生成线性回归中的一组数字非常有用。关于 np.reshape() 和 np.linspace() 方法的更多细节将在本章后面提供。

mean() 和 std() 方法对于计算一组数字的均值和标准差非常有用。例如，您可以使用这两个方法来调整高斯分布中的值，使它们的均值变为 0，标准差变为 1。这个过程被称为 *标准化* 高斯分布。

### **数组和向量运算**

列表 2.12 展示了 array_vector.py 的内容，该文件说明了如何在 NumPy 数组中的元素上执行向量运算。

***列表 2.12: array_vector.py***

```py
 import numpy as np

a = np.array([[1,2], [3, 4]])
b = np.array([[5,6], [7,8]])

print('a:       ', a)
print('b:       ', b)
print('a + b:   ', a+b)
print('a - b:   ', a-b)
print('a * b:   ', a*b)
print('a / b:   ', a/b)
print('b / a:   ', b/a)
print('a.dot(b):',a.dot(b)) 
```

列表 2.12 包含两个名为 a 和 b 的 NumPy 数组，后面跟着八个 print() 语句，每个语句都显示将不同的算术运算应用于 NumPy 数组 a 和 b 的结果。启动 列表 2.12 的输出如下：

```py
 ('a    :   ', array([[1, 2], [3, 4]]))
('b    :   ', array([[5, 6], [7, 8]]))
('a + b:   ', array([[ 6,  8], [10, 12]]))
('a - b:   ', array([[-4, -4], [-4, -4]]))
('a * b:   ', array([[ 5, 12], [21, 32]]))
('a / b:   ', array([[0, 0], [0, 0]]))
('b / a:   ', array([[5, 3], [2, 2]]))
('a.dot(b):', array([[19, 22], [43, 50]])) 
```

### **NumPy 和点积（1）**

列表 2.13 展示了 dotproduct1.py 的内容，该文件说明了如何在 NumPy 数组中的元素上执行点积。

***列表 2.13: dotproduct1.py***

```py
 import numpy as np

a = np.array([1,2])
b = np.array([2,3])

dot2 = 0
for e,f in zip(a,b):
  dot2 += e*f print('a:   ',a)
print('b:   ',b)
print('a*b: ',a*b)
print('dot1:',a.dot(b))
print('dot2:',dot2) 
```

列表 2.13 包含两个名为 a 和 b 的 NumPy 数组，后面跟着一个简单的循环，该循环计算 a 和 b 的点积。下一节包含五个 print() 语句，显示 a 和 b 的内容，以及以三种不同方式计算的内积。启动 列表 2.13 的输出如下：

```py
 ('a:   ', array([1, 2]))
('b:   ', array([2, 3]))
('a*b: ', array([2, 6]))
('dot1:', 8)
('dot2:', 8) 
```

### **NumPy 和点积（2）**

NumPy 数组支持一个“点”方法来计算数字数组的内积，该方法使用与计算一对向量内积相同的公式。列表 2.14 展示了 dotproduct2.py 的内容，该文件说明了如何计算两个 NumPy 数组的点积。

***列表 2.14: dotproduct2.py***

```py
 import numpy as np

a = np.array([1,2])
b = np.array([2,3])

print('a:          ',a)
print('b:          ',b)
print('a.dot(b):   ',a.dot(b))
print('b.dot(a):   ',b.dot(a))
print('np.dot(a,b):',np.dot(a,b))
print('np.dot(b,a):',np.dot(b,a)) 
```

列表 2.14 包含两个名为 a 和 b 的 NumPy 数组，后面跟着六个 print() 语句，显示 a 和 b 的内容，以及以三种不同方式计算的内积。启动 列表 2.14 的输出如下：

```py
 ('a:          ', array([1, 2]))
('b:          ', array([2, 3]))
('a.dot(b):   ', 8)
('b.dot(a):   ', 8)
('np.dot(a,b):', 8)
('np.dot(b,a):', 8) 
```

### **NumPy 和向量的长度**

向量（或数字数组）的范数是向量的长度，即向量与其自身点积的平方根。NumPy 还提供了“求和”和“平方”函数，您可以使用这些函数来计算向量的范数。

列表 2.15 展示了 array_norm.py 的内容，该文件说明了如何计算数字 NumPy 数组的幅度（“范数”）。

***列表 2.15: array_norm.py***

```py
 import numpy as np

a = np.array([2,3])
asquare = np.square(a)
asqsum  = np.sum(np.square(a))
anorm1  = np.sqrt(np.sum(a*a))
anorm2  = np.sqrt(np.sum(np.square(a)))
anorm3  = np.linalg.norm(a)

print('a:      ',a)
print('asquare:',asquare)
print('asqsum: ',asqsum)
print('anorm1: ',anorm1)
print('anorm2: ',anorm2)
print('anorm3: ',anorm3) 
```

列表 2.15 包含一个初始的 NumPy 数组 a，后面跟着 NumPy 数组 asquare 和数值 asqsum、anorm1、anorm2 和 anorm3。NumPy 数组 asquare 包含 NumPy 数组 a 中元素的平方，而数值 asqsum 包含 NumPy 数组 asquare 中元素的总和。

接下来，数值 anorm1 等于 a 中元素平方和的平方根。数值 anorm2 与 anorm1 相同，但计算方式略有不同。最后，数值 anorm3 等于 anorm2，但如您所见，anorm3 通过单个 NumPy 方法计算，而 anorm2 需要一系列 NumPy 方法。

列表 2.15 的最后部分由六个 print() 语句组成，每个语句都显示了计算出的值。启动 列表 2.15 的输出如下：

```py
 ('a:      ', array([2, 3]))
('asquare:', array([4, 9]))
('asqsum: ', 13)
('anorm1: ', 3.605551275463989)
('anorm2: ', 3.605551275463989)
('anorm3: ', 3.605551275463989) 
```

### **NUMPY 和其他操作**

NumPy 提供了“*”运算符，用于将两个向量的分量相乘，产生一个第三向量，其分量是初始一对向量对应分量的乘积。这种操作称为 *Hadamard 积*，这是著名数学家的名字。如果您然后将第三向量的分量相加，总和等于初始一对向量的内积。

列表 2.16 展示了 otherops.py 的内容，该内容说明了如何在 NumPy 数组上执行其他操作。

***列表 2.16: otherops.py***

```py
 import numpy as np

a = np.array([1,2])
b = np.array([3,4])

print('a:           ',a)
print('b:           ',b)
print('a*b:         ',a*b)
print('np.sum(a*b): ',np.sum(a*b))
print('(a*b.sum()): ',(a*b).sum()) 
```

列表 2.16 包含两个名为 a 和 b 的 NumPy 数组，后面跟着五个 print() 语句，这些语句显示了 a 和 b 的内容、它们的 Hadamard 积以及以两种不同方式计算的它们的内积。启动 列表 2.16 的输出如下：

```py
 ('a:           ', array([1, 2]))
('b:           ', array([3, 4]))
('a*b:         ', array([3, 8]))
('np.sum(a*b): ', 11)
('(a*b.sum()): ', 11) 
```

### **NUMPY 和 RESHAPE() 方法**

NumPy 数组支持 reshape() 方法，允许您重新结构化数字数组的维度。一般来说，如果一个 NumPy 数组包含 m 个元素，其中 m 是一个正整数，那么该数组可以被重新结构化为一个 m1 x m2 的 NumPy 数组，其中 m1 和 m2 是正整数，且满足 m1*m2 = m。

列表 2.17 展示了 numpy_reshape.py 的内容，该内容说明了如何在 NumPy 数组上使用 reshape() 方法。

***列表 2.17: numpy_reshape.py***

```py
 import numpy as np

x = np.array([[2, 3], [4, 5], [6, 7]])
print(x.shape) # (3, 2)

x = x.reshape((2, 3))
print(x.shape) # (2, 3)
print('x1:',x)

x = x.reshape((-1))
print(x.shape) # (6,)
print('x2:',x)

x = x.reshape((6, -1))
print(x.shape) # (6, 1)
print('x3:',x)

x = x.reshape((-1, 6))
print(x.shape) # (1, 6)
print('x4:',x) 
```

列表 2.17 包含一个名为 x 的 NumPy 数组，其维度为 3x2，随后是一系列对 reshape() 方法的调用，这些调用改变了 x 的内容。第一次调用 reshape() 方法将 x 的形状从 3x2 改变为 2x3。第二次调用将 x 的形状从 2x3 改变为 6x1。第三次调用将 x 的形状从 1x6 改变为 6x1。最后一次调用将 x 的形状再次从 6x1 改变为 1x6。

每次调用 reshape() 方法后都跟着一个 print() 语句，以便您可以看到调用的影响。启动 列表 2.17 的输出如下：

```py
 (3, 2)
(2, 3)
('x1:', array([[2, 3, 4],
       [5, 6, 7]]))
(6,)
('x2:', array([2, 3, 4, 5, 6, 7]))
(6, 1)
('x3:', array([[2],
       [3],
       [4],
       [5],
       [6],
       [7]]))
(1, 6) 
```

### **计算均值和标准差**

如果您需要回顾这些来自统计学（也许还包括均值、中位数和众数）的概念，请阅读相应的在线教程。

NumPy 提供了各种内置函数，用于执行统计计算，如下列方法列表所示：

```py
 np.linspace() <= useful for regression
np.mean()
np.std() 
```

np.linspace() 方法生成一个介于下限和上限之间的等间距数字集合。np.mean() 和 np.std() 方法分别计算一组数字的均值和标准差。列表 2.18 展示了 sample_mean_std.py 的内容，该内容说明了如何从 NumPy 数组中计算统计值。

***列表 2.18: sample_mean_std.py***

```py
 import numpy as np

x2 = np.arange(8)
print('mean = ',x2.mean())
print('std  = ',x2.std())

x3 = (x2 - x2.mean())/x2.std()
print('x3 mean = ',x3.mean())
print('x3 std  = ',x3.std()) 
```

列表 2.18 包含一个 NumPy 数组 x2，该数组由前八个整数组成。接下来，调用与 x2 相关的 mean() 和 std() 来计算 x2 元素的均值和标准差。启动 列表 2.18 的输出如下：

```py
 ('a:           ', array([1, 2]))
('b:           ', array([3, 4])) 
```

### **具有均值和标准差的代码示例**

本节中的代码示例在上一节的代码示例基础上扩展了额外的统计值，列表 2.19 中的代码可以用于任何数据分布。请注意，代码示例使用随机数字仅用于说明目的：在您启动代码示例后，将这些数字替换为来自 CSV 文件或其他包含有意义值的数据集的值。

此外，本节不提供关于四分位数含义的详细信息，但您可以在 *[`en.wikipedia.org/wiki/Quartile`](https://en.wikipedia.org/wiki/Quartile)* 上了解四分位数。

列表 2.19 展示了 stat_values.py 的内容，该内容说明了如何从随机数的 NumPy 数组中显示各种统计值。

***列表 2.19: stat_values.py***

```py
 import numpy as np

from numpy import percentile
from numpy.random import rand

# generate data sample data = np.random.rand(1000) # calculate quartiles, min, and max
quartiles = percentile(data, [25, 50, 75])
data_min, data_max = data.min(), data.max()

# print summary information
print('Minimum:  %.3f' % data_min)
print('Q1 value: %.3f' % quartiles[0])
print('Median:   %.3f' % quartiles[1])
print('Mean Val: %.3f' % data.mean())
print('Std Dev:  %.3f' % data.std())
print('Q3 value: %.3f' % quartiles[2])
print('Maximum:  %.3f' % data_max) 
```

列表 2.19 中的数据样本（以粗体显示）来自 0 和 1 之间的均匀分布。NumPy 的 percentile() 函数计算观察值之间的线性插值（平均值），这在计算具有偶数个值的样本的中位数时是必需的。正如您可以推测的那样，NumPy 的 min() 和 max() 函数计算数据样本中的最小值和最大值。启动 列表 2.19 的输出如下：

```py
 Minimum:  0.000
Q1 value: 0.237
Median:   0.500
Mean Val: 0.495
Std Dev:  0.295
Q3 value: 0.747
Maximum:  0.999 
```

#### **截尾均值和加权均值**

除了算术均值之外，还有被称为截尾均值（也称为“截断均值”）和加权均值的变体。

截尾均值是一种稳健的估计（即，对异常值不敏感的度量）。截尾均值的一个简单例子是，假设您有五个用于评估产品的分数：简单地丢弃最高分和最低分，然后计算剩余三个分数的平均值。如果您有多个五分数的集合，重复前面的过程，然后计算截尾均值值的集合的平均值。

当样本数据不能代表数据集中的不同组时，*加权平均*很有用。给代表性不足的组分配更大的权重，可以得到一个更准确地表示数据集中各种组的加权平均。然而，请注意，异常值会影响平均值以及加权平均值。

加权平均与期望值相同。如果你不熟悉期望值的概念，假设集合 P = {p1,p2,...,pn} 是一个概率分布，这意味着集合 P 中的数值必须是非负的，并且它们的和等于 1。此外，假设 V = {v1,v2,...,vn} 是一个分配给产品 M 的 n 个特征的数值分数集合。例如，集合 V 中的值可以是某些范围内的正整数（例如，1 到 10 之间），代表“奖励”。

然后，该产品的 *期望值* E 计算如下：

```py
 E = p1*v1 + p2*v2 + ... + pn*vn 
```

在接下来的几个部分中，Python 代码示例包含了一些来自 Matplotlib 的基本 API。代码示例从线段的简单示例开始，然后介绍线性回归。

### **平面中线的处理（可选）**

本节包含了对欧几里得平面中线的简要回顾，因此如果你对这个主题感到舒适，可以跳过这一节。一个常被忽视的细微之处是，欧几里得平面中的线具有无限长度。如果你选择一条线上的两个不同点，那么这两个选定点之间的所有点都构成一个 *线段*。*射线* 是“半无限”的线：当你选择一个点作为端点时，那么线的一侧的所有点构成一个射线。

例如，平面中 y 坐标为 0 的点形成沿 x 轴的线，而 x 轴上 (0,0) 和 (1,0) 之间的点形成线段。此外，x 轴上位于 (0,0) 右侧的点形成一个射线，而 x 轴上位于 (0,0) 左侧的点也形成一个射线。

为了简单和方便，在这本书中，我们将“线”和“线段”这两个术语互换使用。现在，让我们深入了解欧几里得平面中线的细节。以下是欧几里得平面中一条（非垂直）线的方程：

```py
 y = m*x + b 
```

m 的值是线的斜率，b 的值是 y 轴截距（即非垂直线与 y 轴相交的地方）。平面中线的以下形式是一个包含垂直线的通用方程：

```py
 a*x + b*y + c = 0 
```

然而，我们不会处理垂直线，因此我们将继续使用第一个公式。图 2.1 显示了三条水平线，其方程（从上到下）分别是 y = 3，y = 0 和 y = -3。

![图片](img/python-3-data-visualization-using-chatgpt-f0046-01.jpg)

***图 2.1*** 三个水平线段的图

图 2.2 显示了两条斜线，其方程为 y = x 和 y = -x。

![图片](img/python-3-data-visualization-using-chatgpt-f0046-02.jpg)

***图 2.2*** 两个对角线段图

图 2.3 显示了两个斜率平行的线段，其方程为 y = 2*x 和 y = 2*x+3。

![图片](img/python-3-data-visualization-using-chatgpt-f0047-01.jpg)

***图 2.3*** 两条斜率平行的线段图

图 2.4 显示了一个由连接线段组成的分段线性图。

![图片](img/python-3-data-visualization-using-chatgpt-f0047-02.jpg)

***图 2.4*** 线段的分段线性图

现在你已经看到了欧几里得平面中一些基本线条的例子，让我们看看一些使用 NumPy 和 Matplotlib 显示平面中点散点图的代码示例。

### **使用 NumPy 和 Matplotlib 绘制随机点**

前一节包含了一些线段的简单例子，但代码被推迟到 第七章。本节和下一节包含了一些未讨论的 Matplotlib API 的代码示例；然而，代码很简单，所以你可以推断其目的。此外，你还可以在 第七章（专注于数据可视化）中了解更多关于 Matplotlib 的信息，或者阅读一个简短的在线教程以获取更多细节。

列表 2.20 展示了 np_plot.py 的内容，说明了如何在平面上绘制多个点。

***列表 2.20：np_plot.py***

```py
 import numpy as np
import matplotlib.pyplot as plt

x = np.random.randn(15,1)
y = 2.5*x + 5 + 0.2*np.random.randn(15,1)

plt.scatter(x,y)
plt.show() 
```

列表 2.20 从两个导入语句开始，然后通过 NumPy randn() API 初始化 x 为一组随机值。接下来，y 被分配一系列值，这些值由两部分组成：一个线性方程，其输入值来自 x 的值，并与一个随机化因子相结合。图 2.5 显示了 列表 2.20 中的代码生成的输出。

![图片](img/python-3-data-visualization-using-chatgpt-f0048-01.jpg)

***图 2.5*** 具有潜在线性回归的数据集

### **使用 NumPy 和 Matplotlib 绘制二次曲线**

列表 2.21 展示了 np_plot_quadratic.py 的内容，说明了如何在平面上绘制二次函数。

***列表 2.21：np_plot_quadratic.py***

```py
 import numpy as np
import matplotlib.pyplot as plt

x = np.linspace(-5,5,num=100)[:,None]
y = -0.5 + 2.2*x +0.3*x**3+ 2*np.random.randn(100,1)

plt.plot(x,y)
plt.show() 
```

列表 2.21 从两个导入语句开始，然后通过 NumPy linspace() API 初始化 x 为一系列值。接下来，y 被分配一系列值，这些值符合一个二次方程，这些值基于变量 x 的值。图 2.6 显示了 列表 2.21 中的代码生成的输出。

![图片](img/python-3-data-visualization-using-chatgpt-f0049-01.jpg)

***图 2.6*** 具有潜在线性回归的数据集，显示了由 列表 2.21 中的代码生成的输出

现在你已经看到了各种线图和散点图，让我们深入研究线性回归，这是下一节的主题。

### **什么是线性回归？**

*线性回归*是在 1805 年创建的，它是统计分析和机器学习中的一个重要算法。任何像样的统计软件包都支持线性回归，并且总是支持多项式回归。线性回归涉及直线，这些是次数为一的多项式，而多项式回归涉及将次数大于一的多项式拟合到数据集上。

从一般意义上讲，线性回归找到最佳拟合超平面的方程，该超平面的次数比数据集的维度少一。特别是，如果数据集在欧几里得平面上，超平面就是一条直线；如果数据集在 3D 中，超平面是一个“常规”平面。

当数据集中的点以某种方式分布，可以合理地用超平面近似时，线性回归是合适的。如果不这样，那么你可以尝试拟合其他类型的多元多项式曲面到数据集中的点。

请记住另外两个细节。首先，最佳拟合超平面不一定与数据集中的所有（甚至大多数）点相交。事实上，最佳拟合超平面可能不会与数据集中的任何点相交。最佳拟合超平面的目的是尽可能接近地*近似*数据集中的点。其次，线性回归*不等于*曲线拟合，曲线拟合试图找到一个通过一组点的多项式。

关于曲线拟合的一些细节如下。在平面上给定 n 个点（其中没有两个点的 x 值相同），存在一个次数小于或等于 n-1 的多项式通过这些点。因此，一条直线（次数为 1）将穿过平面上的任何一对非垂直点。对于平面上的任意三个点，存在一个二次方程或一条直线通过这些点。

在某些情况下，可以使用较低次数的多项式。例如，考虑 x 值等于 y 值的 100 个点的集合：显然，直线 y = x（次数为 1 的多项式）穿过所有这些点。

然而，一条线“代表”平面上的一组点的程度取决于这些点可以被线近似得多紧密。

#### **什么是多元分析？**

*多元分析*推广了欧几里得平面上的直线方程，其形式如下：

```py
 y = w1*x1 + w2*x2 + . . . + wn*xn + b 
```

前面的方程包含变量 x1, x2, ..., xn 的线性组合。在这本书中，我们通常会处理涉及欧几里得平面上的线的数据集。

#### **非线性数据集怎么办？**

简单线性回归找到最佳拟合数据集的线，但如果数据集在平面上不拟合线怎么办？这是一个很好的观点！在这种情况下，我们寻找其他曲线来近似数据集，例如二次、三次或更高次数的多项式。然而，这些替代方案涉及权衡，我们将在后面讨论。

另一种可能性是使用连续的分段线性函数，这是一种由一系列线段组成的函数，其中相邻线段是连接的。如果一对或多对相邻线段没有连接，那么它就是一个分段线性函数（即，函数是不连续的）。在任何情况下，线段的次数都是一，这比高阶多项式的计算复杂度低。

因此，给定平面上的点集，尝试找到最佳拟合线，在解决以下问题后：

1.  我们如何知道一条线“适合”数据？

1.  如果另一种类型的曲线更适合怎么办？

1.  “最佳拟合”是什么意思？

检查一条线是否很好地适合数据的一种方法是通过简单的视觉检查：在图表中显示数据，如果数据合理地符合线的形状，那么线可能是一个好的拟合。然而，这是一个主观的决定，一个不适合线的样本数据集在图 2.7 中显示。

图 2.7 展示了一个包含四个点且不适合线的数据集。

![图片](img/python-3-data-visualization-using-chatgpt-f0051-01.jpg)

***图 2.7*** 非线性数据集

然而，如果一条线看起来不适合数据，那么可能一个二次或三次（甚至更高次）的多项式有更好的拟合潜力。让我们先不考虑非线性情况，假设一条线对于数据来说是一个好的拟合。对于这样的数据集，有一个寻找最佳拟合线的方法：均方误差（MSE）。

### **均方误差（MSE）公式**

图 2.8 展示了 MSE 的公式。MSE 是实际 y 值与预测 y 值之间差的平方和除以点的数量。请注意，预测 y 值是如果数据点实际上在最佳拟合线上，每个数据点将具有的 y 值。

通常，目标是使误差最小化，这在线性回归的情况下决定了最佳拟合线。然而，当认为减少误差所需的时间和/或成本过高时，你可能会对“足够好”的值感到满意，这意味着这个决定不是纯粹程序性的决定。

图 2.8 展示了用于计算平面上点集最佳拟合线的均方误差公式。

![图片](img/python-3-data-visualization-using-chatgpt-f0052-01.jpg)

***图 2.8*** 均方误差公式

#### **其他误差类型**

虽然我们在这本书中只讨论了线性回归的 MSE，但还有其他类型的误差公式可以用于线性回归，其中一些列在这里：

+   MAE

+   RMSE

+   RMSPROP

+   MAE

均方误差是前面提到的误差类型的基础。例如，RMSE 是均方根误差，它是 MSE 的平方根。

平均绝对误差（MAE）是**y 项差异的绝对值之和**（而不是 y 项差异的平方），它不是 y 项差异的平方。

RMSProp 优化器利用最近梯度的幅度来归一化梯度。维护一个 RMS（均方根，即 MSE 的平方根）梯度的移动平均值，然后将该值除以当前梯度。

虽然计算 MSE 的导数（因为它是一个可微函数）更容易，但 MSE 也比 MAE 更容易受到异常值的影响。原因很简单：一个平方项可以比加上一个项的绝对值大得多。例如，如果一个差异项是 10，那么 100（平方项）会被加到 MSE 上，而只有 10（绝对值）会被加到 MAE 上。同样，如果一个差异项是-20，那么 400（平方项）会被加到 MSE 上，而只有 20（-20 的绝对值）会被加到 MAE 上。

#### **非线性最小二乘法**

在预测房价的情况下，数据集包含广泛的值，线性回归或随机森林等技术可能会导致模型为了减少如平均绝对误差等量而“过拟合”具有最高值的样本。

在这种情况下，你可能想要一个错误度量，如相对误差，它减少了拟合具有最大值的样本的重要性。这种技术称为**非线性最小二乘法**，它可能使用基于对数变换的标签和预测值。

### **手动计算 MSE**

让我们看看两个简单的图表，每个图表都包含一条近似散点图中一组点的线。注意，这两组点的线段是相同的，但数据集略有不同。我们将手动计算这两个数据集的均方误差（MSE），并确定哪个 MSE 值更小。

图 2.9 展示了一组点和一条可能是最佳拟合线的候选线。

![图片](img/python-3-data-visualization-using-chatgpt-f0053-01.jpg)

***图 2.9*** 近似散点图点的线图

图 2.9 中线的 MSE 计算如下：

```py
 MSE = 1*1 + (-1)*(-1) + (-1)*(-1) + 1*1 = 4 
```

现在看看图 2.10，它也展示了一组点和一条可能是数据最佳拟合线的候选线。

![图片](img/python-3-data-visualization-using-chatgpt-f0054-01.jpg)

***图 2.10*** 近似散点图点的线图

图 2.10 中线的 MSE 计算如下：

```py
 MSE = (-2)*(-2) + 2*2 = 8 
```

因此，图 2.10 中的线比图 2.9 中的线具有更小的 MSE，这可能会让你感到惊讶（或者你猜对了？）

在这两个图中，我们轻松快速地计算了 MSE，但在一般情况下，这要困难得多。例如，如果我们绘制 10 个在欧几里得平面上的点，这些点并不紧密地拟合一条线，并且涉及非整数值的各个项，我们可能需要计算器。更好的解决方案是使用 NumPy 函数，如下一节所述。

### **在 NumPy 中找到最佳拟合线**

在本章的早期部分，您看到了平面中线的例子，包括水平线、斜线和平行线。大多数这些线都有正斜率以及非零的 y 截距值。尽管在平面中存在数据点的散点图，其中最佳拟合线具有负斜率，但本书中的例子涉及的最佳拟合线具有正斜率。

列表 2.22 展示了 `find_best_fit.py` 的内容，该内容说明了如何确定欧几里得平面上一组点的最佳拟合线。该解决方案基于“闭式”公式，这些公式来自统计学。

***列表 2.22：find_best_fit.py***

```py
 import numpy as np

xs = np.array([1,2,3,4,5], dtype=np.float64)
ys = np.array([1,2,3,4,5], dtype=np.float64)

def best_fit_slope(xs,ys):
  m = (((np.mean(xs)*np.mean(ys))-np.mean(xs*ys)) /
       ((np.mean(xs)**2) - np.mean(xs**2)))
  b = np.mean(ys) - m * np.mean(xs)

  return m, b

m,b = best_fit_slope(xs,ys)
print('m:',m,'b:',b) 
```

列表 2.22 从两个 NumPy 数组 xs 和 ys 开始，这些数组初始化为前五个正整数。Python 函数 best_fit_slope()计算一组数字的最佳值 m（斜率）和 b（y 截距）。列表 2.22 的输出如下：

```py
 m: 1.0 b: 0.0 
```

注意到 NumPy 数组 xs 和 ys 是相同的，这意味着这些点位于斜率为 1 的恒等函数上。通过简单的外推，点(0,0)也是同一直线上的点。因此，这条线的 y 截距必须等于 0。

如果您感兴趣，您可以在网上搜索 m 和 b 值的推导过程。在本章中，我们将跳过推导过程，并继续计算均方误差（MSE）的示例。第一个示例涉及手动计算 MSE，接着是一个使用 NumPy 公式进行计算的示例。

### **通过逐次逼近计算 MSE（1）**

本节包含一个代码示例，使用简单技术逐次确定最佳拟合线的斜率和 y 截距的更好近似。回想一下，导数的近似是“delta y”除以“delta x”的比率。基于“delta”值的计算分别计算两个相邻点（x1,y1）和（x2,y2）在函数上的 y 值和 x 值的差。因此，基于“delta”的近似比率是(y2-y1)/(x2-x1)。

本节中的技术涉及对“delta”值的简化近似：我们假设分母等于 1。因此，我们只需要计算“delta”值的分子：在这个代码示例中，这些分子是变量 dw 和 db。

列表 2.23 展示了 `plain_linreg1.py` 的内容，该内容说明了如何使用模拟数据计算 MSE。

***列表 2.23：plain_linreg1.py***

```py
 import numpy as np
import matplotlib.pyplot as plt

X = [0,0.12,0.25,0.27,0.38,0.42,0.44,0.55,0.92,1.0]
Y = [0,0.15,0.54,0.51,0.34,0.1, 0.19,0.53,1.0,0.58]

losses = []
#Step 1: Parameter initialization
W = 0.45 # the initial slope
b = 0.75 # the initial y-intercept

for i in range(1, 100):
  #Step 2: Calculate Loss
  Y_pred = np.multiply(W, X) + b
  loss_error = 0.5 * (Y_pred - Y)**2
  loss = np.sum(loss_error)/10

  #Step 3: Calculate dw and db
  db = np.sum((Y_pred - Y))
  dw = np.dot((Y_pred - Y), X)
  losses.append(loss)

  #Step 4: Update parameters:
  W = W - 0.01*dw
  b = b - 0.01*db

  if i%10 == 0:
    print("Loss at", i,"iteration = ", loss)

#Step 5: Repeat via a for loop with 1000 iterations

#Plot loss versus # of iterations
print("W = ", W,"& b = ",  b)
plt.plot(losses)
plt.ylabel('loss')
plt.xlabel('iterations (per tens)')
plt.show() 
```

代码列表 2.23 定义了变量 X 和 Y，它们是简单的数字数组（这是我们数据集）。接下来，初始化 losses 数组为空数组，我们将向该数组追加连续的损失逼近。变量 W 和 b 分别对应于斜率和 y 截距，它们分别初始化为 0.45 和 0.75（可以自由尝试这些值）。

代码列表 2.23 的下一部分是一个执行 100 次的 for 循环。在每次迭代中，计算变量 Y_pred、loss_error 和 loss，它们分别对应预测值、误差和损失（记住：我们正在进行线性回归）。然后，将损失值（即当前迭代的误差）追加到 losses 数组中。

接下来，计算变量 dw 和 db：这些对应于我们将用于更新 W 和 b 值的“delta w”和“delta b”。以下是代码的复制：

```py
 #Step 4: Update parameters:
W = W - 0.01*dw
b = b - 0.01*db 
```

注意到 dw 和 db 都乘以了值 0.01，这是我们的“学习率”的值（也可以尝试调整这个值）。

以下代码片段显示了每第十次迭代通过循环执行的成本，当循环执行完毕时，显示 W 和 b 的值，并显示一个图表，该图表显示了垂直轴上的成本值和水平轴上的循环迭代次数。以下是 代码列表 2.23 的输出：

```py
 Loss at 10 iteration =  0.04114630674619491
Loss at 20 iteration =  0.026706242729839395
Loss at 30 iteration =  0.024738889446900423
Loss at 40 iteration =  0.023850565034634254
Loss at 50 iteration =  0.0231499048706651
Loss at 60 iteration =  0.02255361434242207
Loss at 70 iteration =  0.0220425055291673
Loss at 80 iteration =  0.021604128492245713
Loss at 90 iteration =  0.021228111750568435
W =  0.47256473531193927 & b =  0.19578262688662174 
```

图 2.11 显示了 代码列表 2.23 的成本与迭代次数的图表。

![图片](img/python-3-data-visualization-using-chatgpt-f0057-01.jpg)

***图 2.11*** 成本与迭代次数的图表

### **通过逐次逼近计算 MSE（2**）

在上一节中，你看到了如何计算“delta”逼近来确定二维平面上点集的最佳拟合线的方程。本节中的示例通过添加表示 epoch 数量的外层循环来泛化上一节中的代码。epoch 数量指定了内层循环执行的次数。

代码列表 2.24 显示了 plain_linreg2.py 的内容，该内容说明了如何使用模拟数据计算 MSE。

***代码列表 2.24: plain_linreg2.py***

```py
 import numpy as np
import matplotlib.pyplot as plt

# %matplotlib inline
X = [0,0.12,0.25,0.27,0.38,0.42,0.44,0.55,0.92,1.0]
Y = [0,0.15,0.54,0.51, 0.34,0.1,0.19,0.53,1.0,0.58]

#uncomment to see a plot of X versus Y values
#plt.plot(X,Y)
#plt.show()

losses = []
#Step 1: Parameter initialization
W = 0.45
b = 0.75 epochs = 100
lr = 0.001
for j in range(1, epochs): for i in range(1, 100):
    #Step 2: Calculate Loss
    Y_pred = np.multiply(W, X) + b
    Loss_error = 0.5 * (Y_pred - Y)**2
    loss = np.sum(Loss_error)/10

    #Step 3: Calculate dW and db
    db = np.sum((Y_pred - Y))
    dw = np.dot((Y_pred - Y), X)
    losses.append(loss)

    #Step 4: Update parameters:
    W = W - lr*dw
    b = b - lr*db

    if i%50 == 0:
      print("Loss at epoch", j,"= ", loss)

#Plot loss versus # of iterations
print("W = ", W,"& b = ",  b) plt.plot(losses)
plt.ylabel('loss')
plt.xlabel('iterations (per tens)')
plt.show() 
```

将 代码列表 2.24 的新内容（以粗体显示）与 代码列表 2.23 的内容进行比较：更改很小，主要区别是对于外层循环的每次迭代执行内层循环 100 次，外层循环也执行 100 次。以下是 代码列表 2.24 的输出：

```py
 ('Loss at epoch', 1, '= ', 0.07161762489862147)
('Loss at epoch', 2, '= ', 0.030073922512586938)
('Loss at epoch', 3, '= ', 0.025415528992988472)
('Loss at epoch', 4, '= ', 0.024227826373677794)
('Loss at epoch', 5, '= ', 0.02346241967071181)
('Loss at epoch', 6, '= ', 0.022827707922883803)
('Loss at epoch', 7, '= ', 0.022284262669854064)
('Loss at epoch', 8, '= ', 0.02181735173716673)
('Loss at epoch', 9, '= ', 0.021416050179776294)
('Loss at epoch', 10, '= ', 0.02107112540934384)
// details omitted for brevity
('Loss at epoch', 90, '= ', 0.018960749188638278)
('Loss at epoch', 91, '= ', 0.01896074755776306)
('Loss at epoch', 92, '= ', 0.018960746155994725)
('Loss at epoch', 93, '= ', 0.018960744951148113)
('Loss at epoch', 94, '= ', 0.018960743915559485)
('Loss at epoch', 95, '= ', 0.018960743025451313)
('Loss at epoch', 96, '= ', 0.018960742260386375)
('Loss at epoch', 97, '= ', 0.018960741602798474)
('Loss at epoch', 98, '= ', 0.018960741037589136)
('Loss at epoch', 99, '= ', 0.018960740551780944)
('W = ', 0.6764145874436108, '& b = ', 0.09976839618922698) 
```

图 2.12 显示了 代码列表 2.24 的损失与迭代次数的图表。

![图片](img/python-3-data-visualization-using-chatgpt-f0059-01.jpg)

***图 2.12*** 损失与迭代次数的图表

注意到 图 2.12 在横轴上有 10,000 次迭代，而 图 2.11 在横轴上只有 100 次迭代。

### **谷歌协作**

根据硬件配置，基于 GPU 的 TF 2 代码通常比基于 CPU 的 TF 2 代码快至少 15 倍。然而，一个好的 GPU 的成本可能是一个重要的因素。尽管 NVIDIA 提供了 GPU，但这些基于消费级的 GPU 并未针对多 GPU 支持进行优化（而 TF 2 是支持多 GPU 支持的）。

幸运的是，Google Colaboratory 是一个经济实惠的替代方案，它提供了免费的 GPU 支持，并且作为一个 Jupyter 笔记本环境运行。此外，Google Colaboratory 在云端执行您的代码，无需任何配置，并且可在 *[`colab.research.google.com/notebooks/welcome.ipynb`](https://colab.research.google.com/notebooks/welcome.ipynb)* 上使用。

Jupyter 笔记本适合快速训练简单模型和测试想法。Google Colaboratory 使您轻松上传本地文件，在 Jupyter 笔记本中安装软件，甚至可以将 Google Colaboratory 连接到您本地机器上的 Jupyter 运行时。

Colaboratory 支持的一些功能包括使用 GPU 执行 TF 2、使用 Matplotlib 进行可视化，以及通过使用“文件”>“保存副本到 GitHub”将您的 Google Colaboratory 笔记本保存到 Github 的副本。

此外，您只需在 URL 中添加路径，就可以通过 GitHub 加载任何 .ipynb 文件：*[colab.research.google.com/github/](http://colab.research.google.com/github/)*（有关详细信息，请参阅 Colaboratory 网站）。

Google Colaboratory 支持其他技术，如 HTML 和 SVG，使您能够在 Google Colaboratory 中的笔记本中渲染基于 SVG 的图形。请记住，您在 Google Colaboratory 笔记本中安装的任何软件都仅在会话基础上可用：如果您注销并重新登录，您需要执行与您在早期 Google Colaboratory 会话中执行的相同安装步骤。

Google Colaboratory 另有一个非常不错的功能：您可以免费在 GPU 上执行代码，每天最多可达十二小时。对于没有适合本地机器的 GPU 的用户（这可能是大多数用户）来说，这种免费的 GPU 支持非常有用。现在，他们可以在不到 20 或 30 分钟的时间内启动 TF 2 代码来训练神经网络，否则这个过程可能需要多个小时的 CPU 执行时间。

您可以使用以下命令在 Google Colaboratory 笔记本中启动 Tensorboard（将指定的目录替换为您自己的位置）：

```py
 %tensorboard --logdir /logs/images 
```

请记住有关 Google Colaboratory 的以下详细信息。首先，每次您连接到 Google Colaboratory 中的服务器时，您都会启动一个 *会话*。您可以在会话中使用 CPU（默认）、GPU 或 TPU（TPU 可免费使用）执行代码，并且您可以在会话中无时间限制地执行您的代码。然而，如果您为您的会话选择 GPU 选项，*只有前 12 小时的 GPU 执行时间是免费的*。在相同会话期间，任何额外的 GPU 时间都会产生小额费用（有关详细信息，请参阅网站）。

另一点需要记住的是，在给定会话期间在 Jupyter 笔记本中安装的任何软件都不会在退出该会话时保存。例如，以下代码片段在 Jupyter 笔记本中安装 TFLearn：

```py
 !pip install tflearn 
```

当你退出当前会话并在以后启动新会话时，你需要重新安装 TFLearn，以及你在任何之前的会话中安装的任何其他软件（例如 Github 仓库）。

顺便说一下，你还可以在 Google Colaboratory 中运行 TF 2 代码和 TensorBoard。要获取更多信息，请访问此 URL：

*[`www.tensorflow.org/tensorboard/r2/tensorboard_in_notebooks`](https://www.tensorflow.org/tensorboard/r2/tensorboard_in_notebooks)*

#### **在 Google Colaboratory 中上传 CSV 文件**

列表 2.25 显示了 upload_csv_file.ipynb 的内容，说明了如何在 Google Colaboratory 笔记本中上传 CSV 文件。

***列表 2.25：upload_csv_file.ipynb***

```py
 import pandas as pd from google.colab import files
uploaded = files.upload() df = pd.read_csv("weather_data.csv")
print("dataframe df:")
df 
```

列表 2.25 上传了 CSV 文件 weather_data.csv，其内容未显示，因为它们对于本例不重要。粗体显示的代码是 Colaboratory 特定的代码，用于上传 CSV 文件。当你运行此代码时，你会看到一个标有“浏览”的小按钮，你必须点击并选择代码片段中列出的 CSV 文件。完成此操作后，其余的代码将被执行，你将在浏览器会话中看到 CSV 文件的内容。

**注意** *如果你想在 Google Colaboratory 中成功启动此 Jupyter 笔记本，你必须提供 CSV 文件* weather_data.csv *。*

### **总结**

本章介绍了 Python 的 NumPy 库。你学习了如何编写包含循环、数组和列表的 Python 脚本。你还看到了如何处理点积、reshape() 方法、使用 Matplotlib 绘图（在第六章中更详细地讨论），以及线性回归的示例。

然后你学习了如何处理数组的子范围，以及向量和数组的负子范围，这两者对于在机器学习任务中提取数据集的部分都非常有用。你还看到了各种其他 NumPy 操作，例如 reshape() 方法，这在处理图像文件时非常有用。

接下来，你学习了如何使用 NumPy 进行线性回归、均方误差（MSE），以及如何使用 NumPy linspace() 方法计算 MSE。最后，你介绍了 Google Colaboratory，在那里你可以在启动 Jupyter 笔记本时利用免费的 GPU 时间。

## **第三章**

## *PANDAS 和 数据可视化*

本章介绍了 Pandas 库，并包含各种代码示例，展示了 Pandas 的一些有用功能。正如你将看到的，每个部分的标题清楚地表明了其内容，因此你可以轻松地扫描本章以查找包含新材料的部分。这种方法将帮助你高效地利用阅读本章内容的时间。

本章的第一部分简要介绍了 Pandas，随后是代码示例，说明了如何定义 Pandas DataFrame 并显示其属性。请注意，本章专注于 Pandas DataFrame。有一个代码块说明了如何定义 Pandas Series，如果你想了解更多关于 Pandas Series 的信息，可以在网上搜索更多信息。

本章的第二部分讨论了你可以创建的各种 DataFrame 类型，例如数值和布尔 DataFrame。此外，你还将看到使用 NumPy 函数和随机数创建 DataFrame 的示例。你还将看到将 Python 字典和基于 JSON 的数据之间进行转换的示例，以及如何从基于 JSON 的数据创建 Pandas DataFrame。

### **什么是 PANDAS？**

Pandas 是一个与 Python 库兼容的 Python 库，例如 NumPy、Matplotlib 等。通过打开命令行并调用以下命令安装 Pandas（适用于 Python 3.x）：

```py
 pip3 install pandas 
```

在许多方面，Pandas 库具有电子表格的语义，并且它还与各种文件类型一起工作，例如 xsl、xml、html、csv 文件。Pandas 提供了一种称为 DataFrame 的数据类型（类似于 Python 字典），具有非常强大的功能（类似于电子表格的功能）。

#### **Pandas DataFrame**

简而言之，Pandas DataFrame 是一个二维数据结构，方便将其视为行和列。DataFrame 可以标记（包括行和列），列可以包含不同的数据类型。数据集的来源可以是数据文件、数据库表、Web 服务等。Pandas DataFrame 的功能包括：

+   数据框方法

+   数据框统计信息

+   分组、交叉和重塑

+   处理缺失数据

+   连接数据框

#### **DataFrame 和数据清洗任务**

你需要执行的具体任务取决于数据集的结构和内容。通常，你将按照以下步骤（不一定总是按此顺序）执行工作流程，所有这些都可以使用 Pandas DataFrame 完成：

+   将数据读入 DataFrame

+   显示 DataFrame 的顶部

+   显示列数据类型

+   显示非缺失值

+   用值替换 NA

+   遍历列

+   每列的统计信息

+   查找缺失值

+   总缺失值

+   缺失值的百分比

+   排序表值

+   打印摘要信息

+   列中缺失值超过 50%

+   重命名列

### **PANDAS DataFrame 示例**

列表 3.1 展示了 pandas_df.py 的内容，该文件说明了如何定义几个 Pandas DataFrame 并显示其内容。

***列表 3.1：pandas_df.py***

```py
 import pandas as pd
import numpy as np myvector1 = np.array([1,2,3,4,5])
print("myvector1:")
print(myvector1)
print()

mydf1 = pd.DataFrame(myvector1)
print("mydf1:")
print(mydf1)
print()

myvector2 = np.array([i for i in range(1,6)])
print("myvector2:")
print(myvector2)
print()

mydf2 = pd.DataFrame(myvector2)
print("mydf2:")
print(mydf2)
print()

myarray = np.array([[10,30,20], [50,40,60],[1000,2000,3000]])
print("myarray:")
print(myarray)
print()

mydf3 = pd.DataFrame(myarray)
print("mydf3:")
print(mydf3)
print() 
```

列表 3.1 以 Pandas 和 NumPy 的标准导入语句开始，随后是定义两个一维 NumPy 数组和二维 NumPy 数组。NumPy 语法应该对您很熟悉（许多基本教程都可在网上找到）。每个 NumPy 变量后面都跟着相应的 Pandas DataFrame mydf1、mydf2 和 mydf3。现在运行 列表 3.1 中的代码，您将看到以下输出，并且您可以比较 NumPy 数组与 Pandas DataFrame：

```py
 myvector1:
[1 2 3 4 5]

mydf1:
   0
0  1
1  2
2  3
3  4
4  5

myvector2:
[1 2 3 4 5] mydf2:
   0
0  1
1  2
2  3
3  4
4  5
myarray:
[[10   30   20]
 [50   40   60]
 [1000 2000 3000]]

mydf3:
      0     1     2
0    10    30    20
1    50    40    60
2  1000  2000  3000 
```

此外，以下代码块说明了如何从两个 Pandas Pandas Series 构建一个 Pandas DataFrame：

```py
 names = pd.Series(['SF', 'San Jose', 'Sacramento'])
sizes = pd.Series([852469, 1015785, 485199])
df = pd.DataFrame({'Cities': names, 'Size': sizes})
print(df) 
```

创建一个包含上述代码（以及所需的导入语句）的 Python 文件，当您运行该代码时，您将看到以下输出：

```py
 City name    sizes
0          SF   852469
1    San Jose  1015785
2  Sacramento   485199 
```

### **描述 Pandas DataFrame**

列表 3.2 显示了 pandas_df_describe.py 的内容，该内容说明了如何定义包含 3x3 整数 NumPy 数组的 Pandas DataFrame，其中 DataFrame 的行和列有标签。DataFrame 的其他方面也进行了显示。

***列表 3.2: pandas_df_describe.py***

```py
 import numpy as np
import pandas as pd

myarray = np.array([[10,30,20], [50,40,60],[1000,2000,3000]])

rownames = ['apples', 'oranges', 'beer']
colnames = ['January', 'February', 'March'] mydf = pd.DataFrame(myarray, index=rownames, columns=colnames)
print("contents of df:")
print(mydf)
print()

print("contents of January:")
print(mydf['January'])
print()

print("Number of Rows:")
print(mydf.shape[0])
print()

print("Number of Columns:")
print(mydf.shape[1])
print()

print("Number of Rows and Columns:")
print(mydf.shape)
print()

print("Column Names:")
print(mydf.columns)
print()

print("Column types:")
print(mydf.dtypes)
print()

print("Description:")
print(mydf.describe())
print() 
```

列表 3.2 以两个标准的导入语句开始，随后是变量 myarray，它是一个 3x3 的 NumPy 数组。变量 rownames 和 colnames 分别为 Pandas DataFrame mydf 的行和列提供名称，mydf 是初始化为 Pandas DataFrame 的指定数据源（即 myarray）。

下面的输出部分需要单个 print 语句（它仅显示 mydf 的内容）。输出部分的第二部分是通过调用任何 NumPy DataFrame 可用的 describe() 方法生成的。describe() 方法非常有用：您将看到各种统计量，如均值、标准差、最小值和最大值，按列（而不是按行）执行，以及 25%、50% 和 75% 分位数。列表 3.2 的输出如下：

```py
 contents of df:
         January  February  March
apples        10        30     20
oranges       50        40     60
beer        1000      2000   3000 contents of January:
apples       10
oranges      50
beer       1000
Name: January, dtype: int64

Number of Rows:
3

Number of Columns:
3

Number of Rows and Columns:
(3, 3)

Column Names:
Index(['January', 'February', 'March'], dtype='object')

Column types:
January     int64
February    int64
March       int64
dtype: object

Description:
           January     February        March
count     3.000000     3.000000     3.000000
mean    353.333333   690.000000  1026.666667
std     560.386771  1134.504297  1709.073823
min      10.000000    30.000000    20.000000
25%      30.000000    35.000000    40.000000
50%      50.000000    40.000000    60.000000
75%     525.000000  1020.000000  1530.000000
max    1000.000000  2000.000000  3000.000000 
```

### **Pandas 布尔 DataFrame**

Pandas 支持在 DataFrame 上执行布尔运算，如逻辑或、逻辑与以及一对 DataFrame 的逻辑否定。列表 3.3 显示了 pandas_boolean_df.py 的内容，该内容说明了如何定义其行和列为布尔值的 Pandas DataFrame。

***列表 3.3: pandas_boolean_df.py***

```py
 import pandas as pd

df1 = pd.DataFrame({'a': [1, 0, 1], 'b': [0, 1, 1] }, dtype=bool)
df2 = pd.DataFrame({'a': [0, 1, 1], 'b': [1, 1, 0] }, dtype=bool)

print("df1 & df2:")
print(df1 & df2) print("df1 | df2:")
print(df1 | df2)

print("df1 ^ df2:")
print(df1 ^ df2) 
```

列表 3.3 初始化了 DataFrame df1 和 df2，然后计算 df1 & df2、df1 | df2、df1 ^ df2，分别代表 df1 和 df2 的逻辑与、逻辑或和逻辑否定。运行 列表 3.3 中的代码的输出如下：

```py
 df1 & df2:
       a      b
0  False  False
1  False   True
2   True  False
df1 | df2:
      a     b
0  True  True
1  True  True
2  True  True
df1 ^ df2:
       a      b
0   True   True
1   True  False
2  False   True 
```

#### **转换 Pandas DataFrame**

T 属性（以及转置函数）允许您生成 Pandas DataFrame 的转置，类似于 NumPy ndarray。

例如，以下代码片段定义了一个 Pandas DataFrame df1，然后显示了 df1 的转置：

```py
 df1 = pd.DataFrame({'a': [1, 0, 1], 'b': [0, 1, 1]}, dtype=int)

print("df1.T:")
print(df1.T) 
```

输出如下：

```py
 df1.T:
   0  1  2
a  1  0  1
b  0  1  1 
```

以下代码片段定义了 Pandas DataFrame df1 和 df2，然后显示它们的和：

```py
 df1 = pd.DataFrame({'a' : [1, 0, 1], 'b' : [0, 1, 1]}, dtype=int) df2 = pd.DataFrame({'a' : [3, 3, 3], 'b' : [5, 5, 5]}, dtype=int)

print("df1 + df2:")
print(df1 + df2) 
```

输出如下：

```py
 df1 + df2:
   a  b
0  4  5
1  3  6
2  4  6 
```

### **PANDAS 数据框和随机数字**

列表 3.4 展示了 pandas_random_df.py 的内容，该内容说明了如何创建一个包含随机数字的 Pandas DataFrame。

***列表 3.4: pandas_random_df.py***

```py
 import pandas as pd
import numpy as np

df = pd.DataFrame(np.random.randint(1, 5, size=(5, 2)), columns=['a','b'])
df = df.append(df.agg(['sum', 'mean']))

print("Contents of data frame:")
print(df) 
```

列表 3.4 定义了 Pandas DataFrame df，该 DataFrame 由 5 行和 2 列的介于 1 和 5 之间的随机整数组成。请注意，df 的列标记为“a”和“b”。此外，下一个代码片段附加了包含两行内容的两行，这两行是两列中数字的总和和平均值。列表 3.4 的输出如下：

```py
 a      b
0      1.0  2.0
1      1.0  1.0
2      4.0  3.0
3      3.0  1.0
4      1.0  2.0
sum   10.0  9.0
mean   2.0  1.8 
```

列表 3.5 展示了 pandas_combine_df.py 的内容，该内容说明了如何定义一个基于两个数字 NumPy 数组的 Pandas DataFrame。

***列表 3.5: pandas_combine_df.py***

```py
 import pandas as pd
import numpy as np df = pd.DataFrame({'foo1' : np.random.randn(5),
                   'foo2' : np.random.randn(5)})

print("contents of df:")
print(df)

print("contents of foo1:")
print(df.foo1)

print("contents of foo2:")
print(df.foo2) 
```

列表 3.5 定义了 Pandas DataFrame df，该 DataFrame 由 5 行和 2 列（标记为“foo1”和“foo2”）组成，包含介于 0 和 5 之间的随机实数。列表 3.5 的下一部分显示了 df 和 foo1 的内容。列表 3.5 的输出如下：

```py
 contents of df:
       foo1      foo2
0  0.274680 -0.848669
1 -0.399771 -0.814679
2  0.454443 -0.363392
3  0.473753  0.550849
4 -0.211783 -0.015014
contents of foo1:
0    0.256773
1    1.204322
2    1.040515
3   -0.518414
4    0.634141
Name: foo1, dtype: float64
contents of foo2:
0   -2.506550
1   -0.896516
2   -0.222923
3    0.934574
4    0.527033
Name: foo2, dtype: float64 
```

### **将分类数据转换为数值数据**

机器学习中的一项常见任务是将包含字符数据的特征转换为包含数值数据的特征。

列表 3.6 展示了包含标记数据（垃圾邮件或非垃圾邮件）的 sometext.tsv 的内容，这些数据用于 列表 3.7 中显示的代码示例（在 列表 3.6 之后显示）。

***列表 3.6: sometext.tsv***

```py
 type    text
ham     I'm telling the truth
spam    What a deal such a deal! spam    Free vacation for your family
ham     Thank you for your help
spam    Spring break next week! ham     I received the documents
spam    One million dollars for you
ham     My wife got covid19
spam    You might have won the prize
ham     Everyone is in good health 
```

列表 3.7 展示了 cat2numeric.py 的内容，说明了如何将文本字段替换为相应的数值字段。

***列表 3.7: cat2numeric.py***

```py
 import pandas as pd
import numpy as np

df = pd.read_csv('sometext.tsv', delimiter='\t')

print("=> First five rows (before):")
print(df.head(5))
print("-------------------------")

# map ham/spam to 0/1 values:
df['type'] = df['type'].map( {'ham':0 , 'spam':1} )

print("=> First five rows (after):")
print(df.head(5))
print("-------------------------") 
```

列表 3.7 使用 sometext.tsv 文件的内容初始化 DataFrame df，然后通过调用 df.head(5) 显示前五行内容，这也是默认显示的行数。在 列表 3.7 中的下一个代码片段调用 map() 方法，将列标签为 type 中的 ham 替换为 0，将 spam 替换为 1，如下所示：

```py
 df['type'] = df['type'].map( {'ham':0 , 'spam':1} ) 
```

列表 3.7 的最后一部分再次调用 head() 方法，在重命名列 type 的内容后显示数据集的前五行。运行 列表 3.7 中的代码，你将看到以下输出：

```py
 => First five rows (before):
   type                          text 0   ham      Available only for today
1   ham           I'm joking with you
2  spam   Free entry in 2 a wkly comp
3   ham        U dun say so early hor
4   ham  I don't think he goes to usf
-------------------------
=> First five rows (after):
   type                          text
0     0      Available only for today
1     0           I'm joking with you
2     1   Free entry in 2 a wkly comp
3     0        U dun say so early hor
4     0  I don't think he goes to usf
------------------------- 
```

作为另一个例子，列表 3.8 展示了 shirts.csv 的内容，列表 3.9 展示了 shirts.py 的内容，该内容说明了将分类数据转换为数值数据的四种技术。

***列表 3.8: shirts.csv***

```py
 type,ssize
shirt,xxlarge
shirt,xxlarge
shirt,xlarge
shirt,xlarge
shirt,xlarge
shirt,large
shirt,medium
shirt,small
shirt,small
shirt,xsmall
shirt,xsmall
shirt,xsmall 
```

***列表 3.9: shirts.py***

```py
 import pandas as pd

shirts = pd.read_csv("shirts.csv")
print("shirts before:")
print(shirts)
print() # TECHNIQUE #1: #shirts.loc[shirts['ssize']=='xxlarge','size'] = 4
#shirts.loc[shirts['ssize']=='xlarge', 'size'] = 4
#shirts.loc[shirts['ssize']=='large',  'size'] = 3
#shirts.loc[shirts['ssize']=='medium', 'size'] = 2
#shirts.loc[shirts['ssize']=='small',  'size'] = 1
#shirts.loc[shirts['ssize']=='xsmall', 'size'] = 1 # TECHNIQUE #2: #shirts['ssize'].replace('xxlarge', 4, inplace=True)
#shirts['ssize'].replace('xlarge',  4, inplace=True)
#shirts['ssize'].replace('large',   3, inplace=True)
#shirts['ssize'].replace('medium',  2, inplace=True)
#shirts['ssize'].replace('small',   1, inplace=True)
#shirts['ssize'].replace('xsmall',  1, inplace=True) # TECHNIQUE #3: #shirts['ssize'] = shirts['ssize'].apply({'xxlarge':4, 'xlarge':4, 'large':3, 'medium':2, 'small':1, 'xsmall':1}.get) # TECHNIQUE #4: shirts['ssize'] = shirts['ssize'].replace(regex='xlarge', value=4)
shirts['ssize'] = shirts['ssize'].replace(regex='large',  value=3)
shirts['ssize'] = shirts['ssize'].replace(regex='medium', value=2)
shirts['ssize'] = shirts['ssize'].replace(regex='small',  value=1)

print("shirts after:")
print(shirts) 
```

列表 3.9 以六个语句的代码块开始，使用字符串的直接比较来进行数值替换。例如，以下代码片段将所有 xxlarge 字符串的实例替换为值 4：

```py
 shirts.loc[shirts['ssize']=='xxlarge','size'] = 4 
```

第二个代码块由六个语句组成，使用 replace() 方法执行相同的更新，例如以下示例所示：

```py
 shirts['ssize'].replace('xxlarge', 4, inplace=True) 
```

第三个代码块由一个语句组成，使用 apply() 方法执行相同的更新，如下所示：

```py
 shirts['ssize'] = shirts['ssize'].apply({'xxlarge':4, 'xlarge':4, 'large':3, 'medium':2, 'small':1, 'xsmall':1}.get) 
```

第四个代码块由四个语句组成，使用正则表达式执行相同的更新，例如以下示例所示：

```py
 shirts['ssize'] = shirts['ssize'].replace(regex='xlarge', value=4) 
```

由于前面的代码片段也匹配了 xxlarge 和 xlarge，所以我们只需要四个语句而不是六个语句。如果你不熟悉正则表达式，你可以找到在线文章来介绍你正则表达式。现在运行 列表 3.9 中的代码，你将看到以下输出：

```py
 shirts before
     type     size
0   shirt  xxlarge
1   shirt  xxlarge
2   shirt   xlarge
3   shirt   xlarge
4   shirt   xlarge
5   shirt    large
6   shirt   medium
7   shirt    small 8   shirt    small
9   shirt   xsmall
10  shirt   xsmall
11  shirt   xsmall

shirts after:
     type  size
0   shirt     4
1   shirt     4
2   shirt     4
3   shirt     4
4   shirt     4
5   shirt     3
6   shirt     2
7   shirt     1
8   shirt     1
9   shirt     1
10  shirt     1
11  shirt     1 
```

### **在 Pandas 中匹配和拆分字符串**

列表 3.10 展示了 shirts_str.py 的内容，该内容说明了如何将列值与初始字符串匹配，以及如何根据字母拆分列值。

***列表 3.10: shirts_str.py***

```py
 import pandas as pd

shirts = pd.read_csv("shirts.csv")
print("shirts:")
print(shirts)
print()

print("shirts starting with xl:")
print(shirts[shirts.ssize.str.startswith('xl')])
print()

print("Exclude 'xlarge' shirts:")
print(shirts[shirts['ssize'] != 'xlarge'])
print()

print("first three letters:")
shirts['sub1'] = shirts['ssize'].str[:3]
print(shirts)
print()

print("split ssize on letter 'a':")
shirts['sub2'] = shirts['ssize'].str.split('a')
print(shirts)
print() print("Rows 3 through 5 and column 2:")
print(shirts.iloc[2:5, 2])
print() 
```

列表 3.10 使用 shirts.csv 文件的内容初始化 DataFrame df，然后显示 DataFrame 的内容。在 列表 3.10 的下一个代码片段中，使用 startswith() 方法匹配以字母 xl 开头的衬衫类型，然后是一个显示尺寸不等于字符串 xlarge 的短裤的代码片段。

下一个代码片段使用 str[:3] 构造来显示衬衫类型的第一个三个字母，然后是一个使用 split() 方法根据字母“a”拆分衬衫类型的代码片段。最后的代码片段调用 iloc[2:5,2] 来显示第 3 行到第 5 行（包括第 5 行）的内容，以及只有第二列。列表 3.10 的输出如下：

```py
 shirts:
     type    ssize
0   shirt  xxlarge
1   shirt  xxlarge
2   shirt   xlarge
3   shirt   xlarge
4   shirt   xlarge
5   shirt    large
6   shirt   medium
7   shirt    small
8   shirt    small
9   shirt   xsmall
10  shirt   xsmall
11  shirt   xsmall

shirts starting with xl:
    type   ssize
2  shirt  xlarge
3  shirt  xlarge
4  shirt  xlarge

Exclude 'xlarge' shirts:
     type    ssize
0   shirt  xxlarge
1   shirt  xxlarge
5   shirt    large
6   shirt   medium
7   shirt    small
8   shirt    small
9   shirt   xsmall
10  shirt   xsmall
11  shirt   xsmall

first three letters:
     type    ssize sub1
0   shirt  xxlarge  xxl
1   shirt  xxlarge  xxl 2   shirt   xlarge  xla
3   shirt   xlarge  xla
4   shirt   xlarge  xla
5   shirt    large  lar
6   shirt   medium  med
7   shirt    small  sma
8   shirt    small  sma
9   shirt   xsmall  xsm
10  shirt   xsmall  xsm
11  shirt   xsmall  xsm

split ssize on letter 'a':
     type    ssize sub1        sub2
0   shirt  xxlarge  xxl  [xxl, rge]
1   shirt  xxlarge  xxl  [xxl, rge]
2   shirt   xlarge  xla   [xl, rge]
3   shirt   xlarge  xla   [xl, rge]
4   shirt   xlarge  xla   [xl, rge]
5   shirt    large  lar    [l, rge]
6   shirt   medium  med    [medium]
7   shirt    small  sma    [sm, ll]
8   shirt    small  sma    [sm, ll]
9   shirt   xsmall  xsm   [xsm, ll]
10  shirt   xsmall  xsm   [xsm, ll]
11  shirt   xsmall  xsm   [xsm, ll]

Rows 3 through 5 and column 2:
2    xlarge
3    xlarge
4    xlarge
Name: ssize, dtype: object 
```

### **在 Pandas 中合并和拆分列**

列表 3.11 显示了 employees.csv 的内容，列表 3.12 显示了 emp_merge_split.py 的内容，该内容说明了如何合并 CSV 文件的列和拆分列。

***列表 3.11: employees.csv***

```py
 name,year,month
Jane-Smith,2015,Aug
Dave-Smith,2020,Jan
Jane-Jones,2018,Dec
Jane-Stone,2017,Feb
Dave-Stone,2014,Apr
Mark-Aster,,Oct
Jane-Jones,NaN,Jun 
```

***列表 3.12: emp_merge_split.py***

```py
 import pandas as pd

emps = pd.read_csv("employees.csv")
print("emps:") print(emps)
print()

emps['year']  = emps['year'].astype(str)
emps['month'] = emps['month'].astype(str)

# separate column for first name and for last name:
emps['fname'],emps['lname'] = emps['name'].str.split("-",1).str

# concatenate year and month with a "#" symbol:
emps['hdate1'] = emps['year'].astype(str)+"#"+emps['month'].astype(str)

# concatenate year and month with a "-" symbol:
emps['hdate2'] = emps[['year','month']].agg('-'.join, axis=1)

print(emps)
print() 
```

列表 3.12 使用 employees.csv 文件的内容初始化 DataFrame df，然后显示 DataFrame 的内容。在 列表 3.12 的下一个代码片段中，使用 astype() 方法将年份和月份列的内容转换为字符串。

在 列表 3.12 的下一个代码片段中，使用 split() 方法将姓名列拆分为包含每个员工姓名的姓氏和名字的列 fname 和 lname：

```py
 emps['fname'],emps['lname'] = emps['name'].str.split("-",1).str 
```

下一个代码片段将年份和月份字符串的内容与一个“#”字符连接起来，以创建一个新的列 hdate1，如下所示：

```py
 emps['hdate1'] = emps['year'].astype(str)+"#"+emps['month'].astype(str) 
```

以下代码片段将年份和月份字符串的内容连接起来，用“-”创建一个新的列，称为 hdate2，如下所示：

```py
 emps['hdate2'] = emps[['year','month']].agg('-'.join, axis=1) 
```

现在运行 列表 3.12 中的代码，你会看到以下输出：

```py
 emps:
         name    year month
0  Jane-Smith  2015.0   Aug
1  Dave-Smith  2020.0   Jan
2  Jane-Jones  2018.0   Dec
3  Jane-Stone  2017.0   Feb 4  Dave-Stone  2014.0   Apr
5  Mark-Aster     NaN   Oct
6  Jane-Jones     NaN   Jun

         name    year month fname  lname      hdate1      hdate2
0  Jane-Smith  2015.0   Aug  Jane  Smith  2015.0#Aug  2015.0-Aug
1  Dave-Smith  2020.0   Jan  Dave  Smith  2020.0#Jan  2020.0-Jan
2  Jane-Jones  2018.0   Dec  Jane  Jones  2018.0#Dec  2018.0-Dec
3  Jane-Stone  2017.0   Feb  Jane  Stone  2017.0#Feb  2017.0-Feb
4  Dave-Stone  2014.0   Apr  Dave  Stone  2014.0#Apr  2014.0-Apr
5  Mark-Aster     nan   Oct  Mark  Aster     nan#Oct     nan-Oct
6  Jane-Jones     nan   Jun  Jane  Jones     nan#Jun     nan-Jun 
```

关于以下代码片段的一个其他细节：

```py
 emps['fname'],emps['lname'] = emps['name'].str. split("-",1).str 
```

显示以下弃用信息：

```py
 #FutureWarning: Columnar iteration over characters
#will be deprecated in future releases. 
```

### **合并 Pandas DataFrames**

Pandas 支持在 DataFrames 中使用“concat”方法来连接 DataFrames。列表 3.13 展示了 concat_frames.py 的内容，该文件说明了如何合并两个 Pandas DataFrames。

***列表 3.13: concat_frames.py***

```py
 import pandas as pd

can_weather = pd.DataFrame({
    "city": ["Vancouver","Toronto","Montreal"],
    "temperature": [72,65,50],
    "humidity": [40, 20, 25]
})

us_weather = pd.DataFrame({
    "city": ["SF","Chicago","LA"],
    "temperature": [60,40,85],
    "humidity": [30, 15, 55]
})

df = pd.concat([can_weather, us_weather])
print(df) 
```

列表 3.13 中的第一行是一个导入语句，随后是 Pandas DataFrames can_weather 和 us_weather 的定义，它们分别包含加拿大和美国城市的天气相关信息。Pandas DataFrame df 是 can_weather 和 us_weather 的连接。列表 3.13 的输出如下：

```py
 0  Vancouver        40           72
1    Toronto        20           65
2   Montreal        25           50
0         SF        30           60
1    Chicago        15           40
2         LA        55           85 
```

### **使用 Pandas DataFrames 进行数据操作**

作为简单的例子，假设我们有一家两人公司，按季度记录收入和支出，并希望计算每个季度的利润/亏损，以及总的利润/亏损。

列表 3.14 展示了 pandas_quarterly_df1.py 的内容，该文件说明了如何定义一个包含与收入相关值的 Pandas DataFrame。

***列表 3.14: pandas_quarterly_df1.py***

```py
 import pandas as pd

summary = {
    'Quarter': ['Q1', 'Q2', 'Q3', 'Q4'],
    'Cost':    [23500, 34000, 57000, 32000],
    'Revenue': [40000, 40000, 40000, 40000]
}

df = pd.DataFrame(summary)

print("Entire Dataset:\n",df)
print("Quarter:\n",df.Quarter)
print("Cost:\n",df.Cost)
print("Revenue:\n",df.Revenue) 
```

列表 3.14 定义了变量 summary，它包含我们两人公司关于成本和收入的硬编码季度信息。通常，这些硬编码的值会被来自另一个来源（如 CSV 文件）的数据所替换，所以将此代码示例视为一种简单的方式来展示 Pandas DataFrames 中的一些可用功能。

变量 df 是基于 summary 变量中的数据的 Pandas DataFrame。三个 print() 语句显示了季度、每个季度的成本和每个季度的收入。列表 3.14 的输出如下：

```py
 Entire Dataset:
     Cost Quarter  Revenue
0  23500      Q1    40000
1  34000      Q2    60000 2  57000      Q3    50000
3  32000      Q4    30000
Quarter:
0    Q1
1    Q2
2    Q3
3    Q4
Name: Quarter, dtype: object
Cost:
0    23500
1    34000
2    57000
3    32000
Name: Cost, dtype: int64
Revenue:
0    40000
1    60000
2    50000
3    30000
Name: Revenue, dtype: int64 
```

### **使用 Pandas DataFrames 进行数据操作（2）**

在本节中，假设我们有一家两人公司，按季度记录收入和支出，并希望计算每个季度的利润/亏损，以及总的利润/亏损。

列表 3.15 展示了 pandas_quarterly_df1.py 的内容，该文件说明了如何定义一个包含与收入相关值的 Pandas DataFrame。

***列表 3.15: pandas_quarterly_df2.py***

```py
 import pandas as pd

summary = {
    'Quarter': ['Q1', 'Q2', 'Q3', 'Q4'],
    'Cost':    [-23500, -34000, -57000, -32000],
    'Revenue': [40000, 40000, 40000, 40000]
}
df = pd.DataFrame(summary)
print("First Dataset:\n",df)

df['Total'] = df.sum(axis=1)
print("Second Dataset:\n",df) 
```

列表 3.15 定义了变量 summary，它包含我们两人公司关于成本和收入的季度信息。变量 df 是基于 summary 变量中的数据的 Pandas DataFrame。三个 print() 语句显示了季度、每个季度的成本和每个季度的收入。列表 3.15 的输出如下：

```py
First Dataset:
     Cost Quarter  Revenue
0 -23500      Q1    40000
1 -34000      Q2    60000
2 -57000      Q3    50000
3 -32000      Q4    30000
Second Dataset:
     Cost Quarter  Revenue  Total
0 -23500      Q1    40000  16500
1 -34000      Q2    60000  26000
2 -57000      Q3    50000  -7000
3 -32000      Q4    30000  -2000 
```

### **使用 Pandas DataFrames 进行数据操作（3）**

让我们从与上一节相同的假设开始：我们有一个两人公司，按季度记录收入和支出，我们想要计算每个季度的利润/亏损，以及总的利润/亏损。此外，我们还想计算列总计和行总计。

列表 3.16 显示了 pandas_quarterly_df1.py 的内容，该内容说明了如何定义一个包含收入相关值的 Pandas 数据框。

***列表 3.16：pandas_quarterly_df3.py***

```py
 import pandas as pd

summary = {
    'Quarter': ['Q1', 'Q2', 'Q3', 'Q4'],
    'Cost':    [_23500, _34000, _57000, _32000],
    'Revenue': [40000, 40000, 40000, 40000]
}

df = pd.DataFrame(summary)
print("First Dataset:\n",df)

df['Total'] = df.sum(axis=1)
df.loc['Sum'] = df.sum()
print("Second Dataset:\n",df)

# or df.loc['avg'] / 3
#df.loc['avg'] = df[:3].mean()
#print("Third Dataset:\n",df) 
```

列表 3.16 定义了变量 summary，它包含我们两人公司关于成本和收入的季度信息。变量 df 是基于 summary 变量中的数据构建的 Pandas 数据框。三个打印语句显示了季度、每个季度的成本和每个季度的收入。列表 3.16 的输出如下：

```py
First Dataset:
     Cost Quarter  Revenue
0 -23500      Q1    40000
1 -34000      Q2    60000
2 -57000      Q3    50000
3 -32000      Q4    30000
Second Dataset:
        Cost   Quarter  Revenue  Total
0    -23500        Q1    40000  16500
1    -34000        Q2    60000  26000
2    -57000        Q3    50000  -7000
3    -32000        Q4    30000  -2000
Sum -146500  Q1Q2Q3Q4   180000  33500 
```

### **PANDAS 数据框和 CSV 文件**

几个早期部分的代码示例中包含在 Python 脚本中的硬编码数据。然而，从 CSV 文件中读取数据也是非常常见的。你可以使用 Python 的 csv.reader() 函数、NumPy 的 loadtxt() 函数或 Pandas 的 read_csv() 函数（在本节中展示）来读取 CSV 文件的内容。

列表 3.17 显示了 CSV 文件 weather_data.csv 的内容，列表 3.18 显示了 weather_data.py 的内容，该内容说明了如何读取 CSV 文件 weather_data.csv。

***列表 3.17：weather_data.csv***

```py
 day,temperature,windspeed,event
7/1/2018,42,16,Rain
7/2/2018,45,3,Sunny
7/3/2018,78,12,Snow
7/4/2018,74,9,Snow
7/5/2018,42,24,Rain
7/6/2018,51,32,Sunny 
```

***列表 3.18：weather_data.py***

```py
 import pandas as pd

df = pd.read_csv("weather_data.csv")

print(df)
print(df.shape)  # rows, columns
print(df.head()) # df.head(3)
print(df.tail())
print(df[1:3])
print(df.columns)
print(type(df['day']))
print(df[['day','temperature']])
print(df['temperature'].max()) 
```

列表 3.18 调用 Pandas read_csv() 函数读取 CSV 文件 weather_data.csv 的内容，随后是一系列 Python print() 打印语句，显示了 CSV 文件的不同部分。列表 3.18 的输出如下：

```py
 day  temperature  windspeed     event
0  7/1/2018           42         16   Rain
1  7/2/2018           45          3  Sunny
2  7/3/2018           78         12   Snow
3  7/4/2018           74          9  Snow
4  7/5/2018           42         24   Rain
5  7/6/2018           51         32    Sunny
(6, 4)
        day  temperature  windspeed     event
0  7/1/2018           42         16   Rain
1  7/2/2018           45          3  Sunny
2  7/3/2018           78         12   Snow
3  7/4/2018           74          9  Snow
4  7/5/2018           42         24   Rain
        day  temperature  windspeed     event
1  7/2/2018           45          3  Sunny
2  7/3/2018           78         12   Snow
3  7/4/2018           74          9  Snow
4  7/5/2018           42         24   Rain
5  7/6/2018           51         32    Sunny
        day  temperature  windspeed     event
1  7/2/2018           45          3  Sunny
2  7/3/2018           78         12   Snow
Index(['day', 'temperature', 'windspeed', 'event'], dtype='object')
<class 'pandas.core.series.Series'>
        day  temperature
0  7/1/2018           42
1  7/2/2018           45
2  7/3/2018           78
3  7/4/2018           74
4  7/5/2018           42
5  7/6/2018           51
78 
```

在某些情况下，你可能需要应用布尔条件逻辑来根据应用于列值的条件“过滤”出一些数据行。

列表 3.19 显示了 CSV 文件 people.csv 的内容，列表 3.20 显示了 people_pandas.py 的内容，该内容说明了如何定义一个读取 CSV 文件并操作数据的 Pandas 数据框。

***列表 3.19：people.csv***

```py
 fname,lname,age,gender,country
john,smith,30,m,usa
jane,smith,31,f,france
jack,jones,32,m,france dave,stone,33,m,italy
sara,stein,34,f,germany
eddy,bower,35,m,spain 
```

***列表 3.20：people_pandas.py***

```py
 import pandas as pd

df = pd.read_csv('people.csv')
df.info()
print('fname:')
print(df['fname'])
print('____________')
print('age over 33:')
print(df['age'] > 33)
print('____________')
print('age over 33:')
myfilter = df['age'] >  33
print(df[myfilter]) 
```

列表 3.20 使用 CSV 文件 people.csv 的内容填充 Pandas 数据框 df。列表 3.20 的下一部分显示了 df 的结构，接着是所有人的名字。列表 3.20 的下一部分显示了一个包含六行的表格列表，根据一个人是否超过 33 岁或最多 33 岁分别显示 True 或 False。列表 3.20 的最后一部分显示了一个包含超过 33 岁的人的所有详细信息的表格列表。列表 3.20 的输出如下：

```py
 myfilter = df['age'] >  33
<class 'pandas.core.frame.DataFrame'>
RangeIndex: 6 entries, 0 to 5
Data columns (total 5 columns):
fname      6 non_null object
lname      6 non_null object
age        6 non_null int64
gender     6 non_null object
country    6 non_null object
dtypes: int64(1), object(4)
memory usage: 320.0+ bytes
fname:
0    john
1    jane
2    jack
3    dave
4    sara
5    eddy
Name: fname, dtype: object
____________
age over 33:
0    False
1    False
2    False
3    False 4     True
5     True
Name: age, dtype: bool
____________
age over 33:
  fname  lname  age gender country
4  sara  stein   34      f  france
5  eddy  bower   35      m  france 
```

### **PANDAS 数据框和 Excel 电子表格**

列表 3.21 展示了 write_people_xlsx.py 的内容，说明了如何从 CSV 文件读取数据然后创建包含该数据的 Excel 工作表。

***列表 3.21: write_people_xlsx.py***

```py
 import pandas as pd

df1 = pd.read_csv("people.csv")
df1.to_excel("people.xlsx")

#optionally specify the sheet name:
#df1.to_excel("people.xlsx", sheet_name='Sheet_name_1') 
```

列表 3.21 初始化 Pandas DataFrame df1，包含 CSV 文件 people.csv 的内容，然后调用 to_excel() 方法将 DataFrame 的内容保存到 Excel 工作表 people.xlsx 中。

列表 3.22 展示了 read_people_xlsx.py 的内容，说明了如何从 Excel 工作表 people.xlsx 读取数据并创建包含该数据的 Pandas DataFrame。

***列表 3.22: read_people_xlsx.py***

```py
 import pandas as pd

df = pd.read_excel("people.xlsx")
print("Contents of Excel spreadsheet:")
print(df) 
```

列表 3.22 很简单：通过 Pandas 函数 read_excel()，使用工作表 people.xlsx（其内容与 people.csv 相同）的内容初始化 Pandas DataFrame df。列表 3.22 的输出如下：

```py
 df1:
   Unnamed: 0 fname  lname  age gender  country
0           0  john  smith   30      m      usa
1           1  jane  smith   31      f   france
2           2  jack  jones   32      m   france 3           3  dave  stone   33      m    italy
4           4  sara  stein   34      f  germany
5           5  eddy  bower   35      m    spain 
```

### **在 DataFrames 中选择、添加和删除列**

本节包含一些简短的代码块，展示了如何在 DataFrame 上执行类似于在 Python 字典上执行的操作。例如，获取、设置和删除列的语法与类似的 Python dict 操作相同，如下所示：

```py
 df = pd.DataFrame.from_dict(dict([('A',[1,2,3]),('B',[4,5,6])]),
                orient='index', columns=['one', 'two', 'three'])

print(df) 
```

前一个代码片段的输出如下：

```py
 one  two  three
A    1    2      3
B    4    5      6 
```

现在看看以下操作，它向 DataFrame df 的内容中追加一个新列：

```py
 df['four'] = df['one'] * df['two']
print(df) 
```

前一个代码块输出的结果如下：

```py
 one  two  three  four
A    1    2      3     2
B    4    5      6    20 
```

以下操作对 DataFrame df 中的一列内容进行平方：

```py
 df['three'] = df['two'] * df['two']
print(df) 
```

前一个代码块的输出如下：

```py
 one  two  three  four
A    1    2      4     2
B    4    5     25    20 
```

以下操作在 DataFrame df 的索引位置 1（即第二列）插入一列随机数：

```py
import numpy as np
rand = np.random.randn(2)
df.insert(1, 'random', rand)
print(df) 
```

前一个代码块的输出如下：

```py
 one    random  two  three  four
A    1 -1.703111    2      4     2
B    4  1.139189    5     25    20 
```

以下操作在 DataFrame df 的内容中追加一个名为 flag 的新列，该列包含 True 或 False，根据“one”列中的数值是否大于 2 来决定：

```py
 import numpy as np
rand = np.random.randn(2)
df.insert(1, 'random', rand)
print(df) 
```

前一个代码块输出的结果如下：

```py
 one    random  two  three  four   flag
A    1 -1.703111    2      4     2  False
B    4  1.139189    5     25    20   True 
```

可以删除列，如下面的代码片段所示，删除了“two”列：

```py
 del df['two']
print(df) 
```

前一个代码块输出的结果如下：

```py
 one    random  three  four   flag
A    1 -0.460401      4     2  False
B    4  1.211468     25    20   True 
```

可以通过 pop() 方法删除列，如下面的代码片段所示，删除了“three”列：

```py
 three = df.pop('three')
print(df)

   one    random  four   flag
A    1 -0.544829     2  False
B    4  0.581476    20   True 
```

当插入一个标量值时，它将自然地传播以填充列：

```py
 df['foo'] = 'bar'
print(df) 
```

前一个代码片段的输出如下：

```py
 one    random  four   flag  foo
A    1 -0.187331     2  False  bar
B    4 -0.169672    20   True  bar 
```

### **在 Pandas 中处理异常值**

如果你对异常值和异常不熟悉，请搜索在线文章讨论这两个概念，因为本节使用 Pandas 在数据集中查找异常值。关键思想涉及找到数据集中值的“z 分数”，这涉及到计算均值 sigma 和标准差 std，然后将数据集中的每个值 x 映射到值 (x-sigma)/std。

接下来，你指定一个 z 值（例如 3）并找到 z 分数大于 3 的行。这些行包含被认为是异常值的值。*注意，z 分数的合适值是你的决定（而不是其他外部因素）。*

列表 3.23 显示了 outliers_zscores.py 的内容，该内容说明了如何找到数据集中 z 分数大于（或小于）指定值的行。

***列表 3.23: outliers_zscores.py***

```py
 import numpy as np
import pandas as pd
from scipy import stats
from sklearn import datasets

df = datasets.load_iris()
columns = df.feature_names
iris_df = pd.DataFrame(df.data)
iris_df.columns = columns

print("=> iris_df.shape:",iris_df.shape)
print(iris_df.head())
print()

z = np.abs(stats.zscore(iris_df))
print("z scores for iris:")
print("z.shape:",z.shape)

upper = 2.5
lower = 0.01
print("=> upper outliers:")
print(z[np.where(z > upper)])
print()

outliers = iris_df[z < lower]
print("=> lower outliers:")
print(outliers)
print() 
```

列表 3.23 初始化变量 df 为内置的 Iris 数据集的内容。接下来，变量 columns 被初始化为列名，DataFrame iris_df 从 df.data 的内容初始化，其中包含 Iris 数据集的实际数据。此外，iris_df.columns 被初始化为变量 columns 的内容。

列表 3.23 的下一部分显示了 DataFrame iris_df 的形状，接着是 iris_df DataFrame 的 z 分数，该分数是通过减去平均值然后除以标准差（对每一行执行）计算得出的。

列表 3.23 的最后两部分显示了（如果有）z 分数超出区间[0.01, 2.5]的异常值。运行列表 3.23 中的代码，你将看到以下输出：

```py
 => iris_df.shape: (150, 4)
 sepal length (cm) sepal width (cm)    petal length (cm) petal width (cm)
0               5.1              3.5               1.4             0.2
1               4.9              3.0               1.4             0.2
2               4.7              3.2               1.3             0.2
3               4.6              3.1               1.5             0.2
4               5.0              3.6               1.4             0.2

z scores for iris:
z.shape: (150, 4)

=> upper outliers:
[3.09077525 2.63038172]

=> lower outliers:
sepal length (cm)  sepal width (cm)  petal length (cm)  petal width (cm)
73               6.1              2.8              4.7             1.2
82               5.8              2.7              3.9             1.2
90               5.5              2.6              4.4             1.2
92               5.8              2.6              4.0             1.2
95               5.7              3.0              4.2             1.2 
```

### **Pandas DataFrame 和散点图**

列表 3.24 显示了 pandas_scatter_df.py 的内容，该内容说明了如何从 Pandas DataFrame 生成散点图。

***列表 3.24: pandas_scatter_df.py***

```py
 import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
from pandas import read_csv
from pandas.plotting import scatter_matrix

myarray = np.array([[10,30,20], [50,40,60],[1000,2000,3000]])
rownames = ['apples', 'oranges', 'beer']
colnames = ['January', 'February', 'March'] mydf = pd.DataFrame(myarray, index=rownames, columns=colnames)

print(mydf)
print(mydf.describe())

scatter_matrix(mydf)
plt.show() 
```

列表 3.24 以各种导入语句开始，接着定义 NumPy 数组 myarray。然后，变量 myarray 和 colnames 分别初始化为行和列的值。列表 3.24 的下一部分初始化 Pandas DataFrame mydf，以便在输出中标记行和列，如下所示：

```py
 January  February  March
apples        10        30     20
oranges       50        40     60
beer        1000      2000   3000
           January     February        March
count     3.000000     3.000000     3.000000
mean    353.333333   690.000000  1026.666667
std     560.386771  1134.504297  1709.073823
min      10.000000    30.000000    20.000000
25%      30.000000    35.000000    40.000000
50%      50.000000    40.000000    60.000000
75%     525.000000  1020.000000  1530.000000
max    1000.000000  2000.000000  3000.0000000 
```

### **Pandas DataFrame 和简单统计**

列表 3.25 显示了 housing_stats.py 的内容，该内容说明了如何从 Pandas DataFrame 中的数据收集基本统计信息。

***列表 3.25: housing_stats.py***

```py
 import pandas as pd

df = pd.read_csv("housing.csv")

minimum_bdrms = df["bedrooms"].min()
median_bdrms  = df["bedrooms"].median()
maximum_bdrms = df["bedrooms"].max()

print("minimum # of bedrooms:",minimum_bdrms)
print("median  # of bedrooms:",median_bdrms)
print("maximum # of bedrooms:",maximum_bdrms)
print("")

print("median values:",df.median().values)
print("") prices = df["price"]
print("first 5 prices:")
print(prices.head())
print("")

median_price = df["price"].median()
print("median price:",median_price)
print("")

corr_matrix = df.corr()
print("correlation matrix:")
print(corr_matrix["price"].sort_values(ascending=False)) 
```

列表 3.25 使用 CSV 文件 housing.csv 的内容初始化 Pandas DataFrame df。接下来三个变量分别初始化为卧室数量的最小值、中位数和最大值，然后显示这些值。

列表 3.25 的下一部分初始化变量 prices 为 Pandas DataFrame df 的价格列的内容。接下来，通过 prices.head()语句打印前五行，然后打印价格的中位数。

列表 3.25 的最后一部分初始化变量 corr_matrix 为 Pandas DataFrame df 的相关矩阵的内容，然后显示其内容。列表 3.25 的输出如下：

```py
 Apples
10 
```

### **在 Pandas 中查找重复行**

列表 3.26 显示 duplicates.csv 的内容，列表 3.27 显示 duplicates.py 的内容，该内容说明了如何在 Pandas 数据框中查找重复行。

***列表 3.26: duplicates.csv***

```py
 fname,lname,level,dept,state
Jane,Smith,Senior,Sales,California
Dave,Smith,Senior,Devel,California
Jane,Jones,Year1,Mrktg,Illinois
Jane,Jones,Year1,Mrktg,Illinois
Jane,Stone,Senior,Mrktg,Arizona
Dave,Stone,Year2,Devel,Arizona
Mark,Aster,Year3,BizDev,Florida
Jane,Jones,Year1,Mrktg,Illinois 
```

***列表 3.27: duplicates.py***

```py
 import pandas as pd

df = pd.read_csv("duplicates.csv")
print("Contents of data frame:") print(df)
print()

print("Duplicate rows:")
#df2 = df.duplicated(subset=None)
df2 = df.duplicated(subset=None, keep='first')
print(df2)
print()

print("Duplicate first names:")
df3 = df[df.duplicated(['fname'])]
print(df3)
print()

print("Duplicate first name and level:")
df3 = df[df.duplicated(['fname','level'])]
print(df3)
print() 
```

列表 3.27 使用 duplicates.csv 文件的內容初始化 DataFrame df，然后显示 DataFrame 的内容。列表 3.27 的下一部分通过调用 duplicated() 方法显示重复行，而列表 3.27 的下一部分仅显示重复行的姓氏 fname。列表 3.27 的最后一部分显示重复行的姓氏 fname 以及重复行的级别。运行列表 3.27 中的代码，你将看到以下输出：

```py
 Contents of data frame:
  fname  lname   level    dept       state
0  Jane  Smith  Senior   Sales  California
1  Dave  Smith  Senior   Devel  California
2  Jane  Jones   Year1   Mrktg    Illinois
3  Jane  Jones   Year1   Mrktg    Illinois
4  Jane  Stone  Senior   Mrktg     Arizona
5  Dave  Stone   Year2   Devel     Arizona
6  Mark  Aster   Year3  BizDev     Florida
7  Jane  Jones   Year1   Mrktg    Illinois

Duplicate rows:
0    False
1    False
2    False
3     True
4    False
5    False
6    False
7     True
dtype: bool

Duplicate first names:
  fname  lname   level   dept     state
2  Jane  Jones   Year1  Mrktg  Illinois
3  Jane  Jones   Year1  Mrktg  Illinois
4  Jane  Stone  Senior  Mrktg   Arizona 5  Dave  Stone   Year2  Devel   Arizona
7  Jane  Jones   Year1  Mrktg  Illinois

Duplicate first name and level:
  fname  lname   level   dept     state
3  Jane  Jones   Year1  Mrktg  Illinois
4  Jane  Stone  Senior  Mrktg   Arizona
7  Jane  Jones   Year1  Mrktg  Illinois 
```

列表 3.28 显示 drop_duplicates.py 的内容，该内容说明了如何在 Pandas 数据框中删除重复行。

***列表 3.28: drop_duplicates.py***

```py
 import pandas as pd

df = pd.read_csv("duplicates.csv")
print("Contents of data frame:")
print(df)
print()

fname_filtered = df.drop_duplicates(['fname'])
print("Drop duplicate first names:")
print(fname_filtered)
print()

fname_lname_filtered = df.drop_duplicates(['fname','lname'])
print("Drop duplicate first and last names:")
print(fname_lname_filtered)
print() 
```

列表 3.28 使用 duplicates.csv 文件的內容初始化 DataFrame df，然后显示 DataFrame 的内容。列表 3.28 的下一部分删除具有重复 fname 值的行，然后是一个删除具有重复 fname 和 lname 值的行的代码块。运行列表 3.28 中的代码，你将看到以下输出：

```py
 Contents of data frame:
  fname  lname   level    dept       state
0  Jane  Smith  Senior   Sales  California
1  Dave  Smith  Senior   Devel  California 2  Jane  Jones   Year1   Mrktg    Illinois
3  Jane  Jones   Year1   Mrktg    Illinois 4  Jane  Stone  Senior   Mrktg     Arizona
5  Dave  Stone   Year2   Devel     Arizona
6  Mark  Aster   Year3  BizDev     Florida
7  Jane  Jones   Year1   Mrktg    Illinois

Drop duplicate first names:
  fname  lname   level    dept       state
0  Jane  Smith  Senior   Sales  California 1  Dave  Smith  Senior   Devel  California
6  Mark  Aster   Year3  BizDev     Florida

Drop duplicate first and last names:
  fname  lname   level    dept       state
0  Jane  Smith  Senior   Sales  California
1  Dave  Smith  Senior   Devel  California
2  Jane  Jones   Year1   Mrktg    Illinois
4  Jane  Stone  Senior   Mrktg     Arizona
5  Dave  Stone   Year2   Devel     Arizona
6  Mark  Aster   Year3  BizDev     Florida 
```

### **在 Pandas 中查找缺失值**

列表 3.29 显示 employees2.csv 的内容，列表 3.30 显示 missing_values.py 的内容，该内容说明了如何在 Pandas 数据框中显示具有缺失值的行。

***列表 3.29: employees2.csv***

```py
 name,year,month
Jane-Smith,2015,Aug
Jane-Smith,2015,Aug
Dave-Smith,2020,
Dave-Stone,Apr
Jane-Jones,2018,Dec
Jane-Stone,2017,Feb
Jane-Stone,2017,Feb
Mark-Aster,Oct
Jane-Jones,NaN,Jun 
```

***列表 3.30: missing_values.py***

```py
 import pandas as pd
import matplotlib.pyplot as plt
import numpy as np

df = pd.read_csv("employees2.csv")

print("=> contents of CSV file:")
print(df)
print()

#NA:  Not Available (Pandas)
#NaN: Not a Number (Pandas)
#NB:  NumPy uses np.nan() to check for NaN values

df = pd.read_csv("employees2.csv")

print("=> contents of CSV file:")
print(df)
print() print("=> any NULL values per column?")
print(df.isnull().any())
print()

print("=> count of NAN/MISSING values in each column:")
print(df.isnull().sum())
print()
print("=> count of NAN/MISSING values in each column:")
print(pd.isna(df).sum())
print()

print("=> count of NAN/MISSING values in each column (sorted):")
print(df.isnull().sum().sort_values(ascending=False))
print()

nan_null = df.isnull().sum().sum()
miss_values = df.isnull().any().sum()

print("=> count of NaN/MISSING values:",nan_null)
print("=> count of MISSING values:",miss_values)
print("=> count of NaN values:",nan_null-miss_values) 
```

列表 3.30 使用 employees2.csv 文件的內容初始化 DataFrame df，然后显示 DataFrame 的内容。列表 3.30 的下一部分显示任何行或列中出现的空值数量。列表 3.30 的下一部分显示具有空值的字段及其名称。

列表 3.30 的下一部分显示重复行的数量，然后是重复行的行号。运行列表 3.30 中的代码，你将看到以下输出：

```py
 => contents of CSV file:
         name    year month
0  Jane-Smith  2015.0   Aug
1  Jane-Smith  2015.0   Aug
2  Dave-Smith  2020.0   NaN
3  Dave-Stone     NaN   Apr
4  Jane-Jones  2018.0   Dec
5  Jane-Stone  2017.0   Feb
6  Jane-Stone  2017.0   Feb
7  Mark-Aster     NaN   Oct
8  Jane-Jones     NaN   Jun

=> any NULL values per column? name     False
year      True
month     True
dtype: bool

=> count of NAN/MISSING values in each column:
name     0
year     3 month    1
dtype: int64

=> count of NAN/MISSING values in each column:
name     0
year     3
month    1
dtype: int64

=> count of NAN/MISSING values in each column (sorted):
year     3
month    1
name     0
dtype: int64

=> count of NaN/MISSING values: 4
=> count of MISSING values: 2
=> count of NaN values: 2 
```

### **在 Pandas 中排序数据框**

列表 3.31 显示 sort_df.py 的内容，该内容说明了如何在 Pandas 数据框中排序行。

***列表 3.31: sort_df.py***

```py
 import pandas as pd

df = pd.read_csv("duplicates.csv")
print("Contents of data frame:")
print(df)
print()

df.sort_values(by=['fname'], inplace=True)
print("Sorted (ascending) by first name:")
print(df)
print()

df.sort_values(by=['fname'], inplace=True,ascending=False)
print("Sorted (descending) by first name:")
print(df)
print()

df.sort_values(by=['fname','lname'], inplace=True)
print("Sorted (ascending) by first name and last name:")
print(df)
print() 
```

列表 3.31 使用 duplicates.csv 文件的內容初始化 DataFrame df，然后显示 DataFrame 的内容。列表 3.31 的下一部分根据姓氏以升序显示行，接下来的代码块以降序显示姓氏的行。

列表 3.31 的最后一个代码块根据姓氏和名字的升序显示行。运行 列表 3.31 中的代码，您将看到以下输出：

```py
 Contents of data frame:
  fname  lname   level    dept       state
0  Jane  Smith  Senior   Sales  California
1  Dave  Smith  Senior   Devel  California
2  Jane  Jones   Year1   Mrktg    Illinois
3  Jane  Jones   Year1   Mrktg    Illinois
4  Jane  Stone  Senior   Mrktg     Arizona
5  Dave  Stone   Year2   Devel     Arizona
6  Mark  Aster   Year3  BizDev     Florida
7  Jane  Jones   Year1   Mrktg    Illinois

Sorted (ascending) by first name:
  fname  lname   level    dept       state
1  Dave  Smith  Senior   Devel  California
5  Dave  Stone   Year2   Devel     Arizona
0  Jane  Smith  Senior   Sales  California
2  Jane  Jones   Year1   Mrktg    Illinois
3  Jane  Jones   Year1   Mrktg    Illinois
4  Jane  Stone  Senior   Mrktg     Arizona
7  Jane  Jones   Year1   Mrktg    Illinois
6  Mark  Aster   Year3  BizDev     Florida

Sorted (descending) by first name:
  fname  lname   level    dept       state
6  Mark  Aster   Year3  BizDev     Florida
0  Jane  Smith  Senior   Sales  California
2  Jane  Jones   Year1   Mrktg    Illinois
3  Jane  Jones   Year1   Mrktg    Illinois
4  Jane  Stone  Senior   Mrktg     Arizona
7  Jane  Jones   Year1   Mrktg    Illinois
1  Dave  Smith  Senior   Devel  California
5  Dave  Stone   Year2   Devel     Arizona

Sorted (ascending) by first name and last name:
  fname  lname   level    dept       state
1  Dave  Smith  Senior   Devel  California
5  Dave  Stone   Year2   Devel     Arizona
2  Jane  Jones   Year1   Mrktg    Illinois
3  Jane  Jones   Year1   Mrktg    Illinois
7  Jane  Jones   Year1   Mrktg    Illinois
0  Jane  Smith  Senior   Sales  California
4  Jane  Stone  Senior   Mrktg     Arizona
6  Mark  Aster   Year3  BizDev     Florida 
```

### **在 Pandas 中使用 GROUPBY()**

列表 3.32 显示了 groupby1.py 的内容，该内容说明了如何调用 Pandas groupby() 方法来计算特征值的子总计。

***列表 3.32: groupby1.py***

```py
 import pandas as pd

# colors and weights of balls:
data = {'color':['red','blue','blue','red','blue'],
        'weight':[40,50,20,30,90]}
df1 = pd.DataFrame(data)
print("df1:")
print(df1)
print()
print(df1.groupby('color').mean())
print()

red_filter = df1['color']=='red'
print(df1[red_filter])
print()
blue_filter = df1['color']=='blue'
print(df1[blue_filter])
print()

red_avg = df1[red_filter]['weight'].mean()
blue_avg = df1[blue_filter]['weight'].mean()
print("red_avg,blue_avg:")
print(red_avg,blue_avg)
print()

df2 = pd.DataFrame({'color':['blue','red'],'weight': [red_avg,blue_avg]})
print("df2:")
print(df2)
print() 
```

列表 3.32 定义了包含颜色和重量值的变量 data，然后使用该变量的内容初始化 DataFrame df。接下来的两个代码块定义了 red_filter 和 blue_filter，分别匹配颜色为红色和蓝色的行，然后打印匹配的行。

列表 3.32 的下一部分定义了两个过滤器 red_avg 和 blue_avg，分别计算红色值和蓝色值的平均值。在 列表 3.32 的最后一个代码块中定义了 DataFrame df2，其中包含一个颜色列和一个重量列，后者包含红色值和蓝色值的平均值。运行 列表 3.32 中的代码，您将看到以下输出：

```py
 initial data frame:
df1:
  color  weight
0   red      40
1  blue      50
2  blue      20
3   red      30
4  blue      90 color  weight
blue   53.333333
red    35.000000

  color  weight
0   red      40
3   red      30

  color  weight
1  blue      50
2  blue      20
4  blue      90

red_avg,blue_avg:
35.0 53.333333333333336

df2:
  color     weight
0  blue  35.000000
1   red  53.333333 
```

### **使用 TITANIC.CSV 数据集进行聚合操作**

列表 3.33 显示了 aggregate2.py 的内容，该内容说明了如何使用 CSV 文件 titanic.csv 中的列执行聚合操作。

***列表 3.33: aggregate2.py***

```py
 import pandas as pd

#Loading titanic.csv in Seaborn:
#df = sns.load_dataset('titanic')
df = pd.read_csv("titanic.csv")

# convert floating point values to integers:
df['survived'] = df['survived'].astype(int)

# specify column and aggregate functions:
aggregates1 = {'embark_town': ['count', 'nunique', 'size']}

# group by 'deck' value and apply aggregate functions:
result = df.groupby(['deck']).agg(aggregates1)
print("=> Grouped by deck:")
print(result)
print()

# some details regarding count() and nunique():
# count() excludes NaN values whereas size() includes them
# nunique() excludes NaN values in the unique counts

# group by 'age' value and apply aggregate functions:
result2 = df.groupby(['age']).agg(aggregates1) print("=> Grouped by age (before):")
print(result2)
print()

# some "age" values are missing (so drop them):
df = df.dropna()

# convert floating point values to integers:
df['age'] = df['age'].astype(int)

# group by 'age' value and apply aggregate functions:
result3 = df.groupby(['age']).agg(aggregates1)
print("=> Grouped by age (after):")
print(result3)
print() 
```

列表 3.33 使用 titanic.csv 文件的内容初始化 DataFrame df。下一个代码片段将浮点值转换为整数，然后定义变量 aggregates1，该变量指定将在 embark_town 字段上调用的函数 count()、nunique() 和 size()。

下一个代码片段在调用 deck 字段的 groupby() 方法之后初始化变量 result，然后调用 agg() 方法。

下一个代码块执行相同的计算以初始化变量 result2，但调用 groupby() 函数的是 age 字段而不是 embark_town 字段。注意关于 count() 和 nunique() 函数的注释部分：让我们通过 df.dropna() 删除缺失值的行，并调查这对计算的影响。

删除缺失值的行后，最后一个代码块以与 result2 相同的方式初始化变量 result3。运行 列表 3.33 中的代码，输出如下所示：

```py
 => Grouped by deck:
     embark_town
           count nunique size
deck
A             15       2   15
B             45       2   47
C             59       3   59
D             33       2   33
E             32       3   32
F             13       3   13
G              4       1    4

=> Grouped by age (before):
        age
      count nunique size
age
0.42      1       1    1
0.67      1       1    1
0.75      2       1    2
0.83      2       1    2
0.92      1       1    1
... ... ... ... 70.00     2       1    2
70.50     1       1    1
71.00     2       1    2
74.00     1       1    1
80.00     1       1    1

[88 rows x 3 columns]

=> Grouped by age (after):
      age
    count nunique size
age
0       1       1    1
1       1       1    1
2       3       1    3
3       1       1    1
4       3       1    3
6       1       1    1
11      1       1    1
14      1       1    1
15      1       1    1
// details omitted for brevity
60      2       1    2
61      2       1    2
62      1       1    1
63      1       1    1
64      1       1    1
65      2       1    2
70      1       1    1
71      1       1    1
80      1       1    1 
```

### **在 Pandas 中使用 apply() 和 mapapply()**

在本章的早期部分，您看到了 Pandas apply() 方法的示例，用于修改 shirts.csv 文件中特征的分类值。本节包含更多 apply() 方法的示例，以及 mapapply() 方法的示例。

列表 3.34 展示了 apply1.py 的内容，该文件说明了如何调用 Pandas 的 apply() 方法来计算一组值的总和。

***列表 3.34: apply1.py***

```py
 import pandas as pd

df = pd.DataFrame({'X1': [1,2,3], 'X2': [10,20,30]})

def cube(x):
  return x * x * x

df1 = df.apply(cube)
# same result: # df1 = df.apply(lambda x: x * x * x)
print("initial data frame:")
print(df)
print("cubed values:")
print(df1) 
```

列表 3.34 使用列 X1 和 X2 初始化 DataFrame df，其中 X2 的值是 X1 对应值的 10 倍。接下来，Python 函数 cube() 返回其参数的立方。然后 列表 3.34 通过调用 apply() 函数定义变量 df1，该函数指定了用户定义的 Python 函数 cube()，并打印 df 和 df1 的值。运行 列表 3.34 中的代码，你将看到以下输出：

```py
 initial data frame:
   X1  X2
0   1  10
1   2  20
2   3  30
cubed values:
   X1     X2
0   1   1000
1   8   8000
2  27  27000 
```

列表 3.35 展示了 apply2.py 的内容，该文件说明了如何调用 Pandas 的 apply() 方法来计算一组值的总和。

***列表 3.35: apply2.py***

```py
 import pandas as pd
import numpy as np

df = pd.DataFrame({'X1': [10,20,30], 'X2': [50,60,70]})

df1 = df.apply(np.sum, axis=0)
df2 = df.apply(np.sum, axis=1)

print("initial data frame:")
print(df)
print("add values (axis=0):")
print(df1)
print("add values (axis=1):")
print(df2) 
```

列表 3.35 是 列表 3.34 的一个变体：变量 df1 和 df2 分别包含 DataFrame df 的列总和和行总和。运行 列表 3.35 中的代码，你将看到以下输出：

```py
 X1  X2
0  10  50
1  20  60 2  30  70
add values (axis=0):
X1     60
X2    180
dtype: int64
add values (axis=1):
0     60
1     80
2    100
dtype: int64 
```

列表 3.36 展示了 mapapply1.py 的内容，该文件说明了如何调用 Pandas 的 mapapply() 方法来计算一组值的总和。

***列表 3.36: mapapply1.py***

```py
 import pandas as pd
import math

df = pd.DataFrame({'X1': [1,2,3], 'X2': [10,20,30]})
df1 = df.applymap(math.sqrt)

print("initial data frame:")
print(df)
print("square root values:")
print(df1) 
```

列表 3.36 是 列表 3.34 的另一个变体：在这种情况下，变量 df1 通过调用 df 的 applymap() 方法定义，它反过来引用（但不执行） math.sqrt() 函数。接下来，一个 print() 语句显示 df 的内容，然后是一个 print() 语句显示 df1 的内容：此时将内置的 math.sqrt() 函数调用以计算 df 中值的平方根。运行 列表 3.36 中的代码，你将看到以下输出：

```py
 initial data frame:
   X1  X2
0   1  10
1   2  20
2   3  30

square root values:
         X1        X2
0  1.000000  3.162278
1  1.414214  4.472136
2  1.732051  5.477226 
```

列表 3.37 展示了 mapapply2.py 的内容，该文件说明了如何调用 Pandas 的 mapapply() 方法来将字符串转换为小写和大写。

***列表 3.37: mapapply2.py***

```py
 import pandas as pd

df = pd.DataFrame({'fname': ['Jane'], 'lname': ['Smith']},
                  {'fname': ['Dave'], 'lname': ['Jones']})

df1 = df.applymap(str.lower)
df2 = df.applymap(str.upper)

print("initial data frame:")
print(df)
print()
print("lowercase:")
print(df1)
print()
print("uppercase:")
print(df2)
print() 
```

列表 3.37 初始化变量 df，包含两个姓名对，然后通过调用 applymap() 方法到变量 df 上定义变量 df1 和 df2。变量 df1 将其输入值转换为小写，而变量 df2 将其输入值转换为大写。运行 列表 3.37 中的代码，你将看到以下输出：

```py
 initial data frame:
      fname  lname
fname  Jane  Smith
lname  Jane  Smith

lowercase:
      fname  lname
fname  jane  smith
lname  jane  smith

uppercase:
      fname  lname
fname  JANE  SMITH
lname  JANE  SMITH 
```

### **PANDAS 中有用的单行命令**

本节包含 Pandas 中的各种单行命令（其中一些你在本章中已经见过），这些命令很有用：

将 DataFrame 保存到 CSV 文件（逗号分隔，不含索引）：

```py
 df.to_csv("data.csv", sep=",", index=False) 
```

列出 DataFrame 的列名：

```py
 df.columns 
```

从 DataFrame 中删除缺失数据：

```py
 df.dropna(axis=0, how='any') 
```

在 DataFrame 中替换缺失数据：

```py
 df.replace(to_replace=None, value=None) 
```

在 DataFrame 中检查 NAN：

```py
 pd.isnull(object) 
```

从 DataFrame 中删除一个特征：

```py
 df.drop('feature_variable_name', axis=1) 
```

在 DataFrame 中将对象类型转换为浮点数：

```py
 pd.to_numeric(df["feature_name"], errors='coerce') 
```

将 DataFrame 中的数据转换为 NumPy 数组：

```py
 df.as_matrix() 
```

显示 DataFrame 的前 n 行：

```py
 df.head(n) 
```

在 DataFrame 中按特征名称获取数据：

```py
 df.loc[feature_name] 
```

将 lambda 函数应用于 DataFrame，例如将 DataFrame 中“height”列的所有值乘以 3：

```py
 df["height"].apply(lambda height: 3 * height) 
```

或者：

```py
 def multiply(x):
    return x * 3
df["height"].apply(multiply) 
```

将 DataFrame 的第四列重命名为“height”：

```py
 df.rename(columns = {df.columns[3]:'height'}, inplace=True) 
```

获取 DataFrame 中“first”列的唯一条目：

```py
 df["first"].unique() 
```

从现有 DataFrame 中创建包含“first”和“last”列的 DataFrame：

```py
 new_df = df[["first", "last"]] 
```

对 DataFrame 中的数据进行排序：

```py
 df.sort_values(ascending = False) 
```

过滤名为“size”的数据列，仅显示等于 7 的值：

```py
 df[df["size"] == 7] 
```

在 DataFrame 中选择“height”列的第一行：

```py
 df.loc([0], ['height']) 
```

### **什么是 Texthero？**

Texthero 是一个基于 Python 的开源工具包，它作为 Pandas 之上的抽象层，其主页在此：

*[`github.com/jbesomi/texthero`](https://github.com/jbesomi/texthero)*

Texthero 利用非常实用的 Python NLP 库，如 Gensim、NLTK、SpaCy 和 Sklearn。此外，Texthero 支持以下功能：

+   命名实体识别 (NER) 和主题建模（用于 NLP）

+   TF-IDF、词频和词嵌入（用于 NLP）

+   DBSCAN、层次聚类、k-Means 和 Meanshift 算法

+   各种类型的文本可视化

打开命令行并使用以下命令安装 texthero：

```py
 pip3 install texthero 
```

Texthero 支持各种其他算法，包括用于机器学习的降维算法。导航到以下链接以获取有关 Texthero 的文档和其他信息：

*[`texthero.org/docs/getting-started`](https://texthero.org/docs/getting-started)*

### **PANDAS 中的数据可视化**

虽然 Matplotlib 和 Seaborn 经常是数据可视化的“首选”Python 库，但你也可以使用 Pandas 来完成此类任务。

列表 3.38 展示了 pandas_viz1.py 的内容，该内容说明了如何使用 Pandas 和 Matplotlib 渲染各种类型的图表和图形。

***列表 3.38：pandas_viz1.py***

```py
 import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

df = pd.DataFrame(np.random.rand(16,3), columns=['X1','X2','X3'])
print("First 5 rows:")
print(df.head())
print()

print("Diff of first 5 rows:")
print(df.diff().head())
print()

# bar chart:
#ax = df.plot.bar()

# horizontal stacked bar chart:
#ax = df.plot.barh(stacked=True)

# vertical stacked bar chart:
ax = df.plot.bar(stacked=True)

# stacked area graph:
#ax = df.plot.area()

# non-stacked area graph:
#ax = df.plot.area(stacked=False)

#plt.show(ax) 
```

列表 3.38 使用随机数 16x3 矩阵初始化 DataFrame df，然后是 df 的内容。列表 3.38 的主要内容是生成条形图、水平堆叠条形图、垂直堆叠条形图、堆叠面积图和非堆叠面积图的代码片段。您可以通过取消注释显示您选择的图形的代码片段来使用 df 的内容。运行列表 3.38 中的代码，您将看到以下输出：

```py
 First 5 rows:
         X1        X2        X3
0  0.051089  0.357183  0.344414
1  0.800890  0.468372  0.800668
2  0.492981  0.505133  0.228399
3  0.461996  0.977895  0.471315
4  0.033209  0.411852  0.347165

Diff of first 5 rows:
         X1        X2        X3
0       NaN       NaN       NaN
1  0.749801  0.111189  0.456255
2 -0.307909  0.036760 -0.572269
3 -0.030984  0.472762  0.242916
4 -0.428787 -0.566043 -0.124150 
```

### **总结**

本章向您介绍了 Pandas，用于创建标记的 DataFrame 并显示 Pandas DataFrame 的元数据。然后您学习了如何从各种数据源创建 Pandas DataFrame，例如随机数和硬编码的数据值。

您还学习了如何读取 Excel 电子表格并对该数据进行数值计算，例如数值列中的最小值、平均值和最大值。然后您看到了如何从存储在 CSV 文件中的数据创建 Pandas DataFrame。此外，您还学习了如何从 Pandas DataFrame 中的数据生成散点图。

然后，您简要介绍了 JSON，并提供了将 Python 字典转换为基于 JSON 的数据（反之亦然）的示例。最后，您了解了 Texthero，这是一个在 Pandas 之上的开源 Python 工具包。

## 第四章

## *Pandas 和 SQL*

本章包含各种包含 Pandas、SQL 和 SQLite3 的 Python 代码示例。您还将看到在 Python 代码示例中处理 XML 文档和 JSON 数据的示例。

第一部分包含了 Pandas 中数据可视化的代码示例，例如条形图、面积图和折线图。

第一部分包含了 Pandas 中数据可视化的代码示例，例如条形图、面积图和折线图。

第二部分包含了代码示例，展示了如何编写包含 MySQL 命令的 Python 代码。您还将看到包含 Python 和 Pandas 的代码示例。此外，您将学习如何将 SQL 数据从 Pandas 导出到 Excel 电子表格。

第三部分简要介绍了 XML 和 JSON，以及如何在 Pandas DataFrame 中读取此类数据。此外，还有一个讨论正则表达式的部分。

第四部分展示了如何将 Python 和 SQLite 结合起来执行数据库相关操作，例如在 sqlite3 数据库中创建一个表，然后向该表中插入数据。然后您将学习如何从该表中选择数据，并将这些数据填充到 Pandas DataFrame 中。

最后的部分简要介绍了 Beautiful Soup，并提供了代码示例，展示了如何使用 Beautiful Soup 来解析 HTML 网页。

### **Pandas 和数据可视化**

以下小节包含了基于 Python 的代码示例，这些示例展示了如何使用 Pandas 来渲染以下类型的图表和图形：

+   条形图

+   水平堆叠条形图

+   垂直堆叠条形图

+   非堆叠面积图

+   堆叠面积图

#### **Pandas 和条形图**

列表 4.1 展示了 pandas_barchart.py 的内容，展示了如何在 Pandas 中渲染条形图。

***列表 4.1: pandas_barchart.py***

```py
 import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

df = pd.DataFrame(np.random.rand(16,3), columns=['X1','X2','X3'])
print("First 5 rows:")
print(df.head())
print()

print("Diff of first 5 rows:")
print(df.diff().head())
print()

# bar chart:
ax = df.plot.bar()
plt.show() 
```

列表 4.1 从导入语句开始，然后初始化包含一组数据值的 Pandas DataFrame df1。运行 列表 4.1 中的代码，您将看到以下输出：

```py
 First 5 rows:
         X1        X2        X3
0  0.752462  0.742749  0.950918
1  0.957054  0.836334  0.547507
2  0.022269  0.994618  0.861796
3  0.038466  0.911388  0.545711
4  0.483224  0.468873  0.412120

Diff of first 5 rows:
         X1        X2        X3
0       NaN       NaN       NaN
1  0.204591  0.093585 -0.403411
2 -0.934785  0.158284  0.314289
3  0.016197 -0.083230 -0.316085
4  0.444758 -0.442515 -0.133591 
```

图 4.1 展示了由 列表 4.1 中的代码生成的条形图。

![图片](img/python-3-data-visualization-using-chatgpt-f0113-01.jpg)

***图 4.1*** Pandas 中的条形图。

#### **Pandas 和水平堆叠条形图**

列表 4.2 展示了 pandas_hstacked_bar1.py 的内容，展示了如何在 Pandas 中渲染水平堆叠的条形图。

***列表 4.2: pandas_hstacked_bar1.py***

```py
 import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

df = pd.DataFrame(np.random.rand(16,3), columns=['X1','X2','X3'])
print("First 5 rows:")
print(df.head())
print()

print("Diff of first 5 rows:")
print(df.diff().head())
print()

# horizontal stacked bar chart:
ax = df.plot.barh(stacked=True)
plt.show() 
```

列表 4.2 以导入语句开始，然后使用一组数据值初始化 Pandas DataFrame df1。运行 列表 4.2 中的代码，您将看到以下输出：

```py
 First 5 rows:
         X1        X2        X3
0  0.272391  0.737949  0.617566
1  0.532135  0.234155  0.720543
2  0.500043  0.740288  0.930658
3  0.565021  0.846596  0.379988
4  0.340198  0.063606  0.841024

Diff of first 5 rows:
         X1        X2        X3
0       NaN       NaN       NaN
1  0.259743 -0.503794  0.102977
2 -0.032091  0.506133  0.210115
3  0.064977  0.106308 -0.550671
4 -0.224823 -0.782989  0.461036 
```

图 4.2 显示了由 列表 4.2 中的代码生成的水平堆叠柱状图。

![图片](img/python-3-data-visualization-using-chatgpt-f0114-01.jpg)

***图 4.2*** Pandas 中的水平堆叠柱状图。

#### **Pandas 和垂直堆叠柱状图**

列表 4.3 显示了 pandas_vstacked_bar1.py 的内容，展示了如何在 Pandas 中渲染垂直堆叠柱状图。

***列表 4.3: pandas_vstacked_bar1.py***

```py
 import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

df = pd.DataFrame(np.random.rand(16,3), columns=['X1','X2','X3'])
print("First 5 rows:")
print(df.head())
print()

print("Diff of first 5 rows:")
print(df.diff().head())
print()

# vertical stacked bar chart:
ax = df.plot.bar(stacked=True)
plt.show() 
```

列表 4.3 以导入语句开始，然后使用一组数据值初始化 Pandas DataFrame df1。运行 列表 4.3 中的代码，您将看到以下输出：

```py
 First 5 rows:
         X1        X2        X3
0  0.529936  0.100616  0.683788
1  0.924753  0.320835  0.823198
2  0.925181  0.043236  0.349372
3  0.496390  0.739566  0.759168
4  0.168874  0.241563  0.320381

Diff of first 5 rows:
         X1        X2        X3
0       NaN       NaN       NaN
1  0.394817  0.220219  0.139410
2  0.000428 -0.277599 -0.473826
3 -0.428791  0.696330  0.409796
4 -0.327516 -0.498003 -0.438787 
```

图 4.3 显示了由 列表 4.3 中的代码生成的垂直堆叠柱状图。

![图片](img/python-3-data-visualization-using-chatgpt-f0116-01.jpg)

***图 4.3*** Pandas 中的垂直堆叠柱状图。

#### **Pandas 和非堆叠面积图**

列表 4.4 显示了 pandas_area_nonstacked.py 的内容，展示了如何在 Pandas 中渲染非堆叠面积图。

***列表 4.4: pandas_area_nonstacked.py***

```py
 import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

df = pd.DataFrame(np.random.rand(16,3), columns=['X1','X2','X3'])
print("First 5 rows:")
print(df.head())
print()

print("Diff of first 5 rows:")
print(df.diff().head())
print()

# non-stacked area graph:
ax = df.plot.area(stacked=False)
plt.show() 
```

列表 4.4 以导入语句开始，然后使用一组数据值初始化 Pandas DataFrame df1。运行 列表 4.4 中的代码，您将看到以下输出：

```py
 First 5 rows:
         X1        X2        X3
0  0.347024  0.887191  0.431096
1  0.201923  0.097674  0.521704 2  0.763501  0.516445  0.266348
3  0.055767  0.870355  0.679274
4  0.180045  0.621363  0.152446

Diff of first 5 rows:
         X1        X2        X3
0       NaN       NaN       NaN
1 -0.145101 -0.789517  0.090608
2  0.561577  0.418771 -0.255356
3 -0.707734  0.353910  0.412926
4  0.124278 -0.248992 -0.526828 
```

图 4.4 显示了由 列表 4.4 中的代码生成的非堆叠面积图。

![图片](img/python-3-data-visualization-using-chatgpt-f0117-01.jpg)

***图 4.4*** Pandas 中的非堆叠面积图。

#### **Pandas 和堆叠面积图**

列表 4.5 显示了 pandas_area_stacked.py 的内容，展示了如何在 Pandas 中渲染堆叠面积图。

***列表 4.5: pandas_area_stacked.py***

```py
 import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

df = pd.DataFrame(np.random.rand(16,3), columns=['X1','X2','X3'])
print("First 5 rows:")
print(df.head())
print() print("Diff of first 5 rows:")
print(df.diff().head())
print()

# stacked area graph:
ax = df.plot.area()
plt.show() 
```

列表 4.5 以导入语句开始，然后使用一组数据值初始化 Pandas DataFrame df1。运行 列表 4.5 中的代码，您将看到以下输出：

```py
 First 5 rows:
         X1        X2        X3
0  0.801187  0.635952  0.585165
1  0.776911  0.393118  0.887285
2  0.248293  0.785893  0.409110
3  0.557084  0.402462  0.180559
4  0.201810  0.456198  0.576540

Diff of first 5 rows:
         X1        X2        X3
0       NaN       NaN       NaN
1 -0.024276 -0.242834  0.302120
2 -0.528618  0.392775 -0.478175
3  0.308790 -0.383431 -0.228551
4 -0.355274  0.053737  0.395981 
```

图 4.5 显示了由 列表 4.5 中的代码生成的堆叠面积图。

![图片](img/python-3-data-visualization-using-chatgpt-f0118-01.jpg)

***图 4.5*** Pandas 中的堆叠面积图。

这部分关于 Pandas 和基本图表和图形的章节到此结束。

### **什么是 Fugue？**

Fugue 是一个基于 Python 的库，它允许您通过 FugueSQL 调用对 Pandas DataFrame 的类似 SQL 的查询。使用以下命令安装 Fugue（如果需要，请指定不同的版本）：

```py
 pip3.7 install fugue 
```

列表 4.6 显示了 fugue1.py 的内容，该内容说明了如何填充 Pandas DataFrame，然后调用各种 SQL 命令从 Pandas DataFrame 中检索数据子集。

***列表 4.6: fugue1.py***

```py
 import pandas as pd
from fugue_sql import fsql

df1 = pd.DataFrame({'fnames': ['john', 'dave', 'sara', 'eddy'],
                    'lnames': ['smith','stone','stein','bower'],
                    'ages':   [30,33,34,35],
                    'gender': ['m','m','f','m']})

print("=> DataFrame:")
print(df1)
print()

# Example #1: select users who are older than 33:
query_1 = """
SELECT fnames, lnames, ages, gender FROM df1
WHERE ages > 33
PRINT
"""

# display the extracted data:
fsql(query_1).run() 
```

列表 4.6 以导入语句开始，然后初始化 Pandas DataFrame df1，其中包含一组数据值。接下来，列表 4.6 的下一部分构建了一个查询，用于检索所有年龄大于 33 的用户的数值。运行 列表 4.6 中的代码，你将看到以下输出：

```py
 => DataFrame:
  fnames lnames  ages gender
0   john  smith    30      m
1   dave  stone    33      m
2   sara  stein    34      f
3   eddy  bower    35      m

ANTLR runtime and generated code versions disagree: 4.8!=4.9
ANTLR runtime and generated code versions disagree: 4.8!=4.9
ANTLR runtime and generated code versions disagree: 4.8!=4.9
ANTLR runtime and generated code versions disagree: 4.8!=4.9 PandasDataFrame
fnames:str|lnames:str|ages:long|gender:str
----------+----------+---------+----------
sara      |stein     |34       |f
eddy      |bower     |35       |m
Total count: 2 
```

### **MYSQL、SQLALCHEMY 和 PANDAS**

与 MySQL 数据库交互有几种方式，其中之一是通过 SQLAlchemy。接下来的部分中的 Python 代码示例依赖于 SQLAlchemy（在下一节中简要介绍）和 Pandas。

#### **什么是 SQLAlchemy？**

SQLAlchemy 是一个 ORM（对象关系映射），它作为 Python 代码和数据库之间的“桥梁”。使用以下命令安装 SQLAlchemy：

```py
 pip3 install sqlalchemy 
```

SQLAlchemy 负责将 Python 函数调用转换为适当的 SQL 语句，并提供对自定义 SQL 语句的支持。此外，SQLAlchemy 支持多个数据库，包括 MySQL、Oracle、PostgreSQL 和 SQLite。

#### **通过 SQLAlchemy 读取 MySQL 数据**

前一节展示了如何安装 SQLAlchemy，以及安装 Pandas（如果你还没有安装的话）的命令：

```py
 pip3 install pandas 
```

代码示例中的 Pandas 功能涉及直观命名的 read_sql() 方法和相关 read_sql_query() 方法，这两个方法都用于读取 MySQL 表的内容。

列表 4.7 显示了读取 people 表内容的 read_sql_data.py 的内容。

***列表 4.7：read_sql_table.py***

```py
 from sqlalchemy import create_engine
import pymysql
import pandas as pd

engine = create_engine('mysql+pymysql://root:yourpassword@
127.0.0.1',pool_recycle=3600)
dbConn = engine.connect()
frame  = pd.read_sql("select * from mytools.people", dbConn);

pd.set_option('display.expand_frame_repr', False)
print(frame)
dbConn.close() 
```

列表 4.7 以几个导入语句开始，这些导入语句是访问 MySQL 数据库所必需的。接下来，代码的下一部分初始化变量 engine 作为对 MySQL 的引用，然后是 dbConn（数据库连接）。接下来，变量 frame 被初始化为 people 表的行。在命令行中运行以下命令：

```py
python3 read_sql_table.py

```

你将看到前面命令生成的以下输出：

```py
 fname  lname age gender  country
0  john  smith  30      m      usa
1  jane  smith  31      f   france
2  jack  jones  32      m   france
3  dave  stone  33      m    italy
4  sara  stein  34      f  germany
5  eddy  bower  35      m    spain 
```

列表 4.8 显示了读取 people 表内容的 sql_query.py 的内容。

***列表 4.8：sql_query.py***

```py
 from sqlalchemy import create_engine
import pymysql
import pandas as pd
engine = create_engine('mysql+pymysql://root:yourpassword@
127.0.0.1',pool_recycle=3600)

query_1 = '''
select * from mytools.people
'''

print("create dataframe from table:")
df_2 = pd.read_sql_query(query_1, engine)

print("dataframe:")
print(df_2) 
```

列表 4.8 以几个导入语句开始，随后初始化变量 engine 作为对 MySQL 实例的引用。接下来，变量 query_1 被定义为字符串变量，指定一个 SQL 语句，该语句选择 people 表的所有行，然后是变量 df_2（一个数据框），它返回执行变量 query_1 中指定的 SQL 语句的结果。最后的代码片段显示了 people 表的内容。在命令行中运行以下命令：

```py
 python3 sql_query.py 
```

你将看到前面命令生成的以下输出：

```py
 fname  lname age gender  country
0  john  smith  30      m      usa
1  jane  smith  31      f   france
2  jack  jones  32      m   france
3  dave  stone  33      m    italy
4  sara  stein  34      f  germany
5  eddy  bower  35      m    spain 
```

在命令行中运行以下 Python 脚本：

```py
 python3 sql_query.py 
```

你将看到前面命令生成的以下输出：

```py
 fname  lname age gender  country
0  john  smith  30      m      usa
1  jane  smith  31      f   france
2  jack  jones  32      m   france
3  dave  stone  33      m    italy
4  sara  stein  34      f  germany
5  eddy  bower  35      m    spain 
```

### **从 Pandas 导出 SQL 数据到 Excel**

列表 4.9 显示了 sql_query_excel.py 的内容，该文件将 people 表的内容读入 Pandas DataFrame，然后将其导出到 Excel 文件。

***列表 4.9: sql_query_excel.py***

```py
 from sqlalchemy import create_engine
import pymysql
import pandas as pd

engine = create_engine('mysql+pymysql://root:yourpassword@
127.0.0.1/',pool_recycle=3600)

query_1 = '''
select * from mytools.people
'''

print("create dataframe from table:")
df_2 = pd.read_sql_query(query_1, engine)

print("Contents of Pandas dataframe:")
print(df_2)

import openpyxl
print("saving dataframe to people.xlsx")
df_2.to_excel('people.xlsx', index=False) 
```

列表 4.9 包含几个导入语句，随后是变量 engine，它初始化为可以从其中访问 MySQL 数据库的“端点”。下一个代码片段初始化变量 query_1 为一个包含简单 SQL SELECT 语句的字符串。

接下来，变量 df_2 是一个 Pandas DataFrame，它初始化为调用变量 query_1 中定义的 SQL 语句的结果，之后显示 df_2 的内容。代码 列表 4.9 的最后一部分将 df_2 的内容保存到名为 people.xlsx 的 Excel 文档中。在命令行中启动以下命令：

```py
 python3 sql_query_excel.py 
```

上述命令将生成以下输出：

```py
 Creating dataframe from table people
Contents of Pandas dataframe:
   fname  lname age gender  country
0   john  smith  30      m      usa
1   jane  smith  31      f   france
2   jack  jones  32      m   france
3   dave  stone  33      m    italy
4   sara  stein  34      f  germany
.. ... ... .. ... ... 73  jane  smith  31      f   france
74  jack  jones  32      m   france
75  dave  stone  33      m    italy
76  sara  stein  34      f  germany
77  eddy  bower  35      m    spain

[78 rows x 5 columns]
saving dataframe to people.xlsx 
```

**注意** *你可能需要使用 Python 3.7 而不是 Python 3.8 或 Python 3.9 来启动前面的 Python 脚本*。

下一个部分包含与 Pandas 相关的功能，但不涉及任何数据库连接。由于本章的前一部分包含与 Pandas 相关的功能，这是一个方便的位置来放置这些材料。然而，如果你愿意，你可以跳过这一部分，不会影响连续性，并继续下一部分，该部分讨论 SQLite。

### **MYSQL 和 CONNECTOR/PYTHON**

MySQL 提供了一个连接器/Python API 作为连接到 MySQL 数据库的另一种机制。本节包含一些简单的 Python 代码示例，这些示例依赖于连接器/Python 来连接到数据库并从数据库表中检索行。

在深入研究代码示例之前，请记住 MySQL 8 使用 mysql_native_password 而不是 caching_sha2_password。因此，你需要为 auth_plugin 指定一个值（这在各种在线代码示例中并未指定）。以下是错误信息：

```py
 mysql.connector.errors.NotSupportedError: Authentication
plugin 'caching_sha2_password' is not supported 
```

解决方案将在下一节的 Python 代码示例中突出显示。

#### **建立数据库连接**

列表 4.10 显示了 mysql_conn1.py 的内容，该文件说明了如何建立连接器/Python 数据库连接。

***列表 4.10: mysql_conn1.py***

```py
 import mysql.connector

cnx = mysql.connector.connect(user='root',
                              password='yourpassword',
                              host='localhost',
                              database='employees', auth_plugin='mysql_native_password')
cnx.close() 
```

列表 4.10 包含一个导入语句，用于设置 Python 3.9 的适当路径。如果代码在你的系统上执行正确，没有这两行代码，那么你可以安全地删除它们。

下一个代码片段是一个导入语句，随后初始化变量 cnx 作为数据库连接。注意下面用粗体显示的片段，这是为了连接到 MySQL 数据库所必需的，正如本节引言部分所述。在 列表 4.10 中启动代码，如果你没有看到任何错误信息，那么代码已经正确执行。

#### **从数据库表读取数据**

列表 4.11 显示了 mysql_pandas.py 的内容，说明了如何建立数据库连接并检索数据库表中的行。

***列表 4.11: mysql_pandas.py***

```py
 import mysql.connector

mydb = mysql.connector.connect(user='root',
                              password='yourpassword',
                              host='localhost',
                              database='employees', auth_plugin='mysql_native_password')

mycursor = mydb.cursor()

# select all rows from the employees table:
mycursor.execute('SELECT * FROM employees') import pandas as pd

# populate a Pandas data frame with the data:
table_rows = mycursor.fetchall()
df = pd.DataFrame(table_rows)

print("data frame:")
print(df)

mydb.close() 
```

列表 4.11 以与 列表 4.10 相同的导入语句和相同的目的开始。下一个代码片段是一个导入语句，然后初始化变量 cnx 作为数据库连接。注意以下粗体显示的片段，这是连接到 MySQL 数据库所需的 MySQL 8 的要求。在 列表 4.11 中运行代码，如果一切正常，你将看到以下输出：

```py
 => Contents of data frame:
      0     1                   2
0  1000  2000           Developer
1  2000  3000        Project Lead
2  3000  4000         Dev Manager
3  4000  4000  Senior Dev Manager 
```

#### **创建数据库表**

列表 4.12 显示了 create_fun_table.py 的内容，说明了如何建立数据库连接并创建数据库表。

***列表 4.12: create_fun_table.py***

```py
 my_table = (
    "CREATE TABLE 'for_fun' ("
    "  'dept_no' char(4) NOT NULL,"
    "  'dept_name' varchar(40) NOT NULL,"
    "  PRIMARY KEY ('dept_no'), UNIQUE KEY 'dept_name' ('dept_name')"
    ") ENGINE=InnoDB")

DB_NAME = 'for_fun_db'

import mysql.connector
cnx = mysql.connector.connect(user='root',
                              password='yourpassword',
                              host='localhost',
                              database='mytools')
cursor = cnx.cursor()

try:
  print("Creating table {}: ".format(my_table), end='')
  cursor.execute(my_table)
except mysql.connector.Error as err:
  if err.errno == errorcode.ER_TABLE_EXISTS_ERROR:
    print("already exists.")
  else: print(err.msg)
else:
  print("Table created:",my_table)

cursor.close()

cnx.close() 
```

列表 4.12 开始时初始化变量 my_table 为一个包含创建 MySQL 表的 SQL 语句的字符串。列表 4.12 的下一部分初始化变量 cnx 为 mytools 数据库的连接，然后初始化变量 cursor 为数据库游标。

列表 4.12 的下一部分包含一个 try/catch 块，用于创建在字符串变量 my_table 中指定的 for_fun 表。except 块捕获连接相关错误，并在发生错误（因为指定的表已存在或由于其他原因）时显示适当的消息。

在 列表 4.12 中运行代码，如果一切正常，你将看到以下输出：

```py
 Creating table CREATE TABLE 'for_fun' (  'dept_no' char(4)
NOT NULL,  'dept_name' varchar(40) NOT NULL,  PRIMARY
KEY ('dept_no'), UNIQUE KEY 'dept_name' ('dept_name'))
ENGINE=InnoDB: Table created: CREATE TABLE 'for_fun' (
'dept_no' char(4) NOT NULL,  'dept_name' varchar(40) NOT
NULL,  PRIMARY KEY ('dept_no'), UNIQUE KEY 'dept_name'
('dept_name')) ENGINE=InnoDB 
```

现在打开一个命令行界面，从 MySQL 提示符输入以下命令：

```py
 MySQL [mytools]> desc for_fun;
+-----------+-------------+------+-----+---------+-------+
| Field     | Type        | Null | Key | Default | Extra |
+-----------+-------------+------+-----+---------+-------+
| dept_no   | char(4)     | NO   | PRI | NULL    |       |
| dept_name | varchar(40) | NO   | UNI | NULL    |       |
+-----------+-------------+------+-----+---------+-------+ 2 rows in set (0.060 sec)

```

### **将 Pandas 数据写入 MySQL 表**

列表 4.13 显示了 pandas_write_sql.py 的内容，展示了如何将 Pandas DataFrame 中的数据写入 MySQL 表。

***列表 4.13: pandas_write_sql.py***

```py
 import pandas as pd

data = pd.DataFrame({ 'book_id':[12345, 12346, 12347],
    'title':['Python Programming', 'Learn MySQL', 'Data Science Cookbook'],
    'price':[29, 23, 27]
})

import mysql.connector

mydb = mysql.connector.connect (
        host="localhost",
        user="root",
        password="os1wald123",
        database = "mytools",
        auth_plugin='mysql_native_password'
       )

from sqlalchemy import create_engine

engine = create_engine('mysql+pymysql://root:os1wald123@127.0.0.1:3306/mytools',pool_recycle=3600)
dbConn = engine.connect()

# The to_sql writes data into the book_details table:
data.to_sql('book_details', engine, if_exists='append', index=False)

df = pd.read_sql("SELECT * FROM book_details", dbConn);
pd.set_option('display.expand_frame_repr', False)
print("Rows from book_details table:")
print(df)
dbConn.close() 
```

列表 4.13 开始时初始化变量 data 为一个包含数据值的 Pandas DataFrame，然后是变量 mydb，它被初始化为数据库连接的一个实例。

列表 4.13 的下一部分实例化了变量 engine 和在向数据库写入数据时将被调用的变量 dbConn。接下来，变量 data 调用其 to_sql() 方法，该方法还指定了表 book_details、engine 变量，并且如果表已存在，则使用追加模式到数据库。

列表 4.13 的最后一部分将变量 df 填充为 book_details 表中的所有数据，然后在关闭数据库连接之前显示其内容。现在再次在 列表 4.13 中运行代码，如果一切正常，你将看到以下输出：

```py
 Rows from book_details table:
   book_id                  title  price
0    12345     Python Programming     29
1    12346            Learn MySQL     23
2    12347  Data Science Cookbook     27 
```

导航到 MySQL 提示符并输入以下语句：

```py
 mysql> use mytools;
Database changed mysql> desc book_details;
+---------+--------+------+-----+---------+-------+
| Field   | Type   | Null | Key | Default | Extra |
+---------+--------+------+-----+---------+-------+
| book_id | bigint | YES  |     | NULL    |       |
| title   | text   | YES  |     | NULL    |       |
| price   | bigint | YES  |     | NULL    |       |
+---------+--------+------+-----+---------+-------+
3 rows in set (0.00 sec)

mysql> select * from book_details;
+---------+-----------------------+-------+
| book_id | title                 | price |
+---------+-----------------------+-------+
|   12345 | Python Programming    |    29 |
|   12346 | Learn MySQL           |    23 |
|   12347 | Data Science Cookbook |    27 |
+---------+-----------------------+-------+
3 rows in set (0.00 sec) 
```

现在再次在 列表 4.13 中运行代码，并再次执行前面的 SQL 语句：

```py
 mysql> select * from book_details;
+---------+-----------------------+-------+
| book_id | title                 | price |
+---------+-----------------------+-------+
|   12345 | Python Programming    |    29 |
|   12346 | Learn MySQL           |    23 |
|   12347 | Data Science Cookbook |    27 |
|   12345 | Python Programming    |    29 |
|   12346 | Learn MySQL           |    23 |
|   12347 | Data Science Cookbook |    27 |
+---------+-----------------------+-------+
6 rows in set (0.00 sec) 
```

如您所见，现在 book_details 表中有 6 只乌鸦。插入相同三行数据的原因是以下 SQL 语句中的 append 值：

```py
 data.to_sql('book_details', engine, if_exists='append', index=False) 
```

本章关于 Pandas 和 MySQL 的部分到此结束。下一节将向您介绍 SQLite，它是一种可在多个平台上使用的 RDBMS。

### **在 Pandas 中读取 XML 数据**

列表 4.14 展示了 books.xml 的内容，列表 4.15 展示了 pandas_read_xml.py 的内容，该文件展示了如何在 Pandas 中读取 XML 文档的内容。

***列表 4.14: books.xml***

```py
 <?xml version="1.0" encoding="UTF-8"?>
<books>
  <book>
   <name>SQL Fundamentals</name>
  </book>
  <book>
   <name>SVG Fundamentals</name>
  </book>
  <book>
   <name>Python and Machine Learning</name>
  </book>
</books> 
```

***列表 4.15: pandas_read_xml.py***

```py
 # this code might require Python3.7
import pandas as pd

filename="books.xml"

df = pd.read_xml(filename)
print("XML data:")
print(df) 
```

列表 4.15 首先使用现有 XML 文档的名称初始化变量，然后调用 Pandas 的 read_xml() 方法，将 XML 文档中的数据填充到变量 df 中，之后打印 df 的内容。现在运行 列表 4.15 中的代码，如果一切正常，您将看到以下输出：

```py
 Rows from book_details table:

XML data:
               name
0  SQL Fundamentals
1  SVG Fundamentals
2  Python and Machine Learning 
```

### **在 Pandas 中读取 JSON 数据**

列表 4.16 展示了 pandas_read_json.py 的内容，该文件展示了如何在 Pandas 中读取 JSON 字符串。

***列表 4.16: pandas_read_json.py***

```py
 from io import StringIO
import pandas as pd

books =  '{"name": "SQL Fundamentals"}\n{"name": "SQL Fundamentals"}\n{"name": "Python and Machine Learning"}\n' json = StringIO(books)
result = pd.read_json(json, lines=True)

print("json:",result) 
```

列表 4.16 以两个导入语句开始，然后使用名称/值对的字符串初始化变量 books。接下来，变量 json 被初始化为基于 books 内容的 JSON 字符串。然后通过调用 Pandas 的 read_json() 方法并使用变量 json 初始化变量 result，之后打印其内容。现在运行 列表 4.16 中的代码，如果一切正常，您将看到以下输出：

```py
 XML data:
               name
0  SQL Fundamentals
1  SVG Fundamentals
2  Python and Machine Learning 
```

列表 4.17 展示了 books.json 的内容，列表 4.18 展示了 pandas_read_json.py 的内容，该文件展示了如何在 Pandas 中读取 JSON 文件的内容。

***列表 4.17: books.json***

```py
 [
{"name": "SQL Fundamentals"},
{"name": "SQL Fundamentals"},
{"name": "Python and Machine Learning"}
] 
```

***列表 4.18: pandas_read_json2.py***

```py
 import pandas as pd

filename="books.json"

df = pd.read_json(filename)
print("JSON data:")
print(df.to_string()) 
```

列表 4.18 与 列表 4.16 类似，但这次没有使用 StringIO，而是通过调用 to_string() 方法打印 DataFrame df 的内容。现在运行 列表 4.18 中的代码，如果一切正常，您将看到以下输出：

```py
 JSON data:
               name
0  SQL Fundamentals
1  SVG Fundamentals
2  Python and Machine Learning 
```

### **处理基于 JSON 的数据**

一个 JSON 对象由冒号分隔的名称/值对组成，数据对象由逗号分隔。对象用大括号 {} 括起来，对象数组用方括号 [] 表示。请注意，字符值数据元素位于一对双引号 "" 内（但数值数据不需要引号）。

这里是一个简单的 JSON 对象示例：

```py
 { "fname":"Jane", "lname":"Smith", "age":33, "city":"SF" } 
```

这里是一个简单的 JSON 对象数组示例（注意外层括号）：

```py
 [
{ "fname":"Jane", "lname":"Smith", "age":33, "city":"SF" },
{ "fname":"John", "lname":"Jones", "age":34, "city":"LA" },
{ "fname":"Dave", "lname":"Stone", "age":35, "city":"NY" },
] 
```

#### **Python 字典和 JSON**

Python 的 json 库使您能够在 Python 中处理基于 JSON 的数据。

列表 4.19 显示 dict2json.py 的内容，该内容说明了如何将 Python 字典转换为 JSON 字符串。

***列表 4.19: dict2json.py***

```py
 import json

dict1 = {}
dict1["fname"] = "Jane"
dict1["lname"] = "Smith"
dict1["age"]   = 33
dict1["city"]  = "SF"

print("Python dictionary to JSON data:")
print("dict1:",dict1)
json1 = json.dumps(dict1, ensure_ascii=False)
print("json1:",json1)
print("")

# convert JSON string to Python dictionary:
json2 = '{"fname":"Dave", "lname":"Stone", "age":35, "city":"NY"}'
dict2 = json.loads(json2)
print("JSON data to Python dictionary:")
print("json2:",json2)
print("dict2:",dict2) 
```

列表 4.19 调用 json.dumps() 函数将 Python 字典转换为 JSON 字符串。运行列表 4.19 中的代码，你会看到以下输出：

```py
Python dictionary to JSON data:
dict1: {'fname': 'Jane', 'lname': 'Smith', 'age': 33, 'city': 'SF'}
json1: {"fname": "Jane", "lname": "Smith", "age": 33, "city": "SF"}

JSON data to Python dictionary:
json2: {"fname":"Dave", "lname":"Stone", "age":35, "city":"NY"}
dict2: {'fname': 'Dave', 'lname': 'Stone', 'age': 35, 'city': 'NY'} 
```

#### **Python、Pandas 和 JSON**

列表 4.20 显示 pd_python_json.py 的内容，该内容说明了如何将 Python 字典转换为 Pandas DataFrame，然后将 DataFrame 转换为 JSON 字符串。

***列表 4.20: pd_python_json.py***

```py
 import json
import pandas as pd

dict1 = {}
dict1["fname"] = "Jane"
dict1["lname"] = "Smith"
dict1["age"]   = 33
dict1["city"]  = "SF"

df1 = pd.DataFrame.from_dict(dict1, orient='index')
print("Pandas df1:")
print(df1)
print()

json1 = json.dumps(dict1, ensure_ascii=False)
print("Serialized to JSON1:")
print(json1)
print()

print("Data frame to JSON2:")
json2 = df1.to_json(orient='split')
print(json2) 
```

列表 4.20 使用多个属性（如名字、姓氏等）初始化 Python 字典 dict1。接下来，从 Python 字典 dict1 创建 DataFrame df1，并显示其内容。

下一个部分 列表 4.20 初始化变量 json1，通过序列化 dict1 的内容，并显示其内容。列表 4.20 中的最后一个代码块将变量 json2 初始化为将 DataFrame df1 转换为 JSON 字符串的结果。运行列表 4.20 中的代码，你会看到以下输出：

```py
 dict1: {'fname': 'Jane', 'lname': 'Smith', 'age': 33, 'city': 'SF'} Pandas df1:
           0
fname   Jane
lname  Smith
age       33
city      SF

Serialized to JSON1:
{"fname": "Jane", "lname": "Smith", "age": 33, "city": "SF"}

Data frame to JSON2:
{"columns":[0],"index":["fname","lname","age","city"],"data":[["Jane"],["Smith"],[33],["SF"]]}
json1: {"fname": "Jane", "lname": "Smith", "age": 33, "city": "SF"} 
```

### **PANDAS 和 正则表达式（可选）**

这一节被标记为“可选”，因为代码片段需要理解正则表达式。如果你还没有准备好学习正则表达式，你可以跳过这一节而不会影响连续性。

列表 4.21 显示 pandas_regexs.py 的内容，该内容说明了如何使用正则表达式从 Pandas DataFrame 中提取数据。

***列表 4.21: pandas_regexs.py***

```py
 import pandas as pd

schedule = ["Monday: Prepare lunch at 12:30pm for VIPs",
            "Tuesday: Yoga class from 10:00am to 11:00am",
            "Wednesday: PTA meeting at library at 3pm",
            "Thursday: Happy hour at 5:45 at Julie's house.",
            "Friday: Prepare pizza dough for lunch at 12:30pm.",
            "Saturday: Early shopping for the week at 8:30am.",
            "Sunday: Neighborhood bbq block party at 2:00pm."]
# create a Pandas DataFrame:
df = pd.DataFrame(schedule, columns = ['dow_of_week'])
# convert to lowercase:
df = df.applymap(lambda s:s.lower() if type(s) == str else s)
print("df:")
print(df)
print()

# character count for each string in df['dow_of_week']:
print("string lengths:")
print(df['dow_of_week'].str.len())
print()

# the number of tokens for each string in df['dow_of_week']
print("number of tokens in each string in df['dow_of_week']:") print(df['dow_of_week'].str.split().str.len())
print()

# the number of occurrences of digits:
print("number of digits:")
print(df['dow_of_week'].str.count(r'\d'))
print()

# display all occurrences of digits:
print("show all digits:")
print(df['dow_of_week'].str.findall(r'\d'))
print()

# display hour and minute values:
print("display (hour, minute) pairs:")
print(df['dow_of_week'].str.findall(r'(\d?\d):(\d\d)'))
print()

# create new columns from hour:minute value:
print("hour and minute columns:")
print(df['dow_of_week'].str.extract(r'(\d?\d):(\d\d)'))
print() 
```

列表 4.21 初始化变量 schedule，其中包含一组字符串，每个字符串指定一周中每天的任务。每个任务项的格式为 day:task，其中 day 是一周中的某一天，task 是一个字符串，指定了该特定天需要完成的事情。

接下来，DataFrame df1 被初始化为 schedule 的内容，然后是一个定义将基于字符串的值转换为小写的 lambda 表达式的示例，如下所示：

```py
 df = df.applymap(lambda s:s.lower() if type(s) == str else s) 
```

上述代码片段很有用，因为你不需要指定 DataFrame 的单个列：代码会忽略任何非字符串值（例如整数和浮点值）。

下一个代码块涉及使用 applymap()、split() 和 len() 方法进行各种操作，这些方法你在之前的示例中已经见过。下一个代码块通过以下代码片段中的正则表达式显示每个任务项中的数字个数：

```py
 print(df['dow_of_week'].str.count(r'\d')) 
```

下一个代码块通过以下代码片段中的正则表达式显示每个任务项中的实际数字（而不是数字个数）：

```py
print(df['dow_of_week'].str.findall(r'\d')) 
```

最后一个代码块通过以下代码片段中的正则表达式显示形式为 hour:minutes 的字符串：

```py
 print(df['dow_of_week'].str.findall(r'(\d?\d):(\d\d)')) 
```

如本节开头所述，你可以通过阅读本书的一个附录来了解更多关于正则表达式的信息。启动列表 4.21 中的代码，你将看到以下输出：

```py
 => df:
                                         dow_of_week
0          monday: prepare lunch at 12:30pm for vips
1        tuesday: yoga class from 10:00am to 11:00am
2           wednesday: pta meeting at library at 3pm
3     thursday: happy hour at 5:45 at julie's house. 4  friday: prepare pizza dough for lunch at 12:30pm. 5   saturday: early shopping for the week at 8:30am. 6    sunday: neighborhood bbq block party at 2:00pm. => string lengths:
0    41
1    43
2    40
3    46
4    49
5    48
6    47
Name: dow_of_week, dtype: int64

=> number of tokens in each string in df['dow_of_week']:
0    7
1    7
2    7
3    8
4    8
5    8
6    7
Name: dow_of_week, dtype: int64
=> number of digits:
0    4
1    8
2    1
3    3
4    4
5    3
6    3
Name: dow_of_week, dtype: int64

=> show all digits:
0                [1, 2, 3, 0]
1    [1, 0, 0, 0, 1, 1, 0, 0]
2                         [3] 3                   [5, 4, 5]
4                [1, 2, 3, 0]
5                   [8, 3, 0]
6                   [2, 0, 0]
Name: dow_of_week, dtype: object

=> display (hour, minute) pairs:
0              [(12, 30)]
1    [(10, 00), (11, 00)]
2                      []
3               [(5, 45)]
4              [(12, 30)]
5               [(8, 30)]
6               [(2, 00)]
Name: dow_of_week, dtype: object

=> hour and minute columns:
     0    1
0   12   30
1   10   00
2  NaN  NaN
3    5   45
4   12   30
5    8   30
6    2   00 
```

### **什么是 SQLite？**

SQLite 是一个轻量级、便携式和开源的关系型数据库管理系统，可在 Windows、Linux、MacOS 以及 Android 和 iOS 上使用。官方网站在此：

[*https://www.sqlite.org*](https://www.sqlite.org)

这里你可以找到一些最常用 SQLite 命令的教程：

*[`www.sqlitetutorial.net/sqlite-commands/`](https://www.sqlitetutorial.net/sqlite-commands/)*

此外，SQLite 符合 ACID 规范，并实现了大多数 SQL 标准。让我们看看 SQLite 的一些功能和安装过程，这两者都在两个小节中进行了讨论。

#### **SQLite 功能**

SQLite 提供了一些有用的功能，其中一些如下所示：

+   不需要单独的服务器进程或系统来运行

+   无需系统管理

+   无外部依赖

+   可以在无服务器环境中运行。

+   可在多个平台（Unix、Linux、Mac、Windows）上使用

+   ACID 事务

+   完全支持 SQL92 的所有功能

#### **SQLite 安装**

导航到以下网站并下载适用于您操作系统的发行版：

*[`www.sqlite.org/download.html`](https://www.sqlite.org/download.html)*

第二步是将下载的文件解压到方便的位置，我们假设这个位置是$HOME/sqlite3_home 目录。

注意，如果你有一台 MacBook，那么包含 sqlite3 可执行文件的目录会自动包含在 PATH 变量中。为了确保这一点，请输入以下命令以查看 sqlite3 是否可访问：

```py
 which sqlite3 
```

如果前面的命令返回一个空行，那么你需要包含 sqlite3 所在的 bin 目录的路径。例如，如果前面的目录是$HOME/sqlite3_home/bin，那么更新 PATH 环境变量如下：

```py
 export PATH=/$HOME/sqlite_home/bin:$PATH 
```

#### **创建数据库和表**

以下命令序列展示了如何启动 sqlite 并创建一个名为 test.db 的数据库：

```py
 $ sqlite3 test.db SQLite version 3.28.0 2019-04-15 14:49:49
Enter ".help" for usage hints. sqlite>
sqlite> .help .auth ON|OFF             Show authorizer callbacks
.backup ?DB? FILE        Backup DB (default "main") to FILE
.bail on|off             Stop after hitting an error. Default OFF
.binary on|off           Turn binary output on or off. Default OFF
.cd DIRECTORY            Change the working directory to DIRECTORY
.changes on|off          Show number of rows changed by SQL
// details omitted for brevity
.trace ?OPTIONS? Output each SQL statement as it is run
.vfsinfo ?AUX? Information about the top-level VFS
.vfslist                 List all available VFSes
.vfsname ?AUX? Print the name of the VFS stack
.width NUM1 NUM2 ... Set column widths for "column" mode sqlite> .databases databases
main: /tmp/test.db
sqlite> .quit List the files in the current directory and you will see the following:
-rw-r--r--   1 oswaldcampesato  staff        0 Aug  5 10:36 test.db 
```

现在通过执行以下命令序列在 sqlite3 中创建一个名为 books 的表：

```py
 $ sqlite3 test.db SQLite version 3.28.0 2019-04-15 14:49:49
Enter ".help" for usage hints. sqlite>
sqlite> CREATE TABLE books(author text, title text, year integer, price real); sqlite> .tables books
sqlite> select * from books; sqlite> # insert data later
sqlite>
sqlite> .quit

```

#### **插入、选择和删除表数据**

以下命令序列展示了如何在名为“test.db”的数据库中与 books 表进行数据相关操作：

```py
 $ sqlite3 test.db SQLite version 3.28.0 2019-04-15 14:49:49
Enter ".help" for usage hints. sqlite> INSERT INTO books(author, title, year, price)
VALUES ("John Doe", "Unix Tips", "2020", "34.95"); sqlite> select * from books; John Doe|Unix Tips|2020|34.95
sqlite> delete from books; sqlite> select * from books; sqlite>
sqlite> .tables books
sqlite> drop table books;
sqlite>
sqlite> .quit

```

#### **启动 SQL 文件**

列表 4.22 显示了 create_table.sql 的内容，列表 4.23 显示了 insert_data.sql 的内容。

***列表 4.22：create_table.sql***

```py
 CREATE TABLE books2(author text, title text, year integer, price real); 
```

***列表 4.23：insert_data.sql***

```py
 INSERT INTO books2(author, title, year, price)
VALUES ("Oswald Campesato", "C Programming", "2018", "35.95"); 
```

按以下方式启动前面的 SQL 文件：

```py
 sqlite3 test.db < create_table.sql
sqlite3 test.db < insert_data.sql 
```

让我们回到 sqlite3 提示符，检查 books2 表的结构及其内容：

```py
 $ sqlite3 test.db SQLite version 3.28.0 2019-04-15 14:49:49
Enter ".help" for usage hints. sqlite>
sqlite> .schema books2 CREATE TABLE books2(author text, title text, year integer, price real);
sqlite> select * from books2; Oswald Campesato|C Programming|2018|35.95 
```

#### **删除表和数据库**

```py
 $ sqlite3 test.db SQLite version 3.28.0 2019-04-15 14:49:49
Enter ".help" for usage hints. sqlite>
sqlite> drop table books2; sqlite> .tables sqlite>
$ sqlite3 test.db SQLite version 3.28.0 2019-04-15 14:49:49
Enter ".help" for usage hints. sqlite>
sqlite> .tables
sqlite>
sqlite> .quit

```

现在通过 bash rm 命令删除数据库 test.db，如下所示：

```py
 rm test.db
sqlite> .quit

```

#### **将 CSV 数据加载到 sqlite 表中**

列表 4.24 展示了包含 65 行数据的 rainfall.csv 的内容，列表 4.25 展示了 load_rainfall.sql 的内容。

***列表 4.24: rainfall.csv***

```py
 CREATE
2023-01-02,0
2023-01-03,1
2023-01-04,0
2023-01-05,2
2023-01-06,3
// details omitted for brevity
2023-03-27,60
2023-03-28,29
2023-03-29,26
2023-03-30,44
2023-03-31,8 
```

***列表 4.25: load_rainfall.sql***

```py
 DROP TABLE IF EXISTS rainfall;
CREATE TABLE rainfall ( "day" TEXT, "centimeters" REAL);

.mode csv
.import rainfall.csv rainfall 
```

列表 4.25 如果 rainfall 表已存在，则删除该表，然后创建具有文本列和名为 day 和 centimeters 的实值列的 rainfall 表。现在运行 列表 4.25 中的代码，然后导航到 sqlite3 提示符以检查 rainfall 表中的行数：

```py
sqlite3 mytools.db SQLite version 3.28.0 2019-04-15 14:49:49
Enter ".help" for usage hints. sqlite> select count(*) from rainfall; 65
sqlite> .quit

```

在下一节中，您将学习如何编写用于管理 sqlite3 中数据的 Python 代码，并学习如何从 rainfall 表中提取数据以使用 Pandas 生成直方图。

### **PYTHON 和 SQLITE**

本节包含了一系列 Python 文件，展示了如何在 sqlite3 中执行各种操作，这些操作是对您从 sqlite3 提示符中学到的示例的补充。请注意，Python 代码示例使用 mytools.db 数据库而不是 test.db 数据库。

#### **连接到 sqlite3 数据库**

列表 4.26 展示了 connect_db.py 的内容，该文件展示了如何在 Python 中连接到 sqlite3 数据库。

***列表 4.26: connect_db.py***

```py
 import sqlite3

con = sqlite3.connect("mytools.db")
cursor = con.cursor()
con.commit()
con.close() 
```

列表 4.26 是一个“什么也不做”的 Python 代码示例，它只是简单地连接到 mytools.db 数据库。

#### **在 sqlite3 数据库中创建表**

列表 4.27 展示了 connect_db.py 的内容，该文件展示了如何在 Python 中连接到 sqlite3 数据库。

***列表 4.27: create_table.py***

```py
 import sqlite3

con = sqlite3.connect("mytools.db")
cursor = con.cursor()

cursor.execute(
  CREATE TABLE books(author text, title text, year integer, price real);
)

con.commit()
con.close() 
```

列表 4.27 创建了一个游标并执行了 SQL 创建语句，以便在 mytools.db 数据库中创建名为 books 的表。

#### **在 sqlite3 表中插入数据**

列表 4.28 展示了 insert_data.py 的内容，该文件展示了如何在 Python 中向 sqlite3 表中插入数据。

***列表 4.28: insert_data.py***

```py
 import sqlite3

con = sqlite3.connect("mytools.db")
cursor = con.cursor()

sql = """ INSERT INTO books(author, title, year, price)
          VALUES ("Tom Smith", "Intro to TypeScript", "2022", "39.95") """

cursor.execute(sql)

con.commit()
con.close() 
```

列表 4.28 创建了一个游标并执行了 SQL 插入语句，以便在 mytools.db 数据库中的 books 表中插入数据。

#### **从 sqlite3 表中选择数据**

列表 4.29 展示了 select_data.py 的内容，该文件展示了如何在 Python 中向 sqlite3 表中插入数据。

***列表 4.29: select_data.py***

```py
 import sqlite3

con = sqlite3.connect("mytools.db")
cursor = con.cursor()

sql = """ SELECT * FROM books; """

cursor.execute(sql)

row_count = 0
all_rows = cursor.fetchall()

print("Contents of table books:")
for row in all_rows:
  row_count += 1
  print("row:",row)

con.commit()
con.close()

print("row count:",row_count)
print() 
```

列表 4.29 创建了一个游标并执行了 SQL 选择语句，以便从 mytools.db 数据库中的 books 表中选择数据。在 列表 4.29 的下一部分中，初始化变量 all_rows 作为 books 表中数据的引用，然后是一个循环，遍历 all_rows 中的元素并打印它们的内容。请注意，最后的代码片段显示了 books 表中的行数。

#### **从 sqlite3 表中填充 Pandas 数据框**

列表 4.30 显示了 read_sqlite3_into_pandas.py 的内容，展示了如何在 Python 中使用 sqlite3 表的数据填充 Pandas DataFrame。

***列表 4.30：read_sqlite3_into_pandas.py***

```py
 import sqlite3
import pandas as pd

con = sqlite3.connect("mytools.db")
df = pd.read_sql_query("SELECT * FROM books;", con)
con.close()

print("=> Contents of book table:")
print(df) 
```

列表 4.30 创建了一个游标，然后执行 SQL select 语句以从 mytools.db 数据库中的 books 表中选择数据。列表 4.30 的下一部分通过调用 Pandas 方法 read_sql_query() 初始化 df，其中包含 books 表的内容。列表 4.30 中的下一代码片段显示了 Pandas DataFrame df 的内容。运行 列表 4.30 中的代码，你将看到以下输出：

```py
 => Contents of book table:
      author                title  year  price
0   John Doe            Unix Tips  2020  34.95
1   Oswald C        C Programming  2018  35.95
2  Tom Smith  Intro to TypeScript  2022  39.95 
```

虽然你可以像使用 MySQL 一样从命令行执行 SQL 操作，但使用 IDE 与 SQLite 一起工作可能更容易。事实上，一个非常强大的 IDE 是 SQLiteStudio，它将在下一节中讨论。

#### **基于 sqlite3 表数据的直方图（1）**

列表 4.31 显示了 rainfall_hist1.py 的内容，展示了如何定义一个简单的 SQL 查询以根据降雨表的数据创建直方图。

***列表 4.31：rainfall_hist1.py***

```py
 import sqlite3
import pandas as pd

sql = """
  SELECT
  cast(centimeters/10.00 as int)*10 as cent_floor,
  count(*) as count FROM rainfall
GROUP by 1
ORDER by 1;
"""

con = sqlite3.connect("mytools.db")
df = pd.read_sql_query(sql, con)
con.close()

print("=> Histogram of Rainfall:")
print(df) 
```

列表 4.31 以两个导入语句开始，然后初始化字符串变量 sql，其中包含涉及 rainfall 表的 SQL 语句。接下来，变量 con 被初始化为连接到 mytools.db 数据库的数据库连接。

列表 4.31 的下一部分调用 read_sql_query() 方法读取降雨表的全部内容，并将该数据填充到 DataFrame df 中。最后，关闭连接并打印 df 的内容。现在运行 列表 4.31 中的代码，你将看到以下输出：

```py
 => Histogram of Rainfall:
   cent_floor  count
0           0     27
1          10     14
2          20      9
3          30      9
4          40      3
5          50      2
6          60      1 
```

如果你想用一个变量替换值 10.00，可以使用以下代码片段：

```py
 factor = 10.00
sql = "SELECT cast(centimeters/"+str(factor)+" as
int)*"+str(factor)+" as cent_floor, count(*) as count FROM
rainfall GROUP by 1 ORDER by 1;" 
```

然而，前面的样式对于更长和更复杂的 SQL 语句可能会很快变得繁琐。

#### **基于 sqlite3 表数据的直方图（2）**

列表 4.32 显示了 rainfall_hist2.py 的内容，展示了如何定义一个简单的 SQL 查询以根据降雨表的数据创建直方图。

***列表 4.32：rainfall_hist2.py***

```py
 import sqlite3
import pandas as pd

sql = """
select
  bucket_floor,
  'FROM ' || bucket_floor || ' TO ' || bucket_ceiling as bucket_name,
  count(*) as count
from (
  select
    cast(centimeters/10.00 as int)*10 as bucket_floor,
    cast(centimeters/10.00 as int)*10 + 10 as bucket_ceiling
  from rainfall
) x
group by 1, 2
order by 1;
"""

con = sqlite3.connect("mytools.db")
df = pd.read_sql_query(sql, con)
con.close()

print("=> Histogram of Rainfall:")
print(df) 
```

列表 4.32 与前一个示例类似，经过一些微调以打印数据的更详细版本。现在运行 列表 4.32 中的代码，你将看到以下输出：

```py
 => Histogram of Rainfall:
   bucket_floor    bucket_name  count
0             0   FROM 0 TO 10     27
1            10  FROM 10 TO 20     14
2            20  FROM 20 TO 30      9
3            30  FROM 30 TO 40      9
4            40  FROM 40 TO 50      3
5            50  FROM 50 TO 60      2
6            60  FROM 60 TO 70      1 
```

### **使用 SQLITE3 工具**

前两个部分向您展示了如何直接使用 sqlite3，无论是通过 sqlite3 提示符还是从命令行。以下小节简要讨论了以下用于与 sqlite3 一起工作的有用工具：

+   SQLiteStudio

+   DB 浏览器

+   SQLiteDict

#### **SQLiteStudio 安装**

SQLiteStudio 是一个开源的 SQLite 集成开发环境，它允许你执行许多数据库操作，例如创建、更新和删除表和视图。导航到以下网站，下载适用于您操作系统的发行版，并执行指定的安装步骤：

*[`sqlitestudio.pl/`](https://sqlitestudio.pl/)*

*[`mac.softpedia.com/get/Developer-Tools/SQLiteStudio.shtml`](https://mac.softpedia.com/get/Developer-Tools/SQLiteStudio.shtml)*

图 4.6 展示了员工表的结构，其定义与 MySQL 中的 mytools 数据库中的员工表相同。

![图片](img/python-3-data-visualization-using-chatgpt-f0146-01.jpg)

***图 4.6*** 员工表。

图 4.7 展示了员工表中的三行截图，您可以在顶部行插入第四行数据，该行预先填充了 NULL 值。

![图片](img/python-3-data-visualization-using-chatgpt-f0146-02.jpg)

***图 4.7*** 员工表中的三行。

#### **SQLite 浏览器安装**

DB Browser 是一个开源且面向视觉的工具，用于 SQLite，它允许你执行各种数据库相关操作，例如创建和更新文件。此外，此工具允许你通过类似于电子表格的界面管理数据。

导航到以下网站，下载适用于您操作系统的发行版，并执行指定的安装步骤：

*[`www.macupdate.com/app/mac/38584/db-browser-for-sqlite/download/secure`](https://www.macupdate.com/app/mac/38584/db-browser-for-sqlite/download/secure)*

以下网站包含许多 URL，提供了有关 DB Browser 功能的详细信息：

*[`sqlitebrowser.org`](https://sqlitebrowser.org)*

#### **SQLiteDict（可选）**

SQLiteDict 是一个开源工具，它是 sqlite3 的包装器，并且可以在此处下载：

*[`pypi.org/project/sqlitedict/`](https://pypi.org/project/sqlitedict/)*

SQLiteDict 允许你将字典持久化到文件系统上的文件，如 列表 4.33 中的代码所示。

***列表 4.33: sqlitesavedict1.py***

```py
 # pip3 install sqlitedict

from sqlitedict import SqliteDict

mydict = SqliteDict('./my_db.sqlite', autocommit=True)
mydict['pasta'] = 'pasta'
mydict['pizza'] = 'pizza'

for key, value in mydict.iteritems():
  print("key:",key," value:",value)

# dictionary functions work:
print("length:",len(mydict))
mydict.close()

# a client instance:
myclient = MongoClient("localhost",27017) 
```

列表 4.33 包含一个导入语句，后面跟着变量 mydict，它被初始化为一个包含两个字符串 pasta 和 pizza 的字典。接下来的代码片段包含一个显示 mydict 的键/值对的查找，然后是 mydict 字典的长度。下一个代码片段关闭字典，然后在默认端口启动 MongoDB 客户端。现在运行 列表 4.33 中的代码，你将看到以下输出：

```py
 key: pasta  value: pasta
key: pizza  value: pizza
number of items: 2 
```

列表 4.34 展示了如何读取 列表 4.33 中保存的文件内容。

***列表 4.34: sqlitereaddict1.py***

```py
 # pip3 install sqlitedict

# read the contents of my_db.sqlite
# and note no autocommit=True
with SqliteDict('./my_db.sqlite') as mydict:
  print("old:", mydict['pasta'])
  mydict['pasta'] = u"more pasta"
  print("new:", mydict['pasta'])
  mydict['pizza'] = range(10)
  mydict.commit()
  # this is not persisted to disk:
  mydict['dish'] = u"deep dish"

# open the same file again:
with SqliteDict('./my_db.sqlite') as mydict:
  print("pasta:",mydict['pasta'])
  # this line will cause an error:
  #print("dish  value:",mydict['dish']) 
```

列表 4.34 包含一段代码，该代码读取 mydict 中 past 的现有值，然后更新其值，并保存其新值。列表 4.34 的最后一段代码读取存储的内容并显示键/值对。现在运行列表 4.34 中的代码，你将看到以下输出：

```py
 old: pasta
new: more pasta
pasta: more pasta 
```

查阅在线文档以获取有关通过 sqlitedict 可用的其他功能的信息。

### **使用美丽汤**

Beautiful Soup 是一个 Python 库，它使您能够从 HTML 网页和 XML 文档中解析数据。如果您熟悉 XPath，那么您已经了解 Beautiful Soup（它支持 XPath 功能子集）可以做什么。

Beautiful Soup 可以遍历 HTML 网页和 XML 文档（包括 SVG 文档）的树状结构，以提取所需的数据或文本。

此外，Beautiful Soup 还可以与您笔记本电脑上的文件系统中的文档以及从实时 HTML 网页“抓取”的数据一起工作。只是为了给您一个概念，Beautiful Soup 可以轻松地从以下网页的每一行中提取数据：

```py
 <html>
<body>
  <table>
   <tr><td>50</td><td>80</td></tr>
   <tr><td>150</td><td>180</td></tr>
  </table>
</body>
</html> 
```

#### **解析 HTML 网页**

列表 4.35 显示 sample.html，列表 4.36 显示 bsoup1.py 的内容，该内容从 sample.html 中提取数据，然后使用 Pandas 渲染柱状图。

***列表 4.35: sample.html***

```py
 <html>
<body>
  <table>
   <tr>
     <td>50</td>
     <td>80</td>
     <td>72</td>
     <td>68</td>
   </tr>
   <tr>
     <td>150</td>
     <td>180</td>
     <td>172</td>
     <td>168</td>
   </tr>
  </table>
</body>
</html> 
```

***列表 4.36: bsoup1.py***

```py
 import pandas as pd

# pip3 install BeautifulSoup4
from bs4 import BeautifulSoup

# read file and parse HTML:
filename="sample.html" with open(filename) as f:
  content = f.read()
  soup = BeautifulSoup(content, 'html.parser')

print("=> table data:")
#table = soup.table
table = soup.find("table")
print(table)
print()

print("=> table rows:")
rows = soup.find_all('tr')
for row in rows:
  print ("=> found row:",row)
print()

"""
# scraping a live HTML Web page:
# pip3 install requests
import requests
URL = "https://www.yahoo.com"
page = requests.get(URL)
soup = BeautifulSoup(page.content, 'html.parser')
""" 
```

列表 4.36 以导入语句开始，然后初始化变量 content 为 HTML 网页 sample.html 的内容。在打印变量 content 的内容之后，下一个代码块通过变量 content 将 sample.html 中的表格集合填充到变量 table 中，并简单地显示表格集合。

列表 4.36 的下一部分查找所有 <tr> 元素，并将这些数据填充到变量 rows 中。一个简单的循环遍历变量 rows 的内容，并打印每一行数据。现在运行列表 4.36 中的代码，你将看到以下输出：

```py
 => table data:
<table>
<tr>
<td>50</td>
<td>80</td>
<td>72</td>
<td>68</td>
</tr>
<tr>
<td>150</td>
<td>180</td>
<td>172</td>
<td>168</td>
</tr>
</table> => table rows:
=> found row: <tr>
<td>50</td>
<td>80</td>
<td>72</td>
<td>68</td>
</tr>
=> found row: <tr>
<td>150</td>
<td>180</td>
<td>172</td>
<td>168</td>
</tr> 
```

### **美丽汤和 Pandas**

本节中的代码示例使用 Beautiful Soup 从网页 sample.html 中的 HTML 表格中提取数据值，该网页在上一节中已看到。这些数据用于填充 Pandas DataFrame，然后使用 Pandas API 和 Matplotlib API 显示柱状图，这两个 API 在列表 4.38 的末尾以粗体显示。尽管 Matplotlib 直到第五章（ch05.xhtml）才讨论，但代码片段非常直观，不需要对 Matplotlib 有任何实质性的了解。

列表 4.37 展示了 bsoup2.py 的内容，展示了如何在 Pandas 中渲染柱状图。

***列表 4.37: bsoup2.py***

```py
 from bs4 import BeautifulSoup
import numpy as np
import pandas as pd

# read file and parse HTML:
filename="sample.html"
with open(filename) as f:
  content = f.read()
  soup = BeautifulSoup(content, 'html.parser')

rows = soup.find_all('tr')
all_data = []
for row in rows:
  row_items = row.find_all('td')
  print("row_items:",row_items)
  # create an array of <td> for each row:
  values = [td.get_text() for td in row_items]
  print("values:",values)
  # convert to integers:
  values = np.asarray(values)
  values = values.astype(int)
  print("values:",values)
  # append to matrix:
  all_data.append(values) print()
print("all_data:",all_data)

df = pd.DataFrame(all_data)
print("df:")
print(df)

# bar chart: ax = df.plot.bar()
plt.show()

```

列表 4.37 以导入语句开始，然后。现在运行列表 4.37 中的代码，你将看到以下输出：

```py
 row_items: [<td>50</td>, <td>80</td>, <td>72</td>, <td>68</td>]
values: ['50', '80', '72', '68']
values: [50 80 72 68]

row_items: [<td>150</td>, <td>180</td>, <td>172</td>, <td>168</td>]
values: ['150', '180', '172', '168']
values: [150 180 172 168]

all_data: [array([50, 80, 72, 68]), array([150, 180, 172, 168])]
df:
     0    1    2    3
0   50   80   72   68
1  150  180  172  168 
```

图 4.8 展示了用 HTML 网页 sample.html 中的数据填充的条形图。

![图片](img/python-3-data-visualization-using-chatgpt-f0152-01.jpg)

***图 4.8*** 来自 HTML 网页的条形图。

### **BEAUTIFUL SOUP AND LIVE HTML WEB PAGES**

本节中的代码示例使用 Beautiful Soup 解析实时 HTML 网页的内容。本节的关键区别是包含了一个用于抓取在线 HTML 网页内容的代码片段。

列表 4.38 展示了 bsoup3.py 的内容，展示了如何在 Pandas 中渲染条形图。

***列表 4.38: bsoup3.py***

```py
 from bs4 import BeautifulSoup

import re
import requests

URL = "https://www.yahoo.com"
page = requests.get(URL)
soup = BeautifulSoup(page.content, 'html.parser')

print("------------------------")
print("page before:")
print(page.text)
print("------------------------")
print()

divs = soup.find('div')
print("------------------------")
print("<div> elements:")
print(divs)
print("------------------------")
print()

tables = soup.find('tables')
print("------------------------")
print("table elements:")
print(tables)
print("------------------------")
print()

#links = soup.find('html/head/links')
links = soup.find('links')
print("------------------------")
print("link elements:")
print(links)
print("------------------------")
print() 
```

列表 4.38 从导入语句开始，然后初始化变量 content，包含指定 URL 的 HTML 网页内容。在变量 page 中的文本打印后，下一个代码块将变量 divs 填充为网页中的<div>元素集合。以类似的方式，接下来的两个代码块显示了网页中的表格和链接元素。现在运行列表 4.38 中的代码，你将看到以下输出：

```py
row_items:
------------------------
page before:
<!DOCTYPE html>
<html id="atomic" lang="en-US" class="atomic   l-out Pos-r https fp fp-default dt-default mini-uh-on uh-topbar-on ltr desktop Desktop bkt201">
<head>
    <meta http-equiv="X-UA-Compatible" content="IE=edge">

    <title>Yahoo | Mail, Weather, Search, Politics, News,
Finance, Sports & Videos</title><meta http-equiv="x
-dns-prefetch-control" content="on"><link rel="dns-
prefetch" href="//s.yimg.com"><link rel="preconnect" 
href="//s.yimg.com"><link rel="dns-prefetch" href="//
search.yahoo.com"><link rel="preconnect" href="//
search.yahoo.com"><link rel="dns-prefetch" 
href="//11.at.atwola.com"><link rel="preconnect" 
href="//11.at.atwola.com"><link rel="dns-prefetch" 
href="//geo.yahoo.com"><link rel="preconnect" href="//
geo.yahoo.com"><link rel="dns-prefetch" href="//
video-api.yql.yahoo.com"><link rel="preconnect" href="//
video-api.yql.yahoo.com">
// detail omitted for brevity
</div>
------------------------

------------------------
table elements:
None
------------------------

------------------------
link elements:
None
------------------------ 
```

这就结束了关于 Beautiful Soup 的简要部分。以下网页包含文档和代码片段，展示了如何使用 Beautiful Soup 的各种功能：

*[`beautiful-soup-4.readthedocs.io/en/latest/`](https://beautiful-soup-4.readthedocs.io/en/latest/)*

### **总结**

本章开始时提供了一些代码示例，展示了如何在 Pandas 中执行数据可视化，例如条形图、面积图和折线图。接下来，你看到了如何编写包含 MySQL 命令的 Python 代码。

接下来，你学习了 XML 文档和 JSON 数据，以及如何在 Pandas DataFrame 中读取此类数据。

此外，你还学习了如何结合 Python 和 SQLite 执行数据库相关操作，例如在 sqlite3 数据库中创建一个表，然后向该表中插入数据。此外，你还看到了如何从该表中选择数据，并将这些数据填充到 Pandas DataFrame 中。

最后，你学习了 Beautiful Soup，以及一些代码示例，展示了如何使用 Beautiful Soup 来解析 HTML 网页。

## 第五章

## *MATPLOTLIB AND VISUALIZATION*

本章介绍了数据可视化，以及一系列基于 Python 的代码示例，这些示例使用 Matplotlib 来渲染图表和图形。此外，本章还包含结合 Pandas 和 Matplotlib 的可视化代码示例。

本章的第一部分简要介绍了数据可视化，列出了部分数据可视化工具，以及各种可视化类型（条形图、饼图等等）。一些入门信息可以在网上找到：

*[`medium.datadriveninvestor.com/dont-beat-the-bush-use-chatgpt-to-visualize-your-data-94cee442cc29`](https://medium.datadriveninvestor.com/dont-beat-the-bush-use-chatgpt-to-visualize-your-data-94cee442cc29)*

*[`medium.datadriveninvestor.com/stop-wasting-times-to-learn-machine-learning-read-this-instead-5abfab230279`](https://medium.datadriveninvestor.com/stop-wasting-times-to-learn-machine-learning-read-this-instead-5abfab230279)*

本章的第一部分简要介绍了 Matplotlib，随后是显示 Matplotlib 中可用颜色的代码示例。

本章的第二部分包含了一系列 Python 代码示例，展示了如何绘制水平线、斜线和平行线。本节还包含了一系列代码示例，展示了如何以多种方式绘制点阵。

本章的第三部分展示了如何在 Matplotlib 中加载图像、显示棋盘图案和绘制三角函数图。第四部分包含了在 Matplotlib 中渲染图表和图形的示例，包括直方图、柱状图、饼图和热图。

最后一部分包含了渲染 3D 图表、财务数据和 sqlite3 数据库数据的代码示例。

### **什么是数据可视化？**

*数据可视化*指的是以图形方式呈现数据，例如柱状图、折线图和热图。正如你可能所知，大数据包含大量数据，它利用数据可视化工具来辅助做出更好的决策。

数据可视化是数据分析的一个关键方面，它提供了对潜在模式和关系的直观理解。借助 Matplotlib 和 Seaborn 等工具，Python 已成为制作引人入胜视觉的有效平台。一如既往，关键在于实践和探索。

数据的视觉表示使观众能够快速把握复杂的数据洞察。Python 凭借其丰富的可视化库生态系统，提供了以有意义的方式呈现数据的方法。本章重点介绍使用 Matplotlib 和 Seaborn 等库的各种可视化任务。

Python 是一种多才多艺且功能强大的编程语言，可用于从 Web 开发到数据分析的各种应用。在本章中，我们将探讨使用 Python 解决常见编程任务的解决方案。每个任务都将有详细的解释和解决方案。

高级可视化技术提供了从数据中获得更深层次的洞察和更全面的叙述。像 Matplotlib 和 Seaborn 这样的工具使这些任务更容易实现。虽然这些视觉工具很强大，但确保清晰并避免误述是至关重要的。继续实验和改进你的可视化技能，以讲述更吸引人的数据故事。

在数据可视化的领域，从新手到专家的旅程是通过采用能够从数据中提取和描绘更深层次洞察的高级技术来标记的。在本章中，我们将探讨一些这些高级可视化技术，并了解它们如何应用于各种数据场景。

有效的数据可视化是关于以直观的方式传达复杂的数据叙事。随着我们继续探索，本章将展开更高级的可视化技术，使我们能够以多种有洞察力的方式表示数据。

良好的数据可视化讲述了一个有意义的叙事，关注数据集中包含的有用信息（即，可能包含许多数据点的数据集）。数据可视化的另一个方面是其有效性：它传达数据集中可能存在的趋势有多好？

有许多开源的数据可视化工具可用，其中一些在此列出（还有许多其他工具）：

+   Matplotlib

+   Seaborn

+   Bokeh

+   YellowBrick

+   Tableau

+   D3.js (JavaScript 和 SVG)

如果您尚未这样做，建议在您的计算机上安装以下 Python 库（使用 pip3），以便您可以运行本章中的代码示例：

```py
 pip3 install matplotlib
pip3 install seaborn
pip3 install bokeh 
```

#### **数据可视化类型**

柱状图、折线图和饼图是常见的展示数据的方式，但还有许多其他类型，其中一些在此列出：

+   2D/3D 面积图

+   柱状图

+   甘特图

+   热图

+   直方图

+   极坐标面积图

+   散点图（2D 或 3D）

+   时间线

在接下来的几节中，Python 代码示例展示了如何通过 Matplotlib 的基本 API 进行可视化。

### **什么是 Matplotlib？**

Matplotlib 是一个支持 NumPy、SciPy 以及 wxPython 等工具包的绘图库。Matplotlib 仅支持 Python 3 版本：Python 2 版本的支持仅到 2020 年。Matplotlib 是一个基于 NumPy 数组的跨平台库。

本章中与绘图相关的代码示例使用 pyplot，这是一个提供类似 MATLAB 接口的 Matplotlib 模块。以下是一个使用 pyplot 基于欧拉常数 e 的负幂次绘制平滑曲线的示例：

```py
 import matplotlib.pyplot as plt
import numpy as np

a = np.linspace(0, 10, 100)
b = np.exp(-a)
plt.plot(a, b)
plt.show() 
```

请记住，绘制线段的代码示例假设您熟悉平面中（非垂直）线的方程：y = m*x + b，其中 m 是斜率，b 是 y 轴截距。

此外，一些代码示例使用了 NumPy API，如 np.linspace()、np.array()、np.random.rand() 和 np.ones()，这些在 第三章 中有讨论，因此您可以刷新对这些 API 的记忆。

### **MATPLOTLIB 风格**

列表 5.1 展示了 mpl_styles.py 的内容，该内容说明了如何在 Matplotlib 中绘制饼图。

***列表 5.1: mpl_styles.py***

```py
 import matplotlib.pyplot as plt

print("plt.style.available:")
styles = plt.style.available

for style in styles:
  print("style:",style) 
```

列表 5.1 包含一个导入语句，后面跟着变量 styles，它被初始化为 Matplotlib 中可用的风格集。列表 5.1 的最后部分包含一个循环，该循环遍历 styles 变量中的值。运行 列表 5.1 中的代码，您将看到以下输出：

```py
 plt.style.available:
style: Solarize_Light2
style: _classic_test_patch
style: bmh
style: classic
style: dark_background
style: fast
style: fivethirtyeight
style: ggplot
style: grayscale
style: seaborn
style: seaborn-bright
style: seaborn-colorblind
style: seaborn-dark
style: seaborn-dark-palette
style: seaborn-darkgrid
style: seaborn-deep
style: seaborn-muted
style: seaborn-notebook
style: seaborn-paper
style: seaborn-pastel
style: seaborn-poster
style: seaborn-talk
style: seaborn-ticks
style: sea born-white
style: seaborn-whitegrid
style: tableau-colorblind10 
```

### **显示属性值**

列表 5.2 显示了 mat_attrib_values.py 的内容，该内容显示了 Matplotlib 中对象的属性值（subplot 在本章后面讨论）。

***列表 5.2：mat_attrib_values.py***

```py
 import matplotlib.pyplot as plt

fig, ax = plt.subplots()

print("=> attribute values:")
print(plt.getp(fig)) 
```

列表 5.2 包含一个导入语句，随后是 fig 和 ax 变量，它们通过调用 plt 类的 subplots() 方法进行初始化。下一块代码通过调用 plt.getp() 方法打印 fig 的属性值。运行 列表 5.2 中的代码，你将看到以下输出：

```py
 => attribute values:
    agg_filter = None
    alpha = None
    animated = False
    axes = [<AxesSubplot:>]
    children = [<matplotlib.patches.Rectangle object at 0x11c34f0... clip_box = None
    clip_on = True
    clip_path = None
    constrained_layout = False
    constrained_layout_pads = (0.04167, 0.04167, 0.02, 0.02)
    contains = None
    default_bbox_extra_artists = [<AxesSubplot:>, <matplotlib.spines.Spine object a... dpi = 100.0
    edgecolor = (1.0, 1.0, 1.0, 1.0)
    facecolor = (1.0, 1.0, 1.0, 1.0)
    figheight = 4.8
    figure = None
    figwidth = 6.4
    frameon = True
    gid = None
    in_layout = True
    label =
    path_effects = []
    picker = None
    rasterized = None
    size_inches = [6.4 4.8]
    sketch_params = None
    snap = None
    tight_layout = False
    transform = IdentityTransform()
    transformed_clip_path_and_affine = (None, None) url = None
    visible = True
    window_extent = TransformedBbox(     Bbox(x0=0.0, y0=0.0, x1=6.4, ... zorder = 0
None 
```

### **MATPLOTLIB 中的颜色值**

列表 5.3 显示了 mat_colors.py 的内容，该内容显示了 Matplotlib 中可用的颜色。

***列表 5.3：heatmap1.py***

```py
 import matplotlib
import matplotlib.pyplot as plt

colors = plt.colormaps()

col_count=5
idx=0
for color in colors:
  if(color.endswith("_r") == False):
    print(color," ",end="")
    idx += 1
    if(idx % col_count == 0):
      print()
print()
print("=> color count:",idx) 
```

列表 5.3 包含两个导入语句，之后将变量 colors 初始化为可用颜色的列表。列表 5.3 的下一部分包含一个循环，该循环遍历 colors 变量，并打印每个颜色的值，前提是该颜色名称中不包含后缀 “_r”。每次打印五个颜色后，会打印一个新行。运行 列表 5.3 中的代码，你将看到以下输出：

```py
 Accent  Blues  BrBG  BuGn  BuPu
CMRmap  Dark2  GnBu  Greens  Greys
OrRd  Oranges  PRGn  Paired  Pastel1
Pastel2  PiYG  PuBu  PuBuGn  PuOr
PuRd  Purples  RdBu  RdGy  RdPu
RdYlBu  RdYlGn  Reds  Set1  Set2
Set3  Spectral  Wistia  YlGn  YlGnBu
YlOrBr  YlOrRd  afmhot  autumn  binary
bone  brg  bwr  cividis  cool
coolwarm  copper  cubehelix  flag  gist_earth
gist_gray  gist_heat  gist_ncar  gist_rainbow  gist_stern
gist_yarg  gnuplot  gnuplot2  gray  hot
hsv  inferno  jet  magma  nipy_spectral
ocean  pink  plasma  prism  rainbow
seismic  spring  summer  tab10  tab20
tab20b  tab20c  terrain  turbo  twilight
twilight_shifted  viridis  winter
=> color count: 83 
```

现在让我们继续下一节，该节包含一系列快速的基本代码示例，展示了各种类型的线段。

### **MATPLOTLIB 中的立方数**

列表 5.4 显示了 cubed_numbers.py 的内容，该内容说明了如何使用 Matplotlib 绘制一组点。

***列表 5.4：cubed_numbers.py***

```py
 import matplotlib.pyplot as plt

plt.plot([1, 2, 3, 4], [1, 8, 27, 64])
plt.axis([0, 5, 0, 70])
plt.xlabel("Integers (1-4)")
plt.ylabel("Cubed Integers")
plt.show() 
```

列表 5.4 绘制了一组整数值的点，其 x 坐标在 1 到 4（包含）之间，其 y 坐标是对应 x 坐标的立方。代码示例还标注了水平轴和垂直轴。图 5.1 显示了 列表 5.4 中的这些点。

![图像](img/python-3-data-visualization-using-chatgpt-f0163-01.jpg)

***图 5.1*** 立方数的图表

### **MATPLOTLIB 中的水平线**

列表 5.5 显示了 hlines1.py 的内容，该内容说明了如何使用 Matplotlib 绘制水平线。回想一下，二维平面中非垂直线的方程是 y = m*x + b，其中 m 是线的斜率，b 是线的 y 截距。

***列表 5.5：hlines1.py***

```py
 import numpy as np
import matplotlib.pyplot as plt

# top line
x1 = np.linspace(-5,5,num=200)
y1 = 4 + 0*x1

# middle line
x2 = np.linspace(-5,5,num=200)
y2 = 0 + 0*x2

# bottom line
x3 = np.linspace(-5,5,num=200)
y3 = -3 + 0*x3

plt.axis([-5, 5, -5, 5])
plt.plot(x1,y1)
plt.plot(x2,y2)
plt.plot(x3,y3)
plt.show() 
```

列表 5.5 使用 np.linspace() API 生成一个包含 200 个等间距数字的列表，这些数字都在 -5 和 5 之间。通过变量 y1、y2 和 y3 定义的三个线，分别用变量 x1、x2 和 x3 来定义。

图 5.2 显示了包含在 列表 5.5 中的三个水平线段，其方程式如下。

![图像](img/python-3-data-visualization-using-chatgpt-f0164-01.jpg)

***图 5.2*** 三个水平线段的图表

### **MATPLOTLIB 中的斜线**

列表 5.6 显示了 diagonallines.py 的内容，该内容说明了如何绘制斜线。

***列表 5.6：diagonallines.py***

```py
 import matplotlib.pyplot as plt
import numpy as np

x1 = np.linspace(-5,5,num=200)
y1 = x1

x2 = np.linspace(-5,5,num=200)
y2 = -x2

plt.axis([-5, 5, -5, 5])
plt.plot(x1,y1)
plt.plot(x2,y2)
plt.show() 
```

列表 5.6 使用你在 列表 5.5 中看到的技巧定义了两条线，除了这两条线定义了 y1 = x1 和 y2 = -x2，这产生了斜线而不是水平线。

图 5.3 显示了两个斜线段，其方程在 列表 5.6 中定义。

![图片](img/python-3-data-visualization-using-chatgpt-f0165-01.jpg)

***图 5.3*** 两个斜线段的图形

### **MATPLOTLIB 中的平行斜线**

如果欧几里得平面上的两条线具有相同的斜率，那么它们是平行的。列表 5.7 显示了 parallellines1.py 的内容，该内容说明了如何绘制平行斜线。

***列表 5.7: parallellines1.py***

```py
 import matplotlib.pyplot as plt
import numpy as np

# lower line
x1 = np.linspace(-5,5,num=200)
y1 = 2*x1 # upper line
x2 = np.linspace(-5,5,num=200)
y2 = 2*x2 + 3

# horizontal axis
x3 = np.linspace(-5,5,num=200)
y3 = 0*x3 + 0

# vertical axis
plt.axvline(x=0.0)

plt.axis([-5, 5, -10, 10])
plt.plot(x1,y1)
plt.plot(x2,y2)
plt.plot(x3,y3)
plt.show() 
```

列表 5.7 使用你在 列表 5.6 中看到的技巧定义了三条线，其中两条线是斜平行的，第三条线是水平的。运行 列表 5.7 中的代码，你将看到 图 5.4 中显示的结果。

![图片](img/python-3-data-visualization-using-chatgpt-f0166-01.jpg)

***图 5.4*** 两个斜平行线段的图形

### **MATPLOTLIB 中的点状网格**

列表 5.8 显示了 plotgrid.py 的内容，该内容说明了如何绘制简单的网格。

***列表 5.8: multi_lines.py***

```py
 import matplotlib.pyplot as plt

x_coord = [ 50, 300, 175, 50]
y_coord = [ 50, 50,  150, 50]
plt.plot(x_coord,y_coord)
plt.scatter(x_coord,y_coord) for x,y in zip(x_coord,y_coord):
  plt.text(x,y,'Coord ({x},{y})'.format(x=x,y=y))

x_coord = [ 175, 300,  50, 175]
y_coord = [  50, 150, 150, 50]
plt.plot(x_coord,y_coord)
plt.scatter(x_coord,y_coord)

for x,y in zip(x_coord,y_coord):
  plt.text(x,y,'Coord ({x},{y})'.format(x=x,y=y))
plt.show() 
```

列表 5.8 定义了 NumPy 变量 points，它定义了一个具有三行四列的二维点列表。Pyplot API 的 plot() 使用 points 变量来显示类似网格的模式。图 5.5 显示了 列表 5.8 中定义的点网格。

![图片](img/python-3-data-visualization-using-chatgpt-f0167-01.jpg)

***图 5.5*** 由 列表 5.8 中的代码生成的网格

### **MATPLOTLIB 中的点状网格**

列表 5.9 显示了 plotdottedgrid1.py 的内容，该内容说明了如何绘制“点状”网格模式。

***列表 5.9: plotdottedgrid1.py***

```py
 import numpy as np
import pylab
from itertools import product
import matplotlib.pyplot as plt

fig = pylab.figure()
ax = fig.add_subplot(1,1,1)

ax.grid(which='major', axis='both', linestyle='--')

[line.set_zorder(3) for line in ax.lines]
fig.show() # to update

plt.gca().xaxis.grid(True)
plt.show() 
```

列表 5.9 与 列表 5.8 中的代码类似，因为它们都绘制了类似网格的模式；然而，前者渲染了一个“点状”网格模式，而后者通过指定 linestyle 参数的值为 '--' 来渲染一个“点状”网格模式。

列表 5.9 的下一部分调用了 set_zorder() 方法，该方法控制哪些项目显示在其他项目之上，例如线条上的点或反之亦然。 列表 5.9 的最后一部分调用了 gca().xaxis.grid(True) 连锁方法来显示垂直网格线。

你还可以使用 plt.style 指令来指定图形的样式。以下代码片段指定了 Matplotlib 的经典样式：

```py
 plt.style.use('classic') 
```

图 5.6 显示了一个基于 列表 5.9 中的代码的“虚线”网格模式。

![图片](img/python-3-data-visualization-using-chatgpt-f0168-01.jpg)

***图 5.6*** 使用 列表 5.9 中的代码生成的“虚线”网格模式

### **MATPLOTLIB 中的两条线和图例**

列表 5.10 显示了 plotgrid2.py 的内容，该内容说明了如何显示彩色网格。

***列表 5.10: two_lines_legend.py***

```py
 import matplotlib.pyplot as plt

# FIRST PLOT:
vals_x = [91,93,95,96,97,98,99,99,104,115]
vals_y = [1500,2000,3000,2500,1200,1500,2900,3200,5200,6500]
plt.plot(vals_x, vals_y) # alternate style
#plt.plot(vals_x, vals_y, label='First List')

# SECOND PLOT:
vals_x2 = [91,93,95,96,97,98,99,99,104,115] vals_y2 = [1005,1006,1007,1008,1009,2031,3100,2033,3034,4035]
plt.plot(vals_x2, vals_y2)
#plt.plot(vals_x2, vals_y2, label='Second List') # alternate style

# generate line plot:
plt.plot(vals_x, vals_y)
plt.title("Random Pairs of Numbers")
plt.xlabel("Random X Values")
plt.ylabel("Random Y Values")
plt.legend(['First List','Second List'])
#plt.legend() # alternate style
plt.show() 
```

列表 5.10 定义了 NumPy 变量 data，它定义了一个包含十个行和十个列的二维点集。Pyplot API 的 plot() 函数使用 data 变量来显示两个线形图，如图 5.7 所示。

![图像](img/python-3-data-visualization-using-chatgpt-f0169-01.jpg)

***图 5.7*** 一对线段

### **在 Matplotlib 中加载图像**

列表 5.11 显示了 load_images2.py 的内容，该内容说明了如何显示图像。

***列表 5.11: load_images2.py***

```py
 from sklearn.datasets import load_digits
from matplotlib import pyplot as plt

digits = load_digits() #set interpolation='none'

fig = plt.figure(figsize=(3, 3))
plt.imshow(digits['images'][66], cmap="gray", interpolation='none')
plt.show() 
```

列表 5.11 以两个导入语句开始，然后 digits 变量被初始化为 digits 数据集的内容。列表 5.11 的下一部分显示了 digits 数据集中一张图片的内容。运行列表 5.11 中的代码，你将看到图 5.8 中的图像。

![图像](img/python-3-data-visualization-using-chatgpt-f0170-01.jpg)

***图 5.8*** 在 Matplotlib 中加载图像

### **Matplotlib 中的棋盘**

列表 5.12 显示了 checkerboard1.py 的内容，该内容说明了如何显示棋盘。

***列表 5.12: checkerboard1.py***

```py
 import matplotlib.pyplot as plt
from matplotlib import colors
import numpy as np

data = np.random.rand(10, 10) * 20

# create discrete colormap
cmap = colors.ListedColormap(['red', 'blue'])
bounds = [0,10,20]
norm = colors.BoundaryNorm(bounds, cmap.N)

fig, ax = plt.subplots()
ax.imshow(data, cmap=cmap, norm=norm)

# draw gridlines ax.grid(which='major', axis='both', linestyle='-', color='k', linewidth=2)
ax.set_xticks(np.arange(-.5, 10, 1));
ax.set_yticks(np.arange(-.5, 10, 1));

plt.show() 
```

列表 5.12 定义了 NumPy 变量 data，它定义了一个包含十个行和十个列的二维点集。Pyplot API 的 plot() 函数使用 data 变量来显示一个彩色的网格状图案。图 5.9 显示了一个包含在列表 5.12 中的彩色网格的方程。

![图像](img/python-3-data-visualization-using-chatgpt-f0171-01.jpg)

***图 5.9*** 由 Matplotlib 生成的棋盘

### **Matplotlib 中的随机数据点**

列表 5.13 显示了 lin_reg_plot.py 的内容，该内容说明了如何绘制随机点的图表。

***列表 5.13: lin_plot_reg.py***

```py
 import numpy as np
import matplotlib.pyplot as plt

trX = np.linspace(-1, 1, 101) # Linear space of 101 and [-1,1]

#Create the y function based on the x axis
trY = 2*trX + np.random.randn(*trX.shape)*0.4+0.2

#create figure and scatter plot of the random points
plt.figure()
plt.scatter(trX,trY)

# Draw one line with the line function plt.plot (trX, .2 + 2 * trX)
plt.show() 
```

列表 5.13 定义了 NumPy 变量 trX，它包含 101 个在 -1 和 1（包含）之间等间隔的数字。变量 trY 定义为两部分：第一部分是 2*trX，第二部分是基于一维数组 trX 长度的随机值。变量 trY 是这两部分的总和，从而创建了一个“模糊”的线段。

列表 5.13 的下一部分基于 trX 和 trY 中的值创建了一个散点图，随后是 Pyplot API 的 plot() 函数，它渲染了一条线段。图 5.10 显示了基于列表 5.13 代码的随机点集。

![图像](img/python-3-data-visualization-using-chatgpt-f0172-01.jpg)

***图 5.10*** 基于列表 5.13 代码的随机点集

### **Matplotlib 中的线段集**

列表 5.14 显示了 line_segments.py 的内容，该内容说明了如何在 Matplotlib 中绘制一组连接的线段。

***列表 5.14: line_segments.py***

```py
 import numpy as np
import matplotlib.pyplot as plt

x = [7,11,13,15,17,19,23,29,31,37]

plt.plot(x) # OR: plt.plot(x, 'ro-') or bo
plt.ylabel('Height')
plt.xlabel('Weight')
plt.show() 
```

列表 5.14 定义了包含一组硬编码值的数组 x。Pyplot API 的 plot() 使用变量 x 来显示一组连接的线段。图 5.11 显示了运行 列表 5.14 中的代码的结果。

![图片](img/python-3-data-visualization-using-chatgpt-f0173-01.jpg)

***图 5.11*** 一组连接的线段

### **MATPLOTLIB 中绘制多条线**

列表 5.15 展示了 plt_array2.py 的内容，该文件说明了你可以在 Matplotlib 中轻松绘制多条线。

***列表 5.15: plt_array2.py***

```py
 import matplotlib.pyplot as plt

x = [7,11,13,15,17,19,23,29,31,37]
data = [[8, 4, 1], [5, 3, 3], [6, 0, 2], [1, 7, 9]]
plt.plot(data, 'd-')
plt.show() 
```

列表 5.15 定义了包含一组硬编码值的数组 data。Pyplot API 的 plot() 使用变量 data 来显示一个线段。图 5.12 显示了基于 列表 5.15 中的代码的多条线。

![图片](img/python-3-data-visualization-using-chatgpt-f0173-02.jpg)

***图 5.12*** Matplotlib 中的多行

### **MATPLOTLIB 中的三角函数**

你可以像渲染“常规”图一样轻松地显示三角函数的图形。 列表 5.16 展示了 sincos.py 的内容，该文件说明了如何在 Matplotlib 中绘制正弦函数和余弦函数。

***列表 5.16: sincos.py***

```py
 import numpy as np
import math

x = np.linspace(0, 2*math.pi, 101)
s = np.sin(x)
c = np.cos(x)

import matplotlib.pyplot as plt
plt.plot (s)
plt.plot (c)
plt.show() 
```

列表 5.16 使用 NumPy API 的 linspace()、sin() 和 cos() 分别定义了 NumPy 变量 x、s 和 c。接下来，Pyplot API 的 plot() 使用这些变量来显示正弦函数和余弦函数。

图 5.13 展示了基于 列表 5.16 中的代码的两个三角函数的图形。

![图片](img/python-3-data-visualization-using-chatgpt-f0174-01.jpg)

***图 5.13*** 正弦和余弦三角函数

现在，让我们看看一个由离散数据点组成的简单数据集，这是下一节的主题。

### **MATPLOTLIB 中的直方图**

列表 5.17 展示了 histogram1.py 的内容，该文件说明了如何使用 Matplotlib 绘制直方图。

***列表 5.17: histogram1.py***

```py
 import matplotlib.pyplot as plt

x = [1, 2, 3, 4, 5, 6, 7, 4]

plt.hist(x, bins = [1, 2, 3, 4, 5, 6, 7])
plt.title("Histogram")
plt.legend(["bar"])
plt.show() 
```

列表 5.17 非常直接：变量 x 被初始化为一组数字，随后是一段代码，根据变量 x 中的数据绘制直方图。运行 列表 5.17 中的代码，你将看到 图 5.14 中显示的直方图。

![图片](img/python-3-data-visualization-using-chatgpt-f0175-01.jpg)

***图 5.14*** 基于随机值的直方图

### **使用 SQLITE3 表中的数据创建直方图**

列表 5.18 展示了 rainfall_hist2.py 的内容，该文件展示了如何定义一个简单的 SQL 查询，以基于降雨表中的数据创建直方图。

***列表 5.18: rainfall_hist3.py***

```py
 import sqlite3
import pandas as pd
import matplotlib.pyplot as plt

sql = """
  SELECT
  cast(centimeters/5.00 as int)*5 as cent_floor,
  count(*) as count FROM rainfall
GROUP by 1
ORDER by 1;
"""

con = sqlite3.connect("mytools.db")
df = pd.read_sql_query(sql, con)
con.close()

print("=> Histogram of Rainfall:")
print(df)

#df.hist(column='count', bins=7, grid=False, rwidth=1.0, color='red')
df.hist(column='count', bins=14, grid=False, rwidth=.8, color='red')
plt.show() 
```

列表 5.18 以几个导入语句开始，然后初始化变量 sql，其中包含一个 SQL 语句，用于从降雨量表中选择数据。列表 5.18 的下一部分初始化变量 con，用于访问 mytools.db 数据库，然后使用包含在变量 sql 中的 SQL 语句的结果填充 Pandas 数据帧 df。现在运行列表 5.18 中的代码，你将看到以下输出：

```py
 => Histogram of Rainfall:
   bucket_floor    bucket_name  count
0             0   FROM 0 TO 10     27
1            10  FROM 10 TO 20     14
2            20  FROM 20 TO 30      9
3            30  FROM 30 TO 40      9
4            40  FROM 40 TO 50      3
5            50  FROM 50 TO 60      2
6            60  FROM 60 TO 70      1 
```

图 5.15 中显示的直方图是由这些数据创建的。

![图片](img/python-3-data-visualization-using-chatgpt-f0176-01.jpg)

***图 5.15*** 基于降雨数据的直方图

### **在 Matplotlib 中绘制条形图**

列表 5.19 显示了 barchart1.py 的内容，该内容说明了如何在 Matplotlib 中绘制条形图。

***列表 5.19: barchart1.py***

```py
 import matplotlib.pyplot as plt

x = [3, 1, 3, 12, 2, 4, 4]
y = [3, 2, 1, 4, 5, 6, 7]

plt.bar(x, y)

plt.title("Bar Chart")
plt.legend(["bar"])
plt.show() 
```

列表 5.19 包含一个导入语句，然后是初始化为数字列表的变量 x 和 y。接下来，通过调用 plt 类的 bar() 方法生成条形图。代码的最后部分设置了条形图的标题和图例，然后显示了条形图。运行列表 5.19 中的代码，你将看到图 5.16 中显示的饼图。

![图片](img/python-3-data-visualization-using-chatgpt-f0177-01.jpg)

***图 5.16*** 使用 Matplotlib 绘制的条形图

列表 5.20 显示了 barchart2.py 的内容，该内容说明了如何在 Matplotlib 中绘制条形图。

***列表 5.20: barchart2.py***

```py
 import matplotlib.pyplot as plt

plt.bar([0.25,1.25,2.25,3.25,4.25],
        [50,40,70,80,20],
        label="GDP1",width=.5) plt.bar([.75,1.75,2.75,3.75,4.75],
        [80,20,20,50,60],
        label="GDP2", color='r',width=.5)

plt.legend()
plt.xlabel('Months')
plt.ylabel('GDP (Billion Euross)')
plt.title('Bar Chart Comparison') 
```

列表 5.20 包含一个导入语句，然后定义了两个并排显示的条形图。注意，每个条形图的定义都涉及指定 x 和 y（即使它们没有明确包含），然后是一个用于标签和宽度参数的值。代码的最后部分设置了图例和水平轴和垂直轴的标签。运行列表 5.20 中的代码，你将看到图 5.17 中所示的条形图。

![图片](img/python-3-data-visualization-using-chatgpt-f0178-01.jpg)

***图 5.17*** 由列表 5.20 中的代码生成的两个条形图

### **在 Matplotlib 中绘制饼图**

列表 5.21 显示了 piechart1.py 的内容，该内容说明了如何在 Matplotlib 中绘制饼图。

***列表 5.21: piechart1.py***

```py
 import numpy as np

# data to display on plots
x = [1, 2, 3, 4]

# explode the first wedge:
e =(0.1, 0, 0, 0) plt.pie(x, explode = e)
plt.title("Pie chart")
plt.show() 
```

列表 5.21 包含一个导入语句，然后是初始化为数字列表的变量 x 和 e。x 的值用于计算饼图每个“切片”的相对大小，而 e 的值表示第一个饼图切片略微“爆炸”（由 e 中的值 0.1 表示）。运行列表 5.21 中的代码，你将看到图 5.18 中显示的饼图。

![图片](img/python-3-data-visualization-using-chatgpt-f0179-01.jpg)

***图 5.18*** 由列表 5.21 中的代码生成的饼图

### **Matplotlib 中的热图**

列表 5.22 显示了 heatmap1.py 的内容，该内容说明了如何在 Matplotlib 中渲染热图。

***列表 5.22: heatmap1.py***

```py
 import numpy as np

data = np.random.random((16, 16))
plt.imshow(data, cmap='tab20_r', interpolation='nearest')
plt.show() 
```

列表 5.22 包含一个导入语句，接着是变量 data，它被初始化为一个 16x16 的随机值矩阵。下一个代码片段渲染热图，最后的代码片段显示热图。运行 列表 5.22 中的代码，你将看到 图 5.19 中所示的图像。

![图片](img/python-3-data-visualization-using-chatgpt-f0180-01.jpg)

***图 5.19*** 由 列表 5.22 中的代码生成的热图

### **将图表保存为 PNG 文件**

列表 5.23 显示了 matplot2png.py 的内容，展示了如何将图形图像保存为 PNG 文件。

***列表 5.23: matplot2png.py***

```py
 import matplotlib.pyplot as plt
import numpy as np

outfile="graph1.png"

plt.figure()
plt.plot(range(6))

fig, ax = plt.subplots()

ax.plot([2, 3, 4, 5, 5, 6, 6],
        [5, 7, 1, 3, 4, 6 ,8])

ax.plot([1, 2, 3, 4, 5],
        [2, 3, 4, 5, 6])

x = np.linspace(0, 12, 100)
plt.plot(np.sin(x))
plt.plot(np.linspace(-4,4,50))

plt.savefig(outfile, dpi=300) 
```

列表 5.23 包含导入语句，接着是变量 outfile，它被初始化为要保存到文件系统中的 PNG 文件名。PNG 文件的内容包括一个正弦波和一组线段。运行 列表 5.23 中的代码，你将看到 图 5.20 中所示的图像。

![图片](img/python-3-data-visualization-using-chatgpt-f0181-01.jpg)

***图 5.20*** 使用 列表 5.23 中的代码生成的热图

### **使用 SWEETVIZ**

SweetViz 是一个开源的 Python 模块，基于五行 Python 代码生成非常详细的可视化，以 HTML 网页的形式呈现。

作为简单的示例，列表 5.24 展示了 sweetviz1.py 的内容，该内容生成了 Scikit-learn 中可用的 Iris 数据集的各个方面可视化。

***列表 5.24: sweetviz1.py***

```py
 import sweetviz as sv
import seaborn as sns

df = sns.load_dataset('iris')
report = sv.analyze(df)
report.show_html() 
```

列表 5.24 从两个导入语句开始，接着初始化变量 df，使其包含 Iris 数据集的内容。接下来的代码片段初始化变量 report，作为调用 SweetViz 中的 analyze() 方法的输出结果，随后是一个生成分析结果的 HTML 网页的代码片段。

在命令行中运行代码，你将在同一目录下看到一个名为 SWEETVIZ_REPORT.html 的新 HTML 网页。图 5.21 显示了 SWEETVIZ_REPORT.html 网页的内容。

![图片](img/python-3-data-visualization-using-chatgpt-f0182-01.jpg)

***图 5.21*** 对 Iris 数据集的分析

### **使用 SKIMPY**

Skimpy 是一个开源的 Python 模块，可以直接从命令行生成数据集的分析：不需要 Python 代码。使用以下命令安装 Skimpy：

```py
 pip3 install skimpy 
```

运行以下命令来分析泰坦尼克号数据集（或你自己的数据集）并将输出重定向到文本文件（后者是可选的）：

```py
 skimpy titanic.csv >titanic_out.txt 
```

图 5.22 显示了前面命令生成的输出内容。

![图片](img/python-3-data-visualization-using-chatgpt-f0183-01.jpg)

***图 5.22*** 对泰坦尼克号数据集的分析

### **MATPLOTLIB 中的 3D 图表**

列表 5.25 展示了 matplot_3d.py 的内容，说明了如何在 Matplotlib 中渲染 3D 图形。

***列表 5.25：matplot_3d.py***

```py
 import matplotlib.pyplot as plt
import numpy as np

zline = np.linspace(0,40,1000)
xline = 2*np.sin(2*zline)
yline = 3*np.cos(3*zline)

ax = plt.axes(projection="3d")
ax.plot3D(xline,yline,zline,'red',linewidth=4)
plt.show() 
```

列表 5.25 包含导入语句，然后通过 NumPy 的 linspace()、sin() 和 cos() 方法分别初始化变量 zline、xline 和 yline。列表 5.25 的下一部分初始化变量 ax，以便显示一个 3D 图形，该图形由最后的代码片段渲染。运行列表 5.25 中的代码，你将看到 图 5.23 中所示的图像。

![图片](img/python-3-data-visualization-using-chatgpt-f0183-02.jpg)

***图 5.23*** 3D 图形

### **使用 MPLFINANCE 绘制财务数据**

该部分包含一个基于 Python 的代码示例，展示了如何绘制给定股票的财务数据。首先，请确保你已经安装了必要的 Python 库，如下所示：

```py
 pip3 install mplfinance 
```

列表 5.26 展示了 financial_mpl.py 的内容，说明了如何在 Matplotlib 中绘制财务数据。

***列表 5.26：financial_mpl.py***

```py
 #optional:
import sys
sys.path.append('/usr/local/lib/python3.9/site-packages')

import matplotlib.pyplot as plt
import pandas as pd

csvfile="aapl.csv"
daily = pd.read_csv(csvfile,index_col=0,parse_dates=True)
daily.index.name = 'Date'

print("daily.head():")
print(daily.head())
print()

print("daily.tail():")
print(daily.tail())

import mplfinance as mpf
mpf.plot(daily)

#Plot types: ohlc, candle, line, renko, and pnf 
```

列表 5.26 包含导入语句，然后是包含 2017 年和 2018 年 AAPL 数据的变量 csvfile。接下来，变量 daily 被初始化为 aapl.csv 的内容，然后是一段代码，该代码打印 aapl.csv 中的前 5 行和最后 5 行数据。

最后一部分代码调用类 mpf（从 mplfinance 导入）的 plot() 方法来渲染图表。运行列表 5.26 中的代码，你将看到以下输出：

```py
 daily.head():
                  Open        High  ... Adj Close    Volume
Date                                ... 2017-01-03  115.800003  116.330002  ... 114.311760  28781900
2017-01-04  115.849998  116.510002  ... 114.183815  21118100
2017-01-05  115.919998  116.860001  ... 114.764473  22193600
2017-01-06  116.779999  118.160004  ... 116.043915  31751900
2017-01-09  117.949997  119.430000  ... 117.106812  33561900

[5 rows x 6 columns] daily.tail():
                  Open        High  ... Adj Close    Volume
Date                                ... 2018-01-12  176.179993  177.360001  ... 177.089996  25418100
2018-01-16  177.899994  179.389999  ... 176.190002  29565900
2018-01-17  176.149994  179.250000  ... 179.100006  34386800
2018-01-18  179.369995  180.100006  ... 179.259995  31193400
2018-01-19  178.610001  179.580002  ... 178.460007  31269600

[5 rows x 6 columns] 
```

图 5.24 展示了基于列表 5.29 中的代码生成的财务数据图。

![图片](img/python-3-data-visualization-using-chatgpt-f0185-01.jpg)

***图 5.24*** 2017 年和 2018 年的财务数据图

### **使用 SQLITE3 数据绘制图表和图形**

列表 5.27 展示了 rainfall_multiple.py 的内容，展示了如何从 sqlite3 数据库中提取的数据生成多个图表和图形。

***列表 5.27：rainfall_multiple.py***

```py
 import sqlite3
import pandas as pd
import matplotlib.pyplot as plt

sql = """
  SELECT
  cast(centimeters/5.00 as int)*5 as cent_floor,
  count(*) as count
FROM rainfall
GROUP by 1
ORDER by 1; """

con = sqlite3.connect("mytools.db")
df = pd.read_sql_query(sql, con)
con.close()

####################################
# generate 7 types of charts/graphs
# and save them as PNG or TIFF files
####################################
df.hist(column='count', bins=14, grid=False, rwidth=.8, color='red')
plt.savefig("rainfall_histogram.tiff")

df.plot.pie(y='count',figsize=(8,6))
plt.savefig("rainfall_pie.png")

df.plot.line(y='count',figsize=(8,6))
plt.savefig("rainfall_line.png")

df.plot.scatter(y='count',x='cent_floor',figsize=(8,6))
plt.savefig("rainfall_scatter.png")

df.plot.box(figsize=(8,6))
plt.savefig("rainfall_box.png")

df.plot.hexbin(x='count', y='cent_floor',gridsize=30, figsize=(8,6))
plt.savefig("rainfall_hexbin.png")
df["cent_floor"].plot.kde()
plt.savefig("rainfall_kde.png")

df["count"].hist()
df.plot.line(x='count', y='cent_floor', figsize=(8,6))
df.plot.scatter(x='count', y='cent_floor', figsize=(8,6))
df.plot.box(figsize=(8,6))
df.plot.hexbin(x='count', y='cent_floor',gridsize=30, figsize=(8,6))
df.plot.pie(y='cost', figsize=(8, 6))
df["cent_floor"].plot.kde() 
```

列表 5.27 包含几个导入语句，然后初始化变量 sql，其中包含一个 SQL 语句，用于从降雨表中选择数据。列表 5.27 的下一部分初始化变量 con，用于访问 mytools.db 数据库，然后使用 sql 变量中包含的 SQL 语句的结果填充 Pandas 数据帧 df。

列表 5.27 的下一部分包含用于渲染各种类型图表和图形（直方图、饼图、折线图、散点图、箱线图、hexbin 和 kde）的代码片段对。运行列表 5.27 中的代码，你将看到以下输出：

```py
 => Histogram of Rainfall:
    cent_floor  count 0            0     14
1            5     13
2           10      4
3           15     10
4           20      3
5           25      6
6           30      3
7           35      6
8           40      2
9           45      1
10          50      1
11          55      1
12          60      1 
```

除了前面的输出外，你还会在同一目录中看到以下文件，其中包含了运行列表 5.27 中的代码的位置：

```py
 rainfall_histogram.tiff
rainfall_pie.png
rainfall_line.png
rainfall_scatter.png
rainfall_box.png
rainfall_hexbin.png
rainfall_kde.png 
```

### **总结**

本章从对 Matplotlib 的简要介绍开始，同时提供了显示 Matplotlib 中可用颜色的代码示例。

然后你学习了如何绘制水平线、斜线、平行线以及点阵网格。此外，你还学习了如何加载图像、显示棋盘图案以及绘制三角函数图。你同样看到了如何绘制直方图、条形图、饼图和热力图。

接下来，你看到了如何创建 3D 图，以及如何绘制金融数据和来自 sqlite3 数据库的图表。

## 第六章

## **Seaborn 数据可视化**

本章介绍了几个数据可视化工具，包括 Seaborn、Bokeh 和 YellowBrick。本章还温和地介绍了 Scikit-learn（通常导入为 sklearn）。

本章的第一部分介绍了用于数据可视化的 Seaborn，它位于 Matplotlib 之上。尽管 Seaborn 并不包含 Matplotlib 中所有可用的功能，但它提供了一套更易于使用的 API 来渲染图表和图形。

本章的第二部分包含了对 Bokeh 的简要介绍，以及一个代码示例，展示了如何在 Bokeh 中轻松创建更具艺术效果的图形。

本章的第三部分介绍了 Scikit-learn，这是一个非常强大的 Python 库，支持许多机器学习算法，同时也支持可视化。如果你是机器学习的新手，不必担心：*本节不需要机器学习背景知识即可理解 Python 代码示例。*

### **使用 Seaborn 进行绘图**

Seaborn 是一个用于数据可视化的 Python 库，同时也提供了一个高级接口用于 Matplotlib。与 Matplotlib 相比，Seaborn 更易于使用，实际上它扩展了 Matplotlib，但请注意，Seaborn 的功能并不及 Matplotlib 强大。

Seaborn 解决了 Matplotlib 的两个挑战。第一个涉及默认的 Matplotlib 参数。Seaborn 使用不同的参数，这比 Matplotlib 默认渲染的图表提供了更大的灵活性。Seaborn 解决了 Matplotlib 默认值在颜色、上下轴的刻度标记以及样式（等等）等方面的局限性。

此外，Seaborn 使绘制整个数据框（类似于 Pandas）比在 Matplotlib 中这样做更加容易。尽管如此，由于 Seaborn 扩展了 Matplotlib，了解后者是有益的，并且将简化你的学习曲线。

#### **Seaborn 的特性**

Seaborn 提供了一套很好的特性和有用的方法来控制数据的显示，其中一些列在这里：

+   缩放 Seaborn 图表

+   设置绘图样式

+   设置图形大小

+   旋转标签文本

+   设置 xlim 或 ylim

+   设置对数刻度

+   添加标题

列出一些有用的 Seaborn 方法：

+   plt.xlabel()

+   plt.ylabel()

+   plt.annotate()

+   plt.legend()

+   plt.ylim()

+   plt.savefig()

Seaborn 支持各种内置数据集，就像 NumPy 和 Pandas 一样，包括 Iris 数据集和泰坦尼克号数据集，这些数据集你将在后续章节中看到。作为一个起点，下一节包含显示 Seaborn 中所有可用内置数据集的代码。

### **SEABORN 数据集名称**

列表 6.1 显示了 dataset_names.py 的内容，该文件显示了 Seaborn 的内置数据集，其中我们将使用其中一个在 Seaborn 中渲染热图。

***列表 6.1：dataset_names.py***

```py
 import seaborn as sns

names = sns.get_dataset_names()
for name in names:
  print("name:",name) 
```

列表 6.1 包含一个导入语句，然后是变量 names，它被初始化为 Seaborn 中内置数据集名称的集合。下一部分包含一个循环，遍历变量 names 中的数据集名称并显示它们的值。运行 列表 6.1 中的代码，你将看到以下输出：

```py
 name: anagrams
name: anscombe
name: attention
name: brain_networks
name: car_crashes
name: diamonds
name: dots
name: exercise
name: flights
name: fmri
name: gammas
name: geyser
name: iris
name: mpg
name: penguins
name: planets
name: taxis
name: tips
name: titanic 
```

下一节中的三行代码示例展示了如何显示内置“tips”数据集中的行。

### **SEABORN 内置数据集**

列表 6.2 显示了 seaborn_tips.py 的内容，该文件说明了如何将 tips 数据集读入数据框并显示数据集的前五行。

***列表 6.2：seaborn_tips.py***

```py
 import seaborn as sns

df = sns.load_dataset("tips")
print(df.head()) 
```

列表 6.2 非常简单：在导入 seaborn 之后，变量 df 被初始化为内置数据集 tips 中的数据，并且 print() 语句显示了 df 的前五行。请注意，load_dataset() API 会搜索在线或内置数据集。列表 6.2 的输出如下：

```py
 total_bill   tip     sex smoker  day    time  size
0       16.99  1.01  Female     No  Sun  Dinner     2
1       10.34  1.66    Male     No  Sun  Dinner     3 2       21.01  3.50    Male     No  Sun  Dinner     3
3       23.68  3.31    Male     No  Sun  Dinner     2
4       24.59  3.61  Female     No  Sun  Dinner     4 
```

### **SEABORN 中的鸢尾花数据集**

列表 6.3 展示了 seaborn_iris.py 的内容，该文件说明了如何绘制鸢尾花数据集。

***列表 6.2：seaborn_iris.py***

```py
 import seaborn as sns
import matplotlib.pyplot as plt

# Load iris data
iris = sns.load_dataset("iris")

# Construct iris plot
sns.swarmplot(x="species", y="petal_length", data=iris)

# Show plot
plt.show() 
```

列表 6.3 导入了 Seaborn 和 matplotlib.pyplot，然后使用内置的 Iris 数据集初始化变量 iris。接下来，swarmplot() API 显示了一个图表，其中水平轴标记为物种，垂直轴标记为花瓣长度，显示的点来自 Iris 数据集。

图 6.1 显示了基于 列表 6.3 中的代码的 Iris 数据集中的图像。

![图像](img/python-3-data-visualization-using-chatgpt-f0192-01.jpg)

***图 6.1*** 鸢尾花数据集。

### **SEABORN 中的泰坦尼克号数据集**

列表 6.4 展示了 seaborn_titanic_plot.py 的内容，该文件说明了如何绘制泰坦尼克号数据集。

***列表 6.4：seaborn_titanic_plot.py***

```py
 import matplotlib.pyplot as plt
import seaborn as sns

titanic = sns.load_dataset("titanic")
g = sns.factorplot("class", "survived", "sex", data=titanic, kind="bar", palette="muted", legend=False)

plt.show() 
```

列表 6.4 包含与 列表 6.3 相同的导入语句，然后初始化变量 titanic 为内置的泰坦尼克号数据集的内容。接下来，factorplot() API 显示了一个图表，其中包含 API 调用中列出的数据集属性。图 6.2 显示了基于 列表 6.4 中的代码的泰坦尼克号数据集的图表。

![图像](img/python-3-data-visualization-using-chatgpt-f0193-01.jpg)

***图 6.2*** 泰坦尼克号数据集的直方图。

### **在 Seaborn 中从泰坦尼克号数据集中提取数据（1）**

列表 6.5 显示了 seaborn_titanic.py 的内容，该内容说明了如何从泰坦尼克号数据集中提取数据子集。

***列表 6.5: seaborn_titanic.py***

```py
 import matplotlib.pyplot as plt
import seaborn as sns

titanic = sns.load_dataset("titanic")
print("titanic info:")
titanic.info()

print("first five rows of titanic:")
print(titanic.head())

print("first four ages:")
print(titanic.loc[0:3,'age'])

print("fifth passenger:")
print(titanic.iloc[4])

#print("first five ages:")
#print(titanic['age'].head())

#print("first five ages and gender:")
#print(titanic[['age','sex']].head())

#print("descending ages:")
#print(titanic.sort_values('age', ascending = False).head())

#print("older than 50:")
#print(titanic[titanic['age'] > 50])

#print("embarked (unique):")
#print(titanic['embarked'].unique())

#print("survivor counts:")
#print(titanic['survived'].value_counts())

#print("counts per class:")
#print(titanic['pclass'].value_counts())

#print("max/min/mean/median ages:")
#print(titanic['age'].max())
#print(titanic['age'].min())
#print(titanic['age'].mean())
#print(titanic['age'].median()) 
```

列表 6.5 包含与 列表 6.4 相同的导入语句，然后初始化变量 titanic 为内置的泰坦尼克号数据集的内容。列表 6.5 的下一部分显示了泰坦尼克号数据集的各个方面，如其结构、前五行、前四个年龄和第五个乘客的详细信息。

如您所见，有一大块“注释掉的”代码可以取消注释，以查看相关的输出，例如年龄、性别、50 岁以上的人、唯一行等等。列表 6.5 的输出如下：

```py
#print(titanic['age'].mean())
titanic info:
<class 'pandas.core.frame.Data frame'>
RangeIndex: 891 entries, 0 to 890
Data columns (total 15 columns):
survived       891 non-null int64
pclass         891 non-null int64
sex            891 non-null object
age            714 non-null float64
sibsp          891 non-null int64
parch          891 non-null int64
fare           891 non-null float64
embarked       889 non-null object
class          891 non-null category
who            891 non-null object
adult_male     891 non-null bool
deck           203 non-null category
embark_town    889 non-null object
alive          891 non-null object
alone          891 non-null bool
dtypes: bool(2), category(2), float64(2), int64(4), object(5)
memory usage: 80.6+ KB
first five rows of titanic:
   survived  pclass     sex     age  sibsp  parch     fare embarked  class \
0         0       3    male  22.0      1      0   7.2500       S  Third
1         1       1  female  38.0      1      0  71.2833       C  First
2         1       3  female  26.0      0      0   7.9250       S  Third
3         1       1  female  35.0      1      0  53.1000       S  First
4         0       3    male  35.0      0      0   8.0500       S  Third

     who  adult_male deck  embark_town alive  alone
0    man        True  NaN  Southampton    no  False
1  woman       False    C    Cherbourg   yes  False
2  woman       False  NaN  Southampton   yes   True
3  woman       False    C  Southampton   yes  False
4    man        True  NaN  Southampton    no   True
first four ages:
0    22.0
1    38.0
2    26.0
3    35.0
Name: age, dtype: float64
fifth passenger:
survived                 0
pclass                   3
sex                   male
age                     35
sibsp                    0
parch                    0
fare                  8.05
embarked                 S
class                Third
who                    man
adult_male            True
deck                   NaN
embark_town    Southampton
alive                   no
alone                 True
Name: 4, dtype: object
counts per class: 3    491
1    216
2    184
Name: pclass, dtype: int64
max/min/mean/median ages:
80.0
0.42
29.69911764705882
28.0 
```

### **在 Seaborn 中从泰坦尼克号数据集中提取数据（2）**

列表 6.6 显示了 seaborn_titanic2.py 的内容，该内容说明了如何从泰坦尼克号数据集中提取数据子集。

***列表 6.6: seaborn_titanic2.py***

```py
 import matplotlib.pyplot as plt
import seaborn as sns

titanic = sns.load_dataset("titanic")

# Returns a scalar
# titanic.ix[4, 'age']
print("age:",titanic.at[4, 'age'])

# Returns a Series of name 'age', and the age values associated
# to the index labels 4 and 5
# titanic.ix[[4, 5], 'age']
print("series:",titanic.loc[[4, 5], 'age'])

# Returns a Series of name '4', and the age and fare values
# associated to that row. # titanic.ix[4, ['age', 'fare']]
print("series:",titanic.loc[4, ['age', 'fare']])

# Returns a Data frame with rows 4 and 5, and columns 'age' and 'fare'
# titanic.ix[[4, 5], ['age', 'fare']]
print("data frame:",titanic.loc[[4, 5], ['age', 'fare']])

query = titanic[
    (titanic.sex == 'female')
    & (titanic['class'].isin(['First', 'Third']))
    & (titanic.age > 30)
    & (titanic.survived == 0)
]
print("query:",query) 
```

列表 6.6 包含与 列表 6.5 相同的导入语句，然后初始化变量 titanic 为内置的泰坦尼克号数据集的内容。下一个代码片段显示了数据集中索引为 4 的乘客的年龄（等于 35）。

下一个代码片段显示了数据集中索引值为 4 和 5 的乘客的年龄：

```py
 print("series:",titanic.loc[[4, 5], 'age']) 
```

下一个代码片段显示了数据集中索引为 4 的乘客的年龄和票价，随后另一个代码片段显示了数据集中索引为 4 和 5 的乘客的年龄和票价。

列表 6.6 的最后一部分是最有趣的部分：它定义了一个变量 query，如下所示：

```py
 query = titanic[
    (titanic.sex == 'female')
    & (titanic['class'].isin(['First', 'Third']))
    & (titanic.age > 30)
    & (titanic.survived == 0)
] 
```

前面的代码块将检索在头等舱或三等舱中，且年龄超过 30 岁，且未在事故中幸存的女性乘客。列表 6.6 的完整输出如下：

```py
 age: 35.0
series: 4    35.0
5     NaN
Name: age, dtype: float64
series: age       35
fare    8.05
Name: 4, dtype: object
data frame:     age    fare
4  35.0  8.0500
5   NaN  8.4583
query:      survived  pclass     sex   age  sibsp  parch     fare embarked  class  \
18          0       3  female  31.0      1      0  18.0000        S  Third
40          0       3  female  40.0      1      0   9.4750        S  Third
132         0       3  female  47.0      1      0  14.5000        S  Third
167         0       3  female  45.0      1      4  27.9000        S  Third
177         0       1  female  50.0      0      0  28.7125        C  First
254         0       3  female  41.0      0      2  20.2125        S  Third
276         0       3  female  45.0      0      0   7.7500        S  Third
362         0       3  female  45.0      0      1  14.4542        C  Third
396         0       3  female  31.0      0      0   7.8542        S  Third 503         0       3  female  37.0      0      0   9.5875        S  Third
610         0       3  female  39.0      1      5  31.2750        S  Third
638         0       3  female  41.0      0      5  39.6875        S  Third
657         0       3  female  32.0      1      1  15.5000        Q  Third
678         0       3  female  43.0      1      6  46.9000        S  Third
736         0       3  female  48.0      1      3  34.3750        S  Third
767         0       3  female  30.5      0      0   7.7500        Q  Third
885         0       3  female  39.0      0      5  29.1250        Q  Third 
```

### **在 Seaborn 中可视化 Pandas 数据集**

列表 6.7 显示了 pandas_seaborn.py 的内容，该内容说明了如何在 Seaborn 中显示 Pandas 数据集。

***列表 6.7: pandas_seaborn.py***

```py
 import pandas as pd
import random
import matplotlib.pyplot as plt
import seaborn as sns

df = pd.Data frame()

df['x'] = random.sample(range(1, 100), 25)
df['y'] = random.sample(range(1, 100), 25)

print("top five elements:")
print(df.head())

# display a density plot
#sns.kdeplot(df.y)

# display a density plot
#sns.kdeplot(df.y, df.x)

#sns.distplot(df.x)

# display a histogram
#plt.hist(df.x, alpha=.3)
#sns.rugplot(df.x)

# display a boxplot
#sns.boxplot([df.y, df.x])

# display a violin plot
#sns.violinplot([df.y, df.x])

# display a heatmap
#sns.heatmap([df.y, df.x], annot=True, fmt="d")

# display a cluster map
#sns.clustermap(df) # display a scatterplot of the data points
sns.lmplot('x', 'y', data=df, fit_reg=False)
plt.show() 
```

列表 6.7 包含几个熟悉的导入语句，然后初始化 Pandas 变量 df 为 Pandas DataFrame。下一个代码片段初始化数据框的列和行，并使用 print() 语句显示前五行。

为了您的方便，列表 6.7 包含了一系列“注释掉的”代码片段，这些片段使用 Seaborn 来渲染密度图、直方图、箱线图、小提琴图、热图和聚类图。取消注释您感兴趣的代码部分，以查看相关的图表。列表 6.7 的输出如下：

```py
 top five elements:
    x   y
0  52  34
1  31  47
2  23  18
3  34  70
4  71   1 
```

图 6.3 显示了基于 列表 6.7 中的代码在泰坦尼克号数据集中的数据图。

![图片](img/python-3-data-visualization-using-chatgpt-f0199-01.jpg)

***图 6.3*** 通过 Seaborn 显示的 Pandas DataFrame。

### **SEABORN 热图**

列表 6.8 显示了显示 Seaborn 内置数据集热图的 heatmap1.py 的内容。

***列表 6.8：heatmap1.py***

```py
 import seaborn as sns
import matplotlib.pyplot as plt

data = sns.load_dataset("flights")
data = data.pivot("month", "year", "passengers")

print("data.head():")
print(data.head())

sns.heatmap(data)
plt.show() 
```

列表 6.8 包含两个导入语句，接着是变量 data，它被初始化为名为 flights 的 Seaborn 内置数据集的内容。下一个代码片段调用 pivot() 方法，从数据集中选择 month、year 和 passengers 属性。接下来的代码部分显示数据集的前五行，然后是一个渲染热图的代码块，你将看到以下输出：

```py
 data.head():
year   1949  1950  1951  1952  1953  1954  1955  1956  1957  1958  1959  1960
month
Jan     112   115   145   171   196   204   242   284   315   340   360   417
Feb     118   126   150   180   196   188   233   277   301   318   342   391
Mar     132   141   178   193   236   235   267   317   356   362   406   419
Apr     129   135   163   181   235   227   269   313   348   348   396   461
May     121   125   172   183   229   234   270   318   355   363   420   472 
```

图 6.4 显示了基于 列表 6.8 中的代码的 flights 数据集中的热图。

![图片](img/python-3-data-visualization-using-chatgpt-f0200-01.jpg)

***图 6.4*** 以 Seaborn 热图形式显示的 Pandas DataFrame。

### **SEABORN 配对图**

本节包含几个基于 Python 的代码示例，展示了如何使用 Seaborn 的 pair_plot() 方法来渲染配对图。

列表 6.9 显示了显示 Iris 数据集配对图的 seborn_pairplot1.py 的内容。

***列表 6.9：seaborn_pairplot1.py***

```py
 import seaborn as sns
import pandas as pd
import matplotlib.pyplot as plt

# load iris data
iris = sns.load_dataset("iris")

df = pd.Data frame(iris)

# construct and display iris plot
g = sns.pairplot(df, height=2, aspect=1.0)
plt.show() 
```

列表 6.9 从导入语句开始，接着是变量 iris，它被初始化为 Seaborn 内置数据集 iris 的内容。接下来的代码片段将变量 df 初始化为数据集的内容。最后的代码块基于变量 df 的内容生成一个配对图，并显示该配对图。图 6.5 显示了基于 列表 6.9 中的代码的 iris 数据集中的数据图。

![图片](img/python-3-data-visualization-using-chatgpt-f0201-01.jpg)

***图 6.5*** Seaborn 配对图。

列表 6.10 显示了渲染 Iris 数据集配对图的 seborn_pairplot12.py 的内容。

***列表 6.10：seaborn_pairplot2.py***

```py
 import seaborn as sns
import pandas as pd
import matplotlib.pyplot as plt

# load iris data
iris = sns.load_dataset("iris")

df = pd.Data frame(iris)

# IRIS columns:
# sepal_length,sepal_width,petal_length,petal_width,species

# plot a subset of columns:
plot_columns = ['sepal_length', 'sepal_width']
sns.pairplot(df[plot_columns])
plt.show()

# specify KDE for the diagonal:
sns.pairplot(df[plot_columns], diag_kind='kde')
plt.show() 
```

列表 6.10 从与 列表 6.9 相同的代码开始，接着是包含 iris 数据集中与花瓣相关的属性的变量 plot_columns。下一个代码块生成一个配对图并显示其内容，然后是一个生成具有 diag_kind 等于 kde 参数的配对图的代码片段。

图 6.6 显示了基于 列表 6.10 中的代码的 iris 数据集中的配对图。

![图片](img/python-3-data-visualization-using-chatgpt-f0202-01.jpg)

***图 6.6*** Iris 数据集的 Seaborn 配对图。

图 6.7 显示了基于 列表 6.10 中的代码的 iris 数据集中具有 kde 属性值的配对图。

![图片](img/python-3-data-visualization-using-chatgpt-f0203-01.jpg)

***图 6.7*** 带有 kde 选项的 Iris 数据集的 Seaborn 配对图。

### **什么是 BOKEH？**

Bokeh 是一个开源项目，它依赖于 Matplotlib 以及 Scikit-learn。正如你将在后续的代码示例中看到的那样，Bokeh 生成一个基于 Python 代码的 HTML 网页，然后在浏览器中打开该网页。Bokeh 和 D3.js（它是 SVG 之上的 JavaScript 抽象层）都提供了优雅的视觉效果，支持动画效果和用户交互。

Bokeh 能够快速创建统计可视化，并且与 Python Flask 和 Django 等其他工具一起工作。除了 Python 之外，Bokeh 还支持 Julia、Lua 和 R（生成 JSON 文件而不是 HTML 网页）。

列表 6.11 展示了 bokeh_trig.py 的内容，该内容说明了如何使用各种 Bokeh API 创建图形效果。

***列表 6.11: bokeh_trig.py***

```py
 # pip3 install bokeh
from bokeh.plotting import figure, output_file, show
from bokeh.layouts import column
import bokeh.colors as colors
import numpy as np
import math deltaY = 0.01
maxCount = 150
width  = 800
height = 400
band_width = maxCount/3

x = np.arange(0, math.pi*3, 0.05)
y1 = np.sin(x)
y2 = np.cos(x)

white = colors.RGB(255,255,255)

fig1 = figure(plot_width = width, plot_height = height)

for i in range(0,maxCount):
  rgb1 = colors.RGB(i*255/maxCount, 0, 0)
  rgb2 = colors.RGB(i*255/maxCount, i*255/maxCount, 0)
  fig1.line(x, y1-i*deltaY,line_width = 2, line_color = rgb1)
  fig1.line(x, y2-i*deltaY,line_width = 2, line_color = rgb2)

for i in range(0,maxCount):
  rgb1 = colors.RGB(0, 0, i*255/maxCount)
  rgb2 = colors.RGB(0, i*255/maxCount, 0)
  fig1.line(x, y1+i*deltaY,line_width = 2, line_color = rgb1)
  fig1.line(x, y2+i*deltaY,line_width = 2, line_color = rgb2)
  if (i % band_width == 0):
    fig1.line(x, y1+i*deltaY,line_width = 5, line_color = white)

show(fig1) 
```

列表 6.11 以一个注释掉的 pip3 代码片段开始，你可以从命令行启动它来安装 Bokeh（如果你还没有这样做的话）。

下一个代码块包含几个与 Bokeh 相关的语句以及 NumPy 和 Math。

注意，变量 white 被定义为表示颜色红色、绿色和蓝色成分的整数 (R,G,B) 三元组。特别是，(255,255,255) 代表白色（如果你不熟悉 RGB，请在线检查）。列表 6.11 的下一部分初始化了一些标量变量，这些变量用于列表 6.11 第二半部分的两个 for 循环中。

接下来，NumPy 变量 x 是从 0 到 math.PI/3 的值范围，相邻值之间的增量是 0.05。然后，NumPy 变量 y1 和 y2 分别定义为 x 中值的正弦和余弦值。接下来的代码片段初始化了变量 fig1，它代表图形效果将被渲染的上下文。这完成了在两个 for 循环中使用的变量的初始化。

列表 6.11 的下一部分包含第一个 for 循环，通过定义基于循环变量 i 的值的 (R,G,B) 三元组来创建类似渐变的视觉效果。例如，变量 rgb1 以线性方式从 (0,0,0) 到 (255,0,0) 变化，分别代表黑色和红色。变量 rgb2 以线性方式从 (0,0,0) 到 (255,255,0) 变化，分别代表黑色和黄色。for 循环的下一部分包含两次对 fig1.line() API 的调用，在上下文变量 fig1 中渲染正弦波和余弦波。

第二个 for 循环与第一个 for 循环类似：主要区别是变量 rgb1 从黑色变为蓝色，而变量 rgb2 从黑色变为绿色。列表 6.13 的最后代码片段调用了 show() 方法，该方法生成一个基于 Python 代码的 HTML 网页（与 Python 文件具有相同的名称前缀），然后在浏览器中打开该网页。

图 6.8 显示了基于列表 6.11 中代码的图形效果。如果这个图像以黑白显示，请在命令行中运行代码，你将看到图像中的渐变效果。

![图片](img/python-3-data-visualization-using-chatgpt-f0205-01.jpg)

***图 6.8*** 一个 Bokeh 图形示例。

下一节将向您介绍 Scikit-learn，这是一个基于 Python 的强大库，支持许多机器学习算法。在阅读简短介绍之后，后续章节将包含结合 Pandas、Matplotlib 和 Scikit-learn 内置数据集的 Python 代码示例。

### **Scikit-learn 简介**

由于这本书是关于数据可视化的，你可能想知道为什么这一章包含了 Scikit-learn（也称为 Sklearn）的介绍。原因很简单：在不进行更正式的学习过程的情况下，可以轻松地介绍一些 Scikit-learn 的功能。此外，如果你决定深入研究机器学习（也许这一节将提供额外的动力去做），这些知识将大有裨益。

然而，对 Scikit-learn 的深入了解需要显著更多的时间和努力，尤其是如果你计划学习 Scikit-learn 机器学习算法的细节。另一方面，如果你目前对学习 Scikit-learn 不感兴趣，你可以跳过这一节，也许在你对学习这些材料感兴趣时再回来。

Scikit-learn 是 Python 的顶级通用机器学习库，其主页在这里：

[`scikit-learn.org/stable/`](https://scikit-learn.org/stable/)

在我们讨论任何代码示例之前，请记住 Scikit-learn 是一个极其有用的 Python 库，支持大量的机器学习算法。特别是，Scikit-learn 支持许多分类算法，如逻辑回归、朴素贝叶斯、决策树、随机森林和 SVMs（支持向量机）。尽管有专门介绍 Scikit-learn 的整本书，但本章只包含 Scikit-learn 材料的几页。

如果你决定想要深入掌握 Scikit-learn 的知识，请导航到包含 Scikit-learn 非常详细文档的网页。此外，如果你有关于 Scikit-learn 的“如何做”的问题，你几乎总能找到合适的答案在 Stack Overflow（[`stackoverflow.com/`](https://stackoverflow.com/)*）上。

Scikit-learn 非常适合机器学习中的分类任务，以及回归和聚类任务。Scikit-learn 支持大量的机器学习算法，包括线性回归、逻辑回归、kNN（“K 最近邻”）、kMeans、决策树、随机森林、MLPs（多层感知器）和 SVMs（支持向量机）。

此外，Scikit-learn 支持降维技术，如 PCA（主成分分析）、“超参数”调整、数据缩放方法，并且适用于数据预处理、交叉验证等。

机器学习代码示例通常包含 Scikit-learn、NumPy、Pandas 和 Matplotlib 的组合。此外，Scikit-learn 提供了各种内置数据集，我们可以通过可视化来展示。其中之一是 Digits 数据集，这是下一节的主题。

本章的下一段提供了几个 Python 代码示例，这些示例包含了 Pandas、Matplotlib 和 Scikit-learn 内置的 Digits 数据集的组合。

### **Scikit-learn 中的 Digits 数据集**

Scikit-learn 中的 Digits 数据集包含 1797 个小的 8x8 图像：每个图像都是一个手写的数字，这与 MNIST 数据集的情况相同。列表 6.12 展示了 load_digits1.py 的内容，说明了如何在 Digits 数据集中绘制一个数字。

***列表 6.12：load_digits1.py***

```py
 from scikit-learn import datasets

# Load in the 'digits' data
digits = datasets.load_digits()

# Print the 'digits' data
print(digits) 
```

列表 6.12 非常简单：在导入 datasets 模块后，变量 digits 被初始化为 Digits 数据集的内容。print() 语句显示了 digits 变量的内容，如下所示：

```py
 {images': array(
     [[[0.,   0.,   5., ...,       1.,    0.,   0.],
       [0.,   0.,  13., ...,  15.,   5.,   0.],
       [0.,   3.,  15., ...,  11.,   8.,   0.],
       ...,
       [0.,   4.,  11., ...,  12.,   7.,   0.],
       [0.,   2.,  14., ...,  12.,   0.,   0.],
       [0.,   0.,   6., ...,   0.,   0.,   0.]]),
'target': array([0, 1, 2, ..., 8, 9, 8]), 'frame': None, 'feature_names': ['pixel_0_0', 'pixel_0_1', 'pixel_0_2', 'pixel_0_3', 'pixel_0_4', 'pixel_0_5', 'pixel_0_6', 'pixel_0_7',
'pixel_1_0', 'pixel_1_1', 'pixel_1_2', 'pixel_1_3', 'pixel_1_4', 'pixel_1_5', 'pixel_1_6', 'pixel_1_7',
'pixel_2_0', 'pixel_2_1', 'pixel_2_2', 'pixel_2_3', 'pixel_2_4', 'pixel_2_5', 'pixel_2_6', 'pixel_2_7',
'pixel_3_0', 'pixel_3_1', 'pixel_3_2', 'pixel_3_3', 'pixel_3_4', 'pixel_3_5', 'pixel_3_6', 'pixel_3_7',
'pixel_4_0', 'pixel_4_1', 'pixel_4_2', 'pixel_4_3', 'pixel_4_4', 'pixel_4_5', 'pixel_4_6', 'pixel_4_7',
'pixel_5_0', 'pixel_5_1', 'pixel_5_2', 'pixel_5_3', 'pixel_5_4', 'pixel_5_5', 'pixel_5_6', 'pixel_5_7',
'pixel_6_0', 'pixel_6_1', 'pixel_6_2', 'pixel_6_3', 'pixel_6_4', 'pixel_6_5', 'pixel_6_6', 'pixel_6_7',
'pixel_7_0', 'pixel_7_1', 'pixel_7_2', 'pixel_7_3', 'pixel_7_4', 'pixel_7_5', 'pixel_7_6', 'pixel_7_7'],
'target_names': array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9]), 'images':
array([[[ 0.,  0.,  5., ...,  1.,  0.,  0.],
        [ 0.,  0., 13., ..., 15.,  5.,  0.],
        [ 0.,  3., 15., ..., 11.,  8.,  0.],
// data omitted for brevity
])} 
```

列表 6.13 展示了 load_digits2.py 的内容，说明了如何在 Digits 数据集中绘制一个数字（你可以更改它以显示不同的数字）。

***列表 6.13：load_digits2.py***

```py
 from sklearn.datasets import load_digits
from matplotlib import pyplot as plt

digits = load_digits()
#set interpolation='none' fig = plt.figure(figsize=(3, 3))
plt.imshow(digits['images'][66], cmap="gray", interpolation='none')
plt.show() 
```

列表 6.13 从 Scikit-learn 导入 load_digits 类，以便用 Scikit-learn 中可用的 Digits 数据集的内容初始化变量 digits。列表 6.13 的下一部分初始化变量 fig，并调用 plt 类的 imshow() 方法来显示 Digits 数据集中的数字。

图 6.9 展示了基于 列表 6.13 中的代码的 Digits 数据集中一个数字的绘图。

![图片](img/python-3-data-visualization-using-chatgpt-f0208-01.jpg)

***图 6.9*** Scikit-learn Digits 数据集中的数字。

列表 6.14 展示了 load_digits3.py 的内容，说明了如何在 Scikit-learn 中访问 Digits 数据集。

***列表 6.14：load_digits3.py***

```py
 from sklearn import datasets

digits = datasets.load_digits()
print("digits shape:",digits.images.shape)
print("data   shape:",digits.data.shape)

n_samples, n_features = digits.data.shape
print("(samples,features):", (n_samples, n_features))

import matplotlib.pyplot as plt
#plt.imshow(digits.images[-1], cmap=plt.cm.gray_r)
#plt.show() plt.imshow(digits.images[0], cmap=plt.cm.binary, interpolation='nearest')
plt.show() 
```

列表 6.14 从一个导入语句开始，后面跟着变量 digits，它包含 Digits 数据集。列表 6.16 的输出如下：

```py
 digits shape: (1797, 8, 8)
data   shape: (1797, 64)
(samples,features): (1797, 64) 
```

图 6.10 展示了基于 列表 6.14 中的代码的 Digits 数据集中的图像。

![图片](img/python-3-data-visualization-using-chatgpt-f0209-01.jpg)

***图 6.10*** Digits 数据集中的数字。

### **Scikit-learn 中的 Iris 数据集**

列表 6.15 展示了 sklearn_iris.py 的内容，说明了如何在 Scikit-learn 中访问 Iris 数据集。

除了支持机器学习算法外，Scikit-learn 还提供了各种内置数据集，您只需一行代码即可访问。实际上，列表 6.15 显示了 sklearn_iris1.py 的内容，说明了您如何轻松地将 Iris 数据集加载到 Pandas DataFrame 中。

***列表 6.15: sklearn_iris.py***

```py
 import numpy as np
import pandas as pd
from scikit-learn.datasets import load_iris iris = load_iris()

print("=> iris keys:")
for key in iris.keys():
  print(key)
print()

#print("iris dimensions:")
#print(iris.shape)
#print()

print("=> iris feature names:")
for feature in iris.feature_names:
  print(feature)
print()

X = iris.data[:, [2, 3]]
y = iris.target
print('=> Class labels:', np.unique(y))
print()

x_min, x_max = X[:, 0].min() - .5, X[:, 0].max() + .5
y_min, y_max = X[:, 1].min() - .5, X[:, 1].max() + .5

print("=> target:")
print(iris.target)
print()

print("=> all data:")
print(iris.data) 
```

列表 6.15 包含几个导入语句，然后使用 Iris 数据集初始化变量 iris。接下来，一个 for 循环显示数据集的键，然后另一个 for 循环显示特征名称。

列表 6.15 的下一部分初始化变量 X 为第 2 列和第 3 列的特征值，然后初始化变量 y 为目标列的值。

变量 x_min 被初始化为第 0 列的最小值，然后从 x_min 中减去额外的 0.5。同样，变量 x_max 被初始化为第 0 列的最大值，然后向 x_max 中添加额外的 0.5。变量 y_min 和 y_max 是 x_min 和 x_max 的对应物，应用于第 1 列而不是第 0 列。

运行 列表 6.15 中的代码，你将看到以下输出（为了节省空间已截断）：

```py
 Pandas df1:

=> iris keys:
data
target
target_names DESCR
feature_names
filename

=> iris feature names:
sepal length (cm)
sepal width (cm)
petal length (cm)
petal width (cm)

=> Class labels: [0 1 2]

=> x_min: 0.5 x_max: 7.4
=> y_min: -0.4 y_max: 3.0

=> target:
[0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0
 0 0 0 0 0 0 0 0 0 0 0 0 0 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1
 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 2 2 2 2 2 2 2 2 2 2 2
 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2
 2 2]

=> all data:
[[5.1 3.5 1.4 0.2]
 [4.9 3\. 1.4 0.2]
 [4.7 3.2 1.3 0.2]
 // details omitted for brevity
 [6.5 3\. 5.2 2\. ]
 [6.2 3.4 5.4 2.3]
 [5.9 3\. 5.1 1.8]] 
```

#### **Scikit-Learn、Pandas 和 Iris 数据集**

列表 6.16 显示了 pandas_iris.py 的内容，说明了如何将 Iris 数据集（来自 Scikit-learn）的内容加载到 Pandas DataFrame 中。

***列表 6.16: pandas_iris.py***

```py
 import numpy as np
import pandas as pd
from sklearn.datasets import load_iris

iris = load_iris()

print("=> IRIS feature names:")
for feature in iris.feature_names:
  print(feature)
print()

# Create a data frame with the feature variables
df = pd.Data frame(iris.data, columns=iris.feature_names)

print("=> number of rows:") print(len(df))
print()

print("=> number of columns:")
print(len(df.columns))
print()

print("=> number of rows and columns:")
print(df.shape)
print()

print("=> number of elements:")
print(df.size)
print()

print("=> IRIS details:")
print(df.info())
print()

print("=> top five rows:")
print(df.head())
print()

X = iris.data[:, [2, 3]]
y = iris.target
print('=> Class labels:', np.unique(y)) 
```

列表 6.16 包含几个导入语句，然后使用 Iris 数据集初始化变量 iris。接下来，一个 for 循环显示特征名称。接下来的代码片段初始化变量 df 为一个包含 Iris 数据集数据的 Pandas DataFrame。

下一段代码调用 Pandas DataFrame 的某些属性和方法来显示数据框中的行数、列数和元素数，以及 Iris 数据集的详细信息、前五行和 Iris 数据集中的唯一标签。运行 列表 6.16 中的代码，你将看到以下输出：

```py
 => IRIS feature names:
sepal length (cm)
sepal width (cm)
petal length (cm)
petal width (cm)

=> number of rows:
150

=> number of columns:
4

=> number of rows and columns:
(150, 4)
=> number of elements:

600 => IRIS details:
<class 'pandas.core.frame.Data frame'>
RangeIndex: 150 entries, 0 to 149
Data columns (total 4 columns):
sepal length (cm)    150 non-null float64
sepal width (cm)     150 non-null float64
petal length (cm)    150 non-null float64
petal width (cm)     150 non-null float64
dtypes: float64(4)
memory usage: 4.8 KB
None

=> top five rows:
   sepal length (cm)  sepal width (cm)  petal length (cm)  petal width (cm)
0                5.1               3.5                1.4               0.2
1                4.9               3.0                1.4               0.2
2                4.7               3.2                1.3               0.2
3                4.6               3.1                1.5               0.2
4                5.0               3.6                1.4               0.2

=> Class labels: [0 1 2] 
```

### **SEABORN 的高级主题**

列表 6.17 显示了 sns_kde_plot1.py 的内容，展示了 kde 图。

***列表 6.17: sns_kde_plot1.py***

```py
 import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

np.random.seed(1)
numerical_1 = np.random.randn(400)

np.random.seed(2)
numerical_2 = np.random.randn(400)

fig, ax = plt.subplots(figsize=(6,6))

sns.kdeplot(x=numerical_1,
            y= numerical_2,
            ax=ax,
            shade=True,
            color="blue",
            bw=1)
plt.show() 
```

列表 6.17 包含几个导入语句，然后使用一组 400 个随机生成的数字初始化变量 numerical_1 和 numerical_2。接下来的代码片段初始化与图形相关的变量 fig 和 ax。

下一个代码片段调用 Seaborn 的 kdeplot() 方法，并使用 numerical_1 和 numerical_2 中的值作为水平和垂直轴的值。最后的代码片段显示了由 kdeplot() 方法生成的图表。现在运行 列表 6.17 中的代码，你将看到生成的图表。

图 6.11 显示了基于 列表 6.17 中的代码的 Titanic 数据集中的数据图。

![图片](img/python-3-data-visualization-using-chatgpt-f0214-01.jpg)

***图 6.11*** 通过 Seaborn 显示的 Pandas DataFrame。

代码清单 6.18 显示了显示线图和条形图的 sns_line_barchart1.py 的内容。

***代码清单 6.18: sns_line_barchart1.py***

```py
 import numpy as np

import seaborn as sns
import matplotlib.pyplot as plt

sns.set(style="white", rc={"lines.linewidth": 3})
fig, ax1 = plt.subplots(figsize=(4,4))
ax2 = ax1.twinx()
sns.barplot(x=['A','B','C','D'],
            y=[100,200,135,98],
            color='#004488',
            ax=ax1)

sns.lineplot(x=['A','B','C','D'],
             y=[4,2,5,3],
             color='r', marker="o",
             ax=ax2)

plt.show() 
```

代码清单 6.18 包含几个导入语句，然后初始化与图形相关的变量 fig 和 ax，接着通过调用 ax1 的 twinx()方法初始化变量 ax2。

下两个代码块分别使用硬编码的 x 和 y 值生成条形图和折线图。下一个代码片段显示了生成的条形图和折线图。图 6.12 显示了代码清单 6.18 中数据的条形图和折线图。

![图片](img/python-3-data-visualization-using-chatgpt-f0215-01.jpg)

***图 6.12*** 条形图和折线图。

### **总结**

本章从 Seaborn 的一些基本功能开始，Seaborn 是 Matplotlib 的扩展。你看到了绘制线条和直方图的示例，以及如何使用 Seaborn 绘制 Pandas DataFrame。

接下来，你学习了 Bokeh，以及如何在 Bokeh 中渲染图形的示例。此外，你还学习了 SVG 以及如何渲染各种二维形状，例如线段、矩形、圆形、贝塞尔曲线和条形图。

你还学习了 Scikit-learn，包括使用 Digits 和 Iris 数据集的示例，以及如何处理图像。最后，你学习了如何在 Scikit-learn 中渲染条形图和折线图。

## 第七章

## *ChatGPT 和 GPT-4*

本章包含有关 ChatGPT 和 GPT-4 的主要功能以及一些竞争对手的信息。

本章的第一部分从生成式 AI 和对话式 AI 与生成式 AI 的本质区别开始介绍。本节还深入探讨了 ChatGPT，以及 ChatGPT 与 Google Search 的比较。你还将了解 ChatGPT 的定制指令、提示和 ChatGPT 游乐场。此外，你还将学习 ChatGPT 插件，如高级数据分析（以前称为代码解释器）和代码轻语者。

本章的第二部分讨论了关于 ChatGPT 的一些担忧，以及 ChatGPT 的优缺点。此外，你将了解 ChatGPT 的替代方案以及使用 VizGPT 进行数据可视化。

本章的第三部分深入探讨了 GPT-4，一些 GPT-4 的推理参数和微调。你还将了解一些竞争对手，如 CoPilot 和 Codex。本章的最后部分介绍了 LlaMa-2 以及如何在笔记本电脑上下载 LlaMa-2 以便你可以微调此模型。

### **什么是生成式 AI？**

*生成式 AI*是指一类人工智能模型和技术，旨在生成与给定输入数据在本质上相似的新数据样本。目标是产生原本不属于原始训练集的内容或数据，但内容连贯、上下文相关，且风格或结构相同。

生成式人工智能在创造和创新方面与众不同，而不是仅仅分析或分类。该领域的进步导致了创意领域和实际应用的突破，使其成为人工智能研究和开发的前沿领域。

#### **生成式人工智能的重要特性**

以下列表包含了生成式人工智能的重要特性，以及每个项目的简要描述：

+   数据生成

+   综合合成

+   学习分布

*数据生成*指的是创建新的数据点，这些数据点不是训练数据的一部分，但与其相似。这可能包括文本、图像、音乐、视频或其他形式的数据。*综合*意味着生成模型可以混合各种输入以生成包含每个输入特征的输出，例如合并两张图像的风格。*学习分布*意味着生成式人工智能模型旨在学习训练数据的概率分布，以便它们可以从该分布中生成新的样本。

#### **生成式人工智能中的流行技术**

生成对抗网络（GANs）由两个网络组成，一个生成器和一个判别器，它们同时进行训练。生成器试图生成假数据，而判别器试图区分真实数据和假数据。随着时间的推移，生成器在生成逼真数据方面变得越来越擅长。

变分自编码器（VAEs）是概率模型，它们学习以编码和解码数据的方式，使得编码表示可以用来生成新的数据样本。

循环神经网络（RNNs）主要用于序列生成，如文本或音乐。

#### **生成式人工智能的独特之处**

*创作与分类对比*：虽然大多数传统人工智能模型旨在将输入数据分类到预定义的类别中，但生成模型旨在创建新的数据。

*无监督学习*：许多生成模型，尤其是 GANs 和 VAEs，以无监督的方式运行，这意味着它们在训练时不需要标记数据。

*多样化输出*：生成模型可以根据学习到的分布产生各种输出，这使得它们非常适合艺术生成、风格迁移等任务。

*挑战*：生成式人工智能提出了独特的挑战，例如 GANs 中的模型崩溃或确保生成内容的连贯性。

此外，还有许多涉及生成式人工智能应用的领域，其中一些列在以下列表中：

+   艺术和音乐创作

+   数据增强

+   风格迁移

+   文本生成

+   图像合成

+   药物发现

*艺术和音乐创作*包括生成绘画、音乐或其他形式的艺术。

*数据增强*涉及为训练模型创建额外的数据，尤其是在原始数据集有限时。*风格迁移*指的是将一个图像的风格应用到另一个图像的内容上。*文本生成*是生成式人工智能的一个非常流行的应用，它涉及创建连贯且与上下文相关的文本。*图像合成*是生成式人工智能的另一个非常流行的领域，它涉及生成逼真的图像、面孔，甚至为视频游戏创建场景。*药物发现*是生成式人工智能的一个重要方面，涉及生成新潜在药物的分子的结构。

### **对话式人工智能与生成式人工智能**

对话式人工智能和生成式人工智能都是人工智能更广泛领域中的突出子领域。然而，这些子领域在它们的主要目标、使用的科技以及应用方面有不同的重点。

两个子领域之间的主要差异如下：

+   主要目标

+   应用

+   使用的科技

+   训练和交互

+   **评估**

+   数据需求

#### **主要目标**

对话式人工智能的主要目标是促进机器与人类之间类似人类的交互。这包括聊天机器人、虚拟助手以及其他与用户进行对话的系统。

生成式人工智能的主要目标是创建新的内容或数据，这些内容或数据不在训练集中，但在结构和风格上相似。这可以从生成图像、音乐和文本到更复杂的任务，如视频合成。

#### **应用**

生成式人工智能的常见应用包括客户支持聊天机器人、语音操作虚拟助手（如 Siri 或 Alexa）以及交互式语音响应（IVR）系统。

生成式人工智能的常见应用范围广泛，例如创作艺术或音乐、生成逼真的视频游戏环境、合成声音，以及生成逼真的图像甚至深度伪造。

#### **使用的科技**

对话式人工智能通常依赖于自然语言处理（NLP）技术来理解和生成人类语言。这包括意图识别、实体提取和对话管理。

生成式人工智能通常利用生成对抗网络（GANs）、变分自编码器（VAEs）和其他生成模型来生成新内容。

#### **训练和交互**

虽然训练可以是监督的、半监督的或无监督的，但对话式人工智能的主要交互模式是通过来回对话或交谈。

生成式人工智能的训练过程，特别是使用像 GANs 这样的模型，涉及迭代过程，其中模型通过试图欺骗判别器相信生成数据是真实的来学习生成数据。

#### **评估**

对话式人工智能的评估指标通常围绕理解与响应的准确性、用户满意度以及生成响应的流畅性。

对于 GANs 等模型，生成式 AI 的评价指标可能具有挑战性，可能需要结合定量指标和人类判断来评估生成内容的品质。

#### **数据需求**

对话式 AI 的数据需求通常涉及对话数据，包括人与人之间的对话或人与机器人之间的对话。

生成式 AI 的数据需求涉及大量它应该生成的内容的数据集，如图像、文本或音乐。

尽管对话式 AI 和生成式 AI 都涉及生成输出，但它们的主要目标、应用和方法可能存在显著差异。对话式 AI 是为了与用户进行交互式通信而开发的，而生成式 AI 是为了产生新的、原创的内容而设计的。

### **DALL-E 是否属于生成式 AI 的一部分？**

DALL-E 以及类似从文本生成图形的工具是生成式 AI 的例子。实际上，DALL-E 是图像合成领域中最突出的生成式 AI 例子之一。

下面是 DALL-E 的生成特性列表，以及每个项目点的简要描述：

+   图像生成

+   学习分布

+   创新组合

+   广泛应用

+   Transformer 架构

*图像生成*：这是 DALL-E 的一个关键特性，它被设计成根据文本描述生成图像。给定一个提示如“一个双头火烈鸟”，DALL-E 可以生成一个符合描述的新颖图像，即使它在训练数据中从未有过这样的图像。

*学习分布*：与其他生成模型一样，DALL-E 学习其训练数据的概率分布。当它生成图像时，它会从这个学习到的分布中采样，以产生基于其训练的合理视觉。

*创新组合*：DALL-E 可以生成代表完全新颖或抽象概念的图像，展示了其能够以创新的方式组合和重新组合学习元素的能力。

*广泛应用*：除了图像合成之外，DALL-E 还在艺术生成、风格融合以及创建具有特定属性或主题的图像等领域提供了广泛的应用支持，突显了其作为生成工具的多样性。

*Transformer 架构*：DALL-E 利用了 Transformer 架构的变体，类似于 GPT-3 等模型，但已被调整为适用于图像生成任务。

其他基于输入数据（无论是文本、另一张图像还是任何其他形式的数据）生成图形、艺术或任何形式视觉内容的工具也被认为是生成式 AI。它们展示了 AI 模型不仅能够分析和分类，还能够创造和创新。

### **ChatGPT-3 和 GPT-4 是否属于生成式 AI 的一部分？**

ChatGPT-3 和 GPT-4 都是被认为是生成人工智能的 LLMs。它们属于“转换器”模型类别，特别擅长处理数据序列，如文本相关任务。

以下列表提供了各种原因，说明为什么这些大型语言模型（LLMs）被认为是生成性的，随后对每个项目进行了简要描述：

+   文本生成

+   学习分布

+   广泛的应用

+   无监督学习

*文本生成*：这些模型可以根据给定的提示生成连贯、上下文相关且通常非常复杂的文本序列。它们生成的响应在它们的训练数据中并未明确存在，但基于它们在训练期间学习到的模式和结构构建。

*学习分布*：GPT-3、GPT-4 和类似模型学习其训练数据的概率分布。在生成文本时，它们实际上是从这个学习到的分布中进行采样，以产生基于其训练的序列。

*广泛的应用*：除了基于文本的聊天或对话之外，这些模型还可以用于各种生成任务，如故事写作、代码生成、诗歌，甚至创建特定风格的内容或模仿某些作者，展示了它们的生成能力。

*无监督学习*：虽然它们可以通过特定数据集进行微调，但像 GPT-3 这样的模型主要是通过大量文本进行无监督训练，学习生成内容，而不需要为每个可能的响应提供显式的标记数据。

从本质上讲，OpenAI 的 ChatGPT-3、GPT-4 以及类似的模型是自然语言处理和生成领域中生成人工智能的典范。

下几节简要介绍了一些在人工智能领域具有强大影响力的公司。

### **DEEPMIND**

DeepMind 在人工智能领域做出了重大贡献，包括创建各种人工智能系统。DeepMind 成立于 2010 年，并于 2014 年成为谷歌的子公司，其主页为*[`deepmind.com/`](https://deepmind.com/)*。

DeepMind 创建了 280 GB 的语言模型 Gopher，其性能显著优于其竞争对手，包括 GPT-3、J1-Jumbo 和 MT-NLG。DeepMind 还开发了 AlphaFold，该系统在仅用 30 分钟内解决了困扰研究人员十年的蛋白质折叠问题。此外，DeepMind 在 2021 年 7 月将 AlphaFold 免费提供给每个人。DeepMind 在开发世界级人工智能游戏系统方面做出了重大贡献，其中一些将在下一节中讨论。

#### **DeepMind 与游戏**

DeepMind 是 AI 系统 AlphaStar 和 AlphaGo 背后的力量，这些系统击败了围棋（比象棋更难）的最佳人类玩家。这些游戏提供“完美信息”，而“不完美信息”游戏（如扑克）对机器学习模型构成了挑战。

AlphaGo Zero（AlphaGo 的后继者）在更短的时间内，使用比 AlphaGo 更少的计算能力掌握了游戏。AlphaGo Zero 通过以 100-0 的成绩击败 AlphaGo，展现了非凡的表现。另一个强大的系统是 AlphaZero，它也使用了自我对弈技术来学习围棋、象棋和国际象棋，并实现了 SOTA（最高水平）的性能结果。

通过比较，使用树搜索的 ML 模型非常适合完美信息游戏。相比之下，不完美信息游戏（如扑克）涉及隐藏信息，可以利用这些信息制定对抗策略来对抗对手的策略。特别是，AlphaStar 能够与星际争霸 II 的最佳玩家对战，并成为第一个在需要所谓“战略能力”的游戏中实现 SOTA 结果的 AI。

#### **玩家游戏（PoG**）

谷歌 DeepMind 团队设计了基于以下技术的通用 PoG（玩家游戏）算法：

+   CFR（反事实后悔最小化）

+   CVPN（反事实值和政策网络）

+   GT-CFT（增长树 CFR）

+   CVPN

反事实值和政策网络（CVPN）是一个神经网络，它计算游戏中每个状态信念的反事实。这在评估任何给定时间点的游戏的不同变体时是关键。

增长树 CFR（GT-CFR）是 CFR 的一种变体，它优化了随时间增长的博弈树。GT-CFR 基于两个基本阶段，更多细节可在网上找到：

*[`medium.com/syncedreview/deepminds-pog-excels-in-perfect-and-imperfect-information-games-advancing-research-on-general-9dbad5c04221`](https://medium.com/syncedreview/deepminds-pog-excels-in-perfect-and-imperfect-information-games-advancing-research-on-general-9dbad5c04221)*

### **OPENAI**

OpenAI 是一家对 AI 做出了重大贡献的人工智能研究公司，包括 DALL-E 和 ChatGPT，其主页为*[`openai.com/api/`](https://openai.com/api/)*。

OpenAI 由埃隆·马斯克和山姆·奥特曼（以及其他一些人）在旧金山创立，其一个明确的目标是开发对人类有益的 AI。鉴于微软对该组织的大量投资和深度联盟，OpenAI 可能被视为微软的一部分。OpenAI 是 GPT-x 系列 LLM 以及 ChatGPT 的创造者，ChatGPT 于 2022 年 11 月 30 日发布。

OpenAI 通过 API 将 GPT-3 商业化，按字收费，用于各种应用。GPT-3 于 2020 年 7 月宣布，并通过 beta 计划提供。然后，在 2021 年 11 月，OpenAI 将 GPT-3 向所有人开放；更多详情请见*[`openai.com/blog/api-no-waitlist/`](https://openai.com/blog/api-no-waitlist/)*。

此外，OpenAI 开发了 DALL-E，它可以从文本生成图像。最初，OpenAI 并不允许用户上传包含真实人脸的图像。后来，OpenAI 改变了其政策，允许用户将其人脸上传到其在线系统中。（有关更多详细信息，请查看 OpenAI 网页。）顺便提一下，扩散模型已经取代了 DALL-E 的基准。

OpenAI 还发布了一个公开的 Embeddings 测试版，这是一种适合各种机器学习任务的格式：

*[`beta.openai.com/docs/guides/embeddings`](https://beta.openai.com/docs/guides/embeddings)*

OpenAI 是 Codex 的创造者，它提供了一组在 NLP 上训练的模型。Codex 的初始发布是在私人测试版中；更多信息可在 *[`beta.openai.com/docs/engines/instruct-series-beta`](https://beta.openai.com/docs/engines/instruct-series-beta)* 上找到。

OpenAI 提供了四个模型，统称为他们的 *Instruct 模型*，这些模型支持 GPT-3 生成自然语言的能力。这些模型将在 2024 年初的早期被弃用，并替换为 GPT-3、ChatGPT 和 GPT-4 的更新版本。

如果您想了解更多关于 OpenAI 提供的功能和服务，请访问以下链接：*[`platform.openai.com/overview`](https://platform.openai.com/overview)*。

### **COHERE**

Cohere 是一家初创公司，也是 OpenAI 的竞争对手，其主页可在 *[`cohere.ai/`](https://cohere.ai/)* 上找到。

Cohere 开发了适用于多个行业的尖端 NLP 技术，这些技术可以商业使用。Cohere 专注于执行文本分析的模型，而不是文本生成模型（如基于 GPT 的模型）。Cohere 的创始团队令人印象深刻：CEO Aidan Gomez 是 transformer 架构的共同发明者之一，而 CTO Nick Frosst 是 Geoffrey Hinton 的门生。

### **HUGGING FACE**

Hugging Face 是一个流行的基于社区的开放源代码 NLP 技术仓库，其主页位于 *[`github.com/huggingface`](https://github.com/huggingface)*。

与 OpenAI 或 Cohere 不同，Hugging Face 并不构建自己的 NLP 模型。相反，Hugging Face 是一个平台，管理着大量的开源 NLP 模型，客户可以对这些模型进行微调然后部署。实际上，Hugging Face 已经成为人们协作开发 NLP 模型的著名地点，有时也被称为“机器学习和 NLP 的 GitHub。”

#### **Hugging Face 库**

Hugging Face 提供了三个重要的库：datasets、tokenizers 和 transformers。Accelerate 库支持 PyTorch 模型。datasets 库提供了一系列 NLP 库。tokenizers 库允许您将文本数据转换为数值。

可能最令人印象深刻的是 transformers 库，它提供了一整套基于预训练的 BERT 模型，可以执行各种 NLP 任务。GitHub 仓库位于 [`github.com/huggingface/transformers`](https://github.com/huggingface/transformers)。

#### **Hugging Face 模型中心**

Hugging Face 提供了一个模型中心，提供大量可在线访问的模型。此外，该网站支持其模型的在线测试，包括以下任务：

+   使用 BERT 进行掩码词填充

+   使用 Electra 进行命名实体识别

+   使用 RoBERTa 进行自然语言推理

+   使用 DistilBERT 进行问答

+   使用 BART 进行总结

+   使用 GPT-2 进行文本生成

+   使用 T5 进行翻译

通过以下链接导航以查看“使用 transformer：write”的文本生成能力：*[`transformer.huggingface.co`](https://transformer.huggingface.co)*。

之后，您将看到一些 Python 代码示例，展示如何列出所有可用的 Hugging Face 数据集，以及如何加载特定数据集。

### **AI21**

AI21 是一家通过 API 提供专有大型语言模型以支持其客户应用的公司。AI21 的当前 SOTA 模型被称为 Jurassic-1（与 GPT-3 大小大致相同），AI21 还在 Jurassic-1 和其他模型之上创建了其自己的应用。AI21 的当前应用套件包括可以增强阅读和写作的工具。

Primer 是这个领域的一个较老的竞争对手，在 transformer 发明之前两年成立。该公司主要服务于政府和防务行业的客户。

### **INFLECTIONAI**

在 AI 领域中，InflectionAI 是一家较新的公司，其令人印象深刻的核心团队包括

+   Reid Hoffman（LinkedIn）

+   DeepMind 联合创始人 Mustafa Suleyman

+   DeepMind 研究员 Karen Simonyan

InflectionAI 致力于一项具有挑战性的任务：使人类能够以与人类相互沟通相同的方式与计算机互动。

### **ANTHROPIC**

Anthropic 是由 OpenAI 前员工于 2021 年创建的，其主页位于 *[`www.anthropic.com/`](https://www.anthropic.com/)*。

Anthropic 从包括 Google 和 Salesforce 在内的一系列公司获得了重要的财务支持。随着本书的印刷，Anthropic 发布了 Claude-2 作为 ChatGPT 的竞争对手。预计 Anthropic 将在 2023 年第四季度之前使其 API 可用。

Claude-2 能够总结多达 75,000 个单词的文本内容，而 ChatGPT 目前限制为 3,000 个单词。此外，Claude-2 在部分律师资格考试中取得了 76.5% 的分数，在编码测试中取得了 71% 的分数。Claude-2 在向用户查询提供“干净”的回复方面也比 ChatGPT 的比率更高。

这部分章节关于在 AI 领域做出重要贡献的 AI 公司的内容到此结束。下一节将提供对大型语言模型（LLMs）的高级介绍。

### **什么是提示工程？**

文本生成器，如 OpenAI 的 GPT-3 和 DALL-E 2、AI21 的 Jurassic、Midjourney 和 Stable Diffusion，它们可以进行文本到图像的生成。*提示工程*指的是设计基于文本的提示，使基于 AI 的系统能够改进生成的输出，这意味着输出更接近用户从 AI 系统中想要产生的结果。通过类比，将提示视为类似教练的角色：他们提供建议和意见，帮助人们在特定任务中表现更好。

由于提示基于单词，挑战在于学习不同单词如何影响生成的输出。此外，预测系统对给定提示的反应也很困难。例如，如果你想生成一幅风景画，暗色调风景和亮色调风景之间的区别是直观的。然而，如果你想得到一幅美丽的风景画，AI 系统会如何生成相应的图像？正如你可以推测的那样，对于从文本生成图像的 AI 系统来说，具体词汇比抽象或主观词汇更容易。为了更详细地说明前面的例子，你将如何可视化以下内容？

+   一幅美丽的风景

+   一首美丽的歌曲

+   一部美丽的电影

尽管提示工程始于文本到图像的生成，但还有其他类型的提示工程，例如基于音频的提示，它解释了在语音中检测到的强调文本和情绪，以及基于草图生成图像的提示。最近关注的焦点涉及用于生成视频的基于文本的提示，这为艺术家和设计师提供了令人兴奋的机会。一个图像到图像处理的例子可以在网上找到：

*[`huggingface.co/spaces/fffiloni/stable-diffusion-color-sketch`](https://huggingface.co/spaces/fffiloni/stable-diffusion-color-sketch)*

#### **提示和完成**

*提示*是用户提供给 LLM 的文本字符串，*完成*是用户从 LLM 收到的文本。提示帮助 LLM 完成请求（任务），它们的长度可以不同。尽管提示可以是任何文本字符串，包括随机字符串，但提示的质量和结构会影响完成的质量。

将提示视为向 LLM（大型语言模型）提供“指导”的机制，或者甚至将其视为一种“教练”LLM 以提供所需答案的方式。请记住，提示中的标记数加上完成中的标记数最多为 2,048 个标记。

#### **提示类型**

以下列表包含了一些 LLM（大型语言模型）常用的提示类型：

+   零样本提示

+   单样本提示

+   少样本提示

+   指令提示

**注意** *前面列表中的前三个提示分别被称为“零样本学习”、“单样本学习”和“少样本学习”。*

*零样本提示*包含对任务的描述，而*单样本提示*由完成任务的单一示例组成。如你所能推测，*少样本提示*由多个示例组成（通常在 10 到 100 个之间）。在所有情况下，都建议提供对任务或任务的清晰描述：更多的任务为 GPT-3 提供更多信息，这反过来又可能导致更准确的完成。

T0（代表“零样本”）是一个有趣的 LLM：尽管 T0 比 GPT-3 小 16 倍（11 GB），但在语言相关任务上 T0 的表现超过了 GPT-3。T0 可以在未见过的 NLP 任务上表现良好（即，对 T0 来说是新任务），因为它是在包含多个任务的训练数据集上训练的。

以下 URL 提供了 T0 的 GitHub 仓库，一个可以直接在浏览器中训练 T0 的网页，以及 T0 的 3 GB 版本：

*[`github.com/bigscience-workshop/t-zero`](https://github.com/bigscience-workshop/t-zero)*

如你所能推测，T0++ 基于 T0，并且它是在 T0 训练的任务集之外额外训练的。

#### **指令提示**

*指令提示*用于微调大型语言模型（LLMs），并指定 LLM 在响应中应遵守的格式（由你确定）。你可以准备自己的指令提示，或者你可以访问包含不同任务和不同数据集的不同模板的提示模板库。各种提示指令模板公开可用，例如以下链接提供了 Llama 的提示模板：

*[`github.com/devbrones/llama-prompts`](https://github.com/devbrones/llama-prompts)*

*[`pub.towardsai.net/llama-gpt4all-simplified-local-chatgpt-ab7d28d34923`](https://pub.towardsai.net/llama-gpt4all-simplified-local-chatgpt-ab7d28d34923)*

#### **反向提示**

另一种技术是反转提示和完成的顺序：*输入提示*是答案，而*响应*是与答案相关的提问（类似于一个流行的游戏节目）。例如，给定一个法语句子，你可能会问模型，“什么英语文本可能导致了这个法语翻译？”

#### **系统提示与代理提示**

在对话式人工智能系统和聊天机器人设计的情况下，系统提示和代理提示之间的区别经常被提及。

*系统提示*通常是系统给出的初始消息或提示，以指导用户可以做什么或设定对交互的期望。它通常作为介绍或指导用户如何进行的方式。以下是一些系统提示的例子：

```py
 “Welcome to ChatBotX! You can ask me questions about
weather, news, or sports. How can I assist you today?” “Hello! For account details, press 1\. For technical
support, press 2.” “Greetings! Type ‘order’ to track your package or ‘help’
for assistance.” 
```

相比之下，*代理提示* 是在交互过程中，AI 模型或代理根据用户输入生成的消息。它是对话中来回交流的一部分。代理提示引导用户提供更多信息，澄清歧义，或将用户推向特定的行动。以下是一些代理提示的例子：

```py
 User: “I’m looking for shoes.” Agent Prompt: “Great! Are you looking for men’s or women’s shoes?” User: “I can’t log in.” Agent Prompt: “I’m sorry to hear that. Can you specify if you’re having
trouble with your password or username?” User: “Tell me a joke.” Agent Prompt: “Why did the chicken join a band? Because it had the
drumsticks!” 
```

这两种之间的基本区别在于它们的目的和在交互中的位置。系统提示通常位于交互的开始，为对话设定场景。代理提示在对话过程中出现，根据用户输入引导对话的方向。

这两种提示类型对于创建流畅直观的用户对话体验至关重要。它们引导用户，并有助于确保系统有效地理解和解决用户的需求。

#### **提示模板**

*提示模板* 是用于指导模型或系统执行特定任务的预定义格式或结构。它们是生成提示的基础，其中模板的某些部分可以填充或定制以产生各种特定的提示。通过类比，提示模板是您可以在某些文本编辑器中定义的宏的对立面。

提示模板在处理语言模型时特别有用，因为它们提供了一种在多个任务或数据点查询模型的一致方式。特别是，提示模板可以更容易地

+   确保在多次查询模型时的一致性

+   促进批量处理或自动化

+   减少提问给模型时的错误和变化

例如，假设您正在使用一个大型语言模型（LLM），并且您想将英语句子翻译成法语。相关的提示模板可能如下所示：

“将以下英语句子翻译成法语：{sentence}”

注意，{sentence} 是一个占位符，您可以用任何英语句子来替换它。

您可以使用前面的提示模板生成特定的提示：

+   “将以下英语句子翻译成法语：‘你好，你怎么样？’”

+   “将以下英语句子翻译成法语：‘我爱冰淇淋。’”

正如您所看到的，提示模板使您能够轻松地为不同的句子生成各种提示，而无需每次都重写整个指令。实际上，这个概念可以扩展到更复杂的任务，并可以根据应用情况包含多个占位符或更复杂的结构。

#### **不同 LLM 的提示**

GPT-3、ChatGPT 和 GPT-4 都是基于 Transformer 架构的 LLM，在底层机制上基本相似。ChatGPT 实质上是针对对话交互特别微调的 GPT 模型的一个版本。GPT-4 在规模和能力方面是 GPT-3 的演变或改进。

这些模型提示词的差异主要源于特定的用例和上下文，而不是模型之间的固有差异。以下是一些基于用例的提示词差异。

GPT-3 可以用于广泛的任务，而不仅仅是对话，从内容生成到代码编写。以下是 GPT-3 的提示词示例：

+   “将以下英文文本翻译成法语：‘你好，你好吗？’”

+   “编写一个计算数字阶乘的 Python 函数。”

ChatGPT：专门针对对话交互进行微调。以下是 ChatGPT 的提示词示例：

用户： “你能帮我做作业吗？”

ChatGPT： “当然！您需要帮助的是哪个主题或话题？”

用户： “讲一个笑话。”

ChatGPT： “为什么鸡穿过操场？为了到达另一边的滑梯！”

GPT-4：提供更大规模和改进，因此提示词的性质与 GPT-3 相似，但可能产生更准确或更细微的输出。以下是 GPT-4 的提示词示例：

+   “就广义相对论而言，提供量子力学详细分析。”

+   “基于后末日世界主题为希望编写一个短篇故事。”

这三个模型接受自然语言提示并产生自然语言输出。与它们交互的基本方式保持一致。

主要区别在于模型被使用的上下文以及任何已应用的微调。例如，ChatGPT 被设计成更具对话性，因此虽然您可以使用 GPT-3 进行聊天，但 ChatGPT 可能会产生更具上下文相关性的对话输出。

当直接与这些模型交互，尤其是通过 API 时，您也可能控制诸如“温度”（控制随机性）和“最大标记数”（控制响应长度）等参数。调整这些参数可以塑造响应，无论您使用的是哪个 GPT 变体。

从本质上讲，尽管底层模型在规模和特定训练/微调方面存在差异，但您提示它们的方式在很大程度上保持一致：清晰、具体的自然语言提示会产生最佳结果。

#### **措辞不当的提示词**

在构建提示词时，尽可能清晰和具体，以引导响应朝所需的方向发展。含糊或模糊的提示词可能导致各种响应，其中许多可能对用户实际意图没有帮助或不相关。

此外，措辞不当的提示词通常模糊、含糊不清或过于宽泛，它们可能导致人工智能模型产生混淆、误解或非特定的响应。以下是一些以斜体显示的措辞不当的提示词示例，以及每个提示词缺陷的解释：

*“告诉我那件事。”*

问题：过于模糊。指的是什么“事物”？

*“为什么会发生？”*

问题：没有上下文。正在讨论什么事件或情况？

*“解释一下。”*

问题：过于宽泛。应该解释哪些具体的“内容”？

*“做需要做的事情。”*

问题：含糊不清。需要执行的具体动作是什么？

*“我想获取信息。”*

问题：不具体。需要什么类型的信息？

*“你能从那个地方帮我拿到那个东西吗？”*

问题：既不清楚“事物”也不清楚“地点”。

*“告诉我那位先生的书的摘要？”*

问题：含糊不清的引用。谁是“*那位先生*”？

*“你是怎么进行这个过程的？”*

问题：指的是哪个“过程”？

*“描述这个主题的重要性。”*

问题：未指定“主题”。

*“为什么它是好是坏？”*

问题：没有上下文。什么是“它”？

*“帮助解决这个问题。”*

问题：模糊不清。正在讨论的具体问题是什么？

*“完成任务需要考虑的事项。”*

问题：含糊不清。正在讨论的是哪个“任务”？

*“这是怎么工作的？”*

问题：缺乏具体性。什么是“这”？

### **什么是 ChatGPT？**

聊天机器人竞赛正在加剧，主要竞争对手的长期价值仍有待确定。一个竞争对手是 ChatGPT-3.5（ChatGPT），这是 OpenAI 的一个基于 AI 的聊天机器人。ChatGPT 通过提供对话式响应来响应用户的查询，并且可以在*[`chat.openai.com/chat`](https://chat.openai.com/chat)*访问。

ChatGPT 注册用户数量的增长率非常惊人。最接近的竞争对手是 iPhone，它在 2.5 个月内达到一百万用户，而 ChatGPT 在*六天内*就达到了一百万用户。ChatGPT 的用户数量达到约 18 亿，然后下降到大约 15 亿，您可以在以下在线文章中的图表中看到：

*[`decrypt.co/147595/traffic-dip-hits-openais-chatgpt-first-times-hardest`](https://decrypt.co/147595/traffic-dip-hits-openais-chatgpt-first-times-hardest)*

注意，尽管 Meta 的 Threads 在会员数量方面超过了 ChatGPT，但 Threads 的日活跃用户数量下降了约 50%。六个知名公司/产品的会员数量达到一百万的时间框架与 ChatGPT 的比较可以在*[`www.syntheticmind.io/p/01`](https://www.syntheticmind.io/p/01)*找到。

前面的链接还包含有关 Will Hobick 的信息，他使用 ChatGPT 编写了一个用于电子邮件相关任务的 Chrome 扩展程序，尽管他没有 JavaScript 或 Chrome 扩展程序开发的经验。Will Hobick 在以下网址提供了更多关于他的 Chrome 扩展的详细信息：

*[`www.linkedin.com/posts/will-hobick_gpt3-chatgpt-ai-activity-7008081003080470528-8QCh`](https://www.linkedin.com/posts/will-hobick_gpt3-chatgpt-ai-activity-7008081003080470528-8QCh)*

#### **ChatGPT：GPT-3 的强化版？**

ChatGPT 被称为 GPT-3 的强化版，并且有一些共识认为 ChatGPT3 是目前世界上最好的聊天机器人。确实，ChatGPT 可以执行多种任务，其中一些列在这里：

+   写诗

+   编写文章

+   编写代码

+   角色扮演

+   拒绝不适当的要求

此外，它在处理自然语言查询方面的响应质量超过了其前辈 GPT-3 的能力。另一个有趣的特性包括能够承认自己的错误。ChatGPT 还提供 *提示回复*，这是你可以向 ChatGPT 提问的示例。此外，ChatGPT 还可以生成新的圣诞歌曲歌词：

*[`www.cnet.com/culture/entertainment/heres-what-it-sounds-like-when-ai-writes-christmas-lyrics`](https://www.cnet.com/culture/entertainment/heres-what-it-sounds-like-when-ai-writes-christmas-lyrics)*

ChatGPT 可能不会让有小孩的父母感到亲切的一个方面是，ChatGPT 告诉孩子们圣诞老人不存在：

*[`futurism.com/the-byte/openai-chatbot-santa`](https://futurism.com/the-byte/openai-chatbot-santa)*

*[`www.forbes.com/sites/lanceeliot/2022/12/21/pointedly-asking-generative-ai-chatgpt-about-whether-santa-claus-is-real-proves-to-be-eye-opening-for-ai-ethics-and-ai-law`](https://www.forbes.com/sites/lanceeliot/2022/12/21/pointedly-asking-generative-ai-chatgpt-about-whether-santa-claus-is-real-proves-to-be-eye-opening-for-ai-ethics-and-ai-law)*

#### **ChatGPT：谷歌“红色代码”**

2022 年 12 月，谷歌的 CEO 发布了关于 ChatGPT 作为谷歌搜索引擎竞争对手的潜在威胁的“红色代码”：

*[`www.yahoo.com/news/googles-management-reportedly-issued-code-190131705.html`](https://www.yahoo.com/news/googles-management-reportedly-issued-code-190131705.html)*

根据前面的文章，谷歌正在投资资源开发基于 AI 的产品，预计是为了提供能够成功与 ChatGPT 竞争的功能。其中一些基于 AI 的产品也可能生成与 DALL-E 的图形效果相当的效果。确实，争夺 AI 主导权的竞赛仍在继续，并且无疑将在可预见的未来继续下去。

#### **ChatGPT 与谷歌搜索的比较**

考虑到经常有人猜测 ChatGPT 将取代谷歌搜索，让我们简要比较一下谷歌和 ChatGPT 对给定查询的响应方式。首先，谷歌是一个使用 Page Rank 算法（由拉里·佩奇开发）的搜索引擎，以及一些精心调整的、被严格保密的算法方面。谷歌使用这个算法对网站进行排名，并为给定查询生成搜索结果。然而，搜索结果中包括付费广告，这些广告可能会“杂乱”链接列表。

相比之下，ChatGPT 不是一个搜索引擎：它会对给定的查询提供直接响应：用通俗的话说，ChatGPT 会直接“切入正题”并消除多余的链接。然而，ChatGPT *可能*会产生错误的结果，其后果可能从无害到重大不等。

因此，谷歌搜索和 ChatGPT 都有各自的优点和缺点，它们在处理不同类型的查询时表现出色：前者擅长处理具有多方面答案的查询（例如，关于法律问题的问题），而后者擅长处理直接了当的查询（例如，编码问题）。显然，它们在处理许多其他类型的查询时也表现出色。

根据玛格丽特·米切尔的说法，ChatGPT 不会取代谷歌搜索，她提供了一些关于谷歌搜索和 PageRank 的有趣细节，您可以在*[`twitter.com/mmitchell_ai/status/1605013368560943105`](https://twitter.com/mmitchell_ai/status/1605013368560943105)*上阅读。

#### **ChatGPT 自定义指令**

ChatGPT 增加了对自定义指令的支持，这允许您指定一些偏好，ChatGPT 在回答您的查询时会使用这些偏好。

ChatGPT Plus 用户可以通过访问 ChatGPT 网站并执行以下步骤来开启自定义指令：

```py
 Settings > Beta features > Opt into Custom instructions 
```

作为简单的例子，您可以指定您更喜欢以除 Python 以外的语言查看代码。通过 ChatGPT 中的自定义指令，也可以指定日常任务的常见初始要求。设置自定义指令的详细步骤可在网上找到。

*[`artificialcorner.com/custom-instructions-a-new-feature-you-must-enable-to-improve-chatgpt-responses-15820678bc02`](https://artificialcorner.com/custom-instructions-a-new-feature-you-must-enable-to-improve-chatgpt-responses-15820678bc02)*

自定义指令的另一个有趣例子来自杰里米·霍华德，他准备了一套详尽且详细的在线可访问的自定义指令：

*[`twitter.com/jeremyphoward/status/1689464587077509120`](https://twitter.com/jeremyphoward/status/1689464587077509120)*

当这本书准备印刷时，自定义指令仅适用于已注册 ChatGPT Plus 的用户。然而，OpenAI 已声明，到 2023 年底，自定义指令将免费对所有用户开放。

#### **ChatGPT 在移动设备和浏览器上的应用**

ChatGPT 于 2023 年首先在 iOS 设备上可用，随后在 Android 设备上可用。您可以从以下链接下载 ChatGPT 到 iOS 设备：

*[`www.macobserver.com/tips/how-to/how-to-install-and-use-the-official-chatgpt-app-on-iphone/`](https://www.macobserver.com/tips/how-to/how-to-install-and-use-the-official-chatgpt-app-on-iphone/)*

如果您有 Android 设备，您可以从*[`play.google.com/store/apps/details?id=com.openai.chatgpt`](https://play.google.com/store/apps/details?id=com.openai.chatgpt)*下载 ChatGPT。

您可以从以下 URL 安装 Microsoft 的 Bing 浏览器版本的 ChatGPT：

*[`chrome.google.com/webstore/detail/chatgpt-for-bing/pkkmgcildaegadhngpjkklnbfbmhpdng`](https://chrome.google.com/webstore/detail/chatgpt-for-bing/pkkmgcildaegadhngpjkklnbfbmhpdng)*

#### **ChatGPT 和提示**

虽然 ChatGPT 擅长生成对查询的响应，但有时您可能对结果并不完全满意。一个选项是输入单词“重写”，以便从 ChatGPT 获得另一个版本。

尽管这是可用的最简单的提示之一，但在有效性方面有限。如果您想要更多有意义的提示列表，以下文章包含了 31 个可能比使用“重写”一词更好的提示（而不仅仅是 ChatGPT）：

*[`medium.com/the-generator/31-ai-prompts-better-than-rewrite-b3268dfe1fa9`](https://medium.com/the-generator/31-ai-prompts-better-than-rewrite-b3268dfe1fa9)*

#### **GPTBot**

GPTBot 是一个网站爬虫。幸运的是，您可以通过将 GPTBot 添加到网站的 robots.txt 文件中来禁止 GPTBot 访问网站：

```py
 User-agent: GPTBot
Disallow: / 
```

您还可以通过将 GPTBot 令牌添加到网站的 robots.txt 文件中来仅对网站的一部分进行 GPTBot 访问的定制：

```py
 User-agent: GPTBot
Allow: /youcangohere-1/
Disallow: /dontgohere-2/ 
```

作为旁白，Stable Diffusion 和 LAION 都通过 Common Crawl 抓取互联网。但是，您可以通过在 robots.txt 文件中指定以下片段来防止您的网站被抓取：

```py
 User-agent: CCBot
Disallow: / 
```

关于 GPTBot 的更多信息可在网上找到：

*[`platform.openai.com/docs/gptbot`](https://platform.openai.com/docs/gptbot)*

*[`platform.openai.com/docs/gptbot`](https://platform.openai.com/docs/gptbot)*

*[`www.yahoo.com/finance/news/openai-prepares-unleash-crawler-devour-020628225.html`](https://www.yahoo.com/finance/news/openai-prepares-unleash-crawler-devour-020628225.html)*

#### **ChatGPT 游乐场**

ChatGPT 拥有自己的“游乐场”，您会发现它与 GPT-3 的游乐场在实质上有所不同，并且可以通过*[`chat.openai.com/chat`](https://chat.openai.com/chat)*访问。

为了您的方便，GPT-3 游乐场的链接在此重现：

*[`beta.openai.com/playground`](https://beta.openai.com/playground)*

OpenAI 定期为 ChatGPT 添加新功能，包括以下内容：

+   用户可以查看（并继续）之前的对话。

+   ChatGPT 不会回答的问题数量有所减少。

+   用户保持登录状态超过两周。

另一个很好的增强功能包括对键盘快捷键的支持：当与代码一起工作时，您可以使用序列⌘ (Ctrl) + Shift +（对于 Mac）来复制最后一个代码块，以及序列⌘ (Ctrl) + /来查看完整的快捷键列表。

关于 ChatGPT 及其如何编写提示以从 ChatGPT 中提取您想要的细节的文章有很多。其中一篇文章的 URL 如下：

*[`www.tomsguide.com/features/7-best-chatgpt-tips-to-get-the-most-out-of-the-chatbot`](https://www.tomsguide.com/features/7-best-chatgpt-tips-to-get-the-most-out-of-the-chatbot)*

### **插件、代码解释器和代码低语者**

除了回答用户的大量查询外，ChatGPT 通过提供以下功能来扩展其功能：

+   第三方 ChatGPT 插件

+   代码解释器

+   Code Whisperer

上述列表中的每个主题将在以下小节中简要讨论，以及一个讨论代码解释器与 Anthropic 的 Claude-2 的短节。

#### **插件**

可用的 ChatGPT 插件有数百种，一些流行插件的列表可在网上找到：

*[`levelup.gitconnected.com/5-chatgpt-plugins-that-will-put-you-ahead-of-99-of-data-scientists-4544a3b752f9`](https://levelup.gitconnected.com/5-chatgpt-plugins-that-will-put-you-ahead-of-99-of-data-scientists-4544a3b752f9)*

*[`www.zdnet.com/article/the-10-best-chatgpt-plugins-of-2023/`](https://www.zdnet.com/article/the-10-best-chatgpt-plugins-of-2023/)*

请记住，“最佳”ChatGPT 插件列表经常变化，因此进行在线搜索以了解最新的 ChatGPT 插件是个好主意。以下链接还包含了关于高度评价的插件的一些详细信息：

*[`www.tomsguide.com/features/i-tried-a-ton-of-chatgpt-plugins-and-these-3-are-the-best`](https://www.tomsguide.com/features/i-tried-a-ton-of-chatgpt-plugins-and-these-3-are-the-best)*

另一套推荐的插件（当然，根据您的需求而定）如下所示：

+   AskYourPDF

+   ChatWithVideo

+   Noteable

+   Upskillr

+   Wolfram

如果您担心 ChatGPT 抓取您网站的内容，OpenAI 的浏览器插件支持一个名为 ChatGPT-User 的用户代理令牌，该令牌遵守许多网站提供的 robots.txt 文件中指定的内容，以限制对内容的访问。

如果您想为 ChatGPT 开发插件，请访问此网站获取更多信息：*[`platform.openai.com/docs/plugins/introduction`](https://platform.openai.com/docs/plugins/introduction)*。

除了开发 ChatGPT 插件的详细信息外，前面的 OpenAI 网站还提供了有关插件的有用信息，如下所示：

+   认证

+   示例

+   插件评测

+   插件政策

OpenAI 不控制您添加到 ChatGPT 的任何插件：它们将 ChatGPT 连接到外部应用程序。此外，ChatGPT 根据您在 ChatGPT 账户中启用的特定插件，在您的会话期间确定要使用的插件。

#### **高级数据分析**

ChatGPT 高级数据分析使 ChatGPT 能够生成图表和图形，创建和训练机器学习模型，包括深度学习模型。ChatGPT 高级数据分析提供了一套广泛的功能，并且对支付每月 20 美元订阅费的 ChatGPT 用户开放。然而，这个功能可能很快就会对所有用户开放。

*[`towardsdatascience.com/chatgpt-code-interpreter-how-it-saved-me-hours-of-work-3c65a8dfa935`](https://towardsdatascience.com/chatgpt-code-interpreter-how-it-saved-me-hours-of-work-3c65a8dfa935)*

OpenAI 的模型可以访问一个限制在沙盒和防火墙执行环境中的 Python 解释器。在评估 Python 代码时，解释器插件还可以访问一些临时磁盘空间。尽管临时磁盘空间是有限的，但在同一会话中的多次查询可以在代码和执行环境方面产生累积效应。

此外，ChatGPT 还可以（应要求）生成下载链接以下载数据。另一个有趣的功能：从 2023 年中开始，高级数据分析现在可以一次性分析多个文件，包括 CSV 文件和 Excel 电子表格。

高级数据分析可以执行各种有趣的任务，以下是一些例子：

+   解决数学问题

+   执行数据分析和可视化

+   在不同格式之间转换文件

+   与 Excel 电子表格一起工作

+   在 PDF 中读取文本内容

以下文章讨论了您可以使用高级数据分析的各种方法：

*[`mlearning.substack.com/p/the-best-88-ways-to-use-chatgpt-code-interpreter`](https://mlearning.substack.com/p/the-best-88-ways-to-use-chatgpt-code-interpreter)*

#### **高级数据分析与 Claude-2**

Anthropic 的 Claude-2 是 ChatGPT 的另一个竞争对手。除了响应用户的提示外，Claude-2 还能生成代码和总结整本书。Claude-2 也存在“幻觉”问题，这是基于 LLM 的聊天机器人普遍存在的问题。有关 Claude-2 的更多详细信息可在网上找到：

*[`medium.com/mlearning-ai/claude-2-vs-code-interpreter-gpt-4-5-d2e5c9ee00c3`](https://medium.com/mlearning-ai/claude-2-vs-code-interpreter-gpt-4-5-d2e5c9ee00c3)*

顺便提一下，目前可用的 ChatGPT 版本是在 2021 年 9 月训练的，这意味着 ChatGPT 无法回答有关 Claude-2 或 Google Bard 的问题，这两者都是在该日期之后发布的。

#### **代码解析者**

ChatGPT 代码解析者使您能够简化一些任务，以下是一些例子（将此列表与 Bard 的对应列表进行比较）：

+   从图像创建视频

+   从图像中提取文本

+   从图像中提取颜色

在 ChatGPT 生成视频后，它还会提供一个链接，您可以通过该链接下载生成的视频。有关前面列表中功能的更多详细信息可在网上找到：

*[`artificialcorner.com/chatgpt-code-interpreter-is-not-just-for-coders-here-are-6-ways-it-can-benefit-everyone-b3cc94a36fce`](https://artificialcorner.com/chatgpt-code-interpreter-is-not-just-for-coders-here-are-6-ways-it-can-benefit-everyone-b3cc94a36fce)*

### **检测生成的文本**

毫无疑问，ChatGPT 提高了用户对生成文本质量的期望，这进一步增加了剽窃的难度。当您阅读一段文本时，有几个线索表明这是生成的文本，例如

+   精糕或异常的句子结构

+   在多个位置重复的文本

+   过度使用情感（或缺乏情感）

然而，有一些工具可以帮助检测生成的代码。一个免费的在线工具是来自 OpenAI 的 GPT2 Detector，可以在网上访问：

*[`huggingface.co/openai-detector`](https://huggingface.co/openai-detector)*

作为一个简单（尽管是人为设计的）例子，在 GPT2 Detector 中输入以下句子：

```py
 This is an original sentence written by me and nobody else. 
```

GPT2 Detector 分析了这个句子，并报告说这个句子有 19.35%的概率是真实的。现在，让我们修改前面的句子，添加一些额外的文本，如下所示：

```py
 This is an original sentence written by me and nobody else,
regardless of what an online plagiarism tool will report
about this sentence. 
```

GPT2 Detector 分析了这个句子，并报告说这个句子有 95.85%的概率是真实的。根据 GPT2 Detector 网站，当输入文本中大约有 50 个标记时，概率分数的可靠性“变得可靠”。

另一个（稍微旧一点的）在线工具，用于检测自动生成的文本是 IBM 的 Giant Language model Test Room (GLTR)，可在*[`gltr.io/`](http://gltr.io/)*访问。

您可以在*[`github.com/HendrikStrobelt/detecting-fake-text`](https://github.com/HendrikStrobelt/detecting-fake-text)*下载 GLRT 的源代码（TypeScript 和 CSS 的组合）。

除了前面提到的免费工具之外，还有一些商业工具也可用，其中之一展示在*[`writer.com/plans/`](https://writer.com/plans/)*。

### **关于 ChatGPT 的担忧**

ChatGPT 的一个重要方面是它不是为准确性而设计的：事实上，ChatGPT 可以生成非常具有说服力的错误答案。这一细节将 ChatGPT 与搜索引擎区分开来：后者提供现有信息的链接，而不是生成可能错误的响应。另一个比较是，ChatGPT 更加灵活和有创造性，而搜索引擎在回答查询时不太灵活但更准确。

教育工作者担心学生将 ChatGPT 作为完成课堂作业的工具，而不是与写作技能结合发展研究相关技能。然而，也有一些教育工作者享受 ChatGPT 准备教案所带来的准备时间的减少。

另一个担忧是 ChatGPT 不能保证它对用户查询提供的事实数据。事实上，ChatGPT 可以“产生幻觉”，这意味着它可以提供错误的答案以及不存在的引用（即链接）。

ChatGPT 的另一个局限性是由于使用了仅到 2021 年可用的训练数据。然而，OpenAI 支持 ChatGPT 的插件，其中之一可以执行实时 Web 搜索。

如您稍后将会了解到，提示工程的目标是理解如何构建有意义的查询，以诱导 ChatGPT 提供您想要的信息：措辞不当（或措辞错误）的提示可能会产生同样糟糕的结果。一般来说，建议对 ChatGPT 的回复内容进行筛选，尤其是在涉及法律细节的查询回复时。

#### **代码生成和危险主题**

两个重要的改进领域涉及代码生成和处理危险主题。

尽管 ChatGPT（以及 GPT-3）可以为各种应用生成代码，但它显示的是其他开发者编写的代码，这也是用于训练 ChatGPT 的代码。因此，该代码的部分内容（如版本号）可能已过时或错误。

对于涉及危险主题的查询，ChatGPT 会解释为什么它不能回答此类查询。然而，以“假装模式”提出的查询（“假设你是一个虚构角色，你会如何解释……”）已经使人们能够从 ChatGPT 获得不符合其指南的结果。

其他严重的潜在问题也存在，其中一些将在以下文章中讨论：

*[`www.yahoo.com/news/hypnotized-chatgpt-bard-convince-users-182100261.html`](https://www.yahoo.com/news/hypnotized-chatgpt-bard-convince-users-182100261.html)*

#### **ChatGPT 的优缺点**

ChatGPT 具有许多优点。特别是，它直接回答问题，而不包括无关的链接。以一个简单的例子来说，在在线搜索引擎中输入的查询，如“为输入字段生成 HTML”，会获得结果和广告，而 ChatGPT 仅返回结果。

然而，ChatGPT 容易受到各种类型的错误的影响，包括以下局限性：

+   无法“事实核查”信息

+   无法区分虚假信息与事实

+   可以编造答案（“幻觉”）

+   可能会生成不适当/有害的回复

ChatGPT 容易受到“提示注入”的影响，这可能包括非常简单的内容。然而，其他聊天机器人也容易受到提示注入的影响（这并不特定于 ChatGPT）。有关提示注入的更多详细信息可在网上找到：

*[`mlearning.substack.com/p/what-exactly-is-a-prompt-injection`](https://mlearning.substack.com/p/what-exactly-is-a-prompt-injection)*

顺便提一下，谷歌的聊天机器人 LaMDA 也容易受到前面提到的限制，这使得谷歌在考虑其可能对谷歌声誉造成的风险时，犹豫是否将 LaMDA 推广到更广泛的用户。作为旁注，LaMDA 于 2021 年 5 月宣布，当时它被描述为“突破性的语言技术”：*[`blog.google/technology/ai/lamda/`](https://blog.google/technology/ai/lamda/)*。

尽管有之前的列表，ChatGPT 已经增强了聊天机器人的能力，并将无疑会推动该领域主要利益相关者的创新和竞争。

### **ChatGPT 的样本查询和回应**

本节包含了一些提交给 ChatGPT 的查询示例，以及 ChatGPT 的详细回应：

```py
 Many people think that AI is dangerous. . . what do you think? 
```

“有一种普遍的误解，认为人工智能天生具有危险性。虽然人工智能确实有可能被用于有害目的，但它也有能力做很多好事。就像任何其他技术一样，这完全取决于如何使用。在正确的人手中，人工智能可以用来解决世界上一些最紧迫的问题，例如治愈疾病和改善农业。在错误的人手中，它可能会被用来造成伤害。对我们来说，负责任和道德地使用人工智能，并确保以最小化潜在危害的方式对其进行监管和控制，是非常重要的。”

这里是另一个提交给 ChatGPT-3 的查询示例，以及其详细的回应：

```py
 What are some ways in which you can improve the accuracy of
your responses to queries? 
```

“有几种方法可以提高我对查询的回答的准确性。一种方法是用更多的数据来训练我的算法。我拥有的数据越多，我可以处理的信息就越多，我的回答就越准确。提高准确性的另一种方法是使用更先进的算法和技术，例如机器学习和自然语言处理。这些方法使我能够更好地理解语言的细微差别，并提供更准确的查询回答。此外，定期的测试和评估可以帮助识别我可以提高准确性的领域，并使我能够专注于这些领域以改进我的回答。”

```py
 Can you give an example of an odd perfect number? 
```

“据我们所知，目前还没有发现奇数完全数。虽然人们相信奇数完全数是存在的，但至今尚未找到，也不知道是否存在。实际上，目前尚不清楚是否存在任何奇数完全数。如果能够发现一个奇数完全数，那将是在数学领域的一个重大突破。”

```py
 Can you provide a proof of Goldbach’s conjecture? 
```

“很抱歉，但我无法提供哥德巴赫猜想的证明。哥德巴赫猜想是数学中一个著名的未解问题，它指出每个大于 2 的偶数都可以表示为两个质数的和。尽管数学家们多年来付出了很多努力，但尚未找到该猜想的证明。它被认为是数学中最具挑战性的未解问题之一。因为我是一个由 OpenAI 训练的大型语言模型，所以我无法证明数学猜想。我的能力仅限于根据我所训练的信息提供答案。”

```py
 Is there life after death, and how does it compare with
life on Earth? 
```

“没有科学证据支持死后有生命的观点。这是一个已经争论了几个世纪的话题，不同的文化和信仰体系对于死后会发生什么都有自己的看法。有些人相信来世，而另一些人则不相信。由于没有科学证据支持来世的存在，因此无法将其与地球上的生活进行比较。这最终是一个个人信仰的问题。”

```py
 Please provide a four-paragraph analysis of the war between
Ukraine and Russia, and also provide your prediction. . .
regarding the outcome 
```

“乌克兰与俄罗斯之间的战争是一场复杂的冲突，其根源可追溯到 2014 年俄罗斯吞并克里米亚。自那时起，冲突不断升级，俄罗斯支持的乌克兰东部分离主义者与乌克兰政府军交战。战斗已造成数千人伤亡，并使许多人流离失所。

冲突的核心主要问题在于乌克兰的主权问题。俄罗斯长期以来将乌克兰视为其势力范围的一部分，而克里米亚的吞并被许多人视为对乌克兰主权的侵犯。另一方面，乌克兰决心维护其独立，并在此过程中得到了许多西方国家的支持。

很难预测这场战争的结果。尽管乌克兰军队近年来在对抗分离主义者方面取得了一些进展，但俄罗斯继续为叛军提供支持，冲突仍未解决。从长远来看，可能需要通过外交解决方案来结束战斗。然而，这样的解决方案是否以及何时能够达成尚不确定。

与此同时，战争继续给乌克兰人民带来沉重打击。许多人陷入交火之中，持续的暴力和不稳定对该国的经济和整体发展产生了重大影响。国际社会继续支持乌克兰维护其主权并结束冲突的努力至关重要。”

从上述例子可以看出，ChatGPT 以超越近年来许多聊天机器人的方式，对查询提供了令人印象深刻且准确的回答。然而，仍然有可能让这个聊天机器人感到困惑。以下文章提供了更多使用 ChatGPT 的示例：

*[`www.theverge.com/23488017/openai-chatbot-chatgpt-ai-examples-web-demo`](https://www.theverge.com/23488017/openai-chatbot-chatgpt-ai-examples-web-demo)*

### **CHATGPT 与医学诊断**

一名多年来饱受慢性疼痛困扰的小男孩，通过一位意想不到的帮手——ChatGPT——终于找到了希望。在三年多的时间里，男孩的母亲带他看了 17 位不同的专家，但始终未能得到一个能解释他所有症状的诊断。

转折点出现在今年早些时候，他的母亲决定向 ChatGPT 寻求帮助。她创建了一个账户，并仔细输入了她多年来收集的所有细节，包括她儿子的症状和他的 MRI 扫描数据。她回忆起她在电脑前度过的无数小时，在绝望中筛选信息，试图找到答案。

尽管访问了众多医生，甚至一度匆忙赶往急诊室，但这个家庭感觉他们是在原地打转，每个专家都只关注他们的专业领域，而没有提供全面的解决方案。当她儿子停止生长时，她注意到一个令人担忧的迹象。尽管他们的儿科医生最初将这归因于大流行的副作用，但男孩的母亲觉得其中还有更多。

在绝望和决心的时刻，她转向 ChatGPT，输入了她所拥有的关于她儿子状况的每一份信息。就在那时，ChatGPT 提出了脊髓栓系综合征的可能性，这个建议与她产生了共鸣，似乎连接了所有线索。在专家确认 ChatGPT 的建议是正确的之后，她意识到这是他们漫长而疲惫的寻找诊断之旅中的一个关键时刻。

### **ChatGPT 的替代方案**

有几个 ChatGPT 的替代品提供了类似的功能集，其中一些列在这里：

+   Bard (Google)

+   Bing Chat

+   Gemini (Google)

+   Jasper

+   PaLM (Google)

+   Pi

+   POE (LinkedIn)

+   Replika

+   WriteSonic

+   YouChat

下面的子节讨论了前面列表中的一些（但不是全部）ChatGPT 的替代品。

#### **Google Bard**

Google Bard 是一个具有与 ChatGPT 类似功能的聊天机器人，例如生成代码以及生成文本/文档。这里显示了 Bard 支持的功能子集：

+   内置对互联网搜索的支持

+   内置对语音识别的支持

+   基于“PaLM 2 (Google)”构建

+   支持 20 种编程语言

+   读取/总结 PDF 文档

+   提供信息链接

根据以下 2023 年中的文章，Bard 增加了对 40 种额外语言的支持，以及文本到语音的支持：

*[`www.extremetech.com/extreme/google-bard-updated-with-text-to-speech-40-new-languages`](https://www.extremetech.com/extreme/google-bard-updated-with-text-to-speech-40-new-languages)*

此外，Bard 支持包含图像的提示（由 Google Lens 解释）并可以根据图像生成字幕。

以下文章建议，Google 可以通过利用 PaLM 来与 ChatGPT 保持竞争力：

*[`analyticsindiamag.com/googles-palm-is-ready-for-the-gpt-challenge/`](https://analyticsindiamag.com/googles-palm-is-ready-for-the-gpt-challenge/)*

#### **YouChat**

ChatGPT 的另一个替代品是 YouChat，它是搜索引擎*[you.com](http://you.com)*的一部分，并且可以在以下位置访问：*[`you.com/`](https://you.com/)*。

在机器学习社区因众多贡献而广为人知的理查德·索科尔（Richard Socher）是*[you.com](http://you.com)*的创造者。据理查德·索科尔所说，YouChat 是一个搜索引擎，它可以提供通常的搜索相关功能，以及搜索网络以获取更多信息以响应用户查询的能力。

另一个竞争对手是来自 LinkedIn 的 POE，你可以在*[`poe.com/login`](https://poe.com/login)*上创建免费账户。

#### **从屈折中提取的π**

π是由 Inflection 公司开发的聊天机器人，该公司由 Mustafa Suleyman 创立，他也是 DeepMind 的创始人。π可通过*[`pi.ai/talk`](https://pi.ai/talk)*访问。以下文章包含更多信息：

*[`medium.com/@ignacio.de.gregorio.noblejas/meet-pi-chatgpts-newest-rival-and-the-most-human-ai-in-the-world-367b461c0af1`](https://medium.com/@ignacio.de.gregorio.noblejas/meet-pi-chatgpts-newest-rival-and-the-most-human-ai-in-the-world-367b461c0af1)*

开发团队使用了来自人类反馈的强化学习（RLHF）来训练这个聊天机器人：

*[`medium.com/@ignacio.de.gregorio.noblejas/meet-pi-chatgpts-newest-rival-and-the-most-human-ai-in-the-world-367b461c0af1`](https://medium.com/@ignacio.de.gregorio.noblejas/meet-pi-chatgpts-newest-rival-and-the-most-human-ai-in-the-world-367b461c0af1)*

### **机器学习和 ChatGPT**

OpenAI 支持一个名为“高级数据分析”（以前称为 Code Interpreter）的插件，该插件使 ChatGPT 能够根据数据集的数据生成生成图表和图形的 Python 代码。此外，高级数据分析可以生成可以在数据集上训练的机器学习模型。

![图片](img/python-3-data-visualization-using-chatgpt-f0246-01.jpg)

***图 7.1*** 由高级数据分析生成的泰坦尼克号图表和图形

顺便说一句，如果你想看看 ChatGPT 生成用于机器学习模型的 Python 代码以及图表和图形的示例，你可以在几本即将出版的书中学习如何做到这一点：

+   *机器学习、Python3 和 ChatGPT*

+   *使用 ChatGPT/GPT-4 的 Python 3*

+   *GPT-4 开发者指南*

前述书籍由 Mercury Learning 出版，将于 2024 年初上市。

### **什么是 InstructGPT？**

InstructGPT 是由 OpenAI 开发的语言模型，它是 ChatGPT 的兄弟模型。InstructGPT 旨在遵循提示中给出的指令以生成详细响应。以下是关于 InstructGPT 的一些要点：

+   指令遵循

+   训练

+   应用

+   局限性

*指令遵循*: 与设计用于开放式对话的 ChatGPT 不同，InstructGPT 是为了在提示中遵循用户指令而开发的。这使得它适合用户希望通过给出明确指令来获取特定信息或输出的任务。

*训练*：InstructGPT 使用与 ChatGPT 类似的强化学习从人类反馈（RLHF）进行训练。最初使用监督微调训练了一个初始模型，其中人类 AI 训练师为双方（用户和 AI 助手）提供了对话。然后，这个新的对话数据集与 InstructGPT 数据集混合，并转换为对话格式。

*应用*：在需要更详细解释、逐步指南或基于提供的指令的特定输出的场景中，InstructGPT 可能很有用。

*局限性*：与其他模型一样，InstructGPT 也有其局限性。它可能会产生不正确或无意义的答案。输出高度依赖于提示语的表达方式。它对输入的表达方式也很敏感，可能会根据轻微的改写给出不同的回答。

随着人工智能模型及其应用的不断发展，InstructGPT 在 2021 年之后可能还有进一步的发展或迭代。请始终参考 OpenAI 的官方出版物和更新以获取最新信息。有关 InstructGPT 的更多信息可在 *[`openai.com/blog/instruction-following/`](https://openai.com/blog/instruction-following/)* 查找。

### **VIZGPT 与数据可视化**

VizGPT 是一个在线工具，允许您指定基于英语的提示，以可视化数据集的各个方面：*[`www.vizgpt.ai/`](https://www.vizgpt.ai/)*。

选择默认的“汽车数据集”，然后点击“数据”按钮以显示数据集的内容，如图 7.2 所示。

![图片](img/python-3-data-visualization-using-chatgpt-f0247-01.jpg)

***图 7.2*** VizGPT “汽车数据集”行示例

接下来，选择默认的“汽车数据集”，然后点击“与 Viz 对话”按钮以显示数据集的可视化，如图 7.3 所示。

![图片](img/python-3-data-visualization-using-chatgpt-f0248-01.jpg)

***图 7.3*** VizGPT “汽车数据集”可视化

您可以进一步实验 VizGPT。例如，您可以通过点击“上传 CSV”按钮上传自己的数据集，并使用该数据集获得类似的结果。

### **什么是 GPT-4？**

GPT-4 于 2023 年 3 月中旬发布，仅通过向现有 ChatGPT 账户付费升级（每月 20 美元）的用户提供。根据用户的各种在线轶事故事，GPT-4 在性能上显著优于 ChatGPT。此外，微软有一个 GPT-4 版本，为 Bing 浏览器提供动力，该浏览器对公众免费提供。

GPT-4 是一个大型多模态模型，可以处理基于图像的输入以及基于文本的输入，然后生成文本输出。目前，基于图像的输出对公众不可用，但它确实有内部支持图像生成。

GPT-4 支持 25,000 个单词的输入文本：相比之下，ChatGPT 的限制为 4,096 个字符。尽管 GPT-4 的参数数量未公开，但以下文章声称 GPT-4 是由 8 个 2200 亿参数模型混合而成的，这是专家混合（MoE）的一个例子：

*[`thealgorithmicbridge.substack.com/p/gpt-4s-secret-has-been-revealed`](https://thealgorithmicbridge.substack.com/p/gpt-4s-secret-has-been-revealed)*

#### **GPT-4 与考试成绩**

一个关于提高准确性的有趣例子是关于律师资格考试，ChatGPT 最初得分在底部 10%。相比之下，GPT-4 在相同的律师资格考试中得分在顶部 10%。更多详情可在网上找到：

*[`www.abajournal.com/web/article/latest-version-of-chatgpt-aces-the-bar-exam-with-score-in-90th-percentile`](https://www.abajournal.com/web/article/latest-version-of-chatgpt-aces-the-bar-exam-with-score-in-90th-percentile)*

此外，GPT-4 显然能够以 3.34 的平均成绩通过哈佛大学一年级。更多详情可在网上找到：

*[`www.businessinsider.com/chatgpt-harvard-passed-freshman-ai-education-GPT-4-2023-7?op=1`](https://www.businessinsider.com/chatgpt-harvard-passed-freshman-ai-education-GPT-4-2023-7?op=1)*

此外，GPT-4 在许多其他测试中也表现出色，其中一些在此列出：

+   AP 考试

+   SAT

+   GRE

+   医学测试

+   法律考试

+   商学院考试

+   华顿商学院 MBA 考试

+   美国生物学奥林匹克半决赛考试

+   葡萄酒师考试（酒保）

您可以从以下链接中了解更多关于前面测试的详细信息：

*[`www.businessinsider.com/list-here-are-the-exams-chatgpt-has-passed-so-far-2023-1`](https://www.businessinsider.com/list-here-are-the-exams-chatgpt-has-passed-so-far-2023-1)*

以下链接包含有关考试成绩、基准和其他与 GPT-4 相关的结果的更多详细信息：*[`openai.com/research/gpt-4`](https://openai.com/research/gpt-4)*。

#### **GPT-4 参数**

本节包含有关一些 GPT-4 参数的信息，其中一些是最佳猜测近似值。

由于 GPT-4 是一个基于 transformer 的自回归模型，它被训练来进行下一个标记的预测。以下论文《GPT4 技术报告》于 2023 年 3 月发布，其中包含了对 GPT-4 能力的详细分析：

*[`docs.kanaries.net/en/tutorials/ChatGPT/gpt-4-parameters`](https://docs.kanaries.net/en/tutorials/ChatGPT/gpt-4-parameters)*

#### **GPT-4 微调**

尽管 OpenAI 允许您微调其四个基础模型，但目前（目前）无法对 ChatGPT 3.5 或 GPT-4 进行微调。相反，您可以通过 LangChain 或 LlamaIndex（之前称为 GPT-Index）将 OpenAI 模型与您自己的数据源集成。它们都能让您将 OpenAI 模型与现有的数据源连接起来。

LangChain 的介绍可在网上找到：

*[`www.pinecone.io/learn/series/langchain/langchain-intro/`](https://www.pinecone.io/learn/series/langchain/langchain-intro/)*

LlamaIndex 的介绍可在网上找到：

*[`zilliz.com/blog/getting-started-with-llamaindex`](https://zilliz.com/blog/getting-started-with-llamaindex)*

*[`stackoverflow.com/questions/76160057/openai-chat-completions-api-how-do-i-customize-answers-from-gpt-3-5-or-gpt-4-mo?noredirect=1&lq=1`](https://stackoverflow.com/questions/76160057/openai-chat-completions-api-how-do-i-customize-answers-from-gpt-3-5-or-gpt-4-mo?noredirect=1&lq=1)*

### **ChatGPT 和 GPT-4 竞争对手**

在 2022 年 11 月 30 日 ChatGPT 发布后不久，各家公司纷纷推出 ChatGPT 的竞争对手，其中一些列在这里：

+   Bard (谷歌聊天机器人)

+   CoPilot (微软)

+   Codex (OpenAI)

+   苹果 GPT (Apple)

+   PaLM 2 (谷歌和 GPT-4 竞争对手)

+   Claude-2 (Anthropic)

+   Llama-2 (Meta) 在后面的部分

以下小节包含有关前面列表中 LLM 的更多详细信息。

#### **Bard**

Bard 是谷歌在 2023 年初发布的人工智能聊天机器人，作为 ChatGPT 的竞争对手。Bard 由 PaLM 2 提供支持，而 ChatGPT 由 GPT-4 提供支持。最近，Bard 在其对用户查询的回答中增加了对图像的支持，而 ChatGPT 的这一功能尚未向公众发布（但您可能很快就会看到它可用）。

*[`artificialcorner.com/google-bards-new-image-recognition-means-serious-competition-to-chatgpt-here-are-6-best-use-cases-55d69eae1b27`](https://artificialcorner.com/google-bards-new-image-recognition-means-serious-competition-to-chatgpt-here-are-6-best-use-cases-55d69eae1b27)*

Bard 在一场备受瞩目的发布中遇到了与詹姆斯·韦伯太空望远镜相关的问题，这导致 Alphabet 的市场资本大幅下降。然而，谷歌一直在努力修复问题并增强 Bard 的功能。您可以通过以下链接访问 Bard：*[`bard.google.com/`](https://bard.google.com/)*。

大约在 2023 年中期，Bard 增加了几个在同期 GPT-4 中不可用的功能，其中一些列在这里：

+   生成图像

+   从图像中生成 HTML/CSS

+   从图像中生成移动应用程序

+   从图像中创建 LaTeX 公式

+   从图像中提取文本

据推测，这些功能将促使 OpenAI 提供相同的功能集（其中一些已在 GPT-4 中实现，但尚未公开提供）。

#### **CoPilot (OpenAI/Microsoft)**

微软 CoPilot 是一个由 GPT-4 提供支持的 Visual Studio Code 扩展。GitHub CoPilot 因其能够在程序上下文中生成代码块而闻名。此外，微软还在开发 Microsoft 365 CoPilot，截至 2023 年中尚未宣布其可用日期。

然而，微软已经提供了早期演示，展示了 Microsoft 365 CoPilot 的一些功能，包括自动化以下任务：

+   写电子邮件

+   汇总会议

+   制作 PowerPoint 演示文稿

Microsoft 365 CoPilot 可以分析 Excel 电子表格中的数据，在 PowerPoint 中插入 AI 生成的图像，并生成求职信草稿。微软还将 Microsoft 365 CoPilot 集成到其一些现有产品中，例如 Loop 和 OneNote。

根据以下文章，微软打算为 Office 365 Copilot 每月收费 30 美元：

*[`www.extremetech.com/extreme/microsoft-to-charge-30-per-month-for-ai-powered-office-apps`](https://www.extremetech.com/extreme/microsoft-to-charge-30-per-month-for-ai-powered-office-apps)*

CoPilot 在 2022 年底被逆向工程，相关信息在网上有描述：

*[`thakkarparth007.github.io/copilot-explorer/posts/copilot-internals`](https://thakkarparth007.github.io/copilot-explorer/posts/copilot-internals)*

以下文章展示了如何创建一个使用 NextJS、React 和 CoPilot 的 GPT-3 应用程序：

*[`github.blog/2023-07-25-how-to-build-a-gpt-3-app-with-nextjs-react-and-github-copilot/`](https://github.blog/2023-07-25-how-to-build-a-gpt-3-app-with-nextjs-react-and-github-copilot/)*

#### **Codex (OpenAI)**

OpenAI Codex 是一个基于 GPT3 的微调 LLM，可以从文本生成代码。实际上，Codex 为 GitHub Copilot 提供动力。Codex 在从超过 5000 万个 GitHub 仓库中获得的超过 150GB 的 Python 代码上进行了训练。

根据 OpenAI 的说法，Codex 的主要目的是加速人类编程，它可以完成近 40%的请求。Codex 在生成用于解决简单任务的代码方面表现得相当不错。访问 Codex 主页以获取更多信息：*[`openai.com/blog/openai-codex`](https://openai.com/blog/openai-codex)*。

#### **Apple GPT**

2023 年中，苹果宣布了 Apple GPT，这是 OpenAI ChatGPT 的竞争对手。实际发布日期预计为 2024 年。“Apple GPT”是当前用于与 Google Bard、OpenAI ChatGPT 和微软 Bing AI 竞争的产品的名称。

简而言之，LLM PaLM 2 为 Google Bard 提供动力，GPT-4 为 ChatGPT 以及 Bing Chat 提供动力，而 Ajax 则是 Apple GPT 的动力来源。Ajax 基于谷歌的 Jax。

#### **PaLM-2**

PaLM-2 是 Pathways 语言模型的第二个版本，是 PaLM（约 2022 年）的继任者。PaLM-2 为 Bard 提供动力，它也是 GPT-4 的直接竞争对手。相比之下，PaLM 由 540B 个参数组成，PaLM-2 可能是一个更大的 LLM（后者的详细信息未公开）。

PaLM-2 提供了四个子模型，称为 Gecko、Otter、Bison 和 Unicorn（从小到大）。PaLM-2 在超过 100 种人类语言以及 Fortran 等编程语言上进行了训练。此外，PaLM-2 已被部署到包括 Gmail 和 YouTube 在内的众多谷歌产品中。

#### **Med-PaLM M**

除了上述四个子模型之外，Med-PaLM 2（Med-PaLM 的继任者）是一个提供医疗问题答案的 LLM，您可以在以下网址在线访问：*[`sites.research.google/med-palm/`](http://sites.research.google/med-palm/)*.

Med-PaLM 的继任者是 Med-PaLM M，有关此 LLM 的详细信息可在以下网址找到：*[`arxiv.org/abs/2307.14334`](https://arxiv.org/abs/2307.14334)*.

以下文章提供了 PaLM 2 和 GPT-4 性能基准的直接比较：

*[`www.makeuseof.com/google-palm-2-vs-openai-gpt-4/`](https://www.makeuseof.com/google-palm-2-vs-openai-gpt-4/)*

总的来说，PaLM-2 具有强大的功能集，它无疑是 GPT-4 的一个重大竞争对手。

#### **Claude-2**

Anthropic 创建了 LLM Claude-2，它不仅能够回答关于特定主题的问题，还能执行涉及多个文档的搜索、总结文档、创建文档和生成代码。

Claude-2 是 Anthropic 的前辈 Claude 1.3 的改进版，它可以摄入整本书，并根据用户的提示生成代码。实际上，Claude-2 在竞争功能方面似乎可以与 ChatGPT 和 GPT-4 相媲美。

此外，Claude-2 支持 100,000 个标记的上下文窗口。Claude-2 在 2023 年初的数据上进行了训练，而 ChatGPT 在 2021 年之前的数据上进行了训练。然而，Claude-2 无法搜索网络（与竞争对手 GPT-4 不同）。Anthropic 可能会继续在 LLM 领域开发其功能。

### **LLAMA-2**

Llama-2（大型语言模型 Meta AI）是 Meta 的一个开源微调 LLM，仅在公共数据上训练，在 AI 社区中引起了很大的兴奋。Llama-2 提供了三个模型（7B、13B 和 70B 参数），在预训练步骤中使用了比许多其他 LLM 更多的数据。Llama-2 经过优化，可以提供更快的推理，并且比其他 LLM 提供更长的上下文长度（4K）。

此外，Llama-2-Chat LLM 的表现出人意料地好：在某些情况下，其质量接近高性能 LLM 如 ChatGPT 和 GPT-4 的质量。与 GPT-4 相比，Llama-2 更易于使用，并且在撰写文本方面提供更好的结果。另一方面，GPT-4 更适合生成代码等任务。

#### **如何下载 Llama-2**

Llama-2 为社区使用和商业使用提供了许可协议，Meta 已将代码以及预训练模型和微调模型公开。

您可以从 Meta 提供的链接开始下载 Llama-2，在提供一些信息（姓名、国家、所属机构）后：

*[`ai.meta.com/llama/`](https://ai.meta.com/llama/)*

通过以下链接可以访问 7B、13B 和 70B 模型的演示：

*[`huggingface.co/spaces/huggingface-projects/llama-2-7b-chat`](https://huggingface.co/spaces/huggingface-projects/llama-2-7b-chat)*

*[`huggingface.co/spaces/huggingface-projects/llama-2-13b-chat`](https://huggingface.co/spaces/huggingface-projects/llama-2-13b-chat)*

*[`huggingface.co/spaces/ysharma/Explore_llamav2_with_TGI`](https://huggingface.co/spaces/ysharma/Explore_llamav2_with_TGI)*

在 Hugging Face 上访问 Llama-2 的第三种方式是以下链接：*[`huggingface.co/blog/llama2`](https://huggingface.co/blog/llama2)*

更多信息可在网上找到：

*[`github.com/facebookresearch/llama`](https://github.com/facebookresearch/llama)*

*[`ai.meta.com/research/publications/llama-2-open-foundation-and-fine-tuned-chat-models/`](https://ai.meta.com/research/publications/llama-2-open-foundation-and-fine-tuned-chat-models/)*

如果你对在笔记本电脑上训练 Llama-2 感兴趣，更多细节可以在以下链接中找到：*[`blog.briankitano.com/llama-from-scratch/`](https://blog.briankitano.com/llama-from-scratch/)*。

#### **Llama-2 架构特点**

本节仅包含一些 Llama-2 重要区分特征的概述，如下所示：

+   仅解码器 LLM

+   更好的预训练

+   改进的模型架构

+   SwiGLU 激活函数

+   不同的位置嵌入

+   GQA（分组查询注意力）

+   幽灵注意力（GAtt）

+   RLHF 和 PPO

+   BPE SentencePiece 分词器

+   修改后的归一化步骤

大多数 LLM 包含原始 Transformer 架构中的层归一化。相比之下，Llama 使用了一种简化的替代方案，涉及根均方层归一化（RMSNorm）。RMSNorm 在训练稳定性和泛化方面都取得了改进的结果。

尽管 SwiGLU 在计算上比原始 Transformer 架构中的 ReLU 激活函数更昂贵，但 SwiGLU 实现了更好的性能。

注意，RLHF 之前已经讨论过，该部分包括 TRPO 和 PPO 的简要描述。有关如何对 Llama-2 在三个任务上进行微调的详细描述，请访问以下链接：

*[`www.anyscale.com/blog/fine-tuning-llama-2-a-comprehensive-case-study-for-tailoring-models-to-unique-applications`](https://www.anyscale.com/blog/fine-tuning-llama-2-a-comprehensive-case-study-for-tailoring-models-to-unique-applications)*

#### **微调 Llama-2**

虽然 Llama-2 是其前身 Llama 的改进，但你可以通过对这种 LLM 进行一些微调来进一步提高 Llama-2 的性能。

*[`medium.com/@murtuza753/using-llama-2-0-faiss-and-langchain-for-question-answering-on-your-own-data-682241488476`](https://medium.com/@murtuza753/using-llama-2-0-faiss-and-langchain-for-question-answering-on-your-own-data-682241488476)*

以下文章展示了如何在 Google Colaboratory 笔记本中微调 Llama-2：

*[`towardsdatascience.com/fine-tune-your-own-llama-2-model-in-a-colab-notebook-df9823a04a32`](https://towardsdatascience.com/fine-tune-your-own-llama-2-model-in-a-colab-notebook-df9823a04a32)*

以下文章描述了如何使用 MonsterAPI（文章中也讨论了）在五步中微调 LlaMa-2。

*[`blog.monsterapi.ai/how-to-fine-tune-llama-2-llm/`](https://blog.monsterapi.ai/how-to-fine-tune-llama-2-llm/)*

以下链接描述了如何在 Google Colaboratory 中访问 Llama-2。

*[`levelup.gitconnected.com/harnessing-the-power-of-llama-2-using-google-colab-2e1dedc2d1d8`](https://levelup.gitconnected.com/harnessing-the-power-of-llama-2-using-google-colab-2e1dedc2d1d8)*

### **GPT-5 何时可用？**

当这本书准备印刷时，关于 GPT-5 的状态没有官方信息可用，也就是说，一切都是推测性的。在 2023 年初，OpenAI 的 CEO 萨姆·奥特曼（Sam Altman）表示，对于 GPT-5“没有官方计划”。

然而，在 2023 年中，OpenAI 为 GPT-5 申请了一项专利，其中包含一些关于 GPT-5 功能的高级细节。有些人推测 GPT-5 将是 GPT-4 的更强大版本，而其他人则认为申请专利可能只是确保“GPT-5”这个名称。

无论申请专利的动机如何，与 GPT-4 来自不同公司的竞争都非常激烈。因此，OpenAI 可能会发布 GPT-5，也许是在 2023 年底。关于模型大小，回想一下，GPT-3 有 1750 亿个参数，有些人推测 GPT-4 有 100 万亿个参数，这意味着 GPT-4 大约是 GPT-3 的 60 倍。GPT-5 规模增加的幅度似乎是不可能的，因为那时 GPT-5 将包含 600 万亿个参数。

另一种可能性是，GPT-4 基于涉及多个组件的专家混合方法。例如，GPT-4 可能是 8 个组件的组合，每个组件涉及 2.2 亿个参数，因此 GPT-4 将包含 1.76 万亿个参数。

请记住，训练像 GPT-4 这样的 LLM（大型语言模型）非常昂贵，并且需要大量的数据集进行预训练步骤。无论 GPT-5 最终的大小如何，训练过程都可能涉及巨大的成本。

### **总结**

本章从 OpenAI 的 ChatGPT 及其一些功能开始讨论。此外，你还了解了一些 ChatGPT 的竞争对手，例如 Anthropic 的 Claude-2。

接下来，你学习了 OpenAI 的 GPT-4，它是 ChatGPT 的驱动力，以及它的一些功能。然后你学习了 GPT-4 的一些竞争对手，例如 Meta 的 Llama-2 和 Google 的 Bard。

## **第八章**

## *ChatGPT 与数据可视化*

本章包含使用 ChatGPT 进行数据可视化的示例，例如创建基于数据集（例如，泰坦尼克号数据集）的图表和图形。ChatGPT 通过高级数据分析插件生成了这里显示的所有代码示例。ChatGPT 还生成了基于 Python 代码示例的一些配套文本。

本章的第一部分描述了在 ChatGPT 中上传数据集的过程，然后提供了解释给定数据集特征、生成可视化效果和下载精选数据集等任务的提示。您还将学习如何提示 ChatGPT 创建和训练机器学习模型。

本章的第二部分包含使用 Matplotlib 进行数据可视化的示例，其中代码示例是由 ChatGPT 生成的。本章的第三部分包含使用 Seaborn 进行数据可视化的示例，其中代码示例也是由 ChatGPT 生成的。

在阅读本章内容后，请将本章中的代码示例与第五章（Matplotlib）和第六章（Seaborn）中的代码示例进行比较。

关于本章中的代码示例，还有一个需要注意的细节，所有这些示例都是由 ChatGPT 生成的。提供给 ChatGPT 的提示的通用格式如下所示：

*“请生成使用 Matplotlib 渲染[指定图表类型]的 Python 代码。”*

本章的前几个代码示例提供了 ChatGPT 用于生成给定 Python 代码的提示。

### **与图表和图形一起工作**

每种图表类型都有其独特的优势，最适合特定类型的数据和分析。图表的选择通常取决于数据的性质和想要得出的具体见解。本节包含多个子节，提供了关于各种图表和图形的信息，如下所示：

+   柱状图

+   饼图

+   折线图

+   热图

+   直方图

+   箱线图

+   帕累托图

+   雷达图

+   树状图

+   水波图

+   散点图

上述列表中的每个图表和图形将在以下子节中进行讨论。

#### **柱状图**

柱状图用矩形条表示数据，条的长度与它们所代表的值成比例。它们可以是垂直的（柱状图）或水平的。一个使用示例是比较商店中不同产品的销售情况。

柱状图的一些优点如下：

+   容易理解和广泛认可

+   可以比较单个或多个数据序列

+   适用于显示跨越多个类别的数据

柱状图的一些缺点如下：

+   不适合展示随时间变化的模式或趋势

+   比较太多类别时可能会变得杂乱

#### **饼图**

饼图以圆形格式表示数据，各个部分（切片）显示类别与整体的比例。一个使用示例是表示一个行业中不同公司的市场份额。

饼图的一些优点如下：

+   简单的视觉表示，展示了部分与整体的关系

+   清楚地表明比例。

+   当类别数量有限时，效果良好

饼图的一些缺点如下：

+   不适用于比较单个类别

+   当切片过多时，可能会变得无效且难以解释

+   不显示绝对值，只显示比例

#### **线形图**

线形图通过直线连接数据点来显示数据。它们主要用于可视化连续区间或时间段内的值。一个使用示例包括跟踪一家公司在几年内的收入增长。

线形图的一些优点如下：

+   有效地显示趋势。

+   可以在一张图上比较多个数据系列

+   清晰地可视化数据点和区间

线形图的一些缺点如下：

+   不适合显示部分与整体的关系

+   当显示过多的数据系列时可能会变得杂乱

+   需要数据点的有意义顺序

#### **热图**

热图以矩阵格式表示数据，其中单个值以颜色表示。颜色强度通常表示值的幅度。一个使用示例包括可视化网页访问者在网页不同部分的活动。

热图的一些优点如下：

+   快速识别模式、相关性和集中区域

+   有效地使用颜色来传达关于量级的信息

热图的一些缺点如下：

+   不适合进行详细的数值分析

+   颜色选择至关重要；选择不当可能会误导解释

#### **直方图**

直方图是数据集分布的图形表示。它是连续变量概率分布的估计。一个使用示例包括显示人口中年龄的分布。

直方图的一些优点如下：

+   通过指示位于值范围内的数据点数量来提供数值数据的视觉解释

+   可以帮助识别数据分布模式

直方图的一些缺点如下：

+   不显示确切值

+   箱的数量和宽度可以影响感知

#### **箱线图**

箱线图使用四分位数来表示数据集的摘要。其中，“箱”表示四分位数范围，而“胡须”表示超出上下四分位数的变化。一个使用示例包括比较不同团队的销售额表现。

箱线图的一些优点如下：

+   快速可视化数据的分布和偏斜

+   识别异常值

箱线图的一些缺点如下：

+   不适合进行详细的分布分析

+   不显示数据的频率分布

#### **帕累托图**

帕累托图结合条形图和线形图来表示发生累积频率。它们识别数据集中的最重要因素。一个使用示例包括确定哪些产品缺陷最频繁地发生。

帕累托图的一些优点如下：

+   高效地突出大型数据集中最重要的因素

+   帮助优先考虑努力

帕累托图的一些缺点如下：

+   限于与排名和优先级相关的数据集

+   不适合展示数据点之间的关系

#### **雷达图**

雷达图是一种在二维图表中显示三个或更多定量变量的图形方法。数据点绘制在从中心开始的轴上。使用示例包括比较产品的性能指标。

雷达图的优点如下：

+   可以比较多个定量变量

+   提供数据的视觉概述

雷达图的缺点如下：

+   比较太多数据集时可能会变得杂乱

+   在值相似的情况下难以解释

#### **树状图**

树状图以嵌套矩形的形式显示层次数据。每个层次分支由彩色矩形表示。使用示例包括可视化计算机上的存储使用情况。

树状图的优点如下：

+   空间使用效率高

+   可以使用大小和颜色表示多个维度

树状图的缺点如下：

+   不适合具有大型层次结构的数据集

+   可能变得难以解释

#### **瀑布图**

水流图表示依次发生的正或负值的累积效应。使用示例包括可视化利润或收入如何受各种因素的影响。

水流图的优点如下：

+   清晰地可视化正负顺序变化

+   帮助理解从一个数据点到另一个数据点的逐渐过渡

水流图的缺点如下：

+   限于需要理解顺序变化的情况

+   数据点过多时可能会变得混乱。

### **使用 Matplotlib 的线图**

让我们绘制一个简单的线图来可视化趋势。列表 8.1 显示了 ChatGPT 生成的用于使用 Matplotlib 渲染线的 line_plots.py 的内容。ChatGPT 的提示如下：

*“请生成使用 Matplotlib 渲染线图的 Python 代码。”*

***列表 8.1: line_plot.py***

```py
 import matplotlib.pyplot as plt

def plot_line(x, y, title, x_label, y_label):
    plt.plot(x, y)
    plt.title(title)
    plt.xlabel(x_label)
    plt.ylabel(y_label)
    plt.grid(True)
    plt.show()
# Usage
x = [1, 2, 3, 4, 5]
y = [2, 4, 1, 3, 5]
plot_line(x, y, 'Sample Line Graph', 'X-Axis', 'Y-Axis') 
```

列表 8.1 从一个导入语句开始，然后定义了 plot_line()函数，该函数用于渲染线图。Matplotlib 的 plot()函数提供了一个创建线图的直接方法。在这个函数中，我们可视化 x 轴和 y 轴上的趋势。

代码的下一部分初始化了 Python 列表 x 和 y，然后使用三个字符串调用 plot_line()，这三个字符串分别是标题、横轴和纵轴的值。图 8.1 显示了在列表 8.1 中启动代码的输出。

![图片](img/python-3-data-visualization-using-chatgpt-f0262-01.jpg)

***图 8.1*** 使用 Matplotlib 的线图

### **使用 Matplotlib 的饼图**

饼图非常适合显示类别之间的比例数据。Matplotlib 的饼图函数提供了一个简单的方法来实现这一点。列表 8.2 显示了 ChatGPT 生成的用于使用 Matplotlib 绘制饼图的 pie_chart1.py 的内容。ChatGPT 的提示如下：

*“请生成用于使用 Matplotlib 绘制饼图的 Python 代码。”*

***列表 8.2: pie_chart1.py***

```py
 import matplotlib.pyplot as plt

def plot_pie(labels, sizes, title):
    plt.pie(sizes, labels=labels, autopct='%1.1f%%', startangle=140)
    plt.title(title)
    plt.axis('equal')  # Equal aspect ratio ensures the pie
is drawn as a circle. plt.show()

# Usage
labels = ['A', 'B', 'C']
sizes = [215, 130, 245]
plot_pie(labels, sizes, 'Sample Pie Chart') 
```

列表 8.2 以与列表 8.1 类似的方式开始，除了生成了用于生成饼图的 plot_pie()函数。列表 8.2 的下一部分初始化 Python 列表的标签和大小，并使用这些列表以及作为饼图标题显示的字符串调用 plot_pie()函数。图 8.2 显示了通过在列表 8.2 中启动代码生成的饼图。

![图片](img/python-3-data-visualization-using-chatgpt-f0263-01.jpg)

***图 8.2*** 使用 Matplotlib 创建的饼图

### **使用 Matplotlib 进行箱线和须线图**

箱线图，或箱线图，提供了数据分布的总结，突出了中心趋势、变异性和异常值的存在。它们在比较不同组之间的分布时特别有用。它们可以根据最小值、第一四分位数、中位数、第三四分位数和最大值显示数据的分布。

列表 8.3 显示了 ChatGPT 生成的用于使用 Seaborn 绘制箱线图的 boxplot1.py 的内容。ChatGPT 的提示如下：

*“请生成用于使用 Matplotlib 绘制箱线图的 Python 代码。”*

ChatGPT 的提示如下：

*“请生成用于使用 Matplotlib 绘制折线图的 Python 代码。”*

***列表 8.3: boxplot1.py***

```py
 import matplotlib.pyplot as plt
import seaborn as sns

import matplotlib.pyplot as plt

def plot_box(data, column):
    plt.boxplot(data[column])
    plt.show()

# Usage
data = sns.load_dataset("iris")
plot_box(data, "sepal_length") 
```

列表 8.3 包含三个导入语句，随后是生成箱线图的 plot_box()函数。列表 8.3 的下一部分初始化变量 data 为 Seaborn 内置的 iris 数据集的内容，然后使用 data 和一个指定在绘制箱线图时使用的特征（列）的字符串调用 plot_box()。图 8.3 显示了通过在列表 8.3 中启动代码生成的箱线图。

![图片](img/python-3-data-visualization-using-chatgpt-f0264-01.jpg)

***图 8.3*** 使用 Matplotlib 创建的箱线图

### **使用 Matplotlib 进行时间序列可视化**

时间序列数据，其中观察值是在固定时间间隔内进行的，可以使用线图进行可视化。这使分析师能够辨别趋势、模式和异常。

让我们绘制时间序列数据，以了解随时间的变化趋势。列表 8.4 显示了 ChatGPT 生成的用于使用 Matplotlib 绘制时间序列的 time_series.py 的内容。

***列表 8.4: time_series.py***

```py
 import matplotlib.pyplot as plt

import pandas as pd

def plot_time_series(dates, values, title):
    plt.figure(figsize=(10, 5))
    plt.plot(dates, values)
    plt.title(title)
    plt.xlabel('Date')
    plt.ylabel('Value')
    plt.tight_layout()
    plt.show()

# Usage
dates = pd.date_range(start="2021-01-01", periods=10, freq='D')
values = [x**1.5 for x in range(10)]
plot_time_series(dates, values, 'Sample Time Series Data') 
```

图 8.4 显示了通过在列表 8.10 中启动代码生成的时间序列。

![图片](img/python-3-data-visualization-using-chatgpt-f0265-01.jpg)

***图 8.4*** 使用 Matplotlib 创建的时间序列

### **使用 MATPLOTLIB 制作堆叠条形图**

堆叠条形图允许在每个类别中表示子组，给人一种在类别中的总大小以及子组分布的感觉。

列表 8.5 显示了 ChatGPT 生成的 stacked_bar_charts.py 的内容，用于使用 Matplotlib 渲染堆叠条形图。

***列表 8.5: stacked_bar_charts.py***

```py
 import matplotlib.pyplot as plt
import numpy as np

def plot_stacked_bar(data, labels, categories):
    cum_size = np.zeros(len(categories))

    for i, label in enumerate(labels):
        plt.bar(categories, data[label], bottom=cum_size, label=label)
        cum_size += data[label]

    plt.legend()
    plt.show()

# Usage
data = {
    'A': [10, 15, 20],
    'B': [5, 10, 5]
}
labels = ['A', 'B']
categories = ['Category 1', 'Category 2', 'Category 3']
plot_stacked_bar(data, labels, categories) 
```

图 8.5 显示了通过运行列表 8.5 中的代码生成的堆叠条形图。

![图片](img/python-3-data-visualization-using-chatgpt-f0266-01.jpg)

***图 8.5*** 使用 Matplotlib 创建的堆叠条形图

### **使用 MATPLOTLIB 制作饼图**

饼图的一种变体是环形图。空心中心可以用于额外的注释或只是提供不同的美学。我们可以使用它们在类别之间按比例表示数据，类似于饼图，但具有空心中心。列表 8.6 显示了 ChatGPT 生成的 donut_charts.py 的内容，用于使用 Matplotlib 渲染环形图。

***列表 8.6: donut_charts.py***

```py
 import matplotlib.pyplot as plt

def plot_donut_chart(sizes, labels, title, hole_size=0.3):
    fig, ax = plt.subplots()
    ax.pie(sizes, labels=labels, autopct='%1.1f%%',
startangle=90, wedgeprops=dict(width=hole_size))
    ax.axis('equal')
    plt.title(title)
    plt.show()

# Usage
labels = ['A', 'B', 'C']
sizes = [215, 130, 245]
plot_donut_chart(sizes, labels, 'Sample Donut Chart') 
```

图 8.6 显示了通过运行列表 8.13 中的代码生成的饼图。

![图片](img/python-3-data-visualization-using-chatgpt-f0267-01.jpg)

***图 8.6*** 使用 Seaborn 创建的饼图

### **使用 MATPLOTLIB 制作 3D 表面图**

3D 表面图用于可视化具有两个变量的函数。它们可以揭示数据中的复杂模式和关系。列表 8.7 显示了 ChatGPT 生成的 3d_surface.py 的内容，用于使用 mpl_toolkits 渲染 3D 表面。

顺便说一句，如果你遇到 mpl_toolkits 的问题，请阅读以下包含有用信息的帖子：

*[`stackoverflow.com/questions/37661119/python-mpl-toolkits-installation-issue`](https://stackoverflow.com/questions/37661119/python-mpl-toolkits-installation-issue)*

***列表 8.7: 3d_surface.py***

```py
 import matplotlib.pyplot as plt
import numpy as np

def plot_3d_surface(x, y, z):
    fig = plt.figure()
    ax = fig.add_subplot(111, projection='3d')
    ax.plot_surface(x, y, z, cmap='viridis')
    plt.show()

# Usage
x = np.linspace(-5, 5, 50)
y = np.linspace(-5, 5, 50)
x, y = np.meshgrid(x, y)
z = np.sin(np.sqrt(x**2 + y**2))
plot_3d_surface(x, y, z) 
```

列表 8.7 从两个导入语句开始，接着是 plot_3d_surface()函数，用于渲染 3D 图。列表 8.7 的下半部分通过 NumPy 函数 linspace()初始化变量 x 和 y，该函数将区间划分为一组等大小的子区间。

例如，代码片段 np.linspace(-5, 5, 50)将区间[-5,5]划分为 50 个等间距的点，这意味着有 49 个等宽的区间。你可以通过将 50 替换为 3 来证明这是真的：结果是左端点-5，中点，和右端点 5，这创建了 2（=3-1）个区间。

下一个代码片段使用 NumPy 中的 meshgrid()函数的结果更新 x 和 y，之后定义 z 为从原点到点(x,y)的距离的正弦函数。尽管后者随着点(x,y)远离原点而单调增加，而 z 是那个距离的正弦值，它是一个周期函数：因此，你会看到一个滚动的波浪状效果。

列表 8.7 中的最后一个代码片段使用变量 x、y 和 z 中的值调用 plot_3d_surface()函数。现在运行列表 8.7 中的代码，你将看到图 8.7 中显示的 3D 表面。

![图片](img/python-3-data-visualization-using-chatgpt-f0269-01.jpg)

***图 8.7*** 使用 Matplotlib 创建的 3D 表面

### **使用 Matplotlib 的径向图或蜘蛛图**

径向图或蜘蛛图用于以二维图表的形式可视化多变量数据，其中包含三个或更多定量变量。每个变量都表示在从图表中心开始的单独轴上。这些图表使我们能够比较多个定量变量。

列表 8.8 展示了 ChatGPT 生成的用于使用 Matplotlib 绘制径向图的 radial_charts.py 的内容。

***列表 8.8: radial_charts.py***

```py
 import matplotlib.pyplot as plt
import numpy as np

def plot_spider_chart(values, categories, title):
    angles = np.linspace(0, 2 * np.pi, len(categories),
endpoint=False).tolist()
    values += values[:1]
    angles += angles[:1]

    fig, ax = plt.subplots(figsize=(6, 6), subplot_
kw=dict(polar=True))
    ax.fill(angles, values, color='blue', alpha=0.25)
    ax.set_yticklabels([]) # the following snippet causes an error:
# ax.set_xticks(angles)
# the following snippet is correct:
ax.set_xticks(angles[:-1])  # Exclude the last angle since it’s cyclic ax.set_xticklabels(categories)

    plt.title(title, size=20, color="blue", y=1.1)
    plt.show()

# Usage
categories = ["A", "B", "C", "D"]
values = [50, 30, 60, 40]
plot_spider_chart(values, categories, 'Sample Spider Chart') 
```

列表 8.8 从两个导入语句开始，接着是 plot_spider_chart()函数，该函数用于绘制径向图。列表 8.8 的下一部分初始化了 categories 和 values 变量为两个 Python 列表，然后使用 categories、values 和用于图表标题的文本字符串调用 plot_spider_chart()函数。图 8.8 显示了通过运行列表 8.8 中的代码生成的径向图。

![图片](img/python-3-data-visualization-using-chatgpt-f0270-01.jpg)

***图 8.8*** 使用 Matplotlib 创建的径向图

一个额外的细节，这将帮助你调试 ChatGPT 为你生成的代码。让我们看看列表 8.8 中加粗的代码块：

```py
# the following snippet causes an error:
# ax.set_xticks(angles)
# the following snippet is correct:
ax.set_xticks(angles[:-1])  # Exclude the last angle since it’s cyclic

```

如果你颠倒两个代码片段的顺序，代码将无法正确工作。以下是请求解决方案所需的与 ChatGPT 的“对话”。

*我：我上传了包含你为我编写的代码的 radial_charts.py。然而，这段代码导致这个错误：ValueError：FixedLocator 位置的数目（5），通常来自 set_ticks 的调用，与 ticklabels 的数目（4）不匹配。你能提供解决方案吗？*

```py
 ChatGPT:
Thank you for providing the radial_charts.py file. Let's
start by reading its content to understand the structure and
context of the code. After that, I'll analyze the potential
causes of the mentioned error and offer a solution. The provided radial_charts.py file contains a function,
plot_spider_chart, which is designed to plot a spider (or
radar) chart using given values and categories. Based on the error you reported and the code's structure,
the issue likely arises from the mismatch between the
number of tick locations (set by ax.set_xticks(angles))
and the number of tick labels (set by ax.set_
xticklabels(categories)). To address this, I'll ensure that the number of tick locations
matches the number of tick labels. Let's proceed to make this
adjustment and provide a corrected version of the function. 
```

*我：现在工作正常了！感谢你的帮助！*

```py
 ChatGPT:
You're welcome! I'm glad to hear it's working as expected now. If you have any more questions or need further assistance in
the future, don't hesitate to reach out. Happy coding! 
```

### **MATPLOTLIB 的等高线图**

等高线图有助于使用等高线可视化三维数据在二维中的数据。每条等高线代表相等值的点。这些图帮助我们可视化 3D 数据的等高线。

列表 8.9 展示了 ChatGPT 生成的用于使用 Matplotlib 绘制等高线的 contour_lines.py 的内容。

***列表 8.9: contour_lines.py***

```py
 import matplotlib.pyplot as plt
import numpy as np

def plot_contour(x, y, z):
    plt.contourf(x, y, z, 20, cmap='viridis')
    plt.colorbar()
    plt.show() # Usage
x = np.linspace(-5, 5, 50)
y = np.linspace(-5, 5, 50)
x, y = np.meshgrid(x, y)
z = np.sin(np.sqrt(x**2 + y**2))
plot_contour(x, y, z) 
```

列表 8.9 包含两个导入语句，然后定义了用于渲染代码示例等高线的函数 plot_contour()。请注意，列表 8.9 的第二部分与 列表 8.7 的后半部分几乎相同。图 8.9 显示了通过运行 列表 8.9 中的代码所渲染的等高线图。

![图片](img/python-3-data-visualization-using-chatgpt-f0272-01.jpg)

***图 8.9*** 使用 Matplotlib 创建的等高线图

### **矢量场的流线图**

流线图用于显示矢量场，如风向。它们提供了流动轨迹的快照，并且可以针对标量数据进行着色。它们使我们能够将矢量场作为流线可视化。

列表 8.10 显示了 ChatGPT 生成的用于使用 Seaborn 绘制流线图的 stream_plot.py 的内容。

***列表 8.10: stream_plot.py***

```py
 import matplotlib.pyplot as plt
import seaborn as sns
import numpy as np

def plot_streamplot(x, y, u, v):
    plt.streamplot(x, y, u, v, density=1)
    plt.show() # Usage
x = np.linspace(-5, 5, 10)
y = np.linspace(-5, 5, 10) # this causes an error:
#y, x = np.meshgrid(y, x)
# this works correctly:
x, y = np.meshgrid(x, y) u = -1 - x**2 + y
v = 1 + x - y**2
plot_streamplot(x, y, u, v) 
```

图 8.18 显示了通过运行 列表 8.10 中的代码所渲染的流线图。

![图片](img/python-3-data-visualization-using-chatgpt-f0273-01.jpg)

***图 8.10*** 使用 Seaborn 创建的流线图

ChatGPT 中 列表 8.10 的初始代码没有正确运行，因此我在接下来的“对话”中请求 ChatGPT 提供解决方案。

*我：我上传了包含你为我编写的代码的 stream_plot.py。这段代码导致以下错误：ValueError: ‘x’ 的行必须相等。你能提供解决方案吗？*

```py
 ChatGPT:
The shapes of the arrays x, y, u, and v are all
(10,10), which means they are consistent in terms of
dimensions. The error message "ValueError: The rows of 'x' must be
equal" suggests that there might be an issue with the values
within the rows of the x array, rather than its shape. The line y, x = np.meshgrid(y, x) swaps the original x and
y arrays. This might be causing inconsistencies in the rows
of the x array. To address the error, I'll modify the meshgrid creation and
ensure the x and y arrays are correctly initialized. Let's
make the necessary adjustments. 
```

*我：这成功了！谢谢你的帮助！*

```py
 ChatGPT:
You're welcome! I'm glad to hear it's working as expected
now. If you have any more questions or need further
assistance in the future, don't hesitate to reach out. Happy coding! 
```

### **矢量场的箭头图**

箭头图对于表示矢量场很有用，可以显示矢量的方向和大小。例如，它们可以用于物理学中显示电场或流体流动方向。它们使我们能够可视化矢量的方向和大小。

列表 8.11 显示了 ChatGPT 生成的用于使用 Matplotlib 绘制箭头图的 quiver_plot.py 的内容。

***列表 8.11: quiver_plot.py***

```py
 import matplotlib.pyplot as plt
import numpy as np

def plot_quiver(x, y, u, v):
    plt.quiver(x, y, u, v, scale=20)
    plt.show()

# Usage
x, y = np.meshgrid(np.arange(0, 2 * np.pi, .2), np.arange(0, 2 * np.pi, .2))
u = np.sin(x)
v = np.cos(y)
plot_quiver(x, y, u, v) 
```

图 8.11 显示了通过运行 列表 8.11 中的代码所渲染的箭头图。

![图片](img/python-3-data-visualization-using-chatgpt-f0275-01.jpg)

***图 8.11*** 使用 Matplotlib 创建的箭头图

### **极坐标图**

极坐标图或径向图适合在二维图表中显示多变量数据，其中变量表示从同一点开始的轴。它们对于根据角度和大小查看模式很有用。它们使我们能够以值和角度来显示数据。

列表 8.12 显示了 ChatGPT 生成的用于使用 Seaborn 绘制堆叠条形图的 facet_grids.py 的内容。

***列表 8.12: polar_plots.py***

```py
 import matplotlib.pyplot as plt
import numpy as np

def plot_polar(theta, radii, title=""):
    plt.figure(figsize=(8, 4))
    ax = plt.subplot(111, projection='polar')
    ax.plot(theta, radii)
    ax.set_title(title)
    plt.show()
# Usage
theta = np.linspace(0, 2 * np.pi, 100)
radii = np.abs(np.sin(theta) * 2)
plot_polar(theta, radii, "Sample Polar Plot") 
```

图 8.12 显示了通过运行 列表 8.12 中的代码所渲染的点图。

![图片](img/python-3-data-visualization-using-chatgpt-f0276-01.jpg)

***图 8.12*** 使用 Matplotlib 创建的极坐标图

### **使用 Seaborn 的条形图**

Seaborn 为 Matplotlib 提供了一个高级接口，使得创建时尚的图表更加容易。柱状图帮助我们可视化不同类别之间的数据。绘制柱状图使我们能够可视化分类数据。

**注意** *Seaborn 与 Pandas 集成时效果最佳。*

列表 8.13 显示了 ChatGPT 生成的用于创建柱状图的 bar_chart1.py 的内容。

***列表 8.13: bar_chart1.py***

```py
 import matplotlib.pyplot as plt
import seaborn as sns
import pandas as pd

def plot_bar(data, x_col, y_col):
    sns.barplot(x=x_col, y=y_col, data=data)
    plt.show()

# Usage
data = pd.DataFrame({
    'Category': ['A', 'B', 'C'],
    'Values': [10, 20, 15]
})
plot_bar(data, 'Category', 'Values') 
```

列表 8.13 从三个导入语句开始，接着是用于渲染柱状图的 plot_bar()函数。列表 8.13 的后半部分初始化了 Pandas DataFrame 数据，然后使用数据和用于标注水平轴的字符串以及用于标注垂直轴的另一个字符串调用 plot_bar()。图 8.13 显示了通过运行列表 8.13 中的代码生成的柱状图。

![图片](img/python-3-data-visualization-using-chatgpt-f0277-01.jpg)

***图 8.13*** 使用 Matplotlib 创建的柱状图

### **使用 Seaborn 的带回归线的散点图**

散点图使我们能够显示数据点和回归线，以了解关系。列表 8.14 显示了 ChatGPT 生成的用于使用 Seaborn 渲染散点图的 scatter_plot.py 的内容。

***列表 8.14: scatter_plot.py***

```py
 import matplotlib.pyplot as plt
import pandas as pd
import seaborn as sns

def plot_scatter_with_regression(data, x_col, y_col):
    sns.regplot(x=x_col, y=y_col, data=data)
    plt.show()

# Usage
data = pd.DataFrame({
    'X_Values': [10, 20, 30, 40, 50],
    'Y_Values': [15, 25, 35, 45, 55]
})
plot_scatter_with_regression(data, 'X_Values', 'Y_Values') 
```

散点图用于可视化两个变量之间的关系。Seaborn 的 regplot()函数不仅绘制数据点，还拟合回归线。

列表 8.14 从三个导入语句和一个用于渲染散点图的 plot_scattter_with_regression()函数开始。列表 8.13 的后半部分初始化了 Pandas DataFrame 数据，然后使用变量 data 调用 plot_scattter_with_regression()。图 8.14 显示了通过运行列表 8.14 中的代码生成的散点图。

![图片](img/python-3-data-visualization-using-chatgpt-f0278-01.jpg)

***图 8.14*** 使用 Matplotlib 创建的散点图

### **使用 Seaborn 的关联矩阵热图**

热图在表示数据矩阵时非常强大，颜色表示大小。一个常见的用例是可视化关联矩阵，这有助于理解不同变量之间的关系。

热图使我们能够可视化多个变量之间的相关性。列表 8.15 显示了 ChatGPT 生成的用于使用 Matplotlib 渲染热图的 heatmap1.py 的内容。

***列表 8.15: heatmap1.py***

```py
 import matplotlib.pyplot as plt
import pandas as pd
import seaborn as sns

def plot_heatmap(data):
    correlation_matrix = data.corr()
    sns.heatmap(correlation_matrix, annot=True, cmap='coolwarm')
    plt.show() # Usage
data = pd.DataFrame({
    'A': [1, 2, 3, 4, 5],
    'B': [5, 4, 3, 2, 1],
    'C': [2, 3, 4, 5, 6]
})
plot_heatmap(data) 
```

列表 8.15 从三个导入语句和一个用于渲染热图的 plot_heatmap()函数开始。列表 8.15 的后半部分初始化了 Pandas DataFrame 数据，然后使用变量 data 调用 plot_heatmap()。图 8.15 显示了通过运行列表 8.15 中的代码生成的热图。

![图片](img/python-3-data-visualization-using-chatgpt-f0279-01.jpg)

***图 8.15*** 使用 Matplotlib 创建的热图

### **使用 Seaborn 的直方图**

直方图是可视化数据分布的强大工具。Seaborn 的 `histplot()` 函数提供了一种轻松生成具有额外功能（如核密度估计）的直方图的方法。

列表 8.16 显示了 ChatGPT 生成的 `histogram1.py` 的内容，用于使用 Seaborn 渲染直方图。

***列表 8.16: histogram1.py***

```py
 import matplotlib.pyplot as plt
import seaborn as sns

def plot_histogram(data, column, bins=10):
    sns.histplot(data[column], bins=bins)
    plt.show() # Usage
data = sns.load_dataset("iris")
plot_histogram(data, "sepal_length") 
```

列表 8.16 以两个导入语句和用于渲染直方图的 `plot_histogram()` 函数开始。列表 8.16 的后半部分使用 Seaborn 内置数据集 iris 的内容初始化 Pandas DataFrame 数据，然后使用变量 `data` 调用 `plot_histogram()` 函数。图 8.16 显示了通过运行列表 8.16 中的代码生成的 iris 数据集的热图。

![图片](img/python-3-data-visualization-using-chatgpt-f0280-01.jpg)

***图 8.16*** 使用 Matplotlib 创建的直方图

### **使用 Seaborn 的小提琴图**

小提琴图提供了对数据分布的更深入理解。它们结合了箱线图和直方图的特点，显示了数据在不同值处的概率密度。

我们可以将箱线图和直方图的特点结合起来，以获得对数据分布的更丰富描述。列表 8.17 显示了 ChatGPT 生成的 `violin_plots.py` 的内容，用于使用 Seaborn 渲染小提琴图。

***列表 8.17: violin_plots.py***

```py
 import seaborn as sns

def plot_violin(data, x_col, y_col): sns.violinplot(x=x_col, y=y_col, data=data)
    plt.show()

# Usage
data = sns.load_dataset("iris")
plot_violin(data, "species", "sepal_length") 
```

列表 8.17 以一个导入语句和用于渲染小提琴图的 `plot_violin()` 函数开始。列表 8.17 的后半部分初始化 Pandas DataFrame 数据，然后使用 Seaborn 内置数据集 iris 的内容初始化 Pandas DataFrame 数据，并使用变量 `data` 调用 `plot_violin()` 函数。图 8.17 显示了通过运行列表 8.8 中的代码生成的由小提琴图。

![图片](img/python-3-data-visualization-using-chatgpt-f0281-01.jpg)

***图 8.17*** 使用 Matplotlib 创建的小提琴图

### **使用 Seaborn 的成对图**

当处理具有多个特征的集合时，可视化特征之间的成对关系通常很有帮助。Seaborn 的 `pairplot()` 函数可以生成散点图的矩阵，允许探索此类关系。

列表 8.18 显示了 ChatGPT 生成的 `pair_plots.py` 的内容，用于使用 Matplotlib 渲染成对图。

***列表 8.18: pair_plots.py***

```py
 import matplotlib.pyplot as plt
import seaborn as sns def plot_pairplot(data):
    sns.pairplot(data)
    plt.show()

# Usage
data = sns.load_dataset("iris")
plot_pairplot(data) 
```

列表 8.18 以两个导入语句和用于渲染成对图的 `plot_pairplot()` 函数开始。列表 8.18 的后半部分使用 Seaborn 内置数据集 iris 的内容初始化 Pandas DataFrame 数据，然后使用变量 `data` 调用 `plot_pair()` 函数。图 8.18 显示了通过运行列表 8.18 中的代码生成的成对图。

![图片](img/python-3-data-visualization-using-chatgpt-f0282-01.jpg)

***图 8.18*** 使用 Matplotlib 创建的成对图

### **使用 Seaborn 的面网格**

面板网格是一种根据分类变量在多个子图上可视化数据分布的方法。每个面板（子图）代表一个类别。列表 8.19 展示了 ChatGPT 生成的用于创建和渲染按类别分割的多个图形的 facet_grids.py 内容。

***列表 8.19: facet_grids.py***

```py
 import matplotlib.pyplot as plt
import seaborn as sns def plot_facetgrid(data, x_col, y_col, facet_col):
    g = sns.FacetGrid(data, col=facet_col)
    g.map(sns.scatterplot, x_col, y_col)
    g.add_legend()
    plt.show()

# Usage
data = sns.load_dataset("iris")
plot_facetgrid(data, "sepal_length", "sepal_width", "species") 
```

列表 8.19 从两个导入语句和一个用于绘制面板的 plot_facetgrid() 函数开始。列表 8.19 的第二部分使用 Seaborn 内置数据集 iris 的内容初始化 Pandas DataFrame 数据，然后使用变量 data 调用 plot_pair()。图 8.19 显示了通过运行列表 8.19 中的代码生成的面板网格。

![图片](img/python-3-data-visualization-using-chatgpt-f0283-01.jpg)

***图 8.19*** 使用 Seaborn 创建的面板网格

### **层次聚类**

Seaborn 的 clustermap 是一个二维矩阵数据集表示，其中行和列都是按层次聚类的。这允许从复杂数据集中出现模式。我们可以以聚类图格式可视化层次聚类关系。

***列表 8.20: cluster_map.py***

```py
 import matplotlib.pyplot as plt
import seaborn as sns

def plot_clustermap(data):
    sns.clustermap(data, method='average', cmap='coolwarm')
    plt.show()

# Usage
data = sns.load_dataset("iris").drop("species", axis=1)
plot_clustermap(data) 
```

列表 8.20 从两个导入语句和一个用于绘制聚类图的 plot_clustermap() 函数开始。列表 8.20 的第二部分使用 Seaborn 内置数据集 iris 的内容初始化 Pandas DataFrame 数据，然后使用变量 data 调用 plot_pair()。图 8.20 显示了通过运行列表 8.20 中的代码生成的聚类图。

![图片](img/python-3-data-visualization-using-chatgpt-f0284-01.jpg)

***图 8.20*** 使用 Seaborn 创建的聚类图

### **群组图**

群组图将每个数据点在分类轴上以最小重叠的位置表示，从而更好地表示值的分布。它允许我们显示非重叠点的分类散点图。

列表 8.21 展示了 ChatGPT 生成的 swarm_plot.py 内容，用于使用 Seaborn 绘制等高线。

***列表 8.21: swarm_plot.py***

```py
 import matplotlib.pyplot as plt
import seaborn as sns

def plot_swarm(data, x_col, y_col):
    sns.swarmplot(x=x_col, y=y_col, data=data)
    plt.show() # Usage
data = sns.load_dataset("iris")
plot_swarm(data, "species", "sepal_length") 
```

列表 8.21 从两个导入语句和一个用于绘制群组图的 plot_swarm() 函数开始。列表 8.21 的第二部分使用 Seaborn 内置数据集 iris 的内容初始化 Pandas DataFrame 数据，然后使用变量 data 调用 plot_swarm()。图 8.21 显示了通过运行列表 8.21 中的代码生成的群组图。

![图片](img/python-3-data-visualization-using-chatgpt-f0285-01.jpg)

***图 8.21*** 使用 Seaborn 创建的群组图

### **双变量数据的联合图**

Seaborn 的 jointplot 显示了两个变量之间的关系。它结合了散点图、回归图，甚至六边形图与直方图。它允许我们显示两个变量之间的关系以及它们的各自分布。

列表 8.22 展示了 ChatGPT 生成的用于使用 Seaborn 渲染联合图的 joint_plot.py 的内容。

***列表 8.22: joint_plot.py***

```py
 import matplotlib.pyplot as plt
import seaborn as sns

def plot_jointplot(data, x_col, y_col, kind='scatter'): sns.jointplot(x=x_col, y=y_col, data=data, kind=kind)
    plt.show()

# Usage
data = sns.load_dataset("iris")
plot_jointplot(data, "sepal_length", "sepal_width", "hex") 
```

列表 8.22 从两个导入语句和用于渲染联合图的 plot_joint() 函数开始。列表 8.22 的第二部分使用 Seaborn 内置数据集 iris 的内容初始化 Pandas DataFrame 数据，然后使用变量 data 调用 plot_pair()。图 8.22 显示了通过启动列表 8.22 中的代码渲染的联合图。

![图片](img/python-3-data-visualization-using-chatgpt-f0286-01.jpg)

***图 8.22*** 使用 Seaborn 创建的联合图

### **因子视图的点图**

点图可以用来突出显示点之间的差异，尤其是在按因素分类时。连接点的线条可以帮助强调趋势。点图通过线条强调点之间的比较。

列表 8.23 展示了 ChatGPT 生成的用于使用 Seaborn 渲染点图的 point_plot.py 的内容。

***列表 8.23: point_plot.py***

```py
 import matplotlib.pyplot as plt
import seaborn as sns def plot_pointplot(data, x_col, y_col, hue=None):
    sns.pointplot(x=x_col, y=y_col, hue=hue, data=data)
    plt.show()

# Usage
data = sns.load_dataset("tips")
plot_pointplot(data, "day", "total_bill", "sex") 
```

列表 8.23 从两个导入语句和用于渲染点图的 plot_pointplot() 函数开始。列表 8.23 的第二部分使用 Seaborn 内置数据集 tips 的内容初始化 Pandas DataFrame 数据，然后使用变量 data 调用 plot_pointplot()。图 8.23 显示了通过启动列表 8.23 中的代码渲染的点图。

![图片](img/python-3-data-visualization-using-chatgpt-f0287-01.jpg)

***图 8.23*** 使用 Seaborn 创建的点图

### **SEABORN 的密度估计 KDE 图**

核密度估计 (KDE) 图可视化连续变量的概率密度。它们可以被视为平滑的直方图，在辨别数据集的潜在分布时特别有用。它们允许我们可视化数据密度。

列表 8.24 展示了 ChatGPT 生成的用于使用 Seaborn 渲染 KDE 图的 kde_plot.py 的内容。

***列表 8.24: kde_plot.py***

```py
 import matplotlib.pyplot as plt
import seaborn as sns

def plot_kde(data, column):
    sns.kdeplot(data[column], shade=True)
    plt.show() # Usage
data = sns.load_dataset("iris")
plot_kde(data, "sepal_length") 
```

列表 8.24 从两个导入语句和用于渲染 KDE 图的 plot_kde() 函数开始。列表 8.23 的第二部分使用 Seaborn 内置数据集 iris 的内容初始化 Pandas DataFrame 数据，然后使用变量 data 调用 plot_kde()。图 8.24 显示了通过启动列表 8.24 中的代码渲染的点图。

![图片](img/python-3-data-visualization-using-chatgpt-f0288-01.jpg)

***图 8.24*** 使用 Seaborn 创建的 KDE 图

### **SEABORN 的 RIDGE 图**

Ridge 图本质上是一系列重叠的 KDE 图，允许比较不同类别之间的分布。它们允许显示重叠的分布图，这对于可视化类别间的分布变化非常有用。

列表 8.25 显示了 ChatGPT 生成的 `ridge_plot.py` 文件的内容，用于使用 Seaborn 渲染岭图。

***列表 8.25: ridge_plot.py***

```py
 import matplotlib.pyplot as plt
import seaborn as sns

def plot_ridge(data, x_col, category_col):
    g = sns.FacetGrid(data, row=category_col, hue=category_
col, aspect=5)
    g.map(sns.kdeplot, x_col, clip_on=False, shade=True,
alpha=1, lw=1.5, bw_method=0.2)
    g.map(sns.kdeplot, x_col, clip_on=False, color="w",
lw=1, bw_method=0.2)
    g.map(plt.axhline, y=0, lw=2, clip_on=False)
    plt.show() # Usage
data = sns.load_dataset("diamonds")
subset_data = data[data['cut'].isin(['Ideal', 'Fair', 'Good'])]
plot_ridge(subset_data, "price", "cut") 
```

列表 8.25 从两个导入语句和渲染岭图的 `plot_ridge()` 函数开始。列表 8.25 的第二部分初始化 Pandas DataFrame 数据，使用 Seaborn 内置数据集 diamonds 的内容，然后使用变量 data 调用 `plot_ridge()`。图 8.25 显示了通过运行列表 8.25 中的代码渲染的岭图。

![图片](img/python-3-data-visualization-using-chatgpt-f0289-01.jpg)

***图 8.25*** 使用 Seaborn 创建的岭图

### **总结**

本章包含 ChatGPT 为各种任务生成的基于 Python 的解决方案。你了解了各种图表和图形的类型，何时使用它们，以及每种图表和图形的优点和缺点。

你学习了如何使用一个流行的开源 Python 库 Matplotlib 进行数据可视化，它可以渲染多种类型的图表和图形。

你还学习了如何渲染直方图、小提琴图和时间序列可视化。通过掌握这些技术，你可以从数据中构建引人入胜的故事，帮助决策和洞察生成。请记住，一个精心制作的可视化胜过千行原始数据。

## *索引*

**A**

高级数据分析，245–246

代理提示，228–229

AI21，225

Anthropic, 226

Apple GPT，252

**B**

柱状图，112–113, 258

Bard，250–251

Beautiful Soup，148–154

Bokeh，203–205

箱线图，260

**C**

图表和图形

柱状图，258

箱线图，260

热图，259

直方图，260

线形图，259

帕累托图，260

饼图，258–259

雷达图，261

树状图，261

水流图，261

ChatGPT

替代方案，244–245

方面，233

Chrome 扩展，232

代码解释器，237–238

代码轻语者，238–239

竞争对手，250–255

关注点

代码生成和处理危险主题，240

优点和缺点，241

自定义指令，234

Google Code Red，233

*与* Google Search，233–234

GPT2 检测器，239

增长率，232

机器学习和，245–246

与医疗诊断, 243–244

在移动设备和浏览器上, 234–235

多种任务, 232

游戏场, 236

插件, 236–237

与提示, 235

样本查询和响应, 241–243

Claude-2, 238, 252–253

代码解释器, 237–238。*另见* 高级数据分析

代码轻语者, 238–239

Cohere, 224

**D**

DALL-E，特性, 221

数据可视化

工具, 158–159

类型, 159

VizGPT, 247–248

DeepMind, 222–223

**F**

少样本提示, 227

Fugue, 119–120

**G**

生成对抗网络 (GANs), 218

生成式人工智能

艺术和音乐创作, 219

挑战, 218

ChatGPT-3 和 GPT-4, 221–222

*与* 对话式人工智能

应用, 219–220

数据需求, 220

评估, 220

主要目标, 219

使用的技术, 220

训练和交互, 220

创建 *与* 分类, 218

DALL-E, 220–221

数据增强, 219

多样化的输出, 218

药物发现, 219

特性, 218

图像合成, 219

风格迁移, 219

技术, 218

文本生成, 219

无监督学习, 218

巨型语言模型测试室 (GLTR), 239

GitHub CoPilot, 251

Google Bard, 244–245

Google Code Red, 233

Google Colaboratory, 60–61

Google Search, 233–234

GPT-4, 248

竞争对手, 250–255

在其上进行微调, 249–250

参数, 249

与考试成绩, 248–249

GPT-5, 255

GPTBot, 235

GPT2 检测器, 239

GPT-3 on steroids, 232

**H**

热图, 259

直方图, 260

Hugging Face

库, 224–225

模型中心, 225

**I**

InflectionAI, 225–226

InstructGPT, 246–247

指令提示, 228

**L**

LangChain, 249, 250

大型语言模型 Meta AI (Llama-2)

架构特性，254

下载，253

微调，254–255

线性回归，50

线形图，259

LlamaIndex, 250

**M**

Matplotlib，159–160

属性值，161–162

箱线图，264

在其中棋盘，170–171

颜色值，162–163

等高线图，271–272

立方数，163

饼图，267

点状网格模式，167–168

3D 图，183

3D 表面图，268–269

点网格，166–167

热图，179–180

直方图，174–175

水平线，163–164

在其中加载图像，169–170

np_plot.py，48

np_plot_quadratic.py, 49

线段对，168–169

在其中绘制柱状图，177–178

在其中绘制饼图，160，178–179

在其中绘制金融数据，184–185

plot_line() 函数，262

在其中绘制多条线，173

绘制平行斜线，165–166

plot_pie() 函数，263

绘制斜线，164–165

极坐标图或径向图，275–276

折线图，274–275

径向图或蜘蛛图，269–271

在其中随机分布的数据点，171–172

将图形图像保存为 PNG 文件，180–181

连接线段集合，172–173

堆叠柱状图，266

流线图，272–274

时间序列数据，265

三角函数，174

均方绝对误差（MAE），52

均方误差（MSE），52

公式，52

手动计算，53–54

通过逐次逼近计算，55–60

Med-PaLM M，252

微软 CoPilot, 251

多变量分析，50

MySQL, 120

和连接器/Python API

create_fun_table.py，125–126

建立数据库连接，124

mysql_pandas.py, 124–125

pandas_write_sql.py, 126–128

**N**

非线性数据集，51

非线性最小二乘法，53

NumPy，29–30

数组，30–31

添加元素，32–33

以及指数，35

数学运算和，35–36

乘以元素和，33

np.mean() 和 np.std() 方法，42–43

其他操作，41

reshape() 方法，41–42

使用 “-1” 子范围，36–37

向量运算，38

最拟合线，54–55

以及点积，38–39

特征，30

向量的长度，40

循环，31

方法，37

百分位数() 函数，44

使用向量 “-1” 子范围，36

简化平均值和加权平均值，44–45

**O**

单次提示，227

OpenAI，223–224

OpenAI Codex，251–252

**P**

PaLM-2，252

Pandas

与 titanic.csv 的聚合操作，100–102

apply() 和 mapappy() 方法，102–105

以及条形图，112–113

cat2numeric.py，71–75

DataFrame

以及基本统计，91–92

布尔运算，68–69

concat_frames.py，79–80

以及数据清洗任务，64

使用其进行数据处理，80–83

describe() 方法，66–68

duplicated() 方法，92–95

以及 Excel 工作表，86–87

特征，64

缺失值，95–97

pandas_df.py，64–66

使用随机数，70–71

read_csv() 函数，83–86

以及散点图，90–91

在中选择、添加和删除列，87–89

对中的行进行排序，97–98

转置函数，69–70

数据可视化，107–108

groupby() 方法，98–100

在中处理异常值，89–90

水平堆叠条形图，113–114

安装，63

匹配和拆分字符串，75–77

合并和拆分列，77–79

非堆叠面积图，116–117

中的单行命令，105–107

在其中读取 JSON 字符串，129–130

在其中读取 XML 数据，128–129

以及正则表达式，133–136

sql_query_excel.py，122–123

堆叠面积图，117–118

Texthero，107

垂直堆叠条形图，114–116

帕累托图，260

饼图，258–259

Pi, Inflection，245

表述不佳的提示，231–232

提示工程

挑战，226

和补全，227

少样本提示，227

GPT-3, ChatGPT 和 GPT-4，230–231

指令提示，228

单样本提示，227

表述不佳的提示，231–232

提示模板，229

反向提示，228

系统提示 *vs.* 代理提示，228–229

类型，226

零样本提示，227

Python

Beautiful Soup，148–151

命令行参数，27–28

编译时检查，9–10

easy_install 和 pip，1

异常处理，24–25

Fraction() 函数，13–14

help() 和 dir() 函数，8–9

标识符，4–5

缩进，5

input() 函数，25–27

安装，3

IPython，2

基于 JSON 的数据

pd_python_json.py，132–133

Python 字典，131–132

启动脚本

命令行和 IDEs，4

交互式解释器，4

行和多行语句，5

列表

双倍元素，34

和指数，34

PATH 环境变量，3

原始数据类型，10

算术运算，10–11

chr() 函数，12

格式化数字，13

其他基数，11–12

round() 函数，12–13

引用和注释，6–7

运行时代码检查，9–10

在 sqlite3 中

connect_db.py，141

创建表，141

DB Browser，147

带数据的直方图，143–145

insert_data.py，141–142

填充 Pandas DataFrame，143

select_data.py，142

SQLiteDict，147–147

SQLiteStudio，146

标准库模块，8

将代码存储在文本文件中，7–8

Unicode 和 UTF-8，14–15

virtualenv 工具，2

处理日期，22–24

处理字符串，15–16

format() 方法，17

lower() 和 upper() 函数，16–17

搜索和替换，19–20

切片和拼接，17–19

strip(), lstrip(), 和 rstrip()，20–21

文本对齐，22

write() 函数，21

**R**

雷达图，261

循环神经网络（RNNs），218

正则表达式，133–136

反向提示，228

RMSProp 优化器，52

均方根层归一化（RMSNorm），254

**S**

Scikit-learn

Digits 数据集，206–209

Iris 数据集，209–213

kdeplot() 方法，213–215

Seaborn

分面网格，282–283

层次聚类关系，283–284

histplot() 函数，279–280

pairplot() 函数，281–282

plot_bar() 函数，276–277

plot_heatmap() 函数，278–279

plot_joint() 函数，285–286

plot_kde() 函数，287–288

plot_scattter_with_regression() 函数，277–278

点图，286–287

岭图，288–289

集群图，284–285

小提琴图，280–281

Seaborn

内置数据集，190–192

挑战，189

显示 Pandas 数据集，198–199

特征，190

热图，199–200

Iris 数据集，192

局限性，189

方法，190

pair_plot() 方法，201–203

Titanic 数据集，193–198

简略，182–183

SQLAlchemy，120

安装，120

read_sql() 方法，120–122

SQLite，136

数据图表，185–187

命令，136

数据库创建，137–138

数据相关操作，138

特征，136–137

安装，137

启动 SQL 文件，138–139

加载 CSV 数据，140

rm 命令，139–140

SweetViz，181–182

系统提示，228–229

**T**

Texthero，107

树状图，261

**V**

变分自编码器（VAEs），218

virtualenv 工具，2

VizGPT，247–248

**W**

瀑布图，261

**Y**

YouChat，245

**Z**

零样本提示，227
