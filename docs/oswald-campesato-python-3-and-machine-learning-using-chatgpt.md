# ChatGPT 和 Python3 机器学习


> 原文：[Python 3 and Machine Learning Using ChatGPT.](https://annas-archive.org/md5/f35b1a2bd0cd709b7d80541324081012)
> 
> 译者：[飞龙](https://github.com/wizardforcel)
> 
> 协议：[CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-cover.jpg)

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-halftitleimg.jpg)



前言

本书旨在弥合 Python 编程、机器学习和在数据科学中创新使用 ChatGPT 的理论知识与实际应用之间的差距。它旨在为那些希望深化对这些快速发展的领域理解和技能的人提供全面指南。

动机源于对实用、深入的资源日益增长的需求，这些资源满足学生、数据科学家和希望利用高级技术和工具的 AI 研究人员的需求。随着这些领域在重要性和影响力上的持续增长，熟练地操作数据、理解机器学习算法以及应用 AI 的最新进展变得至关重要。

本书结构旨在促进对几个核心主题的深入理解：

■   Pandas 简介：我们首先详细介绍 Pandas，这是数据操作和分析的 Python 库的基石。本节旨在帮助您熟练掌握数据框，并高效地执行复杂的数据清洗和准备任务。

■   机器学习分类器：接下来，我们将探讨各种机器学习分类器，为您提供选择和实施适合您项目正确算法的知识。从 kNN 到 SVM，您将通过实际示例了解每种方法的细微差别。

■   GPT-4 和线性回归：随着我们探索 GPT-4 的能力，我们讨论了其在增强传统线性回归分析中的应用。本节展示了如何使用 GPT-4 进行和解释回归，从而推动传统数据分析的边界。

■   使用 ChatGPT 进行数据可视化：最后，本书涵盖了 ChatGPT 在数据可视化中的创新应用。本部分重点介绍人工智能如何将数据转化为引人入胜的视觉故事，使复杂的结果易于理解和访问。它包括材料 AI 应用、GAN 和 DALL-E。

每一章都旨在基于前几节的知识进行构建，确保学习体验的连贯性和全面性。为了满足广泛的 学习风格，本书包括逐步教程、实际应用案例，以及基于实际例子的理论概念部分。这种方法不仅巩固了理解，还提高了你在实际场景中应用这些技术的能力。

本书特色

■   涵盖最新的 Python 库：您将掌握使用现代数据科学家必需的尖端库的技能。

■   解决现实世界问题：本书挑战您在真实数据上应用您的技能，为您在专业上的成功做好准备。

■   伴随文件，包括源代码、数据集和图表，可以通过向出版社（提供购买证明）发送电子邮件至 info@merclearning.com 下载。

这本书不仅仅是一个学习工具；它是一本参考书，随着您在职业生涯中的进步，您将反复回到这本书。无论您是希望在学习编程和数据科学方面有一个稳固的起点的新手，还是希望探索 AI 新进展的资深专业人士，“Python 3 和使用 ChatGPT/GPT-4 进行机器学习”都是一项宝贵的资产。

我们希望您会发现这本书是一个宝贵的资源，它能激发您进一步探索并应用您的知识来解决复杂问题。生成式 AI 的未来既令人兴奋又充满可能性。

O. Campesato

2024 年 4 月

第一章

PANDAS 简介

本章向您介绍了 Pandas，并提供了代码示例，展示了其一些有用的特性。如果您熟悉这些主题，可以快速浏览材料并查看代码示例，以防它们包含您未知的信息。

第一部分包含了对 Pandas 的简要介绍。本节包含了一些 Pandas DataFrame 特性的代码示例，并对序列进行了简要讨论，这两者都是 Pandas 的主要特性。

本章的第二部分讨论了您可以创建的各种数据框类型，例如数值和布尔数据框。此外，我们讨论了使用 NumPy 函数和随机数创建数据框的示例。

注意：本章中的几个代码示例引用了 NumPy 库来处理数组和生成随机数，您可以从在线文章中学习这些内容。

什么是 Pandas？

Pandas 是一个与 NumPy 和 Matplotlib 等其他 Python 库兼容的 Python 库。通过打开命令行并调用以下命令安装 Pandas（适用于 Python 3.x）：

pip3 install pandas

在许多方面，Pandas 库中 API 的语义类似于电子表格，同时支持 XSL、XML、HTML 和 CSV 文件类型。Pandas 提供了一个称为数据框的数据类型（类似于 Python 字典），具有极其强大的功能。

Pandas 数据框支持多种输入类型，如 ndarray、列表、字典或序列。

数据类型序列是另一种管理数据的方式。除了在线搜索更多关于序列的详细信息之外，以下文章包含了一个很好的介绍：

[`towardsdatascience.com/20-examples-to-master-pandas-series-bc4c68200324`](https://towardsdatascience.com/20-examples-to-master-pandas-series-bc4c68200324)

Pandas 选项和设置

您可以更改环境变量的默认值，以下是一个示例：

import pandas as pd

display_settings = {

'max_columns': 8,

'expand_frame_repr': True, # 分页显示

'max_rows': 20,

'precision': 3,

'show_dimensions': True

}

for op, value in display_settings.items():

pd.set_option("display.{}".format(op), value)

如果您想使 Pandas 显示最多 20 行和 8 列，并且以三位小数显示浮点数，请在自己的代码中包含前面的代码块。如果要将输出“环绕”到多页，请将 expand_frame_rep 设置为 True。前面的 for 循环遍历 display_settings 并设置选项等于其对应的值。

此外，以下代码片段显示您代码中的所有 Pandas 选项及其当前值：

print(pd.describe_option())

您可以使用选项及其值执行各种其他操作（例如，使用 pd.reset()方法重置值），如 Pandas 用户指南中所述：

[`pandas.pydata.org/pandas-docs/stable/user_guide/options.html`](https://pandas.pydata.org/pandas-docs/stable/user_guide/options.html)

Pandas 数据框

简而言之，Pandas 数据框是一个二维数据结构，方便将其视为行和列的数据结构。数据框可以进行标记（包括行和列），并且列可以包含不同的数据类型。Pandas 数据框的数据集来源可以是数据文件、数据库表或 Web 服务。数据框的特点包括：

+   数据框方法

+   数据框统计信息

+   分组、交叉和重塑

+   处理缺失数据

+   连接数据框

本章中的代码示例几乎展示了上述列表中的所有功能。

数据框和数据清理任务

需要执行的具体任务取决于数据集的结构和内容。通常，您将按照以下步骤执行工作流程，不一定总是按照此顺序（某些步骤可能是可选的）。所有以下步骤都可以使用 Pandas 数据框执行：

+   将数据读入数据框

+   显示数据框顶部

+   显示列数据类型

+   显示缺失值

+   用值替换 NA

+   遍历列

+   每列的统计信息

+   查找缺失值

+   总缺失值

+   缺失值的百分比

+   排序表格值

+   打印摘要信息

+   列中缺失值超过 50%

+   重命名列

本章包含说明如何执行上述列表中许多步骤的章节。

Pandas 的替代方案

在深入研究代码示例之前，有一些提供非常实用功能的 Pandas 替代方案，其中一些如下所示：

+   PySpark（用于大型数据集）

+   Dask（用于分布式处理）

+   Modin（性能更快）

+   数据表（R data.table 的 Python 版本）

包含这些替代方案并不是为了贬低 Pandas。实际上，您可能不需要上述列表中的任何功能。然而，如果您将来需要此类功能，那么现在了解这些替代方案是值得的（未来可能还有更强大的替代方案）。

一个包含 NumPy 示例的 PANDAS 数据框

列表 1.1 展示了 pandas_df.py 的内容，该内容说明了如何定义几个数据框并显示其内容。

列表 1.1: pandas_df.py

import pandas as pd

import numpy as np

myvector1 = np.array([1,2,3,4,5])

print("myvector1:")

print(myvector1)

print()

mydf1 = pd.Data frame(myvector1)

print("mydf1:")

print(mydf1)

print()

myvector2 = np.array([i for i in range(1,6)])

print("myvector2:")

print(myvector2)

print()

mydf2 = pd.Data frame(myvector2)

print("mydf2:")

print(mydf2)

print()

myarray = np.array([[10,30,20], [50,40,60],[1000,2000,3000]])

print("myarray:")

print(myarray)

print()

mydf3 = pd.Data frame(myarray)

print("mydf3:")

print(mydf3)

print()

列表 1.1 以 Pandas 和 NumPy 的标准导入语句开始，接着是定义两个一维 NumPy 数组和二维 NumPy 数组。每个 NumPy 变量后面都跟着一个相应的 Pandas 数据框（mydf1、mydf2 和 mydf3）。现在运行 列表 1.1 中的代码，查看以下输出，并将 NumPy 数组与 Pandas 数据框进行比较：

myvector1:

[1 2 3 4 5]

mydf1:

0

0 1

1 2

2 3

3 4

4 5

myvector2:

[1 2 3 4 5]

mydf2:

0

0 1

1 2

2 3

3 4

4 5

myarray:

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-img_5a.jpg)

mydf3:

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-img_5.jpg)

相比之下，下面的代码块说明了如何定义两个 Pandas Series，这两个 Series 是 Pandas 数据框定义的一部分：

names = pd.Series(['SF', 'San Jose', 'Sacramento'])

sizes = pd.Series([852469, 1015785, 485199])

df = pd.DataFrame({'Cities': names, 'Size': sizes})

print(df)

创建一个包含上述代码（以及所需的导入语句）的 Python 文件，当你运行该代码时，你会看到以下输出：

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-img_6.jpg)

描述一个 Pandas 数据框

列表 1.2 展示了 pandas_df_describe.py 的内容，它说明了如何定义一个包含 3x3 整数 NumPy 数组的 Pandas 数据框，其中数据框的行和列都有标签。数据框的其他方面也显示了出来。

列表 1.2：pandas_df_describe.py

导入 numpy as np

导入 pandas as pd

myarray = np.array([[10,30,20], [50,40,60],[1000,2000,3000]])

rownames = ['苹果', '橙子', '啤酒']

colnames = ['一月', '二月', '三月']

mydf = pd.DataFrame(myarray, index=rownames, columns=colnames)

print("df 的内容：")

print(mydf)

print()

print("一月的内容：")

print(mydf['一月'])

print()

print("行数：")

print(mydf.shape[0])

print()

print("列数：")

print(mydf.shape[1])

print()

print("行数和列数：")

print(mydf.shape)

print()

print("列名：")

print(mydf.columns)

print()

print("列类型：")

print(mydf.dtypes)

print()

print("描述：")

print(mydf.describe())

print()

列表 1.2 以两个标准的导入语句开始，接着是变量 myarray，它是一个 3x3 的数字 NumPy 数组。rownames 和 colnames 变量分别为 Pandas 数据框 mydf 的行和列提供名称，mydf 是初始化为 Pandas 数据框的指定数据源（即 myarray）。

下面的输出第一部分需要一条单独的 print() 语句（它只是简单地显示 mydf 的内容）。输出第二部分是通过调用 Pandas 数据框可用的 describe() 方法生成的。describe() 方法很有用：您将看到各种统计量，例如均值、标准差、最小值和最大值，这些统计量是按列（而不是按行）执行的，还包括 25^(th)、50^(th) 和 75^(th) 分位数。列表 1.2 的输出如下：

df 的内容：

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-img_7.jpg)

一月的内容：

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-img_7a.jpg)

名称：一月，数据类型：int64

行数：

3

列数：

3

行数和列数：

(3, 3)

列名：

索引(['一月', '二月', '三月'], 数据类型='object')

列类型：

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-img_7b.jpg)

数据类型：object

描述：

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-img_8.jpg)

Pandas 布尔数据框

Pandas 支持在数据框上进行布尔运算，例如逻辑或、逻辑与以及一对数据框的逻辑否定。列表 1.3 展示了 pandas_boolean_df.py 的内容，该内容说明了如何定义一个 Pandas 数据框，其行和列都是布尔值。

列表 1.3: pandas_boolean_df.py

import pandas as pd

df1 = pd.DataFrame({'a': [1, 0, 1], 'b': [0, 1, 1]}, dtype=bool)

df2 = pd.DataFrame({'a': [0, 1, 1], 'b': [1, 1, 0]}, dtype=bool)

print("df1 & df2:")

print(df1 & df2)

print("df1 | df2:")

print(df1 | df2)

print("df1 ^ df2:")

print(df1 ^ df2)

列表 1.3 初始化数据框 df1 和 df2，然后计算 df1 & df2、df1 | df2 和 df1 ^ df2，分别代表 df1 和 df2 的逻辑与、逻辑或和逻辑否定。启动 列表 1.3 中的代码的输出如下：

df1 & df2:

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-img_8a.jpg)

转置 Pandas 数据框

T 属性（以及转置函数）允许您生成 Pandas 数据框的转置，类似于 NumPy 数组。转置操作将行转换为列，列转换为行。例如，以下代码段定义了一个 Pandas 数据框 df1，然后显示 df1 的转置：

df1 = pd.DataFrame({'a': [1, 0, 1], 'b': [0, 1, 1]}, dtype=int)

print("df1.T:")

print(df1.T)

上一段代码的输出如下：

df1.T:

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-img_9.jpg)

以下代码段定义了 Pandas 数据框 df1 和 df2，然后显示它们的和：

df1 = pd.DataFrame({'a': [1, 0, 1], 'b': [0, 1, 1]}, dtype=int)

df2 = pd.DataFrame({'a': [3, 3, 3], 'b': [5, 5, 5]}, dtype=int)

print("df1 + df2:")

print(df1 + df2)

输出如下：

df1 + df2:

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-img_9a.jpg)

PANDAS 数据框和随机数

列表 1.4 展示了 pandas_random_df.py 的内容，该内容说明了如何创建一个包含随机整数的 Pandas 数据框。

列表 1.4: pandas_random_df.py

import pandas as pd

import numpy as np

df = pd.DataFrame(np.random.randint(1, 5, size=(5, 2)), columns=['a','b'])

df = df.append(df.agg(['sum', 'mean']))

print("数据框的内容：")

print(df)

列表 1.4 定义了 Pandas 数据框 df，它由 5 行和 2 列的 1 到 5 之间的随机整数组成。注意，df 的列被标记为“a”和“b”。此外，接下来的代码段附加了包含两列数字之和和平均值的两行。列表 1.4 的输出如下：

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-img_10.jpg)

列表 1.5 展示了 pandas_combine_df.py 的内容，该内容说明了如何合并 Pandas 数据框。

列表 1.5: pandas_combine_df.py

import pandas as pd

import numpy as np

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-img_10a.jpg)

print("df 的内容：")

print(df)

print("foo1 的内容：")

print(df.foo1)

print("foo2 的内容：")

print(df.foo2)

列表 1.5 定义了包含 5 行和 2 列（标记为“foo1”和“foo2”）的随机实数（介于 0 和 5 之间）的 Pandas 数据框 df。列表 1.5 的下一部分显示了 df 和 foo1 的内容。列表 1.5 的输出如下：

df 的内容：

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-img_11.jpg)

在 Pandas 中读取 CSV 文件

Pandas 提供了 read-csv()方法来读取 CSV 文件的内容。例如，列表 1.6 显示了包含标记数据（垃圾邮件或鸡肉）的 sometext.csv 的内容，列表 1.7 显示了 read-csv-file.py 的内容，说明了如何读取 CSV 文件的内容。

列表 1.6：sometext.csv

| 类型 | 文本 |
| --- | --- |
| 鸡肉 | 今天可用 |
| 鸡肉 | 我在和你开玩笑 |
| 垃圾邮件 | 每周两次比赛的免费入场 |
| 鸡肉 | 你这么早就说出来了 |
| 鸡肉 | 我不相信他会去 usf |
| 垃圾邮件 | 嘿，你好 |
| 鸡肉 | 我兄弟没病 |
| 鸡肉 | 按照你的要求，Melle |
| 垃圾邮件 | 胜利！！作为一位尊贵的客户 |

列表 1.7：read-csv-file.py

import pandas as pd

import numpy as np

df = pd.read_csv('sometext.csv', delimiter='\t')

print("=> 前五行:")

print(df.head(5))

列表 1.7 读取 sometext.csv 的内容，其列由制表符（“\t”）分隔符分隔。运行列表 1.7 中的代码，可以看到以下输出：

=> 前五行：

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-img_12.jpg)

head()方法的默认值是 5，但你可以使用 df.head(n)代码片段显示数据框 df 的前 n 行。

在文本文件中指定分隔符和列集

前一节向你展示了如何使用 delimiter 属性在文本文件中指定分隔符。你还可以使用 sep 参数指定不同的分隔符。此外，你可以将 names 参数分配给你想要读取的数据中的列名。使用 delimiter 和 sep 的一个例子如下：

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-img_12a.jpg)

Pandas 还提供了 read_table()方法来读取 CSV 文件的内容，它使用与 read_csv()方法相同的语法。

在文本文件中指定索引

假设你知道文本文件中的一个特定列包含文本文件行索引的值。例如，包含关系型表数据的文本文件通常包含一个索引列。

幸运的是，Pandas 允许你指定文本文件中的第 k 列作为索引，如下所示：

df = pd.read_csv('myfile.csv', index_col=k)

Pandas 中的 loc()和 iloc()方法

如果你想显示 Pandas 数据框中记录的内容，请在 loc()方法中指定行的索引。例如，以下代码片段通过特征名称在数据框 df 中显示数据：

df.loc[feature_name]

选择数据框中“高度”列的第一行：

df.loc([0], ['height'])

以下代码片段使用 iloc()函数通过此代码片段显示 name 列的前 8 条记录：

df.iloc[0:8]['name']

将分类数据转换为数值数据

机器学习中一个常见的任务是将包含字符数据的特征转换为包含数值数据的特征。列表 1.8 展示了 cat2numeric.py 的内容，说明了如何将文本字段替换为相应的数值字段。

列表 1.8：cat2numeric.py

导入 pandas 库作为 pd

导入 numpy 库作为 np

df = pd.read_csv('sometext.csv', delimiter='\t')

打印("=> 前五行（之前）:")

打印(df.head(5))

打印("-------------------------")

打印()

# 将 ham/spam 映射到 0/1 值：

df['type'] = df['type'].map( {'ham':0 , 'spam':1} )

打印("=> 前五行（之后）:")

打印(df.head(5))

打印("-------------------------")

列表 1.8 初始化数据框 df，包含 CSV 文件 sometext.csv 的内容，然后通过调用 df.head(5)显示前五行内容，这也是默认显示的行数。

列表 1.8 中的下一个代码片段调用 map()方法，将 type 列中的 ham 替换为 0，将 spam 替换为 1，如下所示：

df['type'] = df['type'].map( {'ham':0 , 'spam':1} )

列表 1.8 的最后部分再次调用 head()方法，显示在重命名 type 列的内容后数据集的前五行。运行列表 1.8 中的代码，以查看以下输出：

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-img_13.jpg)

-------------------------

作为另一个例子，列表 1.9 展示了 shirts.csv 的内容，列表 1.10 展示了 shirts.py 的内容；这些示例说明了将分类数据转换为数值数据的四种技巧。

列表 1.9：shirts.csv

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

列表 1.10：shirts.py

导入 pandas 库作为 pd

shirts = pd.read_csv("shirts.csv")

打印("shirts before:")

打印(shirts)

打印()

# 技巧#1:

#shirts.loc[shirts['ssize']=='xxlarge','size'] = 4

#shirts.loc[shirts['ssize']=='xlarge', 'size'] = 4

#shirts.loc[shirts['ssize']=='large', 'size'] = 3

#shirts.loc[shirts['ssize']=='medium', 'size'] = 2

#shirts.loc[shirts['ssize']=='small', 'size'] = 1

#shirts.loc[shirts['ssize']=='xsmall', 'size'] = 1

# 技巧#2:

#shirts['ssize'].replace('xxlarge', 4, inplace=True)

#shirts['ssize'].replace('xlarge', 4, inplace=True)

#shirts['ssize'].replace('large', 3, inplace=True)

#shirts['ssize'].replace('medium', 2, inplace=True)

#shirts['ssize'].replace('small', 1, inplace=True)

#shirts['ssize'].replace('xsmall', 1, inplace=True)

# 技巧#3:

#shirts['ssize'] = shirts['ssize'].apply({'xxlarge':4, 'xlarge':4, 'large':3, 'medium':2, 'small':1, 'xsmall':1}.get)

# 技巧#4:

shirts['ssize'] = shirts['ssize'].replace(regex='xlarge', value=4)

shirts['ssize'] = shirts['ssize'].replace(regex='large', value=3)

shirts['ssize'] = shirts['ssize'].replace(regex='medium', value=2)

shirts['ssize'] = shirts['ssize'].replace(regex='small', value=1)

print("shirts after:")

print(shirts)

列表 1.10 从一个包含六个语句的代码块开始，该代码块使用字符串的直接比较来进行数值替换。例如，以下代码片段将所有 xxlarge 字符串替换为值 4：

shirts.loc[shirts['ssize']=='xxlarge','size'] = 4

第二个代码块由六个语句组成，使用 replace() 方法执行相同的更新，以下是一个示例：

shirts['ssize'].replace('xxlarge', 4, inplace=True)

第三个代码块由一个使用 apply() 方法执行相同更新的单语句组成，如下所示：

shirts['ssize'] = shirts['ssize'].apply({'xxlarge':4, 'xlarge':4, 'large':3, 'medium':2, 'small':1, 'xsmall':1}.get)

第四个代码块由四个语句组成，使用正则表达式执行相同的更新，以下是一个示例：

shirts['ssize'] = shirts['ssize'].replace(regex='xlarge', value=4)

由于前面的代码片段也匹配 xlarge，所以我们只需要四个语句而不是六个语句。（如果你不熟悉正则表达式，你可以在网上找到讨论正则表达式的文章。）现在运行 列表 1.10 以查看以下输出：

shirts before

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p16.jpg)

MATCHING AND SPLITTING STRINGS IN PANDAS

列表 1.11 展示了 shirts_str.py 的内容，它说明了如何匹配列值与初始字符串，以及如何根据字母拆分列值。

列表 1.11：shirts_str.py

import pandas as pd

shirts = pd.read_csv("shirts2.csv")

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

print()

print("Rows 3 through 5 and column 2:")

print(shirts.iloc[2:5, 2])

print()

列表 1.11 使用 shirts.csv 文件的包含内容初始化数据帧 df，然后显示 df 的内容。在 列表 1.11 中的下一个代码片段使用 startswith() 方法匹配以字母 xl 开头的衬衫类型，然后是一个显示尺寸不等于字符串 xlarge 的短裤的代码片段。

下一个代码片段使用构造 str[:3] 显示衬衫类型的第一个三个字母，然后是一个使用 split() 方法根据字母“a”拆分衬衫类型的代码片段。

最后一段代码使用 iloc[2:5,2] 调用显示第 3 行至第 5 行（包含）的内容，以及仅第二列。列表 1.11 的输出如下：

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p17.jpg)

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p18.jpg)

PANDAS 中将字符串转换为日期

列表 1.12 展示了 string2date.py 的内容，该内容说明了如何将字符串转换为日期格式。

列表 1.12：string2date.py

导入 pandas as pd

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-img_19.jpg)

df1 = pd.Data frame(bdates1, columns = ['strdates','people'])

df1['dates'] = pd.to_datetime(df1['strdates'], format='%Y%m%d')

print("=> 数据框 df1 的内容：")

print(df1)

print()

print(df1.dtypes)

print()

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-img_19a.jpg)

df2 = pd.Data frame(bdates2, columns = ['strdates','people'])

df2['dates'] = pd.to_datetime(df2['strdates'], format='%d%b%Y')

print("=> 数据框 df2 的内容：")

print(df2)

print()

print(df2.dtypes)

print()

列表 1.12 使用 bdates1 的内容初始化数据框 df1，然后使用 %Y%m%d 格式将 strdates 列转换为日期。列表 1.12 的下一部分使用 bdates2 的内容初始化数据框 df2，然后使用 %d%b%Y 格式将 strdates 列转换为日期。现在运行列表 1.12 中的代码，以查看以下输出：

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p19.jpg)

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p20.jpg)

PANDAS 中处理日期范围

列表 1.13 展示了 pand_parse_dates.py 的内容，该内容说明了如何在 CSV 文件中处理日期范围。

列表 1.13：pand_parse_dates.py

import pandas as pd

df = pd.read_csv('multiple_dates.csv', parse_dates=['dates'])

print("df:")

print(df)

print()

df = df.set_index(['dates'])

start_d = "2021-04-30"

end_d = "2021-08-31"

print("日期范围：",start_d,"至",end_d,":")

print(df.loc[start_d:end_d])

print()

print("日期在",start_d,"之前：")

print(df.loc[df.index < start_d])

years = ['2020','2021','2022']

for year in years:

year_sum = df.loc[year].sum()[0]

print("年份",year,"的数值总和：",year_sum)

列表 1.13 首先使用 CSV 文件 multiple_dates.csv 的内容初始化变量 df，然后显示其内容。接下来的代码片段将日期列设置为索引列，并初始化包含起始日期和结束日期的变量 start_d 和 end_d。

列表 1.13 的下一部分显示 start_d 和 end_d 之间的日期，然后是早于 start_d 的日期列表。最后的代码块遍历年份列表，然后计算列表中每个年份的值字段中的数值总和。现在运行列表 1.13 中的代码，以查看以下输出：

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p21.jpg)

2020 年数值总和：141.0

2021 年数值总和：235.0

2022 年数值总和：160.0

PANDAS 中检测缺失日期

列表 1.14 显示了 pandas_missing_dates.py 的内容，该文件说明了如何在 CSV 文件中检测缺失的日期值。

列表 1.14: pandas_missing_dates.py

导入 pandas 库

# 从列表字典创建数据框

数据 = {'Date': ['2021-01-18', '2021-01-20', '2021-01-21', '2021-01-24'],

'Name': ['Joe', 'John', 'Jane', 'Jim']}

df = pd.Data frame(data)

# 设置日期值作为索引：

df = df.set_index('Date')

# to_datetime()将字符串格式转换为 DateTime 对象：

df.index = pd.to_datetime(df.index)

start_d="2021-01-18"

end_d="2021-01-25"

# 显示非顺序的日期：

打印("在",start_d,"和",end_d,"之间的缺失日期：")

dates = pd.date_range(start=start_d, end=end_d).difference(df.index)

for date in dates:

打印("日期：",date)

打印()

列表 1.14 初始化字典 data，包含日期字段和名称字段的值列表，之后变量 df 被初始化为一个数据框，其内容来自 data 变量。

下一个代码片段将数据框 df 的日期字段设置为索引，之后基于字符串的日期被转换为 DateTime 对象。另一对代码片段分别初始化变量 start_d 和 end_d 为起始日期和结束日期。

列表 1.14 的最后一部分初始化变量 dates 为 start_d 和 end_d 之间的缺失日期列表，之后显示 dates 的内容。现在运行列表 1.14 中的代码，可以看到以下输出：

在 2021-01-18 和 2021-01-25 之间的缺失日期：

日期：2022-01-19 00:00:00

日期：2022-01-22 00:00:00

日期：2022-01-23 00:00:00

日期：2022-01-25 00:00:00

PANDAS 中的缺失日期插值

列表 1.15 显示了 missing_dates.csv 的内容，列表 1.16 显示了 pandas_interpolate.py 的内容，该文件说明了如何以多种方式计算并替换 NaN 值。

列表 1.15: missing_dates.csv

"日期","值"

2021-01-31,40

2021-02-28,45

2021-03-31,56

2021-04-30,NaN

2021-05-31,NaN

2021-06-30,140

2021-07-31,95

2021-08-31,40

2021-09-30,55

2021-10-31,NaN

2021-11-15,65

注意列表 1.15 中显示的值 140（粗体）：这个值是一个异常值，它将影响插值值的计算，并可能生成额外的异常值。

列表 1.16: pandas_interpolate.py

导入 pandas 库

df = pd.read_csv("missing_dates.csv")

# 使用线性插值填充 NaN 值：

df1 = df.interpolate()

# 使用二次多项式插值填充 NaN 值：

df2 = df.interpolate(method='polynomial', order=2)

# 使用三次多项式插值填充 NaN 值：

df3 = df.interpolate(method='polynomial', order=3)

打印("原始数据框：")

打印(df)

打印()

打印("线性插值：")

打印(df1)

打印()

打印("二次插值：")

打印(df2)

打印()

打印("三次插值：")

打印(df3)

打印()

列表 1.16 使用 missing_dates.csv CSV 文件的内容初始化 df，然后通过 interpolate() 方法分别基于线性、二次和三次插值初始化三个数据帧 df1、df2 和 df3。现在运行 列表 1.16 中的代码以查看以下输出：

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p23.jpg)

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p24.jpg)

PANDAS 中日期的其他操作

列表 1.17 展示了 pandas_misc1.py 的内容，说明了如何从一个数据帧的列中提取年份列表。

列表 1.17: pandas_misc1.py

import pandas as pd

import numpy as np

df = pd.read_csv('multiple_dates.csv', parse_dates=['dates'])

print("df:")

print(df)

print()

year_list = df['dates']

arr1 = np.array([])

for long_year in year_list:

year = str(long_year)

short_year = year[0:4]

arr1 = np.append(arr1,short_year)

unique_years = set(arr1)

print("unique_years:")

print(unique_years)

print()

unique_arr = np.array(pd.Data frame.from_dict(unique_years))

print("unique_arr:")

print(unique_arr)

print()

列表 1.17 使用 pandasMisc1.py 的内容初始化 df，并显示其内容。然后，列表 1.17 的下一部分初始化 year_list 为 df 的日期列。

下一个代码块包含一个循环，遍历 year_list 中的元素，提取前四个字符（即年份值）并将其子字符串追加到 NumPy 数组 arr1 中。最后的代码块将变量 unique_arr 初始化为包含字典 unique_years 中唯一年份的 NumPy 数组。现在运行 列表 1.17 中的代码以查看以下输出：

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p25.jpg)

unique_years:

{'2022', '2020', '2021'}

unique_arr:

[['2022']

['2020']

['2021']]

列表 1.18 展示了 pandas_misc2.py 的内容，说明了如何遍历数据帧的行。请注意，不建议按行迭代，因为它可能导致大型数据集中的性能问题。

列表 1.18: pandas_misc2.py

import pandas as pd

df = pd.read_csv('multiple_dates.csv', parse_dates=['dates'])

print("df:")

print(df)

print()

print("=> 遍历行：")

for idx,row in df.iterrows():

print("idx:",idx," 年:",row['dates'])

print()

列表 1.18 使用 pandas_misc2.py 的内容初始化 Pandas 数据帧 df，打印其内容，然后通过循环处理 df 的行。在每次迭代中，显示当前索引和行内容。现在运行 列表 1.18 中的代码以查看以下输出：

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p26.jpg)

列表 1.19 展示了 pandas_misc3.py 的内容，该内容说明了如何显示介于开始日期和结束日期之间的每周日期集。

列表 1.19: pandas_misc3.py

import pandas as pd

start_d="01/02/2022"

end_d="12/02/2022"

weekly_dates=pd.date_range(start=start_d, end=end_d, freq='W')

print("从",start_d,"到",end_d,"的每周日期：")

print(weekly_dates)

列表 1.19 从初始化变量 start_d 和 end_d 开始，分别包含起始日期和结束日期，然后初始化变量 weekly_dates，包含从起始日期到结束日期之间的每周日期列表。现在运行 列表 1.19 代码以查看以下输出：

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p27.jpg)

在 Pandas 中合并和拆分列

列表 1.20 展示了 employees.csv 的内容，列表 1.21 展示了 emp_merge_split.py 的内容。这些示例说明了如何合并和拆分 CSV 文件的列。

列表 1.20：employees.csv

name,year,month

Jane-Smith,2015,Aug

Dave-Smith,2020,Jan

Jane-Jones,2018,Dec

Jane-Stone,2017,Feb

Dave-Stone,2014,Apr

Mark-Aster,,Oct

Jane-Jones,NaN,Jun

列表 1.21：emp_merge_split.py

import pandas as pd

emps = pd.read_csv("employees.csv")

print("员工列表:")

print(emps)

print()

emps['year'] = emps['year'].astype(str)

emps['month'] = emps['month'].astype(str)

# 分别为姓氏和名字创建单独的列：

emps['fname'],emps['lname'] = emps['name'].str.split("-",1).str

# 使用“#”符号连接年份和月份：

emps['hdate1'] = emps['year'].

astype(str)+"#"+emps['month'].astype(str)

# 使用“-”符号连接年份和月份：

emps['hdate2'] = emps[['year','month']].agg('-'.join, axis=1)

print(emps)

print()

列表 1.21 使用 employees.csv 文件的内容初始化数据框 df，然后显示 df 的内容。接下来的两个代码片段调用 astype() 方法将年份和月份列的内容转换为字符串。

在 列表 1.21 中的下一个代码片段使用 split() 方法将姓名列拆分为包含每个员工姓名中姓氏和名字的列 fname 和 lname：

emps['fname'],emps['lname'] = emps['name'].str.split("-",1).str

下一个代码片段将年份和月份字符串的内容连接起来，使用“#”字符创建一个新的列 hdate1：

emps['hdate1'] = emps['year'].

astype(str)+"#"+emps['month'].astype(str)

最后一个代码片段将年份和月份字符串的内容连接起来，使用“-”创建一个新的列 hdate2，如下所示：

emps['hdate2'] = emps[['year','month']].agg('-'.join, axis=1)

现在运行 列表 1.21 代码以查看以下输出：

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p29.jpg)

关于以下注释掉的代码片段还有一个细节：

#emps['fname'],emps['lname'] = emps['name'].str.split("-",1).str

如果取消注释前面的代码片段，将显示以下弃用消息：

#FutureWarning: Columnar iteration over characters

#将在未来的版本中弃用。

使用 Pandas 读取 HTML 网页

列表 1.22 显示了 HTML 网页 abc.html 的内容。列表 1.23 展示了 read_html_page.py 的内容，该内容说明了如何从 Pandas 中读取 HTML 网页的内容。请注意，此代码仅适用于包含至少一个 HTML `<table>` 元素的网页。

列表 1.22: abc.html

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p30.jpg)

列表 1.23: read_html_page.py

import pandas as pd

file_name="abc.html"

with open(file_name, "r") as f:

dfs = pd.read_html(f.read())

print("Contents of HTML Table(s) in the HTML Web Page:")

print(dfs)

列表 1.23 以一个导入语句开始，随后将变量 file_name 初始化为 列表 1.22 中显示的 abc.html。接下来的代码片段将变量 dfs 初始化为包含 HTML 网页 abc.html 内容的数据框。列表 1.23 的最后部分显示了数据框 dsf 的内容。现在运行 列表 1.23 中的代码以查看以下输出：

HTML 网页中的 HTML 表格内容：

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p30-1.jpg)

有关 Pandas read_html() 方法的更多信息，请访问此 URL：

[`pandas.pydata.org/pandas-docs/stable/reference/api/`](https://pandas.pydata.org/pandas-docs/stable/reference/api/)

将 Pandas 数据框保存为 HTML 网页

列表 1.24 展示了 read_html_page.py 的内容，该内容说明了如何从 Pandas 中读取 HTML 网页的内容。请注意，此代码仅适用于包含至少一个 HTML `<table>` 元素的网页。

列表 1.24: read_html_page.py

import pandas as pd

emps = pd.read_csv("employees.csv")

print("emps:")

print(emps)

print()

emps['year'] = emps['year'].astype(str)

emps['month'] = emps['month'].astype(str)

# 分离出用于姓氏和名字的单独列：

emps['fname'],emps['lname'] = emps['name'].str.split("-",1).str

# 使用“#”符号连接年份和月份：

emps['hdate1'] = emps['year']

.astype(str)+"#"+emps['month'].astype(str)

# 使用“-”符号连接年份和月份：

emps['hdate2'] = emps[['year','month']].agg('-'.join, axis=1)

print(emps)

print()

html = emps.to_html()

print("Data frame as an HTML Web Page:")

print(html)

列表 1.24 将 employees.csv 的内容填充到数据框 temps 中，然后将年份和月份属性转换为字符串类型。接下来的代码片段使用“-”符号作为分隔符拆分名称字段的内容。因此，此代码片段将拆分的字段的前半部分填充到新的 fname 字段中，后半部分填充到 lname 字段中。

列表 1.24 中的下一段代码将年份和月份字段转换为字符串，然后使用“#”作为分隔符将它们连接起来。另一个代码片段将年份和月份字段的连接填充到 hdate2 字段中。

在显示数据帧 emps 的内容后，最后的代码片段通过调用 Pandas 的 to_html() 方法将数据帧 emps 转换为 HTML 网页的结果，并将结果存储在变量 html 中。现在运行 列表 1.24 中的代码，以查看以下输出：

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p32.jpg)

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p33.jpg)

摘要

本章介绍了 Pandas，用于创建带标签的数据帧和显示数据帧的元数据。然后你学习了如何从各种数据源创建数据帧，例如随机数和硬编码的数据值。此外，你还看到了如何在 Pandas 数据帧中执行基于列和行的操作。

你还学习了如何读取 Excel 工作表并对这些工作表中的数据进行数值计算，例如数值列中的最小值、平均值和最大值。然后，你看到了如何从存储在 CSV 文件中的数据创建 Pandas 数据帧。

第二章

机器学习简介

本章介绍了机器学习中的许多概念，例如特征选择、特征工程、数据清洗、训练集和测试集。

本章的第一部分简要讨论了机器学习以及准备数据集通常所需的步骤序列。这些步骤包括可以使用各种算法执行的“特征选择”或“特征提取”。

第二部分描述了你可以遇到的数据类型，数据集中可能出现的各种问题以及如何纠正这些问题。当你执行训练步骤时，你还将了解“保留”和“k-折”之间的区别。

本章的第三部分简要讨论了线性回归中涉及的基本概念。尽管线性回归在 200 多年前就已经发展起来，但这项技术仍然是解决统计学和机器学习（尽管是简单）问题的主要技术之一。实际上，用于在二维平面（或更高维度的超平面）上找到最佳拟合线的均值平方误差（MSE）技术，在 Python 中实现以最小化后面讨论的损失函数。

本章的第四部分包含使用 NumPy 标准技术进行线性回归任务的额外代码示例。因此，如果你熟悉这个主题，你可能会快速浏览本章的前两节。

什么是机器学习？

从高层次来说，机器学习是人工智能的一个子集，可以解决传统编程语言难以实现或过于繁琐的任务。垃圾邮件过滤器是机器学习的早期例子。通常，机器学习优于旧算法的准确性。

尽管机器学习算法种类繁多，但数据的重要性可能比选定的算法更重要。数据可能存在许多问题，例如数据不足、数据质量差、数据错误、数据缺失、数据不相关和数据值重复。在本章的后面部分，您将看到解决许多这些与数据相关问题的技术。

如果您不熟悉机器学习术语，数据集是一组数据值，可以是 CSV 文件或电子表格的形式。每一列称为特征，每一行是一个数据点，包含每个特征的特定值集合。如果数据集包含有关客户的信息，那么每一行都与一个特定客户相关。

机器学习类型

您将遇到三种主要的机器学习类型（这些类型的组合也是可能的）：

+   监督学习

+   无监督学习

+   半监督学习

监督学习意味着数据集中的数据点有一个标签来标识其内容。例如，MNIST 数据集包含 28x28 的 PNG 文件，每个文件包含一个手绘数字（即 0 到 9 inclusive）。每个包含数字 0 的图像都有标签“0”，每个包含数字 1 的图像都有标签“1”，所有其他图像都根据显示在图像中的数字进行标记。

另一个例子，泰坦尼克号数据集中的列是关于乘客的特征，例如他们的性别、船舱等级、票价以及乘客是否存活。每一行包含有关单个乘客的信息，包括如果乘客存活则值为 1。MNIST 数据集和泰坦尼克号数据集涉及分类任务：目标是训练一个模型，然后预测测试数据集中每一行的类别（MNIST）或存活（泰坦尼克号）。

通常，用于分类任务的数据集具有少量可能的值：0 到 9 范围内的九个数字中的一个、四种动物（狗、猫、马、长颈鹿）中的一个，或者两个值（存活与死亡、购买与未购买）中的一个。一般来说，如果结果的数量可以在下拉列表中合理地显示，那么这很可能是一个分类任务。

在包含房地产数据的数据集中，每一行包含有关特定房屋的信息，例如卧室数量、房屋平方英尺数、浴室数量和房屋价格。在这个数据集中，房屋价格是每一行的标签。请注意，可能的房价范围太大，无法合理地适合下拉列表。房地产数据集涉及回归任务：目标是基于训练数据集训练一个模型，然后预测测试数据集中每一所房屋的价格。

无监督学习涉及未标记的数据，这通常是聚类算法的情况（将在稍后讨论）。一些重要的涉及聚类的无监督学习算法将在下面列出：

+   k-means

+   层次聚类分析（HCA）

+   期望最大化

一些重要的涉及降维的无监督学习算法将在下面列出（将在稍后更详细地讨论）：

+   PCA（主成分分析）

+   核主成分分析

+   LLE（局部线性嵌入）

+   t-SNE（t-分布随机邻域嵌入）

还有一个非常重要的无监督任务称为异常检测。这项任务与欺诈检测和检测异常值（将在下一章中更详细地讨论）相关。

半监督学习是监督学习和无监督学习的结合：一些数据点是标记的，而一些数据点是没有标记的。一种技术是使用标记数据来分类（即标记）未标记的数据，之后你可以应用分类算法。

机器学习算法类型

机器学习算法主要有三种类型：

+   回归（例如：线性回归）

+   分类（例如：k-最近邻）

+   聚类（例如：k-means）

回归是一种监督学习技术，用于预测数值量。一个回归任务的例子是预测特定股票的价值。请注意，这项任务与预测特定股票明天（或某个其他未来时间段）的价值是否会增加或减少是不同的。另一个回归任务的例子是预测房地产数据集中房屋的损失。这两个任务都是回归任务的例子。

机器学习中的回归算法包括线性回归和广义线性回归（在传统统计学中也称为多元分析）。

分类也是一种监督学习技术，但它用于预测分类量。一个分类任务的例子是检测垃圾邮件、欺诈或确定 PNG 文件中的数字（如 MNIST 数据集）。在这种情况下，数据已经标记，因此你可以将预测与分配给给定 PNG 的标签进行比较。

机器学习中的分类算法包括以下算法列表（它们将在下一章中更详细地讨论）：

+   决策树（单一树）

+   随机森林（多棵树）

+   kNN（k-最近邻）

+   逻辑回归（尽管其名称如此）

+   天真贝叶斯

+   支持向量机（SVM）

一些机器学习算法（如 SVM、随机森林和 kNN）支持回归和分类。在 SVM 的情况下，scikit-learn 对该算法的实现提供了两个 API：SVC 用于分类，SVR 用于回归。

前述的每个算法都涉及一个在数据集上训练的模型，之后该模型被用来做出预测。相比之下，随机森林由多个独立的树组成（数量由你指定），每棵树对特征的值做出预测。如果特征是数值型的，取平均值或众数（或执行其他计算）以确定“最终”预测。如果特征是分类型的，使用众数（即最频繁出现的类别）作为结果；在出现平局的情况下，你可以随机选择其中之一。

顺便提一下，以下 URL 包含有关 kNN 算法（包括分类和回归）的更多信息：

[`saedsayad.com/k_nearest_neighbors_reg.htm`](http://saedsayad.com/k_nearest_neighbors_reg.htm)

聚类是一种无监督学习技术，用于将相似数据分组在一起。聚类算法将数据点放入不同的簇中，而不了解数据点的性质。数据被分离到不同的簇之后，你可以使用 SVM 算法进行分类。

机器学习中的聚类算法包括以下内容（其中一些是彼此的变体）：

+   k-means

+   均值漂移

+   层次聚类分析 (HCA)

+   期望最大化

请记住以下要点。首先，k-means 中的 k 值是一个超参数，通常是一个奇数，以避免两个类别之间的平局。其次，均值漂移算法结合了 k-means 算法，不需要你指定 k 的值。实际上，均值漂移算法确定最佳簇的数量。然而，这个算法在大数据集上扩展性不好。

机器学习任务

除非你有一个已经被清洗过的数据集，否则你需要检查数据集中的数据，以确保它们处于合适的状态。数据准备阶段包括检查行（“数据清洗”）以确保它们包含有效数据（可能需要特定领域的知识），以及检查列（特征选择或特征提取）以确定你是否可以仅保留最重要的列。

下面是一个高级的机器学习任务序列列表（其中一些可能不是必需的）：

+   获取数据集

+   数据清洗

+   特征选择

+   维度约简

+   算法选择

+   训练集与测试集

+   训练模型

+   测试模型

+   微调模型

+   获取模型的度量指标

首先，显然你需要为你的任务获取一个数据集。在理想情况下，这个数据集已经存在；否则，你需要从一个或多个数据源（例如 CSV 文件、关系型数据库、NoSQL 数据库和 Web 服务）中提取数据。

其次，你需要进行数据清洗，你可以通过以下技术来完成：

+   缺失值比率

+   低方差滤波器

+   高相关性滤波器

通常，数据清理涉及检查数据集中的数据值，以解决以下一个或多个问题：

+   修复不正确的值

+   解决重复值

+   解决缺失值

+   决定如何处理异常值

如果数据集有太多缺失值，请使用缺失值比率技术。在极端情况下，你可能能够删除具有大量缺失值的特征。使用低方差过滤器技术来识别并从数据集中删除具有常数值的特征。使用高相关性过滤器技术来找到高度相关的特征，这些特征会增加数据集中的多重共线性：可以从数据集中删除这些特征（但在这样做之前请咨询你的领域专家）。

根据你的背景和数据集的性质，你可能需要与领域专家合作，他们是对数据集内容有深入了解的人。

例如，你可以使用统计值（均值、众数等）来用合适的值替换不正确的值。重复值可以以类似的方式处理。你可以用零、最小值、均值、众数或数值列中的最大值替换缺失的数值值。你可以用分类列的众数替换缺失的分类值。

如果数据集中的一行包含一个异常值，你有三个选择：

+   删除该行

+   保留该行

+   用其他值（均值？）替换异常值

当一个数据集包含异常值时，你需要根据特定于给定数据集的领域知识做出决定。

假设一个数据集包含与股票相关的信息。正如你所知，1929 年发生了股市崩盘，你可以将其视为一个异常值。这样的发生是罕见的，但它可能包含有意义的信息。顺便说一句，20 世纪一些家庭的财富来源是基于大萧条期间以非常低的价格购买大量股票。

特征工程、选择和提取

除了创建数据集和“清理”其值之外，你还需要检查该数据集中的特征，以确定你是否可以减少数据集的维度（即特征的数目）。这样做涉及三个主要技术：

+   特征工程

+   特征选择

+   特征提取（也称为“特征投影”）

特征工程是将基于现有特征组合的新特征集确定下来的过程，以创建针对特定任务的有意义的数据集。即使是在相对简单的数据集的情况下，这个过程通常也需要领域专业知识。特征工程可能既繁琐又昂贵，在某些情况下，你可能会考虑使用自动特征学习。在你创建数据集之后，执行特征选择或特征提取（或两者都执行）以确保你有一个高质量的数据集是一个好主意。

特征选择也称为“变量选择”、“属性选择”或“变量子集选择”。特征选择涉及在数据集中选择相关特征的一个子集。本质上，特征选择涉及选择数据集中最重要的特征，这提供了以下优势：

+   减少了训练时间

+   更简单且易于解释的模型

+   避免维度灾难

+   由于过拟合减少（“方差减少”）而具有更好的泛化能力

特征选择技术通常用于具有许多特征和相对较少样本（或数据点）的领域。请记住，低价值特征可能是冗余的或不相关的，这两个概念是不同的。例如，当与另一个强相关特征结合时，一个相关特征可能是冗余的。

特征选择可以使用三种策略：过滤器策略（例如，信息增益），包装器策略（例如，由准确度引导的搜索），以及嵌入式策略（在构建模型时使用预测误差来确定是否包含或排除特征）。另一个有趣的观点是，特征选择对于回归任务以及分类任务也可能是有用的。

特征提取从产生原始特征组合的函数中创建新的特征。相比之下，特征选择涉及确定现有特征的一个子集。

特征选择和特征提取都会导致给定数据集的维度降低，这是下一节的主题。

维度降低

维度降低是指减少数据集中特征数量的算法。正如您将看到的，有许多技术可用，它们涉及特征选择或特征提取。

使用特征选择进行维度降低的算法如下：

+   后向特征消除

+   前向特征选择

+   因子分析

+   独立成分分析（Independent Component Analysis）

使用特征提取进行维度降低的算法如下：

+   主成分分析（PCA）

+   非负矩阵分解（NMF）

+   核主成分分析（kernel PCA）

+   基于图的核主成分分析（graph-based kernel PCA）

+   线性判别分析（LDA）

+   广义判别分析（GDA）

+   自动编码器

以下算法结合了特征提取和维度降低：

+   主成分分析（PCA）

+   线性判别分析（LDA）

+   标准相关分析（CCA）

+   非负矩阵分解（NMF）

这些算法可以在使用聚类或其他算法（如 kNN）对数据集进行预处理步骤中使用。另一组算法包括基于投影的方法，其中包括 t-Distributed Stochastic Neighbor Embedding（t-SNE）以及 UMAP。

本章讨论了 PCA，您可以通过在线搜索找到有关其他算法的更多信息。

主成分分析（PCA）

主成分是数据集中初始特征的一组线性组合的新成分。此外，这些成分是不相关的，并且最有意义或最重要的信息包含在这些新成分中。

PCA 有两个优点：由于特征数量大大减少，计算时间减少，以及在最多有三个成分时能够绘制成分的能力。如果你有四个或五个成分，你将无法直观地显示它们，但你可以选择三个成分的子集进行可视化，并可能对数据集有更深入的了解。

PCA 使用方差作为信息量的度量：方差越高，成分越重要。实际上，PCA 确定协方差矩阵（稍后讨论）的特征值和特征向量，并构建一个新的矩阵，其列是特征向量，从左到右按左列中最大特征值排序，直到最右侧的特征向量也有最小的特征值。

协方差矩阵

作为提醒，随机变量 X 的统计量称为方差，定义为以下：

variance(x) = [SUM (x – xbar)*(x-xbar)]/n

协方差矩阵 C 是一个 nxn 矩阵，其主对角线上的值是变量 X1, X2, . . ., Xn 的方差。C 的其他值是每对变量 Xi 和 Xj 的协方差值。

变量 X 和 Y 的协方差公式是变量方差的推广，公式如下所示：

covariance(X, Y) = [SUM (x – xbar)*(y-ybar)]/n

注意，你可以反转项乘积的顺序（乘法是交换律的），因此协方差矩阵 C 是一个对称矩阵：

covariance(X, Y) = covariance(Y,X)

PCA 计算协方差矩阵 A 的特征值和特征向量。

工作与数据集

除了数据清洗之外，你还需要执行几个其他步骤，例如选择训练数据与测试数据，并在训练过程中决定是否使用“保留”或交叉验证。更多细节将在后续章节中提供。

训练数据与测试数据

在你完成了本章前面描述的任务（即数据清洗和可能的数据降维）之后，你就可以将数据集分成两部分。第一部分是训练集，用于训练模型，第二部分是测试集，用于“推断”（预测的另一种说法）。确保你的测试集符合以下指南：

1. 集合足够大，可以产生具有统计意义的成果。

2. 它代表了整个数据集。

3. 永远不要在测试数据上训练。

4. 永远不要在训练数据上测试。

什么是交叉验证？

交叉验证的目的是使用非重叠的测试集来测试模型，其执行方式如下：

第一步）将数据分成大小相等的 k 个子集。

第二步）选择一个子集进行测试，其余的用于训练。

第三步）对其他 k-1 个子集重复第二步。

这个过程被称为 k 折交叉验证，总体误差估计是误差估计的平均值。一种标准的评估方法涉及十折交叉验证。大量实验表明，使用十个子集是获得准确估计的最佳选择。实际上，你可以重复十折交叉验证十次，并计算结果的平均值，这有助于减少方差。

下一个部分讨论正则化，这是本书中一个重要但可选的主题。如果你计划精通机器学习，你需要了解正则化。

**什么是正则化**？

正则化有助于解决过拟合问题，即模型在训练数据上表现良好，但在验证或测试数据上表现不佳。正则化通过向损失函数添加惩罚项来解决此问题，从而通过此惩罚项控制模型复杂度。正则化通常对以下情况有用：

+   大量变量

+   (#观察值)/(#变量)的比率低

+   高度多重共线性

正则化主要有两种类型：L1 正则化（与 MAE，即差异的绝对值相关）和 L2 正则化（与 MSE，即差异的平方相关）。一般来说，L2 的性能优于 L1，且在计算效率方面 L2 更优。

机器学习和特征缩放

特征缩放标准化了数据的特征范围。此步骤在数据预处理步骤中执行，部分原因是因为梯度下降从特征缩放中受益。

假设数据符合标准正态分布，标准化涉及从每个数据点减去均值并除以标准差，从而得到 N(0,1)正态分布。

数据标准化与标准化比较

数据标准化是一种线性缩放技术。假设一个数据集具有值 {X1, X2, . . . , Xn} 以及以下术语：

Minx = Xi 值的**最小值**

Maxx = Xi 值的**最大值**

现在按照以下方式计算一组新的 Xi 值：

Xi = (Xi – Minx)/[Maxx – Minx]

新的 Xi 值现在被缩放，使其介于 0 和 1 之间。

**偏差-方差权衡**

机器学习中的偏差可能源于学习算法中错误假设的错误。高偏差可能导致算法错过特征与目标输出之间的相关关系（欠拟合）。预测偏差可能由于“噪声”数据、不完整的特征集或有偏的训练样本而出现。

偏差误差是模型预期的（或平均）预测值与想要预测的正确值之间的差异。多次重复模型构建过程，每次都收集新的数据，并进行分析以生成新的模型。由于基础数据集具有一定的随机性，因此生成的模型具有一系列预测值。偏差衡量这些模型的预测值与正确值之间的程度。

机器学习中方差是平均值的平方偏差的期望值。高方差可能导致算法模型训练数据中的随机噪声，而不是预期的输出（过拟合）。

向模型添加参数会增加其复杂性，增加方差，并减少偏差。处理偏差和方差就是处理欠拟合和过拟合。

方差误差是针对给定数据点的模型预测的变异性。与之前一样，重复整个模型构建过程，方差是针对给定点的预测在不同“实例”中的变化程度。

测量模型的指标

线性回归模型使用 R 平方，它衡量数据与拟合回归线（回归系数）的接近程度。R 平方的值始终是介于 0%和 100%之间的百分比。0%的值表示模型无法解释其均值周围的响应数据的任何可变性。100%的值表示模型可以解释其均值周围的响应数据的所有可变性。一般来说，R 平方值越高，表示模型越好。

R 平方的局限性

虽然高 R 平方值是首选的，但它们并不一定是始终好的值。同样，低 R 平方值也不一定是坏的。例如，预测人类行为的 R 平方值通常小于 50%。此外，R 平方无法确定系数估计和预测是否存在偏差。此外，R 平方值并不表示回归模型是否充分。因此，对于好的模型，可能有一个低 R 平方值，或者对于拟合不良的模型，可能有一个高 R 平方值。结合残差图、其他模型统计信息和领域知识来评估 R 平方值。

混淆矩阵

分类算法使用混淆矩阵（也称为“错误矩阵”），它是一个包含假阳性、假阴性、真阳性和真阴性的平方列联表。2x2 混淆矩阵中的四个条目可以按以下方式标记：

TP：真阳性

FP：假阳性

TN：真阴性

FN：假阴性

混淆矩阵的对角线值是正确预测，而离对角线值是不正确预测。一般来说，较低的 FP 值比 FN 值要好。例如，FP 表示一个健康的人被错误地诊断为患有疾病，而 FN 表示一个不健康的人被错误地诊断为健康。

准确度与精确度与召回率

一个 2x2 的混淆矩阵有四个条目，代表正确和错误分类的各种组合。根据前面章节的定义，精确度、准确度和召回率的定义如下公式所示：

精确度 = TP/(TP + FP)

准确度 = (TP + TN)/[TP + FP + FN + TN]

召回率 = TP/[TP + FN]

准确度可能是一个不可靠的指标，因为它在数据不平衡的情况下会产生误导性的结果。当不同类别的观察数量显著不同时，它会给错误阳性分类和错误阴性分类以同等的重要性。例如，宣布癌症为良性比错误地告知患者他们正在遭受癌症更糟糕。不幸的是，准确度无法区分这两种情况。

请记住，混淆矩阵可以是一个 nxn 的矩阵，而不仅仅是 2x2 的矩阵。例如，如果一个类别有 5 个可能的值，那么混淆矩阵就是一个 5x5 的矩阵，而主对角线上的数字是“真正”的结果。

ROC 曲线

接收者操作特征（ROC）曲线是一条曲线，它绘制了真正率（TPR，即召回率）与假正率（FPR）的关系。请注意，真正负率（TNR）也称为特异性。

以下网页包含了一个使用 sklearn 和 Iris 数据集的 Python 代码示例，以及绘制 ROC 的代码：

[`scikit-learn.org/stable/auto_examples/model_selection/plot_roc.html`](https://scikit-learn.org/stable/auto_examples/model_selection/plot_roc.html)

以下网页包含了一系列用于绘制 ROC 曲线的 Python 代码示例：

[`stackoverflow.com/questions/25009284/how-to-plot-roc-curve-in-python`](https://stackoverflow.com/questions/25009284/how-to-plot-roc-curve-in-python)

其他有用的统计术语

机器学习依赖于许多统计量来评估模型的有效性，其中一些列在这里：

+   RSS

+   TSS

+   R²

+   F1 分数

+   p 值

RSS、TSS 和 R² 的定义如下，其中 y^是最佳拟合线上一点的 y 坐标，y_ 是数据集中点的 y 值的平均值：

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p47.jpg)

F1 分数是什么？

*F1 分数*是测试准确度的度量，定义为精确度和召回率的调和平均值。以下是相关公式，其中 p 是精确度，r 是召回率：

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p48.jpg)

F1 分数的最佳值是 0，最差值也是 0。F1 分数通常用于分类问题，而 R² 值通常用于回归任务（如线性回归）。

什么是 p 值？

如果 p 值足够小（< 0.005），则可以使用 p 值来拒绝零假设，这表明更高的显著性。回想一下，零假设表明一个因变量（如 y）和一个自变量（如 x）之间没有相关性。p 的阈值通常是 1%或 5%。

计算 p 值并没有一个直接的公式，p 值总是在 0 和 1 之间。实际上，p 值是用于评估“零假设”的统计量，它们是通过 p 值表或电子表格/统计软件来计算的。

什么是线性回归？

线性回归的目标是找到代表数据集的最佳拟合线。记住两个关键点。首先，最佳拟合线不一定通过数据集中的所有（甚至大多数）点。最佳拟合线的目的是使该线与数据集中点的垂直距离最小化。其次，线性回归并不确定最佳拟合的多项式：后者涉及找到通过数据集中许多点的更高次多项式。

此外，平面上的数据集可以包含两个或更多位于同一直线上的点，也就是说，这些点的 x 值相同。然而，一个函数不能通过这样的点对：如果两个点(x1,y1)和(x2,y2)具有相同的 x 值，那么它们必须具有相同的 y 值（即 y1=y2）。一个函数可以有多个位于同一直线上的点。

现在考虑一个在平面上有许多点，这些点以某种“聚集”的形状排列成拉长的云状：最佳拟合线可能只会与有限数量的点相交（实际上，最佳拟合线可能不会与任何点相交）。

考虑另一种情况：假设一个数据集包含一组位于同一直线上的点。例如，假设 x 值在集合{1,2,3,...,10}中，y 值在集合{2,4,6,...,20}中。那么最佳拟合线的方程是 y=2*x+0。在这种情况下，所有点都是共线的，也就是说，它们位于同一直线上。

线性回归与曲线拟合的比较

假设一个数据集由 n 个形式为 (x, y) 的数据点组成，并且这些数据点中没有两个具有相同的 x 值。那么，根据数学中的一个已知结果，存在一个次数小于或等于 n-1 的多项式穿过这些 n 个点（如果你真的感兴趣，你可以在在线文章中找到这个陈述的数学证明）。例如，一条直线是一个一次多项式，它可以与平面上任何一对非垂直点相交。对于平面上任何三个不在同一直线上的点，都存在一个通过这些点的二次方程。

此外，有时可以使用低次多项式。例如，考虑一组 100 个点，其中 x 值等于 y 值：在这种情况下，直线 y = x（这是一个一次多项式）穿过所有 100 个点。

然而，一条直线“代表”平面上一组点的程度取决于这些点可以被直线多紧密地近似，这通过点的方差来衡量（方差是一个统计量）。点越线性，方差越小；相反，点越“分散”，方差越大。

解何时为精确值？

虽然基于统计学的解为线性回归提供了封闭形式的解，但神经网络提供的是近似解。这是因为线性回归的机器学习算法涉及一系列近似，这些近似“收敛”到最优值，这意味着机器学习算法产生的是精确值的估计。例如，对于二维平面上的一组点，最佳拟合线的斜率 m 和 y 轴截距 b 在统计学中有一个封闭形式的解，但它们只能通过机器学习算法来近似（虽然存在例外，但这种情况很少见）。

尽管传统的线性回归的封闭形式解为 m 和 b 提供了精确值，但有时你只能使用精确值的近似。例如，假设最佳拟合线的斜率 m 等于 3 的平方根，而 y 轴截距 b 是 2 的平方根。如果你计划在源代码中使用这些值，你只能处理这两个数的近似值。在相同的情况下，神经网络计算 m 和 b 的近似值，无论 m 和 b 的精确值是有理数、无理数还是整数。然而，机器学习算法更适合复杂、非线性、多维数据集。

作为简单的例子，假设线性回归问题的封闭形式解对于斜率 m 和 y 轴截距 b 都产生了整数或有理数。具体来说，假设封闭形式解给出了斜率为 2.0 和 y 轴截距为 1.0 的最佳拟合线的值。这条直线的方程看起来是这样的：

y = 2.0 * x + 1.0

然而，从训练神经网络得到的相应解可能会产生斜率 m 和 y 轴截距 b 的值分别为 2.0001 和 0.9997，作为最佳拟合线的 m 和 b 的值。始终记住这一点，尤其是在你训练神经网络时。

什么是多元分析？

多元分析将欧几里得平面上的直线方程推广到更高维度，并称之为超平面而不是直线。推广后的方程具有以下形式：

y = w1*x1 + w2*x2 + . . . + wn*xn + b

在二维线性回归的情况下，你只需要找到斜率（m）和 y 轴截距（b）的值，而在多元分析中，你需要找到 w1、w2、...、wn 的值。请注意，多元分析是统计学中的一个术语，在机器学习中通常被称为“广义线性回归”。本书中涉及线性回归的大多数代码示例都涉及欧几里得平面中的二维点。

其他回归类型

线性回归找到最佳拟合线，以“代表”数据集，但如果平面中的直线不适合数据集呢？当你处理数据集时，这是一个相关的问题。

线性回归的一些替代方案包括二次方程、三次方程或更高次的多项式。然而，这些替代方案涉及权衡，我们将在后面讨论。

另一种可能性是一种混合方法，涉及分段线性函数，它由一系列线段组成。如果连续的线段是连接的，那么它是一个分段线性连续函数；否则，它是一个分段线性不连续函数。

因此，给定平面上的点集，回归涉及解决以下问题：

1. 哪种类型的曲线适合数据？我们如何知道？

2. 另一种类型的曲线是否更适合数据？

3. “最佳拟合”是什么意思？

检查一条直线是否适合数据的一种方法涉及视觉检查，但这种方法不适用于高于二维的数据点。此外，这是一个主观的决定，本章后面将展示一些样本数据集。通过数据集的视觉检查，你可能会决定二次或三次（甚至更高次）多项式有潜力成为数据的更好拟合。然而，视觉检查可能仅限于二维平面或三维空间中的点。

让我们暂时不考虑非线性情况，并假设一条直线会是一个良好的数据拟合。有一种已知的技术可以找到此类数据集的“最佳拟合”线，这涉及到最小化均方误差（我们将在本章后面讨论）。

下一个部分提供了平面中线性方程的快速回顾，以及一些说明线性方程示例的图像。

在平面中处理直线（可选）

本节简要回顾了欧几里得平面中的线，如果你对这个主题感到舒适，可以跳过这一节。一个常被忽视的细微之处是，欧几里得平面中的线具有无限长度。如果你选择一条线上的两个不同点，那么这两个点之间的所有点构成一条线段。射线是一条“半无限”的线：当你选择一个点作为端点时，那么直线一侧的所有点构成一条射线。

例如，平面上 y 坐标为 0 的点是一条线，也是 x 轴，而 x 轴上(0,0)和(1,0)之间的点形成一条线段。此外，x 轴上位于(0,0)右侧的点形成一条射线，而 x 轴上位于(0,0)左侧的点也形成一条射线。

为了简便和方便，在这本书中，我们将“线”和“线段”这两个术语互换使用。现在让我们深入了解欧几里得平面中线的细节。以下是欧几里得平面中一条（非垂直）线的方程：

y = m*x + b

m 的值是直线的斜率，b 的值是 y 轴截距（即直线与 y 轴相交的点）。

如果需要，你可以使用一个更通用的方程，它可以表示垂直线，如下所示：

a*x + b*y + c = 0

然而，我们不会处理垂直线，所以我们将使用第一个公式。

图 2.1 展示了三条水平线，其方程（从上到下）分别为 y = 3，y = 0 和 y = -3。

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p52-1.jpg)

图 2.1 三条水平线段的图形

图 2.2 展示了两条斜率不同的直线，其方程分别为 y = x 和 y = -x。

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p52-2.jpg)

图 2.2 两条对角线段的图形

图 2.3 展示了两条斜率平行的直线，其方程分别为 y = 2*x 和 y = 2*x + 3。

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p53-1.jpg)

图 2.3 两条斜率平行的线段的图形

图 2.4 展示了一个由连接线段组成的分段线性图形。

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p53-2.jpg)

图 2.4 线段的分段线性图形

让我们关注使用 NumPy API 生成准随机数据，然后我们将使用 Matplotlib 绘制数据。

使用 NumPy 和 Matplotlib 绘制散点图（1）

列表 2.1 展示了 np_plot1.py 的内容，该内容说明了如何使用 NumPy 的 randn() API 生成数据集，然后使用 Matplotlib 的 scatter() API 在数据集中绘制点。

需要注意的一个细节是，所有相邻的水平值都是等间距的，而垂直值是基于一个线性方程加上一个“扰动”值。这种“扰动技术”（这不是一个标准术语）在本章的其他代码示例中用于在绘制点时添加略微随机化的效果。这种技术的优点是，m 和 b 的最佳拟合值是事先已知的，因此我们不需要猜测它们的值。

列表 2.1: np_plot1.py

import numpy as np

import matplotlib.pyplot as plt

x = np.random.randn(15,1)

y = 2.5*x + 5 + 0.2*np.random.randn(15,1)

print("x:",x)

print("y:",y)

plt.scatter(x,y)

plt.show()

列表 2.1 包含两个导入语句，然后初始化数组变量 x 为 0 到 1 之间的 15 个随机数。

接下来，数组变量 y 在两部分中定义：第一部分是一个线性方程 2.5*x + 5，第二部分是基于随机数的“扰动”值。因此，数组变量 y 模拟了一组接近线段的一组值。

这种技术在模拟线段的代码示例中使用，然后训练部分近似 m 和 b 的最佳拟合线值。显然，我们已知最佳拟合线的方程：这种技术的目的是比较训练得到的斜率 m 和 y 轴截距 b 的值与已知值（在这种情况下，是 2.5 和 5）。列表 2.1 的部分输出如下：

x: [[-1.42736308]

[ 0.09482338]

[-0.45071331]

[ 0.19536304]

[-0.22295205]

// 省略值以节省篇幅

y: [[1.12530514]

[5.05168677]

[3.93320782]

[5.49760999]

[4.46994978]

// 省略值以节省篇幅

图 2.5 显示了基于 x 和 y 值的点散点图。

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p55.jpg)

图 2.5 线段的点散点图

为什么扰动技术是有用的

您已经看到了如何使用扰动技术，为了比较，考虑以下数据集，这些点定义在 Python 数组变量 X 和 Y 中：

X = [0,0.12,0.25,0.27,0.38,0.42,0.44,0.55,0.92,1.0]

Y = [0,0.15,0.54,0.51, 0.34,0.1,0.19,0.53,1.0,0.58]

如果您需要为前面的数据集找到最佳拟合线，您会如何猜测斜率 m 和 y 轴截距 b 的值？在大多数情况下，您可能无法猜测它们的值。然而，扰动技术使您能够稍微移动一条线的点，该线的斜率 m（以及可选的 y 轴截距 b）的值是事先指定的。

扰动技术仅在您引入的小随机值不会导致 m 和 b 的值不同时才有效。

使用 NumPy 和 Matplotlib 绘制散点图（2）

列表 2.1（前一部分）中的代码将随机值分配给变量 x，而斜率 m 是硬编码的值。y 值是 x 值的硬编码倍数，加上通过扰动技术计算出的随机值。因此，我们不知道 y 截距 b 的值。

在本节中，trainX 的值基于 np.linspace() API，而 trainY 的值涉及前一部分中描述的扰动技术。

此示例中的代码简单地打印了 trainX 和 trainY 的值，它们对应于欧几里得平面中的数据点。列表 2.2 显示了 np_plot2.py 的内容，说明了如何在 NumPy 中模拟线性数据集。

列表 2.2: np_plot2.py

import numpy as np

trainX = np.linspace(-1, 1, 11)

trainY = 4*trainX + np.random.randn(*trainX.shape)*0.5

print("trainX: ",trainX)

print("trainY: ",trainY)

列表 2.2 通过 NumPy linspace() API 初始化 NumPy 数组变量 trainX，然后是定义在两部分的数组变量 trainY。第一部分是线性项 4*trainX，第二部分涉及的是随机生成的数字的扰动技术。列表 2.2 的输出如下：

trainX: [-1. -0.8 -0.6 -0.4 -0.2 0. 0.2 0.4 0.6 0.8 1. ]

trainY: [-3.60147459 -2.66593108 -2.26491189 -1.65121314 -0.56454605 0.22746004 0.86830728 1.60673482 2.51151543 3.59573877 3.05506056]

下一个部分包含了一个与 列表 2.2 类似的示例，使用相同的扰动技术生成一组近似二次方程而不是线段的点。

使用 NumPy 和 Matplotlib 的二次散点图

列表 2.3 显示了 np_plot_quadratic.py 的内容，说明了如何在平面上绘制二次函数。

列表 2.3: np_plot_quadratic.py

import numpy as np

import matplotlib.pyplot as plt

#see what happens with this set of values:

#x = np.linspace(-5,5,num=100)

x = np.linspace(-5,5,num=100)[:,None]

y = -0.5 + 2.2*x +0.3*x**2 + 2*np.random.randn(100,1)

print("x:",x)

plt.plot(x,y)

plt.show()

列表 2.3 初始化数组变量 x，其值是通过 np.linspace() API 生成的，在这种情况下，是一组在 -5 和 5 之间等距的 100 个十进制数。注意 x 初始化中的片段 [:,None]，它导致每个元素都是一个包含单个数字的数组的数组。

数组变量 y 定义在两部分：第一部分是二次方程 -0.5 + 2.2*x +0.3*x**2，第二部分是基于随机数的“扰动”值（类似于 列表 2.1 中的代码）。因此，数组变量 y 模拟了一组近似二次方程的值。列表 2.3 的输出如下：

x:

[[-5. ]

[-4.8989899 ]

[-4.7979798 ]

[-4.6969697 ]

[-4.5959596 ]

[-4.49494949]

// 省略值以节省篇幅

[ 4.8989899 ]

[ 5\. ]]

图 2.6 显示了基于 x 和 y 值的点散点图，这些点具有近似二次方程的形状。

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p57.jpg)

图 2.6：二次方程点的散点图

均方误差（MSE）公式

MSE 是实际 y 值与预测 y 值之间差异的平方和，除以点的数量。请注意，预测 y 值是如果该点实际上位于最佳拟合线上，每个点将具有的 y 值。

虽然 MSE 在线性回归中很受欢迎，但还有其他错误类型可供选择，其中一些将在下一节中简要讨论。

错误类型列表

尽管我们将在本书中仅讨论线性回归的 MSE，但还有其他类型的公式可用于线性回归，其中一些列在这里：

+   MSE

+   RMSE

+   RMSPROP

+   MAE

MSE 是先前错误类型的基础。例如，RMSE 是均方根误差，它是 MSE 的平方根。

MAE 是平均绝对误差，它是 y 项差值的绝对值之和（而不是 y 项差值的平方），然后除以项数。

RMSPROP 优化器利用最近梯度的幅度来归一化梯度。具体来说，RMSPROP 维护一个关于 RMS（均方根）梯度的移动平均值，然后将该值除以当前梯度。

虽然计算 MSE 的导数更容易，但 MSE 也更容易受到异常值的影响，而 MAE 则不太容易受到异常值的影响。原因很简单：一个平方项可以比项的绝对值大得多。例如，如果一个差值项是 10，那么 100（10 的平方）将被添加到 MSE 中，而只有 10（-20 的绝对值）被添加到 MAE 中。同样，如果一个差值项是-20，那么 400（-20 的平方）将被添加到 MSE 中，而只有 20（-20 的绝对值）被添加到 MAE 中。

非线性最小二乘法

在预测房价时，数据集包含广泛的价值范围，线性回归或随机森林等技术可能导致模型过度拟合具有最高值的样本，以减少如平均绝对误差等数量。

在这种情况下，你可能需要一个误差度量，如相对误差，它降低了拟合具有最大值的样本的重要性。这种技术称为非线性最小二乘法，它可能使用基于标签和预测值的对数变换。

下一节包含几个代码示例，第一个示例涉及手动计算 MSE，随后是一个使用 NumPy 公式进行计算的示例。

手动计算 MSE

本节包含两个线形图，两个图都包含一条近似散点图中一组点的线。

图 2.7 显示了一个近似散点图点的线段（其中一些点与线段相交）。图 2.7 中线段的 MSE 计算如下（仅比较分子）：

MSE = (1*1 + (-1)*(-1) + (-1)*(-1) + 1*1)/9 = 4/9

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p59.jpg)

图 2.7 展示了一个近似散点图点的线图

图 2.8 显示了一组点和一条可能是最佳拟合线的线。图 2.8 中线的 MSE 计算如下：

MSE = ((-2)*(-2) + 2*2)/7 = 8/7

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p60.jpg)

图 2.8 展示了一个近似散点图点的线图

因此，图 2.7 中的线比图 2.8 中的线具有更小的 MSE，这可能会让你感到惊讶（或者你猜对了？）。

在这两个图中，我们轻松快速地计算了均方误差（MSE），但在一般情况下，这要困难得多。例如，如果我们绘制 10 个点在欧几里得平面上，这些点并不紧密地拟合一条线，且涉及非整数值的各个项，我们可能需要计算器。

一个更好的解决方案涉及 NumPy 函数，如下一节中讨论的 np.linspace() API。

使用 NP.LINSPACE()近似线性数据

列表 2.4 展示了 np_linspace1.py 的内容，说明了如何结合扰动技术使用 np.linspace() API 生成一些数据。

列表 2.4：np_linspace1.py

import numpy as np

trainX = np.linspace(-1, 1, 6)

trainY = 3*trainX+ np.random.randn(*trainX.shape)*0.5

print("trainX: ", trainX)

print("trainY: ", trainY)

此代码示例的目的是生成并显示一组随机生成的数字。在本章的后面部分，我们将使用此代码作为实际线性回归任务的起点。

列表 2.4 从定义通过 np.linspace() API 初始化的数组变量 trainX 开始。接下来，通过在之前的代码示例中使用的扰动技术定义数组变量 trainY。列表 2.4 的输出如下：

trainX: [-1\. -0.6 -0.2 0.2 0.6 1\. ]

trainY: [-2.9008553 -2.26684745 -0.59516253 0.66452207 1.82669051 2.30549295]

trainX: [-1\. -0.6 -0.2 0.2 0.6 1\. ]

trainY: [-2.9008553 -2.26684745 -0.59516253 0.66452207 1.82669051 2.30549295]

现在我们知道了如何生成线性方程的(x,y)值，让我们学习如何计算 MSE，这在下一节中讨论。下一个示例使用 np.linspace()方法和 np.random.randn()方法生成一组数据值，以在数据点中引入一些随机性。

使用 NP.LINSPACE() API 计算 MSE

本节中的代码示例与本章中许多早期的代码示例不同：它使用硬编码的 X 和 Y 的值数组，而不是扰动技术。因此，你将不知道斜率和 y 截距的正确值（你可能也无法猜测它们的正确值）。列表 2.5 显示了 plain_linreg1.py 的内容，说明了如何使用模拟数据计算均方误差。

列表 2.5：plain_linreg1.py

import numpy as np

import matplotlib.pyplot as plt

X = [0,0.12,0.25,0.27,0.38,0.42,0.44,0.55,0.92,1.0]

Y = [0,0.15,0.54,0.51, 0.34,0.1,0.19,0.53,1.0,0.58]

losses = []

#第一步：参数初始化

W = 0.45

b = 0.75

for i in range(1, 100):

#第二步：计算损失

Y_pred = np.multiply(W, X) + b

Loss_error = 0.5 * (Y_pred - Y)**2

loss = np.sum(Loss_error)/10

#第三步：计算 dW 和 db

db = np.sum((Y_pred - Y))

dw = np.dot((Y_pred - Y), X)

losses.append(loss)

#第四步：更新参数：

W = W - 0.01*dw

b = b - 0.01*db

if i%10 == 0:

print("第", i,"次迭代的损失 = ", loss)

#第五步：通过 for 循环重复 1000 次

#绘制损失与迭代次数的关系图

print("W = ", W,"& b = ", b)

plt.plot(losses)

plt.ylabel('loss')

plt.xlabel('iterations (per tens)')

plt.show()

列表 2.5 初始化了数组变量 X 和 Y，并使用硬编码的值，然后初始化了标量变量 W 和 b。列表 2.5 的下一部分包含一个循环，循环 100 次。循环的每次迭代后，都会计算变量 Y_pred、Loss_error 和 loss 的值。接下来，根据数组 Y_pred-Y 中的项的和以及 Y_pred-y 和 X 的内积，计算 dw 和 db 的值。

注意 W 和 b 是如何更新的：它们的值分别通过 0.01*dw 和 0.01*db 的项递减。这个计算应该看起来很熟悉：代码正在程序化地计算 W 和 b 的梯度的近似值，W 和 b 都乘以学习率（硬编码的值 0.01），然后从 W 和 b 的当前值中减去得到的项，以产生 W 和 b 的新近似值。尽管这个技术很简单，但它确实计算了 W 和 b 的合理值。

列表 2.5 中的最后一段代码显示了 W 和 b 的中间近似值，以及损失（垂直轴）与迭代次数（水平轴）的图表。这里提供了列表 2.5 的输出：

第 10 次迭代的损失 = 0.04114630674619492

第 20 次迭代的损失 = 0.026706242729839392

第 30 次迭代的损失 = 0.024738889446900423

第 40 次迭代的损失 = 0.023850565034634254

第 50 次迭代的损失 = 0.0231499048706651

第 60 次迭代的损失 = 0.02255361434242207

第 70 次迭代的损失 = 0.0220425055291673

第 80 次迭代的损失 = 0.021604128492245713

第 90 次迭代的损失 = 0.021228111750568435

W = 0.47256473531193927 & b = 0.19578262688662174

图 2.9 显示了由列表 2.5 中的代码生成的点的散点图。

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p63.jpg)

图 2.9 线性回归的 MSE 值

代码示例 plain-linreg2.py 与列表 2.5 中的代码类似：不同之处在于，它不是单循环 100 次迭代，而是有一个外循环执行 100 次，而在外循环的每次迭代中，内循环也执行 100 次。

摘要

本章介绍了机器学习以及诸如特征选择、特征工程、数据清洗、训练集和测试集等概念。接下来，你学习了监督学习、无监督学习和半监督学习。然后你学习了回归任务、分类任务和聚类，以及准备数据集通常所需的步骤。这些步骤包括“特征选择”或“特征提取”，可以使用各种算法执行。然后你学习了数据集中可能出现的与数据相关的问题以及如何纠正这些问题。

此外，你还学习了线性回归，以及如何计算欧几里得平面上值数据集的最佳拟合线的一个简要描述。你看到了如何使用 NumPy 初始化数据值数组来执行线性回归，以及一种“扰动技术”，该技术为 y 值引入了一些随机性。这种技术很有用，因为你知道最佳拟合线的斜率和 y 截距的正确值，然后你可以将它们与训练值进行比较。

第三章

机器学习中的分类器

本章介绍了机器学习中的许多分类算法。这包括 kNN（k-最近邻）算法、逻辑回归（尽管其名称如此，但它是一个分类器）、决策树、随机森林、SVMs 和贝叶斯分类器。对算法的强调是为了让你了解机器学习，其中包括一个基于 scikit-learn 的树代码示例。

由于篇幅限制，本章没有涵盖其他知名算法，如线性判别分析和 k-means 算法（它是用于无监督学习和聚类的）。然而，有许多在线教程讨论了这些以及其他机器学习算法。

考虑到前面的要点，本章的第一部分简要讨论了引言段落中提到的分类器。本章的第二部分提供了激活函数的概述，如果你决定学习深度神经网络，这将非常有用。你将了解它们在神经网络中是如何以及为什么被使用的。本节还包含 TensorFlow API 激活函数的列表，随后是对其中一些优点的描述。

第三部分介绍了逻辑回归，它依赖于 Sigmoid 函数，也用于 RNNs（循环神经网络）和 LSTMs（长短期记忆）。

为了给您提供一些背景信息，分类器是三种主要算法类型之一：回归算法（例如，线性回归和第四章中的 GPT-4 [12_ch04.xhtml]），分类算法（本章讨论），以及聚类算法（例如 k-means，本书未讨论）。

与激活函数相关的部分确实需要了解神经网络中的隐藏层的基本知识。根据您的经验水平，您在阅读这一部分之前可能需要阅读一些预备材料（网上有很多文章）。

什么是分类？

给定一个包含已知类别成员的观察值的集合，分类的任务是确定新数据点所属的类别。类别指的是类别，也称为“目标”或“标签”。例如，电子邮件服务提供商中的垃圾邮件检测涉及二元分类（只有两个类别）。MNIST 数据集包含一系列图像，其中每个图像都是一个单独的数字，这意味着有十个标签。分类的一些应用包括信用批准、医疗诊断和目标营销。

什么是分类器？

在上一章中，您了解到线性回归结合数值数据使用监督学习。目标是训练一个可以做出数值预测的模型（例如，明天的股票价格，系统的温度或其气压）。相比之下，分类器结合非数值类别的数据使用监督学习：目标是训练一个可以做出分类预测的模型。

例如，假设数据集的每一行都是一种特定的葡萄酒，每一列都涉及特定的葡萄酒特征（单宁、酸度等）。进一步假设数据集中有五种葡萄酒类别：为了简单起见，让我们将它们标记为 A、B、C、D 和 E。给定一个新的数据点，也就是说，新的数据行，这个数据集的分类器试图确定这种葡萄酒的标签。

本章中的一些分类器可以执行分类分类，并且还可以进行数值预测（即它们可以用于回归以及分类）。

常见分类器

这里列出了机器学习中一些最受欢迎的分类器（不分先后）：

+   线性分类器

+   kNN

+   逻辑回归

+   决策树

+   随机森林

+   SVMs

+   贝叶斯分类器

+   CNNs（深度学习）

不同的分类器有不同的优缺点，这通常涉及到复杂性和准确性之间的权衡，类似于人工智能领域之外的领域的算法。

在深度学习的情况下，卷积神经网络（CNN）执行图像分类，这使得它们成为分类器（它们也可以用于音频和文本处理）。

以下部分提供了之前列表中列出的机器学习分类器的简要描述。

二分类与多分类分类

二分类器与具有两个类别的数据集一起工作，而多分类器（有时称为多项式分类器）区分超过两个类别。随机森林分类器和朴素贝叶斯分类器支持多个类别，而 SVM 和线性分类器只能用作二分类器。

此外，还有基于二分类器的多类分类技术：一对多（OvA）和一对一（OvO）。

OvA 技术也称为“一对多”，涉及与类别数量相等的多个二分类器。例如，如果一个数据集有五个类别，那么 OvA 使用五个二分类器，每个二分类器检测五个类别中的一个。为了在这个特定数据集中对数据点进行分类，选择输出最高分数的二分类器。

OvO 技术也涉及多个二分类器，但在此情况下，使用一个二分类器来训练一对类别。例如，如果类别是 A、B、C、D 和 E，则需要十个二分类器：一个用于 A 和 B，一个用于 A 和 C，一个用于 A 和 D，以此类推，直到最后一个用于 D 和 E 的二分类器。

通常，如果有 n 个类别，则需要 n*(n-1)/2 个二分类器。尽管 OvO 技术比 OvA 技术需要更多的二分类器（例如，对于 20 个类别需要 190 个），但 OvO 技术的优势在于每个二分类器只在其所选的两个类别的数据集部分上训练。

多标签分类

多标签分类涉及将多个标签分配给数据集中的实例。因此，多标签分类是多类分类（在上一节中讨论）的推广，后者涉及将单个标签分配给属于具有多个类别的数据集的实例。一篇包含基于 Keras 的代码的多标签分类文章可在网上找到：

[`medium.com/@vijayabhaskar96/multi-label-image-classification-tutorial-with-keras-imagedatagenerator-cd541f8eaf24`](https://medium.com/@vijayabhaskar96/multi-label-image-classification-tutorial-with-keras-imagedatagenerator-cd541f8eaf24)

您还可以在线搜索涉及 SKLearn 或 PyTorch 的多标签分类任务的文章。

什么是线性分类器？

线性分类器将数据集分为两个类别。对于二维点，线性分类器是一条线，对于三维点，是一个平面，对于更高维度的点，是一个超平面（平面的推广）。

线性分类器通常是速度最快的分类器，因此在分类速度非常重要时经常被使用。当输入向量稀疏（即大部分为零值）或维度数量很大时，线性分类器通常表现良好。

什么是 KNN？

kNN（k-最近邻）算法是一种分类算法。简而言之，彼此“靠近”的数据点被分类为属于同一类别。当引入一个新的点时，它被添加到其最近邻多数所属的类别中。例如，假设 k 等于 3，并引入一个新的数据点。查看其 3 个最近邻的类别：假设它们是 A，A 和 B。然后通过多数投票，新的数据点被标记为类别 A 的数据点。

kNN 算法本质上是一种启发式方法，而不是具有复杂数学基础的技巧，尽管如此，它仍然是一个有效且有用的算法。

如果你想使用一个简单的算法，或者当你认为你的数据集性质高度无结构时，请尝试 kNN 算法。尽管 kNN 算法非常简单，但它可以产生高度非线性的决策。你可以在搜索应用中使用 kNN 来寻找“相似”的项目。

通过创建项目的向量表示来衡量相似性，然后使用适当的距离度量（如欧几里得距离）比较向量。

kNN 搜索的一些具体例子包括搜索语义上相似的文档。

如何处理 kNN 中的平局

当 k 的值是奇数时，不太可能导致平局投票，但这并非不可能。例如，假设 k 等于 7，当引入一个新的数据点时，它的 7 个最近邻属于集合{A,B,A,B,A,B,C}。正如你所看到的，没有多数投票，因为类别 A 中有 3 个点，类别 B 中有 3 个点，类别 C 中有 1 个点。

有几种处理 kNN 中平局的技术，如下所示：

+   给较近的点分配更高的权重。

+   增加 k 的值，直到确定赢家。

+   减小 k 的值，直到确定赢家。

+   随机选择一个类别。

如果你将 k 减小到 1，仍然可能存在平局投票：可能有两个点与新的点距离相等，因此你需要一种机制来决定选择这两个点中的哪一个作为 1-邻居。

如果类别 A 和类别 B 之间存在平局，则随机选择类别 A 或类别 B。另一种变体是跟踪“平局”投票，并轮流确保更均匀的分布。

什么是决策树？

决策树是另一种涉及树形结构的分类算法。在“通用”树中，数据点的放置由简单的条件逻辑决定。作为一个简单的说明，假设一个数据集包含一组代表人们年龄的数字，并且假设第一个数字是 50。这个数字被选为树的根，所有小于 50 的数字都添加到树的左分支，而所有大于 50 的数字都添加到树的右分支。

例如，假设我们有一个数字序列如下：{50, 25, 70, 40}。然后我们可以构建如下所示的树：50 是根节点；25 是 50 的左子节点；70 是 50 的右子节点；40 是 20 的右子节点。我们将添加到这个数据集的每个附加数值都经过处理，以确定在树的每个节点处应向哪个方向前进（“左或右”）。

列表 3.1 显示了 sklearn_tree2.py 的内容，它定义了欧几里得平面上的二维点集及其标签，然后预测了欧几里得平面上的其他几个二维点的标签。

列表 3.1: sklearn_tree2.py

from sklearn import tree

# X = 2D 点的对和 Y =每个点的类别

X = [[0, 0], [1, 1], [2,2]]

Y = [0, 1, 1]

tree_clf = tree.DecisionTreeClassifier()

tree_clf = tree_clf.fit(X, Y)

#预测样本的类别：

print("预测[-1., -1.]:")

print(tree_clf.predict([[-1., -1.]]))

print("预测类别[2., 2.]:")

print(tree_clf.predict([[2., 2.]]))

# 训练样本中相同类别的百分比

# 在叶节点上的值等于每个类别的概率

print("预测[2.,2.]中每个类别的概率：")

print(tree_clf.predict_proba([[2., 2.]]))

列表 3.1 导入了 sklearn 中的树类，然后使用数据值初始化了数组 X 和 y。接下来，变量 tree_clf 被初始化为 DecisionTreeClassifier 类的实例，然后通过调用 fit()方法使用 X 和 y 的值对其进行训练。

现在在列表 3.1 中运行代码，你将看到以下输出：

预测类别[-1., -1.]：

[0]

预测类别[2., 2.]：

[1]

预测[2.,2.]中每个类别的概率：

[[0. 1.]]

如你所见，点[-1,-1]和[2,2]被正确地标记为值 0 和 1，分别。

列表 3.2 显示了 sklearn_tree3.py 的内容，它通过添加第三个标签并预测欧几里得平面上的三个点的标签来扩展列表 3.1 中的代码（修改以粗体显示）。

列表 3.2: sklearn_tree3.py

from sklearn import tree

# X = 2D 点的对和 Y =每个点的类别

X = [[0, 0], [1, 1], [2,2]]

Y = [0, 1, 2]

tree_clf = tree.DecisionTreeClassifier()

tree_clf = tree_clf.fit(X, Y)

#预测样本的类别：

print("预测[-1., -1.]:")

打印(tree_clf.predict([[-1., -1.]]))

打印("predict class of [0.8, 0.8]:")

打印(tree_clf.predict([[0.8, 0.8]]))

打印("predict class of [2., 2.]:")

打印(tree_clf.predict([[2., 2.]]))

# 相同类别的训练样本百分比

# 在一个叶子节点中的值等于每个类别的概率

打印("probability of each class in [2.,2.]:")

打印(tree_clf.predict_proba([[2., 2.]]))

现在运行列表 3.2 中的代码，你将看到以下输出：

predict class of [-1., -1.]:

[0]

predict class of [0.8, 0.8]:

[1]

predict class of [2., 2.]:

[2]

在[2.,2.]中的每个类别的概率

[[0.0 0.0 1.0]]

正如你所见，点[-1,-1]，[0.8, 0.8]，和[2,2]分别被正确标记为值 0，1，和 2。

列表 3.3 显示了数据集 partial_wine.csv 的一部分，其中包含两个特征列和一个标签列（有三个类别）。该数据集的总行数为 178。

列表 3.3: partial_wine.csv

酒精，苹果酸，类别

14.23,1.71,1

13.2,1.78,1

13.16,2.36,1

14.37,1.95,1

13.24,2.59,1

14.2,1.76,1

列表 3.4 显示了使用决策树在数据集 partial_wine.csv 上训练模型的 tree_classifier.py 的内容。

列表 3.4: tree_classifier.py

导入 numpy 库作为 np

导入 matplotlib.pyplot 作为 plt

导入 pandas 库作为 pd

# 导入数据集

dataset = pd.read_csv('partial_wine.csv')

X = dataset.iloc[:, [0, 1]].values

y = dataset.iloc[:, 2].values

# 将数据集分割为训练集和测试集

从 sklearn.model_selection 导入 train_test_split

X_train, X_test, y_train, y_test = train_test_split(X, y, test_size = 0.25, random_state = 0)

# 特征缩放

从 sklearn.preprocessing 导入 StandardScaler

sc = StandardScaler()

X_train = sc.fit_transform(X_train)

X_test = sc.transform(X_test)

# ====> 在此处插入您的分类器代码 <====

从 sklearn.tree 导入 DecisionTreeClassifier

classifier = DecisionTreeClassifier(criterion='entropy',rand om_state=0)

classifier.fit(X_train, y_train)

# ====> 在此处插入您的分类器代码 <====

# 预测测试集结果

y_pred = classifier.predict(X_test)

# 生成混淆矩阵

从 sklearn.metrics 导入 confusion_matrix

cm = confusion_matrix(y_test, y_pred)

打印("confusion matrix:")

打印(cm)

列表 3.4 包含一些导入语句，然后使用 CSV 文件 partial_wine.csv 的内容填充 Pandas 数据框 dataset。接下来，变量 X 被初始化为数据集的前两列（以及所有行），变量 y 被初始化为数据集的第三列（以及所有行）。

接下来，变量 X_train，X_test，y_train 和 y_test 使用 75/25 的比例分割从 X 和 y 中填充数据。注意变量 sc（StandardScaler 类的实例）对 X_train 和 X_test 变量执行缩放操作。

在列表 3.4 中用粗体显示的代码块是我们创建决策树分类器类的实例，然后使用变量 X_train 和 X_test 中的数据训练该实例。

列表 3.4 的下一部分将变量 y_pred 填充为从 X_test 变量中的数据生成的预测集。列表 3.4 的最后一部分基于 y_test 中的数据和 y_pred 中的预测数据创建一个混淆矩阵。

记住，混淆矩阵的所有对角线元素都是正确预测（例如真正例和真负例）；所有其他单元格包含一个数值，指定了错误预测的数量（例如假正例和假负例）。

现在运行列表 3.4 中的代码，你将看到以下混淆矩阵的输出，其中包含 36 个正确预测和 9 个错误预测（准确率为 80%）：

混淆矩阵：

[[13  1  2]]

[[ 0 17 4]]

[[ 1  1  6]]

from sklearn.metrics import confusion_matrix

在前面的 3x3 矩阵中总共有 45 个条目，对角线条目是正确识别的标签。因此，准确率为 36/45 = 0.80。

什么是随机森林？

随机森林是决策树的推广：这个分类算法涉及多个树（数量由你指定）。如果数据涉及进行数值预测，则计算树的预测平均值。如果数据涉及进行分类预测，则确定树的预测众数。

通过类比，随机森林以类似于金融投资组合多元化的方式运行：目标是平衡损失与更高的收益。随机森林使用“多数投票”进行预测，这基于这样的假设，即选择多数投票比单个树中的任何单个预测更有可能正确（并且更常见）。

你可以轻松修改列表 3.4 中的代码以使用随机森林，只需将显示的粗体两行代码替换为以下代码：

from sklearn.ensemble import RandomForestClassifier

classifier = RandomForestClassifier(n_estimators = 10, criterion='entropy', random_state = 0)

进行此代码更改，运行代码，并检查混淆矩阵以比较其准确率与列表 3.4 中决策树的准确率。

什么是支持向量机？

支持向量机涉及一个监督机器学习算法，可用于分类或回归问题。SVMs 可以处理非线性可分数据以及线性可分数据。SVMs 使用一种称为“核技巧”的技术来转换数据，然后找到最优边界。这种转换涉及更高的维度。这种技术导致转换后的数据分离，之后可以找到一个超平面将数据分为两类。

SVMs 在分类任务中比回归任务更常见。SVMs 的一些用例包括以下：

+   文本分类任务：类别分配

+   检测垃圾邮件/情感分析

+   用于图像识别：基于方面的识别基于颜色的分类

+   手写数字识别（邮政自动化）

SVMs 的权衡

尽管 SVMs 非常强大，但其中涉及权衡。SVMs 的一些优点如下：

+   高精度

+   在较小的更干净的数据集上表现良好

+   可以更高效，因为它使用训练点的子集

+   在数据集有限的情况下是 CNN 的替代品

+   捕获数据点之间更复杂的关系

尽管 SVMs 非常强大，但它们也有一些缺点，如下列所示：

+   不适合较大的数据集：训练时间可能很高

+   在噪声较大的具有重叠类别的数据集上效果较差

SVMs 涉及的参数比决策树和随机森林更多

一个可以考虑的建议是修改 列表 3.4 以使用 SVM，通过将以下粗体显示的两行替换为以下粗体显示的两行：

from sklearn.svm import SVC

classifier = SVC(kernel = 'linear', random_state = 0)

你现在有一个基于 SVM 的模型，只需通过更新之前的代码即可。修改代码，然后启动代码，检查混淆矩阵以比较其准确性与本章早期提到的决策树模型和随机森林模型的准确性。

什么是贝叶斯推断？

贝叶斯推断是统计学中的一个重要技术，它涉及统计推断和贝叶斯定理，随着更多信息的可用性来更新假设的概率。贝叶斯推断通常被称为“贝叶斯概率”，它在序列数据的动态分析中非常重要。

贝叶斯定理

给定两个集合 A 和 B，让我们定义以下数值（它们都在 0 和 1 之间）：

P(A) = 在集合 A 中存在的概率

P(B) = 在集合 B 中存在的概率

P(Both) = A 和 B 交集存在的概率

P(A|B) = 在 B 中存在的概率（假设你在 B 中）

P(B|A) = 在 A 中存在的概率（假设你在 A 中）

然后，以下公式也是正确的：

P(A|B) = P(Both)/P(B) (#1)

P(B|A) = P(Both)/P(A) (#2)

将前述方程对乘以分母中出现的项，我们得到这些方程：

P(B)*P(A|B) = P(Both) (#3)

P(A)*P(B|A) = P(Both) (#4)

现在，将方程 #3 和 #4 的左侧设置为相等，这就给出了这个方程：

P(B)*P(A|B) = P(A)*P(B|A) (#5)

将方程 #5 的两边除以 P(B)，我们得到这个著名的方程：

P(A|B) = P(A)*P(A|B)/P(B) (#6)

一些贝叶斯术语

在上一节中，我们推导出以下关系：

P(h|d) = (P(d|h) * P(h)) / P(d)

前述方程中的四个项都有名称，如下所述。

首先，后验概率是 P(h|d)，即给定数据 d 的假设 h 的概率。

其次，P(d|h)是在假设 h 为真的条件下数据 d 的概率。

第三，h 的先验概率是 P(h)，这是假设 h 为真的概率（无论数据如何）。

最后，P(d)是数据的概率（无论假设如何）

我们对计算后验概率 P(h|d)从先验概率 p(h)以及 P(D)和 P(d|h)感兴趣。

什么是 MAP？

最大后验（MAP）假设是概率最高的假设，即最可能的假设。这可以写成以下形式：

MAP(h) = max(P(h|d))

或者：

MAP(h) = max((P(d|h) * P(h)) / P(d))

或者：

MAP(h) = max(P(d|h) * P(h))

为什么使用贝叶斯定理？

贝叶斯定理描述了基于与事件可能相关条件先验知识的事件概率。如果我们知道条件概率，我们可以使用贝叶斯规则来找出反向概率。前面的陈述是贝叶斯规则的一般表示。

什么是贝叶斯分类器？

朴素贝叶斯分类器是一种受贝叶斯定理启发的概率分类器。朴素贝叶斯分类器假设属性是条件独立的，即使假设不成立，它也能很好地工作。这种假设大大降低了计算成本，并且实现简单，只需要线性时间。此外，朴素贝叶斯分类器可以轻松扩展到更大的数据集，并且在大多数情况下都能获得良好的结果。朴素贝叶斯分类器的其他优点包括以下内容：

+   可以用于二进制和多类分类

+   提供不同类型的朴素贝叶斯（NB）算法

+   是文本分类问题的良好选择

+   是垃圾邮件分类的流行选择

+   可以轻松地在小数据集上训练

如您所料，朴素贝叶斯分类器确实有一些缺点，如下所示：

+   假设所有特征都是无关的。

+   它无法学习特征之间的关系。

+   它可能受到“零概率问题”的影响。

零概率问题是指当属性的条件下概率为零时的情况，它无法给出有效的预测。然而，可以使用拉普拉斯估计器明确地修复这个问题。

朴素贝叶斯分类器的类型

有三种主要的 NB 分类器：

+   高斯朴素贝叶斯

+   多项式朴素贝叶斯（多项式 NB）

+   伯努利朴素贝叶斯

这些分类器的详细信息超出了本章的范围，但你可以进行在线搜索以获取更多信息。

训练分类器

培训分类器的一些常见技术如下：

+   保留法

+   k-fold 交叉验证

保留法是最常见的方法，它首先将数据集分为两个部分，称为训练集和测试集（分别为 80%和 20%）。训练集用于训练模型，测试数据用于测试其预测能力。

使用 k 折交叉验证技术来验证模型是否过拟合。数据集被随机划分为 k 个互斥的子集，其中每个子集的大小相等。一个子集用于测试，其他子集用于训练。在整个 k 个折中迭代。

评估分类器

无论何时选择一个分类器用于数据集，显然重要的是要评估该分类器的准确性。这里列出了评估分类器的常见技术：

+   精确率和召回率

+   ROC 曲线（接收者操作特征）

精确率和召回率在第二章中讨论，并在此处重现以方便您查阅。让我们定义以下变量：

TP = 真阳性结果的数量

FP = 假阳性结果的数量

TN = 真阴性结果的数量

FN = 假阴性结果的数量

然后给出精确率、准确率和召回率的定义，如下公式所示：

精确率 = TP / (TN + FP)

准确率 = (TP + TN) / [TP + FP + FN + TN]

召回率 = TP / [TP + FN]

ROC 曲线用于可视比较分类模型，显示了真正阳性率和假阳性率之间的权衡。ROC 曲线下的面积是模型准确性的度量。当模型接近对角线时，其准确性较低，完美准确性的模型将具有面积为 1.0。

ROC 曲线绘制了真正阳性率与假阳性率的对比。另一种类型的曲线是 PR 曲线，它绘制了精确率与召回率的对比。当处理高度倾斜的数据集（强类别不平衡）时，精确率-召回率（PR）曲线给出更好的结果。

这部分章节关于统计术语和测量数据集有效性的技术到此结束。现在让我们看看机器学习中的激活函数，这是下一节的主题。

激活函数是什么？

激活函数（通常）是一个非线性函数，它将非线性引入神经网络，从而防止神经网络中隐藏层的“巩固”。具体来说，假设神经网络中相邻的每一对层仅涉及矩阵变换而没有激活函数。这样的网络是一个线性系统，这意味着其层可以被合并成一个更小的系统。

首先，连接输入层和第一隐藏层的边权重可以用一个矩阵表示：让我们称它为 W1。接下来，连接第一隐藏层和第二隐藏层的边权重也可以用一个矩阵表示：让我们称它为 W2。重复此过程，直到我们达到连接最终隐藏层和输出层的边：让我们称这个矩阵为 Wk。由于我们没有激活函数，我们可以简单地乘以矩阵 W1, W2, …, Wk，并产生一个矩阵：让我们称它为 W。我们现在已经用包含一个输入层、一个权重矩阵 W 和一个输出层的等效神经网络替换了原始神经网络。换句话说，我们不再有原来的多层神经网络了！

幸运的是，当我们指定每对相邻层之间的激活函数时，我们可以防止上述情况发生。换句话说，每层的激活函数防止了这种“矩阵合并”。因此，我们可以在训练神经网络的整个过程中保持所有中间隐藏层。

为了简单起见，让我们假设每对相邻层之间都有相同的激活函数（我们很快会去掉这个假设）。在神经网络中使用激活函数的过程涉及几个步骤，如下所述：

1. 从一个数字的输入向量 x1 开始。

2. 将 x1 乘以权重矩阵 W1，它表示连接输入层和第一隐藏层的边。结果是新的向量 x2。

3. “应用”激活函数到 x2 的每个元素，以创建另一个向量 x3。

现在重复步骤 2 和 3，只是我们使用“起始”向量 x3 和权重矩阵 W2 来表示连接第一隐藏层和第二隐藏层的边（如果只有一个隐藏层，则直接使用输出层）。

在完成前面的过程后，我们已经“保留”了神经网络，这意味着它可以在数据集上训练。你可以在每个步骤中使用不同的激活函数来替换每个激活函数（选择权在你）。

我们为什么需要激活函数？

前一节概述了将输入向量从输入层转换，然后通过隐藏层直到达到输出层的过程。激活函数在神经网络中的重要性至关重要，因此在这里重复一遍：激活函数“保持”神经网络的结构，防止它们被简化为输入层和输出层。换句话说，如果我们指定每对连续层之间的非线性激活函数，那么神经网络不能被替换为包含较少层的神经网络。

没有非线性激活函数，我们只需将给定连续层的权重矩阵与从前一连续层产生的输出向量相乘。我们重复这个简单的乘法，直到达到神经网络的输出层。达到输出层后，我们实际上用单个“连接”输入层和输出层的矩阵替换了多个矩阵。

激活函数是如何工作的？

如果这是你第一次遇到激活函数的概念，可能会感到困惑，所以这里有一个可能有助于理解的类比。假设你在深夜开车，高速公路上没有其他人。你可以以恒定的速度行驶，直到没有障碍物（如停车标志和交通灯）。然而，假设你驶入一个大超市的停车场。当你接近减速带时，你必须减速，越过减速带，然后再次加速，并且为每个减速带重复这个过程。

将神经网络中的非线性激活函数想象成减速带的对应物：你无法保持恒定的速度，这（通过类比）意味着你不能首先将所有权重矩阵相乘并将它们“折叠”成一个单一的权重矩阵。另一个类比涉及一个有多个收费站的道路：你必须减速，支付通行费，然后继续驾驶，直到你到达下一个收费站。这些只是不完美的类比，帮助你理解非线性激活函数的需要。

常见激活函数

虽然有许多激活函数（如果你知道如何定义，你也可以定义自己的），以下是一个常见激活函数列表，后面跟着简要描述：

+   sigmoid

+   tanh

+   ReLU

+   ReLU6

+   ELU

+   SELU

sigmoid 激活函数基于欧拉常数 e，其值域在 0 和 1 之间，其公式如下所示：

1/[1+e^(-x)]

tanh 激活函数也基于欧拉常数 e，其公式如下所示：

[e^x – e^(-x)]/[e^x+e^(-x)]

记住前面公式的办法之一是注意分子和分母有相同的成对项：它们在分子中由一个“-”符号分隔，在分母中由一个“+”符号分隔。tanh 函数的值域在-1 和 1 之间。

ReLU（线性整流单元）激活函数很简单：如果 x 是负数，那么 ReLU(x)是 0；对于 x 的所有其他值，ReLU(x)等于 x。ReLU6 是 TensorFlow 特有的，它是 ReLU(x)的变体：额外的约束是当 x >= 6 时，ReLU(x)等于 6（因此得名）。

ELU 是一种指数线性单元，它是 ReLU 的指数“外壳”，用可对所有 x 值（包括 x = 0）可微分的指数激活函数替换 ReLU 的两个线性段。

SELU 是 Scaled Exponential Linear Unit 的缩写，它比其他激活函数稍微复杂一些（并且使用频率较低）。要详细了解这些和其他激活函数（以及描述其形状的图表），请访问以下维基百科网页：

[激活函数](https://en.wikipedia.org/wiki/Activation_function)

前面的链接提供了一个包含许多激活函数及其导数的长列表。

Python 中的激活函数

列表 3.5 显示了包含各种激活函数公式的文件 activations.py 的内容。

列表 3.5：activations.py

import numpy as np

# Python sigmoid 示例：

z = 1/(1 + np.exp(-np.dot(W, x)))

# Python tanh 示例：

z = np.tanh(np.dot(W,x))

# Python ReLU 示例：

z = np.maximum(0, np.dot(W, x))

列表 3.5 包含使用 NumPy 方法定义 sigmoid 函数、tanh 函数和 ReLU 函数的 Python 代码。请注意，您需要指定 x 和 W 的值才能在列表 3.5 中运行代码。

THE RELU AND ELU ACTIVATION FUNCTIONS

目前 ReLU 通常被“首选”作为激活函数；之前，首选的激活函数是 tanh（在 tanh 之前是 sigmoid）。ReLU 由两条线段组成（一条斜率为零，另一条斜率为 1），在二维欧几里得平面的原点相交，并且提供了最佳的训练准确率和验证准确率。

ReLU 就像线性性的开关：不需要时它是“关闭”的，当它激活时其导数是 1，这使得 ReLU 成为所有当前激活函数中最简单的。注意，函数的二阶导数在所有地方都是 0：它是一个非常简单的函数，简化了优化。此外，梯度对于大值也是恒定的，它永远不会“饱和”（即，它不会在正水平轴上缩小到零）。

矩形线性单元及其推广版本基于线性模型更容易优化的原则。ReLU 激活函数或其相关替代方案（稍后讨论）在许多情况下是推荐的激活函数。

ReLU 的优缺点

以下列表包含了 ReLU 激活函数的优点：

+   在正区域不会饱和

+   在计算效率方面非常高效

+   使用 ReLU 的模型通常比使用其他激活函数的模型收敛得更快

然而，当 ReLU 神经元的激活值变为 0 时，ReLU 确实有一个缺点：那么在反向传播过程中，该神经元的梯度也将是 0。你可以通过谨慎地分配初始权重和学习率来减轻这种情况。

ELU

指数线性单元（ELU）基于 ReLU：主要区别在于 ELU 在原点处是可微的（ReLU 是一个连续函数，但在原点处不可微）。然而，请注意以下几点。首先，ELU 以“不朽”（对“死亡”的免疫力）为代价换取计算效率。阅读以下论文以获取更多详细信息：[arxiv.org/abs/1511.07289](http://arxiv.org/abs/1511.07289)。其次，ReLU 仍然很受欢迎，并且比 ELU 更受欢迎，因为使用 ELU 会引入一个额外的新的超参数。

SIGMOID、SOFTMAX 和 HARDMAX 的相似性

sigmoid 激活函数的范围在 (0,1) 之间，它会饱和并“杀死”梯度。与 tanh 激活函数不同，sigmoid 的输出不是零中心的。此外，sigmoid 和 softmax 都不鼓励用于传统的前馈实现。然而，sigmoid 激活函数仍然用于 LSTM（特别是遗忘门、输入门和输出门）、GRU（门控循环单元）和概率模型。此外，一些自动编码器有额外的要求，这阻止了使用分段线性激活函数的使用。

Softmax

Softmax 激活函数将数据集中的值映射到另一组介于 0 和 1 之间的值，且这些值的总和等于 1。因此，softmax 创建了一个概率分布。在卷积神经网络（CNN）进行图像分类的情况下，softmax 激活函数“映射”最终隐藏层中的值到输出层的 10 个神经元。包含最大概率的位置索引与输入图像的一热编码中数字 1 的索引相匹配。如果索引值相等，则表示图像已被分类，否则被认为是错配。

Softplus

Softplus 激活函数是对 ReLU 激活函数的平滑（即可微）近似。回想一下，ReLU 函数的唯一不可微点是原点，它通过 softmax 激活函数被“平滑”，其方程如下：

f(x) = ln(1 + e^x)

Tanh

tanh 激活函数的范围在 (-1,1) 之间，而 sigmoid 函数的范围在 (0,1) 之间。这两个激活函数都会饱和，但与 sigmoid 神经元不同，tanh 的输出是零中心的。因此，在实践中，tanh 非线性总是比 sigmoid 非线性更受欢迎。

Sigmoid 和 tanh 激活函数在 LSTM（sigmoid 用于三个门，tanh 用于内部细胞状态）以及 GRU（门控循环单元）的计算中都会出现，涉及输入门、遗忘门和输出门。

SIGMOID、SOFTMAX 和 HARDMAX 的区别

本节简要讨论了这三个函数之间的一些区别。首先，sigmoid 函数在逻辑回归模型中用于二元分类，以及 LSTMs 和 GRUs 中的门控。在构建神经网络时，sigmoid 函数用作激活函数，但请注意，概率之和不一定等于 1。

第二，softmax 函数是 sigmoid 函数的推广：它在逻辑回归模型中用于多分类。softmax 函数是 CNN 中“全连接层”的激活函数，这是最右侧的隐藏层和输出层。与 sigmoid 函数不同，概率之和必须等于 1。你可以使用 sigmoid 函数或 softmax 函数进行二元（n=2）分类。

第三，hardmax 函数将 0 或 1 分配给输出值（类似于阶跃函数）。例如，假设我们有三个类别 {c1, c2, c3}，其分数分别为 [1, 7, 2]。hardmax 概率是 [0, 1, 0]，而 softmax 概率是 [0.1, 0.7, 0.2]。请注意，hardmax 概率的和为 1，softmax 概率的和也是如此。然而，hardmax 概率是全有或全无的，而 softmax 概率类似于获得“部分分数”。

什么是逻辑回归？

尽管名为逻辑回归，但它实际上是一个具有二元输出的分类器和线性模型。逻辑回归与多个自变量一起工作，并涉及 sigmoid 函数来计算概率。逻辑回归本质上是将 sigmoid 激活函数应用于线性回归以执行二元分类的结果。

逻辑回归在众多无关领域都有用途。这些领域包括机器学习、各种医学领域和社会科学。逻辑回归可以根据患者的各种观察特征来预测某种疾病的发病风险。使用逻辑回归的其他领域包括工程、营销和经济学。

逻辑回归可以是二项式（因变量的结果只有两种），多项式（因变量的结果有三个或更多），或有序（因变量是有序的）。例如，假设一个数据集包含属于类别 A 或类别 B 的数据。如果你得到一个新的数据点，逻辑回归会预测该新数据点属于类别 A 还是类别 B。相比之下，线性回归预测一个数值，例如股票的次日价值。

设置阈值值

阈值值是一个数值，用于确定哪些数据点属于类别 A，哪些点属于类别 B。例如，及格/不及格的阈值可能是 0.70。在加利福尼亚州通过书面驾驶考试及格的阈值是 0.85。

作为另一个例子，假设 p = 0.5 是“截止”概率。那么我们可以将概率大于 0.5 的数据点分配给类别 A，将概率小于等于 0.5 的数据点分配给类别 B。由于只有两个类别，我们确实有一个分类器。

一个类似的场景涉及抛掷一枚平衡良好的硬币。我们知道抛出正面的概率是 50%（让我们将这个结果标记为“类别 A”），抛出反面的概率也是 50%（让我们将这个结果标记为“类别 B”）。如果我们有一个包含标记结果的数据库，那么我们期望大约 50%的结果属于类别 A 和类别 B。

然而，我们无法提前确定有多少比例的人会通过书面驾驶考试，或者有多少比例的人会通过他们的课程。包含这些类型场景结果的数据库需要训练，逻辑回归可以是一个合适的技巧来完成这项工作。

逻辑回归：重要假设

逻辑回归要求观测值彼此独立。此外，逻辑回归要求独立变量之间几乎没有多重共线性。逻辑回归处理数值、分类和连续变量，并假设独立变量和对数几率的线性，这在此处定义：

赔率 = p/(1-p) 和 logit = log(赔率)

这种分析不需要依赖变量和独立变量之间必须是线性相关的；然而，另一个要求是独立变量与对数几率线性相关。

逻辑回归用于在存在多个解释变量的情况下获得赔率比。该过程与多元线性回归非常相似，唯一的区别是响应变量是二元的。结果是每个变量对观察到的感兴趣事件的赔率比的影响。

线性可分数据

线性可分数据是可以被一条线（在 2D 中）、一个平面（在 3D 中）或超平面（在更高维度中）分离的数据。线性不可分数据是不能被一条线或超平面分离的数据（簇）。例如，XOR 函数涉及无法用线分离的数据点。如果你为具有两个输入的 XOR 函数创建一个真值表，点(0,0)和(1,1)属于类别 0，而点(0,1)和(1,0)属于类别 1（在 2D 平面上绘制这些点以说服自己）。解决方案涉及在更高维度中转换数据，使其成为线性可分，这是 SVMs 中使用的技巧。

摘要

本章从分类和分类器的解释开始，然后简要介绍了机器学习中常用的分类器。

然后我们讨论了激活函数，如果你决定学习深度神经网络，这将非常有用。你还收到了关于激活函数的高级介绍，包括 sigmoid、tanh、ReLU、ReLU6、ELU 和 SELU。

接下来，你学习了逻辑回归，它依赖于 sigmoid 函数，以及逻辑回归的潜在假设。最后，你看到了一个涉及逻辑回归和 MNIST 数据集的代码示例。

第四章

CHATGPT 和 GPT-4

本章包含有关 ChatGPT 和 GPT-4 的主要功能以及一些竞争对手的信息。

本章的第一部分从 ChatGPT 关于生成式 AI 和对话式 AI 与生成式 AI 本质的信息开始。根据 ChatGPT 的说法，ChatGPT 本身、GPT-4 和 DALL-E 确实包含在生成式 AI 中。本节还讨论了 ChatGPT 的一些功能和 ChatGPT 的替代方案。

本章的第三部分讨论了 GPT-4 的一些特性，这些特性为 ChatGPT 提供了动力。你将了解 GPT-4 的一些竞争对手，如 Llama 2（Meta）和 Bard（更名为 Google Gemini）。

什么是生成式 AI？

生成式 AI 是指人工智能模型和技术的子集，旨在生成与给定输入数据在本质上相似的新数据样本。目标是生成原本不属于原始训练集但连贯、上下文相关、风格或结构相同的内容或数据。

与仅仅分析或分类相比，生成式 AI 的独特之处在于其创造和创新的能力。该领域的进步导致了创意领域和实际应用的突破，使其成为人工智能研究和开发的前沿领域。

生成式 AI 的重要特性

以下列表包含生成式 AI 的关键特性，每个条目后面都有简要描述：

+   数据生成

+   综合技术

+   学习分布

数据生成指的是创建新的数据点的能力，这些数据点不是训练数据的一部分，但与它们相似。这可能包括文本、图像、音乐、视频或任何其他形式的数据。

综合意味着生成模型可以混合各种输入以生成包含每个输入特征的输出，例如合并两张图片的风格。

学习分布意味着生成式 AI 模型旨在学习训练数据的概率分布，以便它们可以从该分布中生成新的样本。

生成式 AI 的流行技术

生成对抗网络（GANs）：GANs 由两个网络组成，一个生成器和一个判别器，它们同时训练。生成器试图生成假数据，而判别器试图区分真实数据和假数据。随着时间的推移，生成器在生成逼真数据方面变得越来越好。

变分自编码器（VAEs）：VAEs 是概率模型，它们学习以编码和解码数据的方式，使得编码表示可以用来生成新的数据样本。

循环神经网络（RNNs）：主要用于序列生成，如文本或音乐。

生成 AI 的独特之处

创建与分类：虽然大多数传统 AI 模型旨在将输入数据分类到预定义的类别中，但生成模型旨在创建新的数据。

无监督学习：许多生成模型，尤其是 GAN 和 VAE，以无监督的方式运行，这意味着它们在训练时不需要标记数据。

多样化的输出：生成模型可以根据学习到的分布产生各种输出，这使得它们非常适合艺术生成、风格迁移等任务。

挑战：生成 AI 提出了独特的挑战，如 GAN 中的模式崩溃或确保生成内容的连贯性。

有许多领域涉及生成 AI 的应用，其中一些如下列出：

+   艺术与音乐创作

+   数据增强

+   风格迁移

+   文本生成

+   图像合成

+   药物发现

艺术与音乐创作包括生成绘画、音乐或其他形式的艺术。

数据增强涉及为训练模型创建额外的数据，尤其是在原始数据集有限时。

风格迁移是指将一个图像的风格应用到另一个图像的内容上。

文本生成是生成 AI 一个非常流行的应用，涉及创建连贯且与上下文相关的文本。

图像合成是生成 AI 另一个非常流行的领域，涉及生成逼真的图像、面部，甚至为视频游戏创建场景。

药物发现是生成 AI 的一个重要方面，涉及为新潜在药物生成分子结构。

对话式 AI 与生成 AI 的比较

对话式 AI 和生成 AI 都是人工智能更广泛领域中的突出子领域。然而，这些子领域在它们的主要目标、使用的科技以及应用方面有不同的重点。

[`medium.com/@social_65128/differences-between-conversational-ai-and-generative-ai-e3adca2a8e9a`](https://medium.com/@social_65128/differences-between-conversational-ai-and-generative-ai-e3adca2a8e9a)

两个子领域之间的主要区别如下：

+   主要目标

+   应用

+   使用的科技

+   训练与交互

+   评估

+   数据需求

主要目标

对话式 AI 的主要目标是促进机器与人类之间类似人类的交互。这包括聊天机器人、虚拟助手以及其他与用户进行对话的系统。

生成式 AI 的主要目标是创建新的内容或数据，这些内容或数据不在训练集中，但在结构和风格上相似。这可以包括生成图像、音乐和文本，甚至更复杂的任务，如视频合成。

应用

对话式 AI 的常见应用包括客户支持聊天机器人、语音操作虚拟助手（如 Siri 或 Alexa）以及交互式语音响应（IVR）系统。

生成式 AI 的常见应用包括创作艺术或音乐、生成逼真的视频游戏环境、合成声音以及生成逼真的图像甚至深度伪造。

技术应用

对话式 AI 通常依赖于自然语言处理（NLP）技术来理解和生成人类语言。这包括意图识别、实体提取和对话管理。

生成式 AI 通常利用生成对抗网络（GANs）、变分自编码器（VAEs）和其他生成模型来生成新内容。

训练和交互

虽然训练可以是监督的、半监督的或无监督的，但对话式 AI 的主要交互模式是通过来回对话或交谈。

生成式 AI 的训练过程，特别是像 GANs 这样的模型，涉及迭代过程，其中模型通过试图欺骗判别器使其相信生成数据是真实的，来学习生成数据。

评估

对话式 AI 的评估指标通常围绕理解、响应准确性、用户满意度以及生成响应的流畅性展开。

对于 GANs 等模型，生成式 AI 的评估指标可能具有挑战性，可能涉及使用定量指标和人类判断的组合来评估生成内容的品质。

数据需求

对话式 AI 的数据需求通常涉及对话数据，包括人类之间的对话或人类与机器人之间的对话。

生成式 AI 的数据需求涉及它应该生成的内容类型的大型数据集，如图像、文本和音乐。

尽管对话式 AI 和生成式 AI 都涉及生成输出，但它们的主要目标、应用和方法可能存在显著差异。对话式 AI 用于与用户的交互式通信，而生成式 AI 则专注于产生新的、原创的内容。

DALL-E 是否属于生成式 AI 的一部分？

DALL-E 以及类似从文本生成图形的工具是生成式 AI 的例子。实际上，DALL-E 是图像合成领域中最突出的生成式 AI 例子之一。

下面是 DALL-E 的生成特性列表，后面是每个项目的简要描述：

+   图像生成

+   学习分布

+   创新组合

+   广泛应用

+   Transformer 架构

图像生成是 DALL-E 的一个关键特性，它被设计成根据文本描述生成图像。给定一个如“一个双头火烈鸟”的提示，DALL-E 可以生成一个符合描述的新颖图像，即使它在训练数据中从未见过这样的图像。

学习分布：与其他生成模型一样，DALL-E 学习其训练数据的概率分布。当它生成图像时，它从这个学习到的分布中进行采样，以产生基于其训练的合理视觉。

创新组合：DALL-E 可以生成代表完全新颖或抽象概念的图像，展示了其能够以创新的方式组合和重新组合学习到的元素的能力。

除了图像合成之外，DALL-E 还在艺术生成、风格融合以及创建具有特定属性或主题的图像等领域提供了广泛的应用支持，突显了其作为生成工具的多样性。

DALL-E 利用了一种变体的 Transformer 架构，类似于 GPT-3 等模型，但针对图像生成任务进行了调整。

其他基于输入数据（无论是文本、另一张图像还是任何其他形式的数据）生成图形、艺术或任何形式视觉内容的工具，并且可以生成其训练数据中未明确存在的输出，也被认为是生成性人工智能。它们展示了人工智能模型不仅能够分析和分类，还能够创造和创新。

ChatGPT 和 GPT-4 是否属于生成性人工智能？

ChatGPT 和 GPT-4 都被认为是生成性人工智能的例子。它们属于“Transformer”这一类模型，特别擅长处理数据序列，如文本相关任务。

以下列表提供了各种原因，说明为什么这些大型语言模型（LLMs）被认为是生成性的，随后对每个项目进行了简要描述：

+   文本生成

+   学习分布

+   广泛应用

+   无监督学习

文本生成：这些模型可以根据给定的提示生成连贯、上下文相关且通常非常复杂的文本序列。它们生成的响应在它们的训练数据中并未明确存在，但基于它们在训练期间学习到的模式和结构构建。

学习分布：GPT-3、GPT-4 以及类似模型学习其训练数据的概率分布。在生成文本时，它们实际上是从这个学习到的分布中进行采样，以产生基于其训练的序列。

广泛应用：除了基于文本的聊天或对话之外，这些模型还可以用于各种生成任务，如故事写作、代码生成、诗歌，甚至创建特定风格或模仿某些作者的内容，展示了它们的生成能力。

无监督学习：虽然它们可以通过特定数据集进行微调，但像 GPT-3 这样的模型主要是以无监督方式在大量文本上进行训练，学习生成内容，而不需要为每个可能的响应提供显式的标记数据。

OpenAI 的 ChatGPT-3、GPT-4 以及类似模型是自然语言处理和生成领域中生成人工智能的典范例子。

下几节简要介绍了一些在人工智能领域有强大影响力的公司。

DEEPMIND

DeepMind 对人工智能做出了重大贡献，包括创建了各种人工智能系统。DeepMind 成立于 2010 年，并于 2014 年成为谷歌的子公司。其主页为[`deepmind.com/`](https://deepmind.com/)。

DeepMind 创建了 280 GB 的语言模型 Gopher，其性能显著优于其竞争对手，包括 GPT-3、J1-Jumbo 和 MT-NLG。DeepMind 还开发了 AlphaFold，它解决了研究人员十年未能解决的蛋白质折叠任务。DeepMind 于 2021 年 7 月将 AlphaFold 免费提供给每个人。DeepMind 在开发世界级人工智能游戏系统方面做出了重大贡献，其中一些将在下一节中讨论。

DeepMind 和 游戏

DeepMind 是 AlphaStar 和 AlphaGo 等人工智能系统背后的力量，这些系统在围棋（比国际象棋难度大得多）中击败了最优秀的人类选手。这些游戏提供“完美信息”，而“不完美信息”的游戏（如扑克牌）对机器学习模型构成了挑战。

AlphaGo Zero（AlphaGo 的后继者）通过自我对弈在更短的时间内和更少的计算能力下掌握了游戏。AlphaGo Zero 通过以 100-0 的成绩击败 AlphaGo 展现了非凡的表现。另一个强大的系统是 AlphaZero，它使用自我对弈学习技术来玩围棋、国际象棋和将棋，并实现了 SOTA（最高技术水平）的性能结果。

通过比较，使用树搜索的机器学习模型非常适合具有完美信息量的游戏。相比之下，具有不完美信息量的游戏（如扑克牌）涉及隐藏信息，可以利用这些信息制定对抗策略来对抗对手的策略。AlphaStar 能够与星际争霸 II 的最佳选手对战，并成为第一个在需要“在信息不完整的世界中的战略能力”的游戏中实现 SOTA 结果的人工智能。

玩家游戏（PoG）

谷歌的 DeepMind 团队设计了基于以下技术的通用 PoG（玩家游戏）算法：

+   CFR（反事实遗憾最小化）

+   CVPN（反事实价值与策略网络）

+   GT-CFT（增长树 CFR）

+   CVPN

反事实价值与策略网络（CVPN）是一个神经网络，它计算游戏中每个状态信念的反事实。这在评估任何给定时间点的游戏不同变体时至关重要。

增长树 CFR（GT-CFR）是 CFR 的一种变体，它针对随时间增长的博弈树进行了优化。GT-CFR 基于两个基本阶段，更多细节可以在网上找到：

[`medium.com/syncedreview/deepminds-pog-excels-in-perfect-and-imperfect-information-games-advancing-research-on-general-9dbad5c04221`](https://medium.com/syncedreview/deepminds-pog-excels-in-perfect-and-imperfect-information-games-advancing-research-on-general-9dbad5c04221)

OPENAI

OpenAI 是一家对人工智能做出了重大贡献的人工智能研究公司，包括 DALL-E 和 ChatGPT，其主页在这里：[`openai.com/api/`](https://openai.com/api/)。

OpenAI 由埃隆·马斯克和山姆·奥特曼（以及其他一些人）在旧金山创立，其声明的目标之一是开发对人类有益的人工智能。鉴于微软对该组织的大量投资和深度联盟，OpenAI 可能被视为微软的一部分。OpenAI 是 GPT-x 系列大型语言模型（LLM）以及 ChatGPT 的创造者，ChatGPT 于 2022 年 11 月 30 日对外发布。

OpenAI 通过 API 将 GPT-3 商业化，用于各种应用，按字计费。GPT-3 于 2020 年 7 月宣布，并通过测试计划提供。然后，在 2021 年 11 月，OpenAI 将 GPT-3 向所有人开放。更多详细信息可在网上找到：

[`openai.com/blog/api-no-waitlist/`](https://openai.com/blog/api-no-waitlist/).

此外，OpenAI 开发了 DALL-E，它可以从文本生成图像。最初，OpenAI 并不允许用户上传包含真实人脸的图像。后来，在 2022 年第四季度，OpenAI 改变了其政策，允许用户将其人脸上传到其在线系统中。（请查看 OpenAI 网页以获取更多详细信息。）顺便提一下，扩散模型已经超越了 DALL-E 的基准。

OpenAI 还发布了一个公开测试版的 Embeddings，这是一种适合各种类型机器学习（ML）任务的数据格式，如这里所述：

[`beta.openai.com/docs/guides/embeddings`](https://beta.openai.com/docs/guides/embeddings)

OpenAI 是 Codex 的创造者，它提供了一组使用自然语言处理（NLP）训练的模型。Codex 的初始发布处于私密测试阶段，更多信息可在[`beta.openai.com/docs/engines/instruct-series-beta`](https://beta.openai.com/docs/engines/instruct-series-beta)找到。

OpenAI 提供了四个共同称为其指令模型的模型，这些模型支持 GPT-3 生成自然语言的能力。这些模型将在 2024 年初被弃用，并替换为 GPT-3、ChatGPT 和 GPT-4 的更新版本。

如果你想了解更多关于 OpenAI 提供的功能和服务，请访问以下网页：[`platform.openai.com/overview`](https://platform.openai.com/overview)。

COHERE

Cohere 是一家初创公司，也是 OpenAI 的竞争对手，其主页在这里：[`cohere.ai/`](https://cohere.ai/)。

Cohere 开发了商业上可用的尖端 NLP 技术，适用于多个行业。Cohere 专注于执行文本分析的模型，而不是文本生成的模型（如基于 GPT 的模型）。Cohere 的创始团队令人印象深刻：CEO Aidan Gomez 是 Transformer 架构的共同发明人之一，而 CTO Nick Frosst 是 Geoff Hinton 的弟子。

HUGGING FACE

Hugging Face 是一个流行的基于社区的开放源代码 NLP 技术仓库，其主页位于[`github.com/huggingface`](https://github.com/huggingface)。

与 OpenAI 或 Cohere 不同，Hugging Face 并不构建自己的 NLP 模型。相反，Hugging Face 是一个平台，管理着众多开源 NLP 模型，客户可以对这些模型进行微调，然后部署这些微调后的模型。确实，Hugging Face 已经成为人们协作开发 NLP 模型的重要场所，有时也被称为“机器学习和 NLP 的 GitHub”。

Hugging Face 库

Hugging Face 提供了三个重要的库：datasets、tokenizers 和 transformers。Accelerate 库支持 PyTorch 模型。datasets 库提供了一系列 NLP 库。tokenizer 库使您能够将文本数据转换为数值。

可能最令人印象深刻的是 transformers 库，它提供了一整套预训练的基于 BERT 的模型，可以执行各种 NLP 任务。GitHub 仓库在这里：[`github.com/huggingface/transformers`](https://github.com/huggingface/transformers)。

Hugging Face 模型库

Hugging Face 提供了一个模型库，提供大量可在线访问的模型。此外，该网站支持其模型的在线测试，包括以下任务：

+   使用 BERT 进行掩码词填充

+   使用 Electra 进行命名实体识别

+   使用 RoBERTa 进行自然语言推理

+   使用 DistilBERT 进行问答

+   使用 BART 进行摘要

+   使用 GPT-2 进行文本生成

+   使用 T5 进行翻译

导航到以下网页以查看“使用 Transformer 进行写作”的文本生成功能：[`transformer.huggingface.co`](https://transformer.huggingface.co)。

在下一章中，您将看到 Python 代码示例，展示如何列出所有可用的 Hugging Face 数据集以及如何加载特定数据集。

AI21

AI21 是一家公司，通过 API 提供专有的大语言模型，以支持其客户的各项应用。AI21 当前的 SOTA 模型名为 Jurassic-1（与 GPT-3 大小相当），AI21 还在 Jurassic-1 和其他模型之上创建了其自己的应用。AI21 当前的应用套件包括增强阅读和写作的工具。

Primer 是这个领域的老牌竞争者，成立于 Transformer 发明前的两年。该公司主要服务于政府和防务行业的客户。

INFLECTIONAI

在 AI 领域，InflectionAI 是一家较新的公司，其令人印象深刻的核心团队包括：

+   Reid Hoffman（LinkedIn）

+   DeepMind 联合创始人 Mustafa Suleyman

+   DeepMind 研究员 Karen Simonyan

InflectionAI 致力于一项具有挑战性的任务：使人类能够以与人类相互沟通的相同方式与计算机互动。

ANTHROPIC

Anthropic 于 2021 年由 OpenAI 的前员工创建，其主页在此：[`www.anthropic.com/`](https://www.anthropic.com/)。

Anthropic 获得了包括 Google 和 Salesforce 在内的多家公司的显著财务支持。该公司发布了 Claude 2 作为 ChatGPT 的竞争对手。

Claude 2 能够总结多达 75,000 字的文本内容，而 ChatGPT 目前的限制是 3,000 字。此外，Claude 2 在部分律师资格考试中取得了 76.5%的分数，在 Python 编码测试中取得了 71%的分数。Claude 2 在为用户查询提供“干净”的回复方面的比率也高于 ChatGPT。

这部分章节关于在人工智能领域做出重要贡献的 AI 公司的内容到此结束。下一节提供了一个关于大型语言模型（LLMs）的高级介绍。

什么是提示工程？

你已经了解过来自 OpenAI 的文本生成器，如 GPT-3 和 DALL-E 2，以及来自 AI21 的 Jurassic，以及 Midjourney 和 Stable Diffusion，它们可以执行文本到图像的生成。提示工程指的是设计基于文本的提示，使基于 AI 的系统能够改进生成的输出，这意味着输出更接近用户希望从 AI 系统中产生的任何内容。通过类比，将提示视为类似教练的角色：他们提供建议和意见，以帮助人们在特定任务中表现更好。

由于提示是基于单词的，挑战在于学习不同单词如何影响生成的输出。此外，预测系统对给定提示的反应也很困难。例如，如果你想生成一幅风景，暗色风景和亮色风景之间的区别是直观的。然而，如果你想生成一幅美丽的风景，AI 系统将如何生成相应的图像？正如你可以推测的那样，对于从文本生成图像的 AI 系统来说，具体词汇比抽象或主观词汇更容易。仅为了增加更多到前面的例子，你将如何可视化以下内容？

+   一幅美丽的风景

+   一首美丽的歌曲

+   一部美丽的电影

尽管提示工程始于文本到图像的生成，但还有其他类型的提示工程，例如基于音频的提示，它解释强调的文本和语音中检测到的情绪，以及基于草图（sketch-based）的提示，它可以从绘画中生成图像。最近关注的焦点是用于生成视频的基于文本的提示，这为艺术家和设计师提供了令人兴奋的机会。以下网页提供了一个图像到图像处理的示例：

[`huggingface.co/spaces/fffiloni/stable-diffusion-color-sketch`](https://huggingface.co/spaces/fffiloni/stable-diffusion-color-sketch)

提示和完成

提示是用户提供给 LLMs 的文本字符串，而完成是用户从 LLMs 收到的文本。提示帮助 LLMs 完成请求（任务），并且它们的长度可以不同。尽管提示可以是任何文本字符串，包括随机字符串，但提示的质量和结构会影响完成的质量。

将提示视为向 LLMs 提供“指导”的机制，或者甚至将其视为一种“教练”LLMs 以提供所需答案的方式。提示中的标记数加上完成中的标记数最多为 2,048 个标记。

提示类型

以下列表包含 LLMs 已知类型的提示：

+   零样本提示

+   单样本提示

+   少样本提示

+   指令提示

零样本提示包含任务的描述，而单样本提示则由一个用于完成任务的单个示例组成。少样本提示由多个示例（通常在 10 到 100 个之间）组成。在所有情况下，都建议提供任务或任务的清晰描述：更多的任务可以为 GPT-3 提供更多信息，从而可能导致更准确的完成。

T0（对于“零样本”）是一个有趣的 LLM：尽管 T0 比 GPT-3 小 16 倍（11 GB），但在语言相关任务上 T0 的表现超过了 GPT-3。由于 T0 是在包含多个任务的数据集上训练的，因此它可以在未见过的 NLP 任务（即对 T0 来说是新任务）上表现良好。

以下 URL 提供了 T0 的 Github 仓库，其中包含训练和评估模型的信息：

[`github.com/bigscience-workshop/t-zero`](https://github.com/bigscience-workshop/t-zero)

T0++基于 T0，并且它是在 T0 训练的任务集之外额外训练的任务上训练的。

作为旁注，前面列表中的前三个提示也分别被称为“零样本学习”、“单样本学习”和“少样本学习”。 

指令提示

指令提示用于微调 LLMs，并指定 LLMs 在响应中应遵守的格式（由您确定）。您可以准备自己的指令提示，或者您可以访问包含不同任务的不同模板以及不同数据集的提示模板库。各种提示指令模板公开可用，例如以下提供 Llama 提示模板的链接：

[`github.com/devbrones/llama-prompts`](https://github.com/devbrones/llama-prompts)

[`pub.towardsai.net/llama-gpt4all-simplified-local-chatgpt-ab7d28d34923`](https://pub.towardsai.net/llama-gpt4all-simplified-local-chatgpt-ab7d28d34923)

反向提示

另一种技术使用的是反向顺序：输入提示是答案，而响应是与答案相关的疑问（类似于一个流行的游戏节目）。例如，给定一个法语句子，您可能会问模型，“什么英语文本可能导致这个法语翻译？”

系统提示与代理提示的比较

在对话式人工智能系统和聊天机器人设计的情况下，系统提示和代理提示之间的区别经常出现。

系统提示通常是系统给出的初始消息或提示，用于指导用户可以做什么，或设定对交互的期望。它通常作为介绍或指导用户如何继续的方式。以下是一些系统提示的例子：

+   “欢迎使用 ChatBotX！您可以问我关于天气、新闻或体育的问题。今天我能帮您做什么？”

+   “你好！按 1 获取账户详情，按 2 获取技术支持。”

+   “你好！输入‘order’跟踪您的包裹或输入‘help’寻求帮助。”

相比之下，代理提示是 AI 模型或代理在交互过程中对用户输入的响应生成的消息。它是对话中来回交流的一部分。代理提示指导用户提供更多信息，澄清歧义，或引导用户采取特定行动。以下是一些代理提示的例子：

用户：“我在找鞋子。”

代理提示：“太好了！您是在寻找男士还是女士的鞋子？”

用户：“我登录不了。”

代理提示：“很遗憾听到这个消息。你能具体说明是密码还是用户名有问题吗？”

用户：“给我讲一个笑话。”

代理提示：“为什么鸡要加入乐队？因为它有鸡腿！”

两者之间的基本区别在于它们的目的和在交互中的位置。系统提示通常在交互开始时，为对话设定场景。代理提示发生在对话过程中，根据用户输入引导对话的方向。

这两种类型的提示对于创建流畅直观的对话体验至关重要。它们指导用户，并有助于确保系统有效地理解和解决用户的需求。

提示模板

提示模板是预定义的格式或结构，用于指导模型或系统执行特定任务。它们是生成提示的基础，其中模板的某些部分可以填充或定制，以产生各种特定的提示。通过类比，提示模板类似于您可以在某些文本编辑器中定义的宏。

提示模板在与语言模型一起工作时特别有用，因为它们提供了一种在多个任务或数据点查询模型的一致方式。特别是，提示模板可以更容易地：

+   确保在多次查询模型时保持一致性

+   促进批量处理或自动化

+   减少提问方式中错误和变化

例如，假设您正在使用一个 LLM，并且您想将英语句子翻译成法语。相关的提示模板可能如下：

“将以下英文句子翻译成法语：{sentence}”

注意，{sentence} 是一个占位符，您可以用任何英语句子替换它。

您可以使用前面的提示模板来生成特定的提示：

+   “将以下英文句子翻译成法语：‘你好，你好吗？’”

+   “将以下英文句子翻译成法语：‘我爱冰淇淋。’”

如您所见，提示模板使您能够轻松地为不同的句子生成各种提示，而无需每次都重写整个指令。实际上，这个概念可以扩展到更复杂的任务，并且可以根据应用情况包含多个占位符或更复杂的结构。

不同 LLM 的提示

GPT-3、ChatGPT 和 GPT-4 都是基于 Transformer 架构的 LLM，它们在底层机制上本质上是相似的。ChatGPT 实际上是一个针对对话交互进行微调的 GPT 模型版本。GPT-4 在规模和能力方面是 GPT-3 的进化或改进。

这些模型提示的差异主要源于特定的用例和上下文，而不是模型之间的固有差异。以下是基于用例的提示差异。

GPT-3 可以用于广泛的任务，而不仅仅是对话，从内容生成到代码编写。以下是 GPT-3 提示的一些示例：

+   “将以下英文文本翻译成法语：‘你好，你好吗？’”

+   “编写一个计算数字阶乘的 Python 函数。”

ChatGPT 是专门针对对话交互进行微调的。以下是 ChatGPT 提示的一些示例：

用户：“你能帮我做作业吗？”

ChatGPT：“当然可以！你需要帮助哪个科目或主题？”

用户：“讲一个笑话。”

ChatGPT：“为什么鸡穿过操场？为了到达另一边的滑梯！”

GPT-4 提供了更大的规模和改进，因此提示的性质与 GPT-3 相似，但可能产生更准确或更细微的输出。以下是 GPT-4 提示的一些示例：

+   “提供关于量子力学与广义相对论之间关系的详细分析。”

+   “基于后末日世界和希望主题创作一个短篇故事。”

这三个模型接受自然语言提示并产生自然语言输出。与它们交互的基本方式保持一致。

主要差异来自模型被使用的上下文以及任何应用的微调。例如，ChatGPT 设计得更具对话性，因此虽然您可以使用 GPT-3 进行聊天，但 ChatGPT 可能会产生更具上下文相关性的对话输出。

当直接与这些模型交互，尤其是通过 API 时，您也可能控制诸如“温度”（控制随机性）和“最大标记数”（控制响应长度）等参数。调整这些参数可以塑造响应，无论您使用的是哪种 GPT 变体。

尽管底层模型在规模和特定训练/微调方面存在差异，但您提示它们的方式在很大程度上保持一致：清晰、具体的自然语言提示会产生最佳结果。

不当措辞的提示

在制作提示时，尽可能清晰和具体至关重要，以便引导响应朝所需的方向发展。含糊或模糊的提示可能导致各种响应，其中许多可能对用户实际意图没有帮助或不相关。

此外，措辞不当的提示通常含糊不清、模棱两可或过于宽泛，这可能导致 AI 模型产生混淆、误解或非具体响应。以下是一些示例：

+   “告诉我那件事。”

    问题：过于模糊。指的是什么“事物”？

+   “为什么会发生这样的事情？”

    问题：没有上下文。正在讨论的是哪个事件或情况？

+   “解释这些内容。”

    问题：过于宽泛。应该解释哪些具体的“内容”？

+   “做需要做的事情。”

    问题：含糊不清。需要采取哪些具体的行动？

+   “我想获取信息。”

    问题：不具体。需要哪种类型的信息？ 

+   “你能从那个地方为我拿到那个东西吗？”

    问题：既不清楚“事物”也不清楚“地点”。

+   “你能告诉我那个人的书是什么吗？”

    问题：含糊的引用。谁是“他的”？ 

+   “你如何进行这个过程？”

    问题：指的是哪个“过程”？

+   “描述这个主题的重要性。”

    问题：“主题”未指定。

+   “为什么它是好是坏？”

    问题：没有上下文。什么是“它”？ 

+   “帮助解决这个问题。”

    问题：模糊。面临的具体问题是什么？

+   “考虑这个任务的注意事项。”

    问题：歧义。正在讨论的是哪个“任务”？

+   “这是怎么工作的？”

    问题：缺乏具体性。什么是“这个”？

什么是 CHATGPT？

“聊天机器人战争”正在加剧，主要竞争对手的长期价值仍有待确定。一个竞争对手是 ChatGPT-3.5（ChatGPT），这是 OpenAI 的一个基于 AI 的聊天机器人。ChatGPT 通过提供对话式响应来响应用户的查询，并且可以通过以下链接访问：[`chat.openai.com/chat`](https://chat.openai.com/chat)。

ChatGPT 注册用户的增长率非常惊人。其最接近的竞争对手是 iPhone，它在 2.5 个月内达到了一百万用户，而 ChatGPT 仅用了六天时间就突破了百万用户大关。ChatGPT 的用户量峰值约为 18 亿，然后下降到大约 15 亿，您可以在以下链接中的图表中看到：

[`decrypt.co/147595/traffic-dip-hits-openais-chatgpt-first-times-hardest`](https://decrypt.co/147595/traffic-dip-hits-openais-chatgpt-first-times-hardest)

注意，尽管 Meta 的 Threads 在会员数量方面超过了 ChatGPT，但 Threads 的日活跃用户数量下降了约 50%。以下是六个知名公司/产品与 ChatGPT 达到一百万会员所需时间框架的比较：[`www.syntheticmind.io/p/01`](https://www.syntheticmind.io/p/01)。

前面的网页还包含有关 Will Hobick 的信息，他使用 ChatGPT 编写了一个用于电子邮件相关任务的 Chrome 扩展程序，尽管他没有 JavaScript 或 Chrome 扩展程序编程经验。Will Hobick 在这里提供了更多关于他的 Chrome 扩展的详细信息：

[`www.linkedin.com/posts/will-hobick_gpt3-chatgpt-ai-activity-7008081003080470528-8QCh`](https://www.linkedin.com/posts/will-hobick_gpt3-chatgpt-ai-activity-7008081003080470528-8QCh)

ChatGPT

目前，ChatGPT 的付费版本可能是世界上最好的聊天机器人。确实，ChatGPT 可以执行多种任务，以下列出了一些：

+   写诗

+   写作文章

+   编写代码

+   角色扮演

+   拒绝不适当的要求

此外，它对自然语言查询的回答质量超过了其前辈 GPT-3 的能力。另一个有趣的特性包括能够承认自己的错误。ChatGPT 还提供“提示回复”，这是你可以向 ChatGPT 提出的问题的示例。ChatGPT 的一个有趣用途是生成结束关系的短信：

[`www.reddit.com/r/ChatGPT/comments/zgpk6c/breaking_up_with_my_girlfriend/`](https://www.reddit.com/r/ChatGPT/comments/zgpk6c/breaking_up_with_my_girlfriend/)

ChatGPT 生成的圣诞歌词可在以下链接找到：

[`www.cnet.com/culture/entertainment/heres-what-it-sounds-like-when-ai-writes-christmas-lyrics`](https://www.cnet.com/culture/entertainment/heres-what-it-sounds-like-when-ai-writes-christmas-lyrics)

ChatGPT 的一个可能不会让有小孩的父母感到亲切的方面是，ChatGPT 告诉孩子们圣诞老人不存在：

[`futurism.com/the-byte/openai-chatbot-santa`](https://futurism.com/the-byte/openai-chatbot-santa)

[`www.forbes.com/sites/lanceeliot/2022/12/21/pointedly-asking-generative-ai-chatgpt-about-whether-santa-claus-is-real-proves-to-be-eye-opening-for-ai-ethics-and-ai-law`](https://www.forbes.com/sites/lanceeliot/2022/12/21/pointedly-asking-generative-ai-chatgpt-about-whether-santa-claus-is-real-proves-to-be-eye-opening-for-ai-ethics-and-ai-law)

ChatGPT：谷歌“代码红色警报”

2022 年 12 月，谷歌 CEO 发布了关于 ChatGPT 作为谷歌搜索引擎竞争对手潜在威胁的“代码红色警报”，简要讨论如下：

[`www.yahoo.com/news/googles-management-reportedly-issued-code-190131705.html`](https://www.yahoo.com/news/googles-management-reportedly-issued-code-190131705.html)

根据前文，谷歌正在投资资源开发基于 AI 的产品，预计是为了提供能够成功与 ChatGPT 竞争的功能。其中一些基于 AI 的产品也可能生成与 DALL-E 图形效果相当的画面。确实，争夺 AI 主导权的竞赛仍在继续，并且无疑将在可预见的未来持续下去。

ChatGPT 对比 Google 搜索

鉴于经常有人猜测 ChatGPT 注定要取代 Google 搜索，让我们简要比较一下 Google 和 ChatGPT 对特定查询的响应方式。首先，Google 是一个使用 Page Rank 算法（由拉里·佩奇开发，并严格保密）的搜索引擎。Google 使用这个算法对网站进行排名，并为特定查询生成搜索结果。然而，搜索结果中包括付费广告，这可能会“扰乱”链接列表。

相比之下，ChatGPT 不是一个搜索引擎：它对特定查询提供直接响应。用通俗的话说，ChatGPT 将直接“切入正题”，并消除任何提及多余链接的内容。ChatGPT 也可能产生错误的结果，其后果可能从无害到严重不等。

因此，Google 搜索和 ChatGPT 都有优点和缺点，它们在不同类型的查询中表现出色：前者适用于具有多方面答案的查询（例如，关于法律问题的问题）和后者适用于直接了当的查询（例如，编码问题）。显然，它们在许多其他类型的查询中也表现出色。

根据玛格丽特·米切尔的说法，ChatGPT 不会取代 Google 搜索。她提供了一些关于 Google 搜索和 PageRank 的有趣细节，你可以在[`twitter.com/mmitchell_ai/status/1605013368560943105`](https://twitter.com/mmitchell_ai/status/1605013368560943105)上阅读。

ChatGPT 自定义指令

ChatGPT 已添加对自定义指令的支持，这允许你指定一些 ChatGPT 在响应你的查询时将使用的偏好。

ChatGPT Plus 用户可以通过访问 ChatGPT 网站并执行以下步骤来开启自定义指令：

设置 > 测试功能 > 启用自定义指令

作为简单的例子，你可以指定你更喜欢看到除 Python 以外的语言中的代码。通过 ChatGPT 中的自定义指令，也可以指定一组常见的初始要求用于常规任务。设置自定义指令的详细步骤可以在以下网址找到：

[`artificialcorner.com/custom-instructions-a-new-feature-you-must-enable-to-improve-chatgpt-responses-15820678bc02`](https://artificialcorner.com/custom-instructions-a-new-feature-you-must-enable-to-improve-chatgpt-responses-15820678bc02)

自定义指令的另一个有趣例子来自杰里米·豪沃德，他准备了一套详尽且详细的自定义指令，可在以下链接找到：

[`twitter.com/jeremyphoward/status/1689464587077509120`](https://twitter.com/jeremyphoward/status/1689464587077509120)

当这本书准备印刷时，只有注册了 ChatGPT Plus 的用户才能获得自定义说明。

移动设备和浏览器上的 ChatGPT

ChatGPT 在 2023 年首先对 iOS 设备开放，然后是对安卓设备。您可以从以下网页下载 ChatGPT 到 iOS 设备上：

[`www.macobserver.com/tips/how-to/how-to-install-and-use-the-official-chatgpt-app-on-iphone/`](https://www.macobserver.com/tips/how-to/how-to-install-and-use-the-official-chatgpt-app-on-iphone/)

或者，如果您拥有安卓设备，您可以从以下网页下载 ChatGPT：

[`play.google.com/store/apps/details?id=com.openai.chatgpt`](https://play.google.com/store/apps/details?id=com.openai.chatgpt)

如果您想从微软的 Bing 浏览器安装 ChatGPT，请导航到以下网页：

[`chrome.google.com/webstore/detail/chatgpt-for-bing/pkkmgcildaegadhngpjkklnbfbmhpdng`](https://chrome.google.com/webstore/detail/chatgpt-for-bing/pkkmgcildaegadhngpjkklnbfbmhpdng)

ChatGPT 和提示

尽管 ChatGPT 在生成对查询的响应方面很擅长，但有时您可能对结果并不完全满意。一个选项是输入单词“重写”，以便从 ChatGPT 获取另一个版本。

尽管这是可用的最简单的提示之一，但在有效性方面有限。如果您想要更多有意义的提示列表，以下会员专属文章包含了 31 个可能比使用“重写”一词（不仅仅是 ChatGPT）更好的提示：

[`medium.com/the-generator/31-ai-prompts-better-than-rewrite-b3268dfe1fa9`](https://medium.com/the-generator/31-ai-prompts-better-than-rewrite-b3268dfe1fa9)

GPTBot

GPTBot 是一个用于网站的爬虫。幸运的是，您可以通过向网站的 robots.txt 文件中添加 GPTBot 来禁止 GPTBot 访问网站：

User-agent: GPTBot

禁止访问：/

您还可以通过向网站的 robots.txt 类文件中添加 GPTBot 令牌来仅对网站的一部分进行 GPTBot 访问自定义：

User-agent: GPTBot

允许访问：/youcangohere-1/

禁止访问：/dontgohere-2/

顺便说一下，Stable Diffusion 和 LAION 都通过 Common Crawl 爬取互联网。然而，您可以通过在 robots.txt 文件中指定以下片段来防止您的网站被爬取：

User-agent: CCBot

禁止访问：/

关于 GPTBot 的更多信息可在以下网站获取：[`platform.openai.com/docs/gptbot`](https://platform.openai.com/docs/gptbot) [`platform.openai.com/docs/gptbot`](https://platform.openai.com/docs/gptbot)

[`www.yahoo.com/finance/news/openai-prepares-unleash-crawler-devour-020628225.html`](https://www.yahoo.com/finance/news/openai-prepares-unleash-crawler-devour-020628225.html)

ChatGPT 操场

ChatGPT 有一个自己的游乐场，你将看到它与可在此访问的 GPT-3 游乐场在实质上有所不同：[`chat.openai.com/chat`](https://chat.openai.com/chat)。

为了你的方便，GPT-3 游乐场的链接在此重现：

[`beta.openai.com/playground`](https://beta.openai.com/playground)。

OpenAI 定期为 ChatGPT 添加新功能，包括以下内容：

+   用户可以查看（并继续）之前的对话

+   ChatGPT 将不会回答的问题数量减少

+   用户保持登录状态超过两周

另一个不错的增强功能包括对键盘快捷键的支持：当与代码一起工作时，你可以使用序列⌘ (Ctrl) + Shift +（对于 Mac）来复制最后一个代码块，以及序列⌘ (Ctrl) + / 来查看完整的快捷键列表。

关于 ChatGPT 以及如何编写提示以从 ChatGPT 中提取你想要的信息的文章有很多。其中一篇文章如下：

[`www.tomsguide.com/features/7-best-chatgpt-tips-to-get-the-most-out-of-the-chatbot`](https://www.tomsguide.com/features/7-best-chatgpt-tips-to-get-the-most-out-of-the-chatbot)

插件、高级数据分析和代码精灵

除了回答用户的大量查询外，ChatGPT 通过提供以下功能扩展了其功能：

+   第三方 ChatGPT 插件

+   高级数据分析

+   代码精灵

以下小节将简要讨论前面列表中的主题，以及一个讨论高级数据分析与 Claude 2 的简短部分。

插件

可用的 ChatGPT 插件有数百个，一些流行插件的列表可在以下网站上找到：

[`levelup.gitconnected.com/5-chatgpt-plugins-that-will-put-you-ahead-of-99-of-data-scientists-4544a3b752f9`](https://levelup.gitconnected.com/5-chatgpt-plugins-that-will-put-you-ahead-of-99-of-data-scientists-4544a3b752f9)

[`www.zdnet.com/article/the-10-best-chatgpt-plugins-of-2023/`](https://www.zdnet.com/article/the-10-best-chatgpt-plugins-of-2023/)

“最佳”ChatGPT 插件的列表经常变化，因此请进行在线搜索以了解最新的 ChatGPT 插件。以下链接还包含关于高度评价的插件的信息：

[`www.tomsguide.com/features/i-tried-a-ton-of-chatgpt-plugins-and-these-3-are-the-best`](https://www.tomsguide.com/features/i-tried-a-ton-of-chatgpt-plugins-and-these-3-are-the-best)

下面展示的另一组推荐插件（当然，取决于你的需求）：

+   PDF 询问

+   视频聊天

+   Noteable

+   Upskillr

+   Wolfram

如果你担心 ChatGPT 爬取你网站内容的可能性，OpenAI 的浏览器插件支持一个名为 ChatGPT-User 的用户代理令牌，该令牌遵守许多网站提供的 robots.txt 文件中指定的内容，以限制对内容的访问。

如果您想为 ChatGPT 开发插件，请访问此网站获取更多信息：[`platform.openai.com/docs/plugins/introduction`](https://platform.openai.com/docs/plugins/introduction)。

除了开发 ChatGPT 插件的详细信息外，前面的 OpenAI 网站还提供了有关插件的有用信息，如下所示：

+   认证

+   示例

+   插件审查

+   插件政策

OpenAI 不控制您添加到 ChatGPT 的任何插件：它们将 ChatGPT 连接到外部应用程序。此外，ChatGPT 根据您在 ChatGPT 账户中启用的特定插件，在您的会话期间确定要使用的插件。

高级数据分析

ChatGPT 高级数据分析使 ChatGPT 能够生成图表和图形，创建和训练机器学习模型，包括深度学习模型。ChatGPT 高级数据分析提供了一套广泛的功能，并且对支付每月 20 美元订阅费的 ChatGPT 用户开放。然而，这个功能可能很快就会对所有用户开放。

[`towardsdatascience.com/chatgpt-code-interpreter-how-it-saved-me-hours-of-work-3c65a8dfa935`](https://towardsdatascience.com/chatgpt-code-interpreter-how-it-saved-me-hours-of-work-3c65a8dfa935)

OpenAI 的模型可以访问一个受限在沙盒和防火墙执行环境中的 Python 解释器。在评估 Python 代码期间，解释器插件还可以访问一些临时磁盘空间。尽管临时磁盘空间在有限的时间内可用，但在同一会话中的多次查询可以在代码和执行环境方面产生累积效应。

此外，ChatGPT 可以根据请求生成数据的下载链接。现在的高级数据分析可以一次性分析多个文件，包括 CSV 文件和 Excel 电子表格。

高级数据分析可以执行各种有趣的任务，以下列出了一些：

+   解决数学问题

+   执行数据分析和可视化

+   在不同格式之间转换文件

+   与 Excel 电子表格一起工作

+   在 PDF 中读取文本内容

以下文章讨论了您可以使用高级数据分析的各种方法：

[`mlearning.substack.com/p/the-best-88-ways-to-use-chatgpt-code-interpreter`](https://mlearning.substack.com/p/the-best-88-ways-to-use-chatgpt-code-interpreter)

高级数据分析与 Claude 2 的比较

Anthropic 的 Claude 2 是 ChatGPT 的另一个竞争对手。除了响应用户的提示外，Claude 2 还可以生成代码并“摄取”整本书。Claude 2 也受到幻觉的影响，这是基于 LLM 的聊天机器人的共同特点。有关 Claude 2 的更详细信息，请在此处获取：

[`medium.com/mlearning-ai/claude-2-vs-code-interpreter-gpt-4-5-d2e5c9ee00c3`](https://medium.com/mlearning-ai/claude-2-vs-code-interpreter-gpt-4-5-d2e5c9ee00c3)

顺便说一下，目前可用的 ChatGPT 版本是在 2021 年 9 月训练的，这意味着 ChatGPT 无法回答关于 Claude 2 或 Google Gemini 的问题，这两者都是在该日期之后发布的。

代码轻语者

ChatGPT 代码轻语者（Code Whisperer）使你能够简化一些任务，以下是一些例子（将此列表与 Google Gemini 的对应列表进行比较）：

+   从图像创建视频

+   从图像中提取文本

+   从图像中提取颜色

在 ChatGPT 生成视频后，它还会提供一个链接，你可以通过该链接下载生成的视频。有关前面列表中功能的更详细信息，可以在以下网页找到：

[`artificialcorner.com/chatgpt-code-interpreter-is-not-just-for-coders-here-are-6-ways-it-can-benefit-everyone-b3cc94a36fce`](https://artificialcorner.com/chatgpt-code-interpreter-is-not-just-for-coders-here-are-6-ways-it-can-benefit-everyone-b3cc94a36fce)

检测生成的文本

ChatGPT 生成的文本质量很高，这也使得检测剽窃的任务变得更加复杂。当你阅读一段文本时，有几个线索表明这是生成的文本，例如：

+   粗糙或不寻常的句子结构

+   在多个位置重复的文本

+   过度使用情感（或缺乏情感）

然而，有一些工具可以帮助检测生成的代码。一个免费的在线工具是来自 OpenAI 的 GPT2 检测器：

[`huggingface.co/openai-detector`](https://huggingface.co/openai-detector)

作为一个简单（尽管是人为的）例子，在 GPT2 检测器中输入以下句子：“这是一句由我本人撰写的原创句子，其他人都没有写过。”

GPT2 检测器分析了这句话，并报告说这句话有 19.35%的可能性是真实的。现在让我们通过添加一些额外的文本来修改前面的句子，如下所示：“这是一句由我本人撰写的原创句子，其他人都没有写过，无论在线剽窃工具对此句子的报告如何。”

GPT2 检测器分析了这句话，并报告说这句话有 95.85%的可能性是真实的。根据 GPT2 检测器网站，当输入文本中有大约 50 个标记时，概率分数的可靠性“变得可靠”。

另一个（稍微旧一点的）在线检测自动生成文本的工具是 IBM 的 GLTR（Giant Language model Test Room），可在[`gltr.io/`](http://gltr.io/)访问。

你可以在此处下载 GLTR 的源代码（TypeScript 和 CSS 的组合）：

[`github.com/HendrikStrobelt/detecting-fake-text`](https://github.com/HendrikStrobelt/detecting-fake-text)

除了前面提到的免费工具外，还有一些商业工具可供选择，其中之一是[`writer.com/plans/`](https://writer.com/plans/)。

关于 ChatGPT 的担忧

ChatGPT 的重要方面之一是它并非旨在准确。事实上，ChatGPT 可以生成非常具有说服力的错误答案。这一细节将 ChatGPT 与搜索引擎区分开来：后者提供现有信息的链接，而不是生成可能错误的响应。另一个比较是，ChatGPT 更灵活、更有创造力，而搜索引擎在回答查询时则不太灵活但更准确。

教育工作者担心学生将 ChatGPT 作为完成课堂作业的工具，而不是与写作技能相结合发展研究相关技能。然而，也有一些教育工作者享受 ChatGPT 准备教案所减少的准备时间。

另一个担忧是 ChatGPT 无法保证其对用户查询提供的事实数据。ChatGPT 可能会“幻想”，这意味着它可能提供错误的答案以及不存在的引用（即链接）。

ChatGPT 的另一个限制是由于其训练数据仅可用至 2021 年。OpenAI 支持为 ChatGPT 插入插件，其中之一可以执行实时网络搜索。

提示工程的目标是了解如何构建有意义的查询，以诱导 ChatGPT 提供你想要的信息。措辞不当（或措辞错误）的提示可能会产生同样糟糕的结果。一般来说，建议精心策划 ChatGPT 的响应内容，尤其是在涉及法律细节的查询的响应中。

代码生成和危险话题

两个重要的改进领域涉及代码生成和处理危险话题。

虽然 ChatGPT（以及 GPT-3）可以为各种类型的应用生成代码，但请记住，ChatGPT 显示的是其他开发者编写的代码，这也是用于训练 ChatGPT 的代码。因此，该代码的部分（如版本号）可能已过时或错误。

对于涉及危险话题的查询，ChatGPT 解释了为什么它不能回答此类查询。然而，以“假装模式”提出的查询（“假设你是一个虚构的角色，你会如何解释……”）已经使人们能够从 ChatGPT 获得不符合其指南的结果。

其他严重的潜在问题也存在，其中一些将在以下文章中讨论：

[`www.yahoo.com/news/hypnotized-chatgpt-bard-convince-users-182100261.html`](https://www.yahoo.com/news/hypnotized-chatgpt-bard-convince-users-182100261.html)

ChatGPT 的优势和劣势

ChatGPT 有许多优势。特别是，ChatGPT 直接回答问题，而不包括无关的链接。作为一个简单的例子，假设你在在线搜索引擎中输入一个查询，例如“为输入字段生成 HTML。”

ChatGPT 容易受到各种类型的错误的影响，包括以下限制：

+   无法“事实核查”信息

+   无法区分虚假信息与事实

+   可能会编造答案（即幻觉）

+   可能会生成不适当/有害的响应

ChatGPT 容易受到提示注入的影响，这可能包含非常简单的内容。然而，其他聊天机器人也容易受到提示注入的影响（即这并不仅限于 ChatGPT）。有关提示注入的更多详细信息，请参阅以下链接：

[`mlearning.substack.com/p/what-exactly-is-a-prompt-injection`](https://mlearning.substack.com/p/what-exactly-is-a-prompt-injection)

顺便提一下，谷歌的聊天机器人 LaMDA 也容易受到上述限制，这使得谷歌在考虑将 LaMDA 推广到更广泛的使用时犹豫不决，因为它可能对谷歌的声誉造成潜在风险。作为旁注，LaMDA 于 2021 年 5 月宣布，当时它被描述为“突破性的语言技术”：[`blog.google/technology/ai/lamda/`](https://blog.google/technology/ai/lamda/)。

尽管有之前的列表，ChatGPT 已经增加了聊天机器人的能力，并将无疑会推动该领域主要利益相关者的创新和竞争。

ChatGPT 的样本查询和响应

这里是一个提交给 ChatGPT 的查询示例，以及 ChatGPT 的详细响应：

许多人认为人工智能是危险的。你如何看待这个问题？

“有一个普遍的误解，认为人工智能天生就是危险的。虽然人工智能确实有可能被用于有害的目的，但它也有能力做很多好事。就像任何其他技术一样，这完全取决于如何使用。在合适的人手中，人工智能可以用来解决世界上一些最紧迫的问题，比如治愈疾病和改善农业。在不合适的人手中，它可能会被用来造成伤害。对我们来说，负责任和道德地使用人工智能，并确保它以最小化潜在危害的方式进行监管和控制，是非常重要的。”

这里是提交给 ChatGPT-3 的其他查询示例，以及详细的响应：

1. 你有哪些方法可以提高你对查询的响应的准确性？

“有几种方法可以提高我对查询的响应的准确性。一种方法是用更多的数据来训练我的算法。我拥有的数据越多，我可以处理的信息就越多，我的响应就越准确。提高准确性的另一种方法是使用更先进的算法和技术，例如机器学习自然语言处理。这些方法使我能够更好地理解语言的细微差别，并提供更准确的查询响应。此外，定期的测试和评估可以帮助识别我可以提高准确性的领域，并使我能够专注于这些领域以改进我的响应。”

2. 你能给出一个奇数完全数的例子吗？

“据我们所知，目前没有发现奇完全数。虽然人们相信奇完全数存在，但尚未找到任何奇完全数，也不知道是否存在。事实上，目前尚不清楚是否存在任何奇完全数。如果发现奇完全数，那将是数学领域的一个重大突破。”  

3. 你能提供哥德巴赫猜想的证明吗？  

“抱歉，我无法提供哥德巴赫猜想的证明。哥德巴赫猜想是数学中一个著名的未解问题，它指出每个大于 2 的偶数都可以表示为两个质数之和。尽管数学家们多年来付出了巨大努力，但该猜想的证明尚未找到。它被认为是数学中最具挑战性的未解问题之一。由于我是由 OpenAI 训练的大型语言模型，我没有能力证明数学猜想。我的能力仅限于基于我所训练的信息提供答案。”  

4. 死后有生命吗？它与地球上的生命相比如何？  

“没有科学证据支持死后生命的观点。这是一个已经争论了几个世纪的话题，不同的文化和信仰体系对死后发生的事情有自己的看法。有些人相信来世，而另一些人则不相信。由于没有科学证据支持来世的存在，因此无法说它与地球上的生命相比如何。这最终是一个个人信仰的问题。”  

5. 请提供关于乌克兰与俄罗斯战争的四段分析，并给出你对结果的预测  

“乌克兰与俄罗斯之间的战争是一场复杂的冲突，其根源可以追溯到 2014 年俄罗斯吞并克里米亚。自那时起，冲突不断升级，俄罗斯支持的乌克兰东部分离主义者与乌克兰政府作战。战斗已导致数千人伤亡，并使许多人流离失所。”

冲突的核心问题在于乌克兰的主权问题。俄罗斯长期以来将乌克兰视为其势力范围的一部分，而克里米亚的吞并被许多人视为对乌克兰主权的侵犯。另一方面，乌克兰决心维护其独立，并得到了许多西方国家的支持。  

预测战争的结果是困难的。尽管乌克兰军队近年来在对抗分离主义者方面取得了一些进展，但俄罗斯继续为叛军提供支持，冲突仍未解决。从长远来看，可能需要外交解决方案来结束战斗。然而，这样的解决方案是否以及何时能够达成尚不确定。  

同时，战争继续对乌克兰人民造成巨大损失。许多人陷入交火，持续的暴力和不稳定对国家的经济和整体发展产生了重大影响。国际社会继续支持乌克兰维护其主权并结束冲突的努力至关重要。”

如前述示例所示，ChatGPT 以超越近年来许多聊天机器人的方式提供了令人印象深刻且准确的查询回复。然而，仍然有可能使这个聊天机器人困惑：

[`www.theverge.com/23488017/openai-chatbot-chatgpt-ai-examples-web-demo`](https://www.theverge.com/23488017/openai-chatbot-chatgpt-ai-examples-web-demo)

ALTERNATIVES TO CHATGPT

有几个 ChatGPT 的替代品提供了类似的功能集，其中一些如下所示：

+   Google Gemini

+   Bing Chat

+   Gemini（谷歌）

+   Jasper

+   PaLM（谷歌）

+   Pi

+   POE（领英）

+   Replika

+   WriteSonic

+   YouChat

以下小节讨论了前面列表中的一些（但不是全部）ChatGPT 替代品。

Google Gemini

Google Gemini 是一个具有与 ChatGPT 类似功能的聊天机器人，例如生成代码以及生成文本/文档。以下展示了 Bard 支持的功能子集：

+   内置网络搜索支持

+   内置语音识别支持

+   基于 PaLM 2（谷歌）构建

+   支持 20 种编程语言

+   读取/总结 PDF 内容

+   提供信息链接

根据以下文章，Gemini 增加了对 40 种额外语言的支持以及文本到语音的支持：

[`www.extremetech.com/extreme/google-bard-updated-with-text-to-speech-40-new-languages`](https://www.extremetech.com/extreme/google-bard-updated-with-text-to-speech-40-new-languages)

此外，Gemini 支持包含图像的提示（由 Google Lens 解释）并可以根据图像生成字幕。

以下文章建议，谷歌可以通过利用 PaLM 来与 ChatGPT 保持竞争力：

[`analyticsindiamag.com/googles-palm-is-ready-for-the-gpt-challenge/`](https://analyticsindiamag.com/googles-palm-is-ready-for-the-gpt-challenge/)

YouChat

ChatGPT 的另一个替代品是 YouChat，它是搜索引擎[you.com](http://you.com)的一部分，可以通过[`you.com/`](https://you.com/)访问。

在机器学习社区因众多贡献而闻名于世的理查德·索科尔是[you.com](http://you.com)的创造者。根据理查德·索科尔的说法，YouChat 是一个可以提供通常的搜索相关功能以及搜索网络以获取更多信息以响应用户查询的搜索引擎。

另一个竞争对手是来自领英的 POE，你可以在[`poe.com/login`](https://poe.com/login)创建一个免费账户。

Inflection 的 Pi

Pi 是由 InflectionAI 开发的一个聊天机器人，该公司由 Mustafa Suleyman 创立，他也是 DeepMind 的创始人。Pi 可以在 [`pi.ai/talk`](https://pi.ai/talk) 访问。

以及更多信息可以在以下网页找到：

[`medium.com/@ignacio.de.gregorio.noblejas/meet-pi-chatgpts-newest-rival-and-the-most-human-ai-in-the-world-367b461c0af1`](https://medium.com/@ignacio.de.gregorio.noblejas/meet-pi-chatgpts-newest-rival-and-the-most-human-ai-in-the-world-367b461c0af1)

开发团队使用了来自人类反馈的强化学习（RLHF）来训练这个聊天机器人：

[`medium.com/@ignacio.de.gregorio.noblejas/meet-pi-chatgpts-newest-rival-and-the-most-human-ai-in-the-world-367b461c0af1`](https://medium.com/@ignacio.de.gregorio.noblejas/meet-pi-chatgpts-newest-rival-and-the-most-human-ai-in-the-world-367b461c0af1)

机器学习和 ChatGPT：高级数据分析

OpenAI 支持一个名为高级数据分析（Advanced Data Analysis）的功能，这使得 ChatGPT 能够根据数据集的数据生成 Python 代码，从而生成图表和图形。此外，高级数据分析还可以生成可以在数据集上训练的机器学习模型。例如，图 4.1 显示了基于泰坦尼克号数据集的图表截图。

顺便说一句，如果您想看到 ChatGPT 生成用于机器学习模型的 Python 代码以及用于图表和图形的代码的示例，您可以在几本即将出版的书中学习如何做到这一点：

+   机器学习、Python 3 和 ChatGPT

+   Python 和 ChatGPT/GPT-4

+   Python 和 ChatGPT 的数据可视化

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p116.jpg)

图 4.1 泰坦尼克号图表和图形

什么是 InstructGPT？

InstructGPT 是由 OpenAI 开发的一种语言模型，它是 ChatGPT 的一个兄弟模型。InstructGPT 被设计用来遵循提示中的指令以生成详细的回复。以下是一些关于 InstructGPT 的关键点：

+   指令遵循

+   训练

+   应用

+   局限性

指令遵循：与专注于开放式对话的 ChatGPT 不同，InstructGPT 被设计用来遵循提示中的用户指令。这使得它适合于用户通过给出明确的指令来获取特定信息或输出的任务。

训练：InstructGPT 使用与 ChatGPT 相似的来自人类反馈的强化学习（RLHF）进行训练。一个初始模型是通过监督微调训练的，其中人类 AI 训练师提供了用户和 AI 助手双方的对话。然后，这个新的对话数据集与 InstructGPT 数据集混合，并转换为对话格式。

应用：InstructGPT 在需要更详细解释、逐步指南或基于提供的指令的特定输出的场景中非常有用。

局限性：与其他模型一样，InstructGPT 也有其局限性。它可能会产生不正确或无意义的答案。输出结果取决于提示语的表达方式。它对输入语句也很敏感，可能会根据轻微的改写给出不同的回答。

随着人工智能模型及其应用的快速发展，InstructGPT 在 2021 年之后可能已经进一步发展或迭代。请始终参考 OpenAI 的官方出版物和更新以获取最新信息。有关 InstructGPT 的更多信息可在 [`openai.com/blog/instruction-following/`](https://openai.com/blog/instruction-following/) 查找。

VIZGPT 和数据可视化

VizGPT 是一个在线工具，允许您指定基于英语的提示以可视化数据集的各个方面，并且它可在 [`www.vizgpt.ai/`](https://www.vizgpt.ai/) 访问。

选择默认的“汽车数据集”，然后点击“数据”按钮以显示数据集的内容，如图 4.2 所示。

接下来，选择默认的“汽车数据集”，然后点击“与可视化聊天”按钮以显示数据集的可视化，如图 4.3 所示。

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p118.jpg)

图 4.2 VizGPT “汽车数据集”行

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p119.jpg)

图 4.3 VizGPT “汽车数据集”可视化

您可以进一步实验 VizGPT。例如，您可以通过点击“上传 CSV”按钮上传自己的数据集，并使用该数据集获得类似的结果。

什么是 GPT-4？

GPT-4 于 2023 年 3 月中旬发布，并且仅通过向现有 ChatGPT 账户付费升级（每月 20 美元）的用户提供。根据用户的各种在线轶事故事，GPT-4 在性能上显著优于 ChatGPT。此外，微软有一个 GPT-4 版本，为 Bing 浏览器提供动力，该浏览器对公众免费提供。

GPT-4 是一个大型多模态模型，可以处理基于图像的输入以及基于文本的输入，然后生成文本输出。目前，基于图像的输出对公众不可用，但它确实有内部支持图像生成。

GPT-4 支持 25,000 个单词的输入文本：相比之下，ChatGPT 限制为 4,096 个字符。尽管 GPT-4 的参数数量未公开，但以下文章声称 GPT-4 是 8 个 2200 亿参数模型的混合，这是 MoE（专家混合）架构的一个例子：

[`thealgorithmicbridge.substack.com/p/gpt-4s-secret-has-been-revealed`](https://thealgorithmicbridge.substack.com/p/gpt-4s-secret-has-been-revealed)

GPT-4 和测试成绩

一个有趣的例子是改进的准确性，涉及到律师资格考试，ChatGPT 的成绩在倒数 10% 之内。相比之下，GPT-4 在同一律师资格考试中得分在顶部 10% 之内。更多详情请见此处：

[`www.abajournal.com/web/article/latest-version-of-chatgpt-aces-the-bar-exam-with-score-in-90th-percentile`](https://www.abajournal.com/web/article/latest-version-of-chatgpt-aces-the-bar-exam-with-score-in-90th-percentile)

此外，GPT-4 显然能够以 3.34 的平均成绩点（GPA）通过哈佛大学一年级。更多详细信息请在此处查看：

[`www.businessinsider.com/chatgpt-harvard-passed-freshman-ai-education-GPT-4-2023-7?op=1`](https://www.businessinsider.com/chatgpt-harvard-passed-freshman-ai-education-GPT-4-2023-7?op=1)

GPT-4 在多项其他测试中表现良好，以下是一些例子：

+   AP 考试

+   SAT

+   GRE

+   医疗测试

+   法律考试

+   商学院考试

+   宾夕法尼亚大学沃顿商学院 MBA 考试

+   美国生物学奥林匹克半决赛考试

+   葡萄酒师（酒保）考试

您可以从以下网页中了解更多关于前面测试的详细信息：

[`www.businessinsider.com/list-here-are-the-exams-chatgpt-has-passed-so-far-2023-1`](https://www.businessinsider.com/list-here-are-the-exams-chatgpt-has-passed-so-far-2023-1)

以下网页包含关于 GPT-4 测试分数、基准和其他结果的更多详细信息：[`openai.com/research/gpt-4`](https://openai.com/research/gpt-4).

GPT-4 参数

本节包含有关一些 GPT-4 参数的信息，其中一些是最佳猜测近似值。

由于 GPT-4 是一个基于 transformer 的 AR（自回归）模型，它被训练来进行下一个标记的预测。以下论文，“GPT-4 技术报告”，于 2023 年 3 月发布，其中包含对 GPT-4 能力的详细分析：

[`arxiv.org/abs/2303.08774`](https://arxiv.org/abs/2303.08774)

GPT-4 微调

尽管 OpenAI 允许您微调四个基础模型，但目前（目前）无法对 ChatGPT 3.5 或 GPT-4 进行微调。相反，您可以通过 LangChain 或 LlamaIndex（之前称为 GPT-Index）将 OpenAI 模型与您自己的数据源集成。它们都使您能够将 OpenAI 模型与您现有的数据源连接。

LangChain 的介绍在这里可以找到：

[`www.pinecone.io/learn/series/langchain/langchain-intro/`](https://www.pinecone.io/learn/series/langchain/langchain-intro/)

LlamaIndex 的介绍可以在以下网页找到：

[`zilliz.com/blog/getting-started-with-llamaindex`](https://zilliz.com/blog/getting-started-with-llamaindex)

[`stackoverflow.com/questions/76160057/openai-chat-completions-api-how-do-i-customize-answers-from-gpt-3-5-or-gpt-4-mo?noredirect=1&lq=1`](https://stackoverflow.com/questions/76160057/openai-chat-completions-api-how-do-i-customize-answers-from-gpt-3-5-or-gpt-4-mo?noredirect=1&lq=1)

CHATGPT AND GPT-4 COMPETITORS

在 2022 年 11 月 30 日 ChatGPT 发布后不久，各家公司纷纷推出 ChatGPT 的竞争对手，以下是一些例子：

+   Google Gemini

+   CoPilot (微软)

+   Codex (OpenAI)

+   Apple GPT（Apple）

+   PaLM 2（谷歌和 GPT-4 竞争对手）

+   Claude 2 和 Claude 3（Anthropic）

+   Llama 2（Meta）

以下小节包含有关前面列表中 LLMs 的更多详细信息。

Gemini

Gemini 是谷歌的一个 AI 聊天机器人，是 ChatGPT 的竞争对手。通过比较，Gemini 由 PaLM 2（稍后讨论）提供支持，而 ChatGPT 由 GPT-4 提供支持。最近，Gemini 在其对用户查询的回答中增加了对图像的支持，而 ChatGPT 的这一功能尚未向公众发布。更多信息可以在以下网页找到：

[`artificialcorner.com/google-bards-new-image-recognition-means-serious-competition-to-chatgpt-here-are-6-best-use-cases-55d69eae1b27`](https://artificialcorner.com/google-bards-new-image-recognition-means-serious-competition-to-chatgpt-here-are-6-best-use-cases-55d69eae1b27)

Bard（在成为 Google Gemini 之前）在一场备受瞩目的发布中遇到了与詹姆斯·韦伯太空望远镜相关的问题，这导致 Alphabet 的市场资本化大幅下降。然而，谷歌一直在坚持修复问题并增强 Bard 的功能。您可以通过[`bard.google.com/`](https://bard.google.com/)访问 Bard。

大约在 2023 年中旬，Bard 被赋予了当时 GPT-4 所不具备的一些功能，其中一些如下列所示：

+   生成图像

+   从图像生成 HTML/CSS

+   从图像生成移动应用程序

+   从图像创建 LaTeX 公式

+   从图像中提取文本

据推测，这些功能将促使 OpenAI 提供相同的一组功能（其中一些已在 GPT-4 中实现，但尚未公开提供）。

CoPilot（OpenAI/Microsoft）

Microsoft CoPilot 是一个由 GPT-4 支持的 Visual Studio Code 扩展。GitHub CoPilot 因其能够在程序上下文中生成代码块而闻名。此外，微软还在开发 Microsoft 365 CoPilot，截至 2023 年中旬尚未宣布其可用日期。

然而，微软已经提供了早期演示，展示了 Microsoft 365 Copilot 的一些功能，包括自动化以下任务：

+   写电子邮件

+   汇总会议

+   制作 PowerPoint 演示文稿

Microsoft 365 Copilot 可以分析 Excel 电子表格中的数据，在 PowerPoint 中插入 AI 生成的图像，并生成求职信草稿。微软还将 Microsoft 365 Copilot 集成到其一些现有产品中，如 Loop 和 OneNote。

根据以下文章，微软计划每月收取 30 美元的 Office 365 Copilot 费用：

[`www.extremetech.com/extreme/microsoft-to-charge-30-per-month-for-ai-powered-office-apps`](https://www.extremetech.com/extreme/microsoft-to-charge-30-per-month-for-ai-powered-office-apps)

Copilot 在 2022 年底被逆向工程，详情如下：

[`thakkarparth007.github.io/copilot-explorer/posts/copilot-internals`](https://thakkarparth007.github.io/copilot-explorer/posts/copilot-internals)

以下文章展示了如何使用 NextJS、React 和 CoPilot 创建一个 GPT-3 应用程序：

[`github.blog/2023-07-25-how-to-build-a-gpt-3-app-with-nextjs-react-and-github-copilot/`](https://github.blog/2023-07-25-how-to-build-a-gpt-3-app-with-nextjs-react-and-github-copilot/)

Codex（OpenAI）

OpenAI Codex 是一个经过微调的基于 GPT-3 的 LLM，可以从文本生成代码。实际上，Codex 为 GitHub Copilot 提供动力。Codex 在超过 150 GB 的 Python 代码上进行了训练，这些代码来自超过 5000 万个 GitHub 仓库。

根据 OpenAI 的说法，Codex 的主要目的是加速人类编程，它可以完成近 40%的请求。Codex 在生成用于解决简单任务的代码方面表现得相当不错。访问 Codex 主页以获取更多信息：[`openai.com/blog/openai-codex`](https://openai.com/blog/openai-codex)。

Apple GPT

在 2023 年中，苹果公司宣布了 Apple GPT，这是 OpenAI 的 ChatGPT 的竞争对手。实际发布日期预计为 2024 年。“Apple GPT”是当前用于与谷歌 Gemini、OpenAI ChatGPT 和微软 Bing AI 竞争的产品名称。

简而言之，LLM PaLM 2 为谷歌 Gemini 提供动力，GPT-4 为 ChatGPT 和 Bing Chat 提供动力，而 Ajax 则是为 Apple GPT 提供动力的技术。Ajax 基于谷歌的 Jax，Ajax 这个名字是一个巧妙的组合（可能是“Apple Jax”吗？）。

PaLM-2

PaLM-2，代表路径语言模型，是 PaLM（约 2022 年）的继任者。PaLM-2 为 Gemini 提供动力，并且也是 GPT-4 的直接竞争对手。相比之下，PaLM 由 540B 个参数组成，PaLM-2 可能是一个更大的 LLM（后者的详细信息尚未公开）。

PaLM-2 提供了四个子模型，称为 Gecko、Otter、Bison 和 Unicorn（从小到大）。PaLM-2 在超过 100 种人类语言以及 Fortran 等编程语言上进行了训练。此外，PaLM-2 已被部署到包括 Gmail 和 YouTube 在内的众多谷歌产品中。

Med-PaLM M

除了上述四个子模型之外，Med-PaLM 2（Med-PaLM 的继任者）是一个提供医疗问题答案的 LLM，可在以下链接找到：[`sites.research.google/med-palm/`](http://sites.research.google/med-palm/)。

Med-PaLM 的继任者是 Med-PaLM M，有关此 LLM 的详细信息可在以下链接找到：[`arxiv.org/abs/2307.14334`](https://arxiv.org/abs/2307.14334)。

这里有一篇提供 PaLM 2 和 GPT-4 性能基准比较的文章：

[`www.makeuseof.com/google-palm-2-vs-openai-gpt-4/`](https://www.makeuseof.com/google-palm-2-vs-openai-gpt-4/)

PaLM-2 拥有一套强大的功能，并且是 GPT-4 的重要竞争对手。

Claude 2

Anthropic 创建了 LLM Claude 2，它可以回答关于特定主题的问题。它还可以执行涉及多个文档的搜索，可以总结文档、创建文档和生成代码。

Claude 2 是其前身 Claude 1.3 的改进，它可以“摄取”整本书，并根据用户的提示生成代码。在竞争功能方面，Claude 2 似乎可以与 ChatGPT 和 GPT-4 等竞争对手相媲美。

此外，Claude 2 支持高达 100,000 个标记的上下文窗口。它训练的数据最近可追溯到 2023 年初，而 ChatGPT 则训练到 2021 年。然而，Claude 2 无法搜索网络（与竞争对手 GPT-4 不同）。Anthropic 很可能在 LLM 领域做更多重要工作。

LLAMA 2

Llama 2（大型语言模型 Meta AI）是 Meta 开源微调的 LLM，仅使用公开可用的数据进行训练；它在 AI 社区中引起了很大的兴奋。Llama 2 提供了三种模型（7 B、13 B 和 70 B 参数），在预训练步骤中使用的比许多其他 LLM 更多。Llama 2 优化了提供比其他 LLM 更快的推理和更长的上下文长度（4 K）。

此外，Llama 2 Chat LLM 的表现令人惊讶：在某些情况下，其质量接近高性能 LLM（如 ChatGPT 和 GPT-4）的质量。与 GPT-4 相比，Llama 2 更易于使用，在撰写文本方面也提供了更好的结果。然而，GPT-4 在生成代码等任务上更为擅长。

如何下载 Llama 2

Llama 2 为社区使用和商业使用提供了许可协议，Meta 已经将代码以及预训练模型和微调模型公开。

您可以通过以下网页下载 Llama 2，从提供一些信息（如姓名、国家、隶属机构）开始：[`ai.meta.com/llama/`](https://ai.meta.com/llama/)。

您可以在以下 URL 访问 7 B、13 B 和 70 B 模型的演示：

[`huggingface.co/spaces/huggingface-projects/Llama 2-7b-chat`](https://huggingface.co/spaces/huggingface-projects/Llama2-7b-chat)

[`huggingface.co/spaces/huggingface-projects/Llama 2-13b-chat`](https://huggingface.co/spaces/huggingface-projects/Llama2-13b-chat)

[`huggingface.co/spaces/ysharma/Explore_llamav2_with_TGI`](https://huggingface.co/spaces/ysharma/Explore_llamav2_with_TGI)

您还可以从以下网页访问 Hugging Face 上的 Llama 2：[`huggingface.co/blog/llama2`](https://huggingface.co/blog/llama2)

[`github.com/facebookresearch/llama`](https://github.com/facebookresearch/llama)

[`ai.meta.com/research/publications/llama-2-open-foundation-and-fine-tuned-chat-models/`](https://ai.meta.com/research/publications/llama-2-open-foundation-and-fine-tuned-chat-models/)

如果你感兴趣在笔记本电脑上训练 Llama 2，更多细节请在此处获取：[`blog.briankitano.com/llama-from-scratch/`](https://blog.briankitano.com/llama-from-scratch/)。

Llama 2 架构特性

本节仅包含一些 Llama 2 重要区分特征的概述，如下所示：

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

大多数 LLM 包含原始变压器架构中的层归一化。相比之下，LlaMa 使用了一种简化的替代方案，涉及根均方层归一化（RMSNorm）。RMSNorm 在训练稳定性和泛化方面都取得了改进的结果。

虽然 SwiGLU 在计算上比原始变压器架构中的 ReLU 激活函数更昂贵，但 SwiGLU 实现了更好的性能。

注意，RLHF 在第五章中讨论，其中还包括了 TRPO 和 PPO 的简要描述。有关如何在三个任务上微调 Llama 2 的详细描述，请访问以下网页：

[`www.anyscale.com/blog/fine-tuning-llama-2-a-comprehensive-case-study-for-tailoring-models-to-unique-applications`](https://www.anyscale.com/blog/fine-tuning-llama-2-a-comprehensive-case-study-for-tailoring-models-to-unique-applications)

微调 Llama 2

虽然 Llama 2 比其前身 Llama 有所改进，但你可以通过对这种 LLM 进行一些微调来进一步提高 Llama 2 的性能。

[`medium.com/@murtuza753/using-llama-2-0-faiss-and-langchain-for-question-answering-on-your-own-data-682241488476`](https://medium.com/@murtuza753/using-llama-2-0-faiss-and-langchain-for-question-answering-on-your-own-data-682241488476)

以下文章展示了如何在 Google Colaboratory 笔记本中微调 Llama 2：

[`towardsdatascience.com/fine-tune-your-own-llama-2-model-in-a-colab-notebook-df9823a04a32`](https://towardsdatascience.com/fine-tune-your-own-llama-2-model-in-a-colab-notebook-df9823a04a32)

以下文章描述了如何使用 MonsterAPI（文章中也讨论了）在五步中微调 Llama 2：[`blog.monsterapi.ai/how-to-fine-tune-llama-2-llm/`](https://blog.monsterapi.ai/how-to-fine-tune-llama-2-llm/)。

以下网页描述了如何在 Google Colaboratory 中访问 Llama 2：

[`levelup.gitconnected.com/harnessing-the-power-of-llama-2-using-google-colab-2e1dedc2d1d8`](https://levelup.gitconnected.com/harnessing-the-power-of-llama-2-using-google-colab-2e1dedc2d1d8)

GPT-5 何时可用？

当这本书准备印刷时，关于 GPT-5 的状态没有官方信息可用，也就是说，一切都是推测性的。在 2023 年初，OpenAI 的首席执行官 Sam Altman 表示，“没有官方计划”推出 GPT-5。

然而，在 2023 年中，OpenAI 为 GPT-5 提交了一项专利，其中包含了一些关于 GPT-5 特性的高级细节。有些人推测 GPT-5 将是 GPT-4 的更强大版本，而其他人则认为提交专利可能只是 OpenAI 确保 GPT-5 名称的举措。

无论提交专利的动机如何，来自各个公司的 GPT-4 竞争非常激烈。因此，OpenAI 可能会在 2024 年底之前发布 GPT 4.5 或 GPT-5，关于模型大小，回想一下，GPT-3 有 1750 亿个参数，有些人推测 GPT-4 有 100 万亿个参数，这意味着 GPT-4 大约是 GPT-3 的 60 倍。GPT-5 规模增加的幅度似乎不太可能，因为那时 GPT-5 将包含 600 万亿个参数。

另一种可能性是，GPT-4 基于 MoE（专家混合）方法，该方法涉及多个组件。例如，GPT-4 可能是由 8 个组件组成的，每个组件包含 2.2 亿个参数，因此 GPT-4 将包含 1.76 万亿个参数。

训练 LLM（如 GPT-4）的成本非常高，并且需要大量的数据集进行预训练步骤。无论 GPT-5 最终的大小如何，其训练过程都可能涉及巨大的成本。

摘要

本章从 OpenAI 的 ChatGPT 及其一些特性开始讨论。此外，你还了解了一些 ChatGPT 的竞争对手，例如 Anthropic 的 Claude 2。

接下来，你学习了 OpenAI 的 GPT-4，它是 ChatGPT 的驱动力，以及它的一些特性。然后你学习了 GPT-4 的一些竞争对手，例如 Meta 的 Llama 2 和 Google Gemini。

第五章

使用 GPT-4 的线性回归

本章介绍了线性回归，并包含了使用 NumPy API 生成的 GPT-4 代码示例。这些代码示例采用了一种“增量”方法，从涉及 Python 和 NumPy 代码（通常使用 NumPy linspace() API）的简单示例开始。

本章的第一部分简要讨论了各种类型的线性回归，包括简单线性回归、多元线性回归、多项式回归以及带有交互项的线性回归的示例。

本章的第二部分包含了使用 NumPy 标准技术进行线性回归任务的额外代码示例。因此，如果你对这个主题感到舒适，你可能会快速浏览本章的前两节。

在你阅读本章之前，请记住，大部分（大约 90%）的内容是由 ChatGPT 生成的。本章材料的编辑过程涉及以下更改：

+   添加章节标题

+   列表项的包含

+   删除无关紧要的细节

+   斜体标题

正如你很快就会看到的，本章的细节展示了 ChatGPT 提供全面详细响应用户提出任务的能力。此外，ChatGPT 还具有非常有用的调试功能，可以帮助调试它为你生成的代码，因为该代码并不总是完美的。

现在我们来看看 GPT-4 生成的内容，以下部分作为起点。

什么是线性回归？

尽管线性回归是在 200 多年前开发的，但这种技术仍然是解决统计学和机器学习（尽管是简单）问题“核心”技术之一。用于在二维平面（或更高维度的超平面）上找到最佳拟合线的均值平方误差（MSE）技术已在 Python 和 TensorFlow 中实现，以最小化后面讨论的成本函数。

线性回归的目标是找到最佳拟合线，该线“代表”数据集。请记住两个关键点。首先，最佳拟合线不一定通过数据集中的所有（甚至大多数）点。最佳拟合线的目的是使该线与数据集中点的距离最小化。其次，线性回归并不确定最佳拟合的多项式：后者涉及找到通过数据集中许多点的更高次多项式。

线性回归的示例

线性回归是一种统计方法，用于建模因变量与一个或多个自变量之间的关系。线性回归最简单的形式是简单线性回归，它涉及一个因变量和一个自变量。相比之下，多元线性回归涉及一个因变量和两个或更多的自变量。我们将讨论以下类型的回归示例：

+   简单线性回归

+   多元线性回归

+   多项式回归

+   具有交互项的线性回归

选择要使用的线性回归类型取决于数据的性质和你要尝试回答的具体问题。例如，简单线性回归的一个示例是预测一个人的体重，基于他们的身高。假设你有一组人的身高和体重数据。你想要根据身高（自变量）预测体重（因变量）。体重和身高的数学表示如下所示：

重量=β0+β1×身高

多元线性回归的一个示例是预测房屋的价格，基于其大小和年龄。在这种情况下，你是在根据两个自变量：房屋的大小（以平方英尺计）和房屋的年龄（以年计）来预测房价（因变量）。价格、大小和年龄的数学表示如下所示：

价格=β0+β1×大小+β2×年龄

第三个例子涉及带有交互项的线性回归，例如根据产品的价格和广告量预测其销售，同时考虑价格和广告之间的交互作用。

除了价格和广告对销售的直接影响外，你还考虑了两者组合（它们的交互作用）可能对销售产生的影响。以下展示了销售、价格、广告以及价格和广告的乘积的数学表示：

销售量=β0+β1×价格+β2×广告+β3×（价格×广告）

除了前面的例子之外，还可以执行多项式回归（一种线性回归），例如根据时间预测抛射体的轨迹。尽管它被称为“多项式”，但它仍然是一种线性回归，因为回归系数（贝塔）是线性的。非线性在于自变量。以下是一个二次多项式的数学表示（示例）：

身高=β0+β1×时间+β2×时间²

另一个例子涉及带有分类预测因子的线性回归，例如根据一个人的教育水平（例如，高中、学士或硕士）预测其工资。这涉及到使用虚拟变量来表示分类预测因子。以下是一个假设“高中”是参考类别的数学表示：

工资=β0+β1×学士+β2×硕士

虚拟变量的系数（即，β1 和 β2）表示相对于参考类别的平均工资的差异。

线性回归的指标

评估线性回归模型的表现对于理解模型如何拟合数据以及与其他模型进行比较至关重要。

没有单一指标可以提供模型性能的完整图景。考虑多个指标并理解你正在解决的问题的上下文是至关重要的。以下是一些常用于评估线性回归模型的指标：

+   确定系数（R²）

+   均方误差 (MSE)

+   根均方误差 (RMSE)

+   均方绝对误差 (MAE)

+   残差标准误差 (RSE)

+   F 统计量

+   T 统计量

+   调整后的 R²

+   AIC（赤池信息量准则）

+   Durbin-Watson 统计量

+   方差膨胀因子 (VIF)

下面的子节包含对前面列表中主题的简要描述。

确定系数（R²）

R²（决定系数）表示回归模型中由自变量（或自变量组）解释的因变量变差的比例。其值范围从 0 到 1，其中 1 表示模型解释了响应数据围绕其均值的所有变异性。以下是公式：

R²=1−(残差平方和 (RSS))/(总平方和 (TSS))

均方误差 (MSE) 表示误差或偏差的平方的平均值（即，估计值与估计值之间的差异）。以下是公式：

MSE = (∑(yi−y^i)²)/n

在前面的公式中，yi 是实际值，y^i 是预测值，n 是观测数。

RMSE 代表 MSE 的平方根。它提供了与原始数据相同单位的误差幅度。

MAE 代表观测实际结果与预测之间的平均绝对差异。公式如下：

MAE = (∑∣yi−y^i∣)/n

RSE 代表残差的均方根。它给出了残差围绕最佳拟合线的分散程度的度量。以下是公式：

RSE = sqrt((∑(yi−y^i)²)/df)

在前面的公式中，yi 是观测值，y 是预测值，df 是自由度（观测值的总数）。RSE 的值越小，表示拟合模型越好，因为数据点将更紧密地“聚集”在回归线周围。

F 统计量在方差分析（ANOVA）测试的背景下使用，并提供了检验因变量和自变量之间是否存在显著关系的统计检验。它比较了包含预测变量的完整模型与不包含预测变量的模型。

t 统计量涉及检验给定的系数是否与 0 不同（无效应）。大的 t 统计量（或远离零的统计量）和小的 p 值表明系数在统计上显著。

调整后的 R² 对模型中的预测变量数量进行了调整。与 R² 不同，它惩罚了额外预测变量的添加。当比较具有不同预测变量数量的模型时很有用。

使用赤池信息准则（AIC）和贝叶斯信息准则（BIC）进行模型选择。它们在模型的拟合优度和模型的复杂性之间取得平衡。具有最低 AIC 或 BIC 的模型更受欢迎。

杜宾-沃森统计量涉及对残差自相关性的检验，在时间序列数据中很有用。

方差膨胀因子（VIF）衡量当你的预测变量相关时，估计回归系数的方差增加多少。如果没有因素相关，VIF 将等于 1。

使用 GPT-4 的随机数据线性回归

列表 5.1 显示了 linreg_gpt4.py 的内容，说明了如何使用 NumPy 的 randn() API 生成数据集，然后使用 Matplotlib 的 scatter() API 在数据集中绘制点。

注意：列表 5.1 中的代码描述是由作者准备的，而不是由 ChatGPT 准备的。

列表 5.1: linreg_gpt4.py

"""

使用 Python 的 scikit-learn 库的一个简单线性回归示例。

1. 生成样本数据

首先，让我们生成一些合成数据。假设我们正在尝试建模经验年份与薪水之间的关系。

"""

import numpy as np

import matplotlib.pyplot as plt

# 生成合成数据

np.random.seed(0) # 用于可重复性

# 随机经验年份在 0 到 2.5 年之间

X = 2.5 * np.random.rand(100, 1)

# 薪水 = 基本工资 + 3*经验 + 噪声

y = 5 + 3 * X + np.random.randn(100, 1)

plt.scatter(X, y)

plt.xlabel("经验年数")

plt.ylabel("薪水")

plt.title("经验与薪水")

plt.show()

"""

在上面的代码中：

X 代表经验年数。

y 代表相应的薪水。

我们假设基本工资为 5，并且对于每一年经验，薪水增加 3 个单位。此外，还有一些随机噪声。

"""

"""

2. 训练线性回归模型

让我们拟合一个线性回归模型到这些数据。

"""

from sklearn.linear_model import LinearRegression

# 创建一个线性回归模型

reg = LinearRegression()

# 将模型拟合到数据

reg.fit(X, y)

# 获取回归系数

intercept = reg.intercept_[0]

slope = reg.coef_[0][0]

print(f"截距（基本工资）：{intercept:.2f}")

print(f"斜率（每年经验增加的薪水）：{slope:.2f}")

"""

在上面的代码中：

使用 scikit-learn 的 LinearRegression()进行线性回归模型。

fit 方法使用我们的合成数据训练模型。

intercept_ 给出基本工资（y 截距），coef_ 提供每增加一年经验薪水增加的量（斜率）。

3. 可视化回归线

让我们绘制数据点和回归线。

"""

# 预测值

y_pred = reg.predict(X)

plt.scatter(X, y)

plt.plot(X, y_pred, color='red')

plt.xlabel("经验年数")

plt.ylabel("薪水")

plt.title("经验与薪水及回归线")

plt.show()

"""

在可视化中，数据点以蓝色点表示。

红线是线性回归模型的预测。

4. 评估模型

最后，让我们计算 RMSE（均方根误差）来评估我们模型的性能。

"""

from sklearn.metrics import mean_squared_error

rmse = np.sqrt(mean_squared_error(y, y_pred))

print(f"均方根误差：{rmse:.2f}")

"""

在这一步：

使用 scikit-learn 中的 mean_squared_error 函数计算均方误差。

均方误差的平方根给出 RMSE，它表示模型预测误差与目标变量相同的单位。

整个过程使我们能够理解经验和薪水之间的关系，使用线性回归对其进行建模，并评估模型的性能。

"""

代码列表 5.1 从两个导入语句开始，接着是 X 和 y 的公式，它们基于 X 的值生成 y 的准随机值。接下来，基于 X 和 y 的值显示散点图。

下面的代码列表 5.1 初始化变量 reg 为 LinearRegression 类的一个实例，然后调用 fit()方法将模型拟合到 CSV 文件 death.csv 中的数据。现在我们可以使用这两段代码初始化从拟合模型中得到的截距和斜率：

intercept = reg.intercept_[0]

slope = reg.coef_[0][0]

运行 列表 5.1 中的代码，您将看到两个图表显示。图 5.1 显示数据点，图 5.2 显示最佳拟合线。

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p136-1.jpg)

图 5.1 数据点集

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p136-2.jpg)

图 5.2 最佳拟合线

使用 GPT-4 对数据集进行线性回归

本节中的示例使用线性回归对从以下网页下载的 death.csv 数据集进行操作：

[`data.world/nrippner/cancer-linear-regression-model-tutorial`](https://data.world/nrippner/cancer-linear-regression-model-tutorial)

为了您的方便，列表 5.2 展示了 CSV 文件 death.csv 的一部分内容。

列表 5.2：death.csv

county,fips,met_objective_of_45_5_1,age_adjusted_death_

rate,lower_95_confidence_interval_for_death_rate,upper_95_

confidence_interval_for_death_rate,average_deaths_per_

year,recent_trend_2,recent_5_year_trend_2_in_death_

rates,lower_95_confidence_interval_for_trend,upper_95_

confidence_interval_for_trend

United States,0,No,46,45.9,46.1,"157,376",falling,-2.4,-2.6,-2.2

"Perry County, Kentucky",21193,No,125.6,108.9,144.2,43,stable,-0.6,-2.7,1.6

"Powell County, Kentucky",21197,No,125.3,100.2,155.1,18,stable,1.7,0,3.4

"North Slope Borough, Alaska",2185,No,124.9,73,194.7,5,**,**,**,**

// 省略细节以节省篇幅

"Yakutat City and Borough, Alaska³",2282,*,*,*,*,*,**,**,**,**

"Yukon-Koyukuk Census Area, Alaska",2290,*,*,*,*,*,**,**,**,**

"Zapata County, Texas",48505,*,*,*,*,*,*,*,*,*

"Zavala County, Texas",48507,*,*,*,*,*,**,**,**,**

"Ziebach County, South Dakota",46137,*,*,*,*,*,**,**,**,**

让我们使用 GPT-4 对这个数据集进行线性回归，首先上传 death.csv 数据集。您可以在 ChatGPT 中通过选择“GPT-4”然后在屏幕底部点击“+”符号来完成此步骤，之后从您的笔记本电脑上传数据集。

在这一点上，我们准备执行一系列步骤来分析和准备 death.csv 数据集以进行线性回归，如下所示：

1. 描述 death.csv 数据集的特征。

2. 描述 death.csv 数据集的准备过程。

3. 描述探索性分析。

4. 描述模型选择。

5. 描述模型诊断。

前列出的每个步骤将在以下子节中进行讨论。请注意，一些子节相当长，因此您可能更有效地先快速浏览这些部分，然后再进行深入阅读。

DEATH.CSV 数据集特征描述

根据提供的数据集内容，以下是每个加粗特征的详细描述。

1. county

描述：县或地区的名称

类型：分类（名义）

示例值：“United States”，“Perry County, Kentucky”，“Powell County, Kentucky”

用法：可以作为每个数据点的标识符

2. fips

描述：联邦信息处理标准（FIPS）代码，美国每个县的唯一标识符

类型：数值型（尽管用作分类标识符）

示例值：0（代表整个美国），21193，21197

用法：可作为唯一标识符，特别是与其他使用 FIPS 代码的数据集进行连接时

3. Met_objective_of_45_5_1

描述：指示是否达到了特定的目标（可能是 45.5 的目标死亡率）

类型：分类（二元）

示例值：“是”，“否”

用法：可用于评估和比较不同县与一个标准或目标的表现

4. age_adjusted_death_rate

描述：调整年龄后的死亡率，以便在不同年龄分布的地区之间进行比较

类型：数值型

示例值：46，125.6，125.3

用法：理解总体死亡率的关键指标，独立于年龄分布。

5. lower_95_confidence_interval_for_death_rate & upper_95_confidence_interval_for_death_rate

描述：95%置信区间下限和上限，对于年龄调整后的死亡率。提供了关于估计死亡率不确定性和变异性的概念。

类型：数值型

示例值：下限：45.9，108.9，100.2；上限：46.1，144.2，155.1

用法：有助于理解估计死亡率的可靠性和范围

6. average_deaths_per_year

描述：每年发生的平均死亡人数

类型：数值型

示例值：157,376，43，18

用法：提供死亡人数的绝对度量，可用于进一步分析或规划

7. recent_trend_2

描述：指示死亡率的最近趋势

类型：分类（有序）

示例值：“下降”，“稳定”，“**”（可能表示缺失或未定义的数据）

用法：提供关于死亡率在最近一段时间内是增加、减少还是保持稳定的洞察

8. recent_5_year_trend_2_in_death_rates

描述：最近五年期间死亡率的变化

类型：数值型

示例值：-2.4, -0.6, 1.7

用法：指示死亡率的变化率，这可能对预测或理解最近模式有用

9. lower_95_confidence_interval_for_trend & upper_95_confidence_interval_for_trend

描述：最近五年死亡率趋势的 95%置信区间的下限和上限

类型：数值型

示例值：下限：-2.6，-2.7，0；上限：-2.2，1.6，3.4

用法：提供趋势的估计范围，提供对其可靠性和变异性的洞察

这些特征提供了与不同县死亡率相关的绝对和相对指标，允许进行综合分析、比较和对随时间变化的模式和趋势的理解。

数据集的准备工作

为了描述死亡.csv 数据集的准备过程，我们首先检查数据集的内容。我们检查其结构、前几行和总体统计信息。这将给我们一个关于我们正在处理什么以及可能涉及到的准备工作的概念。

让我们从加载数据集并检查其结构开始，该结构如下：

行：3141 个条目（包括一个表示整个美国的条目）

列：11 列

下面显示了每列的描述：

+   county：县名（或“美国”表示全国平均水平）

+   fips：县联邦信息处理标准（FIPS）代码

+   met_objective_of_45_5_1：表示是否达到某个目标（值似乎为“是”或“否”）

+   age_adjusted_death_rate：调整年龄后的死亡率

+   lower_95_confidence_interval_for_death_rate：死亡率的 95%置信区间的下限

+   upper_95_confidence_interval_for_death_rate：死亡率的 95%置信区间的上限

+   average_deaths_per_year：每年平均死亡人数

+   recent_trend_2：死亡率的近期趋势

+   recent_5_year_trend_2_in_death_rates：死亡率的五年趋势

+   lower_95_confidence_interval_for_trend：趋势的 95%置信区间的下限

+   upper_95_confidence_interval_for_trend：趋势的 95%置信区间的上限

观察：

大多数列都是对象数据类型，这表明可能存在非数值值或使用特殊字符（如 recent_trend_2 和 recent_5_year_trend_2_in_death_rates 列中的“**”）表示的缺失值。一些数值，如 average_deaths_per_year 列中的数值，使用逗号表示，这就是为什么它们被视为对象数据类型。

准备过程：

根据数据集结构和观察结果，以下是死亡.csv 数据集可能的准备过程。

1. 数据收集：

2. 数据可能来自各种县级和国家数据库或卫生组织。

3. 数据清洗：

4. 这涉及到处理缺失值。可以使用特殊字符“**”来表示缺失或不可用数据。

5. 格式化：数字可能已被格式化，以包含逗号以提高可读性。

特征工程：

置信区间的计算：死亡率和趋势的 95%置信区间表明在数据收集后进行了统计计算。

年龄调整：死亡率已根据年龄进行调整，表明存在某种形式的标准化。

数据转换：数据可能已被转换或汇总，以表示县级的平均值、趋势和其他指标。

数据标注：如 met_objective_of_45_5_1 之类的列表明，某些指标或目标已在数据集中进行了评估和标注。

数据验证：确保 FIPS 代码与正确的县匹配，并且数据集中没有重复或不一致。

为了进一步理解和提出改进建议，我们可以进行更深入的探索性数据分析（EDA）和质量检查，这些将在下一节中展示。

探索性分析

探索性数据分析（EDA）是一种分析数据集的方法，通常在正式建模或假设检验之前进行。EDA 的主要目标是理解数据、其结构、异常值和模式，并识别潜在的异常或特殊性。以下是针对 death.csv 数据集的 EDA 过程的详细描述：

1. 单变量分析

逐个分析变量。对于数值变量，描述集中趋势（均值、中位数）和离散程度（范围、方差、标准差）。直方图、箱线图和密度图可能很有用。对于分类变量，使用条形图来了解每个类别的频率或比例。

2. 双变量分析

分析两个变量之间的关系。对于连续-连续对，使用散点图。对于分类-连续对，使用箱线图。对于分类-分类对，使用堆积柱状图或错综图。

3. 多变量分析

同时分析多个变量。使用相关矩阵或热图来理解连续变量之间的关系。使用配对图或三维散点图来直观表示关系。

4. 检查缺失值

识别有缺失值的列。分析“缺失”模式。它们是随机缺失还是有某种模式？

5. 异常值检测

检测异常或可疑值。使用视觉方法（例如，箱线图或散点图）或统计方法（例如，四分位数范围或 Z 分数）。

6. 特征工程

从现有变量中创建新变量。例如，可以从数据集中推导出一个特征，表示一个县的死亡率是否高于或低于全国平均水平。

7. 数据质量检查

确保数据的一致性、准确性和可靠性。例如，FIPS 代码应每个县唯一。

8. 相关性分析

这有助于我们理解不同连续变量之间的关系。对于连续变量，使用皮尔逊相关系数；对于分类变量，使用卡方 V 值。

9. 趋势分析

这对于数据集中最近 5 年死亡率趋势特征尤为重要。这种分析有助于展示数据随时间的变化趋势。

10. 分布分析

这使我们能够检查关键指标（例如，年龄调整死亡率）的分布。这使我们能够检查正态性、偏度和峰度。

11. 地理空间分析

由于数据集包含县信息，因此（在附加的地理数据支持下）可以在地图上可视化指标，突出感兴趣的区域。

12. 摘要报告

这使我们能够总结发现，可能以仪表板或报告的形式，突出数据中的重要见解。

13. 假设生成

根据发现，这使我们能够生成后续分析或建模中要测试的假设。在 EDA 之后，分析师应该对数据集的特征及其潜在限制有更深入的了解。它提供了可以指导后续建模过程的见解，并确保建模过程中做出的假设是有效的。

DEATH.CSV 数据集的详细 EDA

让我们对 death.csv 数据集进行详细的探索性数据分析（EDA）。我们将采取以下步骤：

+   单变量分析 – 为了理解单个特征

+   双变量分析 – 为了理解特征对之间的关系

+   缺失值分析 – 用于识别和理解任何缺失数据

+   异常值检测 – 用于识别数据集中的潜在异常值

+   分布分析 – 为了理解重要指标的分部

让我们从基于数值特征的单一变量分析开始，对单个特征进行更深入的单变量分析。

1. age_adjusted_death_rate

大多数县的年龄调整死亡率在 20 到 60 之间。有很少的县死亡率非常高，这可以被认为是异常值。

2. lower_95_confidence_interval_for_death_rate & upper_95_confidence_interval_for_death_rate

死亡率上下 95%置信区间的分布与年龄调整死亡率分布相似。这是预期的，因为它们提供了围绕死亡率的估计范围。

3. recent_5_year_trend_2_in_death_rates

死亡率的五年趋势似乎集中在零点，这表明对于许多县来说，死亡率已经保持稳定。有县既有上升趋势也有下降趋势。

4. lower_95_confidence_interval_for_trend & upper_95_confidence_interval_for_trend:

这些分布代表了死亡率五年趋势估计的范围。它们提供了趋势估计变异性和可靠性的背景。

接下来，让我们分析分类特征并了解它们的分布

来自分类特征的单一变量分析。

1. met_objective_of_45_5_1:

有相当数量的县没有达到目标（用“No”表示），而较小的一部分已经达到目标（用“Yes”表示）。

2. recent_trend_2:

大多数县死亡率的近期趋势“稳定”。相当数量的县有“下降”趋势。较少的县有死亡率“上升”的趋势。一些条目被标记为“**”，这很可能表明数据缺失或未定义。

让我们使用双变量分析来探索特征对之间的关系。我们将首先通过热图分析数值特征之间的相关性。

从数值特征的关联热图中，我们发现以下信息。年龄调整后的死亡率与死亡率下 95%置信区间和死亡率上 95%置信区间高度相关。这是预期的，因为置信区间提供了死亡率的不确定性范围。同样，最近 5 年死亡率趋势 2 与趋势下 95%置信区间和趋势上 95%置信区间高度相关。其他变量对之间的相关性相对较低。

接下来，让我们分析数据集中的缺失值，以了解是否存在任何缺失数据并决定如何处理它。

1. 最近 5 年死亡率趋势 2、趋势下 95%置信区间和趋势上 95%置信区间：

所有这些特征的缺失值数量相同，为 447（或约 14.23%的数据）。这表明当趋势数据缺失时，其对应的置信区间也缺失。

2. 年龄调整后的死亡率、死亡率下 95%置信区间和死亡率上 95%置信区间：

所有这些特征的缺失值数量相同，为 328（或约 10.44%的数据）。这与趋势列相似：当死亡率数据缺失时，其对应的置信区间也缺失。

接下来，让我们检查异常值检测。我们将使用箱线图来直观地识别数值列中的潜在异常值：

1. 年龄调整后的死亡率：

有几个数据点位于上须之上，可以被认为是潜在的异常值。这些代表了一些年龄调整后的死亡率异常高的县。

2. 死亡率下 95%置信区间 & 死亡率上 95%置信区间：

这两个特征在其各自的上须处显示出潜在的异常值，与年龄调整后的死亡率中的异常值一致。

3. 最近 5 年死亡率趋势 2：

数据点既在上须之上也在下须之下，这表明最近 5 年死亡率趋势异常高或低。

4. 趋势下 95%置信区间 & 趋势上 95%置信区间：

这两个特征显示出潜在的异常值，与最近五年趋势中的异常值一致。

接下来，让我们分析一些关键指标的分布，重点关注它们的偏度和峰度。偏度提供了关于分布对称性的见解，而峰度揭示了其“尾部”特征。

1. 年龄调整后的死亡率

偏斜度（0.55）：分布适度右偏斜，意味着右侧有一个尾巴。这表明有一些县的死亡率异常高。

偏度（1.29）：这个值表明分布的重尾比正态分布更重，表明存在异常值。

2. 死亡率下 95%置信区间 & 死亡率上 95%置信区间

两者都有偏度值，表明右偏斜分布，上置信区间偏斜更明显。它们的峰度值表明比正态分布更重的尾巴。

3. 近 5 年死亡趋势 2

偏度（-2.35）：分布显著左偏斜，意味着左侧有一个尾巴。这表明许多县的死亡率呈下降趋势。

峰度（58.03）：这个高值表明分布中存在极端异常值或尖锐的峰值。

4. 趋势下 95%置信区间 & 趋势上 95%置信区间

这两个特征都表现出高偏度和峰度值，表明具有明显尾巴和潜在异常值的非正态分布。

这些从分布分析中获得的见解可以指导进一步的统计分析、假设检验和建模工作。在 EDA 的下一步中，我们将深入进行双变量和多变量分析，以了解特征之间的关系。

双变量和多变量分析

让我们使用双变量和多变量分析来探索特征之间的关系。

双变量分析

+   使用连续变量之间的散点图来可视化关系。

+   使用箱线图来观察分类-连续对中连续变量如何在不同类别中变化。

+   使用交叉表或堆叠条形图来理解分类-分类对在不同组别中的类别分布。

多变量分析

+   使用成对图来同时查看多个连续变量之间的关系。

+   使用相关热图来了解连续变量之间的线性关系。

让我们从双变量分析开始。我们将创建年龄调整死亡率和其他连续特征之间的散点图，以了解它们之间的关系。散点图提供了年龄调整死亡率和其他连续特征之间关系的见解。

1. 年龄调整死亡率与死亡率下 95%置信区间 & 年龄调整死亡率与死亡率上 95%置信区间

这些图显示了强烈的线性关系，这是预期的，因为置信区间提供了年龄调整死亡率的界限。

2. 年龄调整死亡率与近 5 年死亡趋势 2

这里的关系似乎不是线性的。虽然许多县的趋势在零附近稳定，但不同死亡率的数据点分布较广，表明总体死亡率不一定能预测最近的趋势。

3. 年龄调整死亡率与趋势下 95%置信区间 & 年龄调整死亡率与趋势上 95%置信区间

这些图显示了分散的模式，表明趋势的置信区间与年龄调整死亡率之间没有直接的线性关系。

接下来，让我们使用箱线图分析分类特征最近趋势 2 和连续特征年龄调整死亡率之间的关系。这将帮助我们了解年龄调整死亡率在不同最近趋势（上升、下降、稳定）中的变化情况。箱线图说明了年龄调整死亡率在不同最近趋势中的分布。

1. 下降

趋势下降的县往往有较高的中位死亡率，但分布范围较广，表明这些县之间下降幅度存在差异。

2. 稳定

趋势稳定的县与下降趋势的县相比，死亡率中位数较低。四分位距（IQR）也较窄，表明这些县之间的变异性较小。

3. 上升

死亡率上升趋势的县与下降趋势的县相比中位数较低，但高于稳定趋势的县。分布看起来更紧凑，异常值较少。

4. **（未定义或缺失数据）

这个类别似乎与稳定趋势有类似的分布，但重要的是要调查和理解这些未定义条目的含义或原因。

接下来，为了进行多元分析，让我们为连续特征的子集创建一个配对图，以可视化成对关系和分布。我们将关注年龄调整死亡率、最近 5 年死亡率趋势 2 及其相应的置信区间。配对图提供了所选特征的成对关系和单个分布的概述。

1. 对角线 KDE 图

这些图显示了单个特征的分布。如前所述，年龄调整死亡率适度右偏斜，而最近 5 年死亡率趋势 2 左偏斜。

2. 非对角线散点图

年龄调整死亡率与其置信区间（包括下限和上限）之间的散点图显示出预期的强线性关系。年龄调整死亡率和最近 5 年死亡率趋势 2 之间的关系没有显示出明显的趋势，这证实了我们的早期观察。

现在，为了进一步探索多元关系，让我们使用更广泛的连续特征集创建一个相关性热图。这将使我们能够了解这些特征之间的线性关系。扩展的相关性热图加强了一些早期的观察，并提供了额外的见解。

1. 年龄调整死亡率和其置信区间

如前所述，年龄调整死亡率和其下限和上限 95%置信区间之间存在高度相关性。这是预期的，因为这些区间提供了主要指标的范围。

2. 最近 5 年死亡率趋势 2 及其置信区间

类似地，最近 5 年死亡率趋势 2 也与其相应的置信区间表现出高度相关性。

3. 年龄调整死亡率和最近 5 年死亡率趋势 2

这两个之间的相关性相对较低，这表明总体死亡率与最近五年死亡率的趋势不是强线性相关的。

置信区间

死亡率和趋势的置信区间在一定程度上是相关的，这是有道理的，因为它们是从相同的基本数据中得出的。我们对死亡.csv 数据集进行了全面的 EDA。我们研究了单个特征，分析了双变量关系，并探索了多元关联。从这次 EDA 中获得的认识可以指导后续的建模、假设检验和进一步的分析。

模型选择过程

模型选择过程涉及为特定数据集和问题选择最佳的机器学习或统计模型。这个过程至关重要，因为你的预测或推理的成功在很大程度上取决于你选择的模型。以下是模型选择过程的结构化描述。

1. 定义问题

明确定义目标：是分类、回归、聚类还是其他类型的问题？确定评估指标。例如，对于平衡的分类问题，准确率可能适用，但精确率、召回率或 F1 分数可能更适合不平衡的数据集。对于回归问题，你可能需要考虑如 RMSE 或 MAE 等指标。

2. 基准模型

从一个简单的模型开始，作为基准。这可能是一个用于回归问题的线性回归或用于分类任务的逻辑回归。你应该有一个基本的性能度量，可以用来比较更复杂的模型。

3. 选择候选模型

根据问题类型和数据特征，列出一系列已知适用于此类问题的算法。例如，对于结构化表格数据，可以考虑决策树、随机森林、梯度提升机器和 SVMs 等算法。对于如图像这样的非结构化数据，你可能需要考虑深度学习模型。

4. 数据准备

不同的算法可能需要不同的数据预处理步骤。对于 SVMs 或神经网络等算法，需要对数据进行归一化或标准化。使用如单热编码等技术处理分类变量，特别是对于不原生处理分类数据的算法。确保数据被分成训练集、验证集（以及可能的测试集）。

5. 超参数调整

几乎每个算法都有需要设置的超参数，这些参数可以极大地影响性能。使用网格搜索、随机搜索或贝叶斯优化等技术来找到每个候选模型的最佳超参数。

6. 交叉验证

为了确保你的模型性能稳健且不过度乐观，请使用交叉验证。K 折交叉验证是一种常见的技术。交叉验证为模型在未见数据上的性能提供了一个更通用的指标。

7. 模型评估

使用你选择的指标（指标）在验证集上评估每个模型。将不同模型的性能与基线模型以及彼此进行比较。

8. 集成

如果单个模型表现不佳，考虑结合多个模型。例如，使用 bagging、boosting 或 stacking 等技术通常会比单个模型有更好的性能。

9. 模型可解释性

并非总是关于获得最高的准确率；有时理解模型为何做出某些决策是至关重要的。根据领域（如医疗保健或金融），您可能会优先考虑更简单、更可解释的模型，即使后者有略微更好的性能。

10. 最终模型选择

根据验证性能、可解释性和业务目标选择最终模型。在这个结合了训练和验证集的模型上训练，以便在测试集上进行最终预测。

11. 部署和监控

一旦最终模型被选中并评估，它就可以在生产环境中部署。持续监控模型在现实世界中的性能。随着时间的推移，数据的变化可能导致模型需要重新训练或微调。

12. 反馈循环

随着模型的使用和预测的收集，这些数据可以反馈到训练数据集中，以用于未来模型的改进。

模型选择过程的目标并不总是找到具有最高性能指标的模型。目标是找到一个满足业务目标、可靠、可解释（如果需要）并且对未见数据泛化良好的模型。

使用 DEATH.CSV 数据集进行线性回归的代码

让我们使用 death.csv 数据集实现线性回归。以下是我们将遵循的步骤：

1. 数据预处理：处理缺失值并准备数据以进行建模。

2. 特征选择：选择我们将用于预测因变量的独立变量（特征）。

3. 数据拆分：将数据集拆分为训练集和测试集。

4. 模型训练：在训练集上训练一个线性回归模型。

5. 模型评估：评估模型在测试集上的性能。

6. 模型解释：解释模型的系数。

在这个演示中，让我们使用 age_adjusted_death_rate 作为因变量，recent_5_year_trend_2_in_death_rates 作为自变量。

让我们从数据预处理开始。线性回归模型在测试数据上的性能如下：

均方误差（MSE）：145.22

R-squared (R²) 值：0.1114

R2 值表明，大约 11.14% 的年龄调整死亡率的变化可以由 recent_5_year_trend_2_in_death_rates 的最近五年趋势解释。这不是一个非常高的值，表明仅使用最近五年趋势的线性模型可能不足以捕捉死亡率的全部变化。

最后，让我们通过检查模型的系数来继续进行模型解释。线性回归模型可以用以下方程表示：

age_adjusted_death_rate = 1.5506*recent_5_year_trend_2_in_death_rates + 54.9239

解释系数得出以下结果：

recent_5_year_trend_2_in_death_rates 的系数等于 1.5506。对于 recent_5_year_trend_2_in_death_rates 每增加一个单位，age_adjusted_death_rate 大约增加 1.5506 个单位，保持其他因素不变。

截距（54.9239）:

当 recent_5_year_trend_2_in_death_rates 为零时，预测的 age_adjusted_death_rate 大约为 54.9239。

给定适中的 R2 值，如果需要提高预测能力，考虑其他特征或更高级的建模技术是必要的。此线性模型提供了两个变量之间基本理解和关系的理解。

列表 5.3 显示了 linreg2_gpt4.py 的内容，该内容说明了如何使用死亡.csv 数据集的子集执行线性回归。

列表 5.3: linreg2_gpt4.py

import pandas as pd

from sklearn.linear_model import LinearRegression

from sklearn.model_selection import train_test_split

from sklearn.metrics import mean_squared_error, r2_score

# CSV 文件 death_clean.csv 的描述如下：

death_df = pd.read_csv('death_clean.csv')

# 第 1 步：数据预处理

# 在感兴趣的列中删除具有缺失值的行

processed_data = death_df.dropna(subset=["age_adjusted_death_rate", "recent_5_year_trend_2_in_death_rates"])

# 第 2 步：特征选择

X = processed_data[["recent_5_year_trend_2_in_death_rates"]] # 自变量

y = processed_data["age_adjusted_death_rate"] # 依赖变量

# 第 3 步：数据拆分

X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)

# 第 4 步：模型训练

linear_reg = LinearRegression()

linear_reg.fit(X_train, y_train)

# 第 5 步：模型评估

y_pred = linear_reg.predict(X_test)

mse = mean_squared_error(y_test, y_pred)

r2 = r2_score(y_test, y_pred)

# 这段代码片段由作者添加：

print("mse:",mse,"r2:",r2)

列表 5.3 从几个导入语句开始，随后使用 CSV 文件 death_clean.csv 的内容初始化 Pandas 数据框 death_df。请注意，此 CSV 文件是由作者创建的，通过删除包含一个或多个星号的死亡 _clean.csv 中的数据点。

列表 5.3 的下一段初始化了 Pandas 数据框 processed_data，该数据框由删除 Dataframe death_df 中的两列的此代码片段组成：

processed_data = death_df.dropna(subset=["age_adjusted_death_rate", "recent_5_year_trend_2_in_death_rates"])

现在我们有了验证过的数据集，我们可以使用这对代码片段初始化自变量 X 和因变量 y：

X = processed_data[["recent_5_year_trend_2_in_death_rates"]] # 自变量

y = processed_data["age_adjusted_death_rate"]

接下来，执行标准的数据集训练/测试分割，其中 80% 的数据用于训练，20% 的数据集用于测试，如下代码片段所示：

X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)

第四步涉及将 linear_reg 初始化为 LinearRegression 类的实例，之后我们可以将此实例拟合到数据中。列表 5.3 的最后部分通过调用训练模型 linear_reg 的 predict() 方法进行模型评估。在此阶段，我们可以将 use 初始化为 MSE 和 R² 分数，然后打印它们的值。现在运行 列表 5.3 中的代码，你将看到以下输出：

mse: 145.2243931078172 r2: 0.11141880352501743

描述模型诊断

模型诊断在识别回归模型中的潜在问题以及确保线性回归的基本假设得到满足方面发挥着至关重要的作用。以下是线性回归的主要诊断和相关的检查：

1. 线性

2. 错误独立性

3. 同方差性

4. 残差的正态性

5. 多重共线性

6. 异常值和杠杆点

7. 模型指定

线性假设意味着独立变量与因变量之间的关系应该是线性的。

诊断工具：

残差与拟合图：如果此图中有模式（如曲线），则表明非线性。观察值与预测值之间的散点图。

错误独立性的假设意味着残差（误差）应该是独立的。

诊断工具：

Durbin-Watson 检验检测残差中的自相关性（给定时间滞后分离的值之间的关系）。

同方差性假设意味着残差的方差应该在独立变量（s）的所有水平上保持恒定。

诊断工具：

+   残差与拟合图：如果存在漏斗形状，则表明异方差性（非恒定方差）。Breusch-Pagan 或 White 检验用于统计检验异方差性。

残差的正态性假设意味着残差应该近似正态分布。

诊断工具：

+   直方图或核密度图：用于检查正态性。

+   Q-Q（分位数-分位数）图：如果残差位于 45 度参考线上，则它们近似正态分布。

+   Shapiro-Wilk 检验：一个用于检验正态性的正式检验。

多重共线性假设意味着独立变量之间不应高度相关。

诊断工具：

+   VIF：VIF 大于 10 表示高度多重共线性。

+   相关矩阵或热图：用于检查变量之间的相关性。

检测异常值和杠杆点很重要，因为异常值可能会过度影响模型，导致不可靠的估计。

诊断工具：

+   标准化残差与杠杆作用图：有助于识别对回归线有高杠杆作用的点。

+   库克距离：衡量删除给定观测值的影响。

正确的模型指定意味着没有遗漏变量偏差，也没有包含不必要的变量。

诊断工具：

+   添加变量（部分回归）图：有助于检查变量是否向模型添加信息。

+   RESET（回归指定误差测试）：测试模型是否存在指定错误。

对于我们使用 death.csv 数据集的线性回归模型，让我们进行一些这些诊断，从检查线性、同方差性和残差的正态性开始。根据诊断图，我们有以下结果：

残差与拟合值图：

线性：残差与拟合值之间似乎没有明显的模式，这表明线性假设并未被强烈违反。

同方差性：残差的分布似乎在整个拟合值范围内相对均匀，这表明同方差性假设并未被强烈违反。

残差直方图：

直方图显示了残差的分布。虽然它不是完全正态分布，但分布没有出现极端的偏离正态性。

Q-Q 图：

Q-Q 图显示了残差分布与正态分布的匹配程度。残差大体上遵循 45 度参考线，尤其是在中心部分。有一些偏差，尤其是在尾部，表明存在一些偏离完美正态性的小偏差。

为了进一步确保模型的可靠性，还应考虑额外的诊断，如检查多重共线性（对于具有多个预测因子的模型更为相关）、异常值和高杠杆点。对于这个只有一个预测因子的简单线性模型，多重共线性不是问题。

描述额外的模型诊断

在提示 ChatGPT 深入探讨我们线性回归的额外模型诊断后，ChatGPT 响应了以下列表项之后的文本：

+   影响图

+   库克距离

+   VIF（方差膨胀因子）

+   条件数

影响图有助于识别对回归方程有高影响力的点。

库克距离衡量删除给定观测值的影响。具有大库克距离的数据点可能是具有影响力的。

VIF：虽然对于只有一个预测因子的简单模型来说，多重共线性不是问题，但了解这一诊断对于未来模型扩展时的参考是有益的。

条件数：高条件数可能表明多重共线性以及回归中的潜在数值不稳定性。

让我们从影响图和库克距离开始。影响图提供了观察值对回归影响的视觉表示。点的尺寸与库克距离成正比，而更靠右的点具有更高的杠杆作用。大多数观察值都聚集在左侧，表明杠杆作用低。然而，一些点，尤其是那些尺寸较大的点，可能是有影响力的。

库克距离：

我们已经确定了 73 个库克距离大于阈值“4nn4”的观察值，其中“nn”是观察值的数量。这些可能是过度影响模型拟合的潜在有影响力的点。

有影响力的观察值的存在表明有几项潜在的行动方案：

+   调查有影响力的点：在考虑删除任何数据点之前，了解它们可能为何有影响力是至关重要的。它们是错误，还是代表真正的极端情况？

+   鲁棒回归：如果数据集中有有影响力的点或异常值，可以考虑使用降低异常值影响力的鲁棒回归方法。

GPT-4 的更多推荐

根据使用 death.csv 数据集进行的线性回归模型的结果和诊断，以下是一些建议。

1. 处理异常值

调查在诊断过程中确定的潜在异常值。确定它是否是数据错误或实际极端值。如果是错误，则更正或删除它。如果是真实的，可以根据上下文及其对模型可能产生的影响来决定是否保留它。

2. 扩展模型

当前模型仅使用一个预测因子。考虑从数据集中添加其他相关预测因子以提高模型的解释力。在添加更多预测因子时，要注意多重共线性，并确保再次运行诊断。

替代模型：

考虑到适中的 R2 值，可以考虑使用更复杂的回归模型，如多项式回归、岭回归或 Lasso 回归，甚至非线性模型。

像随机森林或梯度提升机这样的集成方法也可能值得探索。

3. 特征工程

探索创建新特征或转换现有特征。例如，如果某些关系不是线性的，非线性变换（例如，对数变换）可能会有所帮助。

4. 更有策略地处理缺失值

为了简化，我们删除了具有缺失值的行。根据缺失数据的性质，考虑使用插补技术来利用更多数据。

5. 模型验证

确保使用如 k 折交叉验证等技术进行稳健的验证。这提供了对未见数据上模型性能的更可靠的估计。

6. 领域知识

与领域专家合作，更好地理解特征，验证模型的发现，并可能识别新的相关特征。

7. 模型可解释性

如果目标是理解影响死亡率的因素，可以考虑使用决策树或 SHAP 值与集成方法相结合的模型，以获得更好的可解释性。

8. 定期更新

根据数据随时间的变化，模型可能需要定期更新或微调。设置一个监控机制。

9. 数据质量和收集

确保数据质量。如果数据收集中存在系统错误或偏差，即使是最好的模型也可能产生误导性结果。

总之，虽然初始的线性回归模型提供了一个基础的理解，但仍有很大的改进和精炼空间。最佳方法将是迭代性的：精炼模型，验证它，解释结果，并根据需要调整。

摘要

本章是本书的第一章，其中包含由 GPT-4 生成的材料。你看到了 GPT-4 如何描述数据集的准备过程以及探索性分析。

然后你看到了对 death.csv 数据集的详细 EDA 分析，模型选择过程以及该数据集的实际线性回归代码。

此外，你还了解了 GPT-4 生成的模型诊断，随后是 GPT-4 生成的推荐列表。

第六章

使用 GPT-4 的机器学习分类器

本章包含 GPT-4 为众多机器学习分类算法提供的基于 Python 的代码示例。

本章的第一部分向 GPT-4 请求有关机器学习分类器的信息。本节还包含 GPT-4 生成的高层次描述的 scikit-learn。

本章的第二部分向 GPT-4 请求描述著名的机器学习算法，如 kNN、逻辑回归、支持向量机（SVM）、决策树、随机森林和朴素贝叶斯。本节还包含每个机器学习算法的基于 Python 的代码示例。

本章包括 GPT-4 生成的各种机器学习算法的 Python 代码，包括 kNN、决策树、随机森林和 SVMs。你还将看到一些关于相同算法的内容，所有这些都是由 GPT-4 生成的。然而，首先，我们将从算法的讨论开始；然后你可以检查包含 GPT-4 生成的 Python 代码的部分。

在阅读本章的材料时，请记住，为了提高 GPT-4 生成的材料的可读性，偶尔会包含额外的注释。例如，在 GPT-4 的文本部分之后，你可能会看到以下内容：“注意：这是 GPT-4 生成的文本的结束。”

机器学习（根据 GPT-4）

机器学习（ML）是人工智能（AI）的一个子集，它专注于构建可以从数据中学习和基于数据做出决策的系统。机器学习算法不是被明确编程来执行任务，而是使用统计技术来学习数据中的模式，并据此做出预测或决策。以下是对此的更深入讨论。

重要概念

+   学习：

+   机器学习涉及使用数据集训练算法以识别模式。数据的质和量越好，算法的学习效果越好。

+   模型：

+   一旦算法从数据中学习，它就会形成一个模型。然后可以使用这个模型来做出预测或决策，而无需明确编程来执行该任务。

+   预测：

+   这涉及到使用模型为新输入确定输出。例如，在垃圾邮件检测中，预测将是新电子邮件是否为垃圾邮件。

机器学习类型

+   监督学习：

+   算法在标记数据集上训练，这意味着数据集中的每个示例都与正确的输出配对。目标是学习从输入到输出的映射。

+   例子：回归、分类

+   无监督学习：

+   算法在无标记数据集上训练，试图学习数据的潜在结构。

+   例子：聚类、降维

+   半监督学习：

+   这种方法使用标记和无标记数据来训练。当获取完全标记的数据集既昂贵又耗时的情况下，通常使用这种方法。

+   强化学习：

+   算法通过与环境的交互并接收关于奖励或惩罚的反馈来学习。

+   例子：训练机器人穿越迷宫

机器学习应用

机器学习有广泛的应用，包括以下内容：

+   图像和语音识别：这用于面部识别或语音激活助手。

+   医疗诊断：根据症状或医学影像协助医生诊断疾病是一个重要的应用。

+   财务预测：机器学习可用于预测股市趋势。

+   推荐系统：这些系统可以根据用户偏好建议产品、电影或音乐。

+   自然语言处理：NLP 常用于聊天机器人和翻译服务。

+   自动驾驶汽车：机器学习使汽车能够在没有人为干预的情况下导航。

机器学习挑战

+   过度拟合：这种情况发生在模型对训练数据学习得太“紧密”，在新数据上表现不佳。

+   低方差：这种情况发生在模型过于简单，无法捕捉数据的潜在结构时。

+   偏见与公平性：确保机器学习模型不会持续或放大数据中存在的偏见对于应用的有用性至关重要。

+   可解释性：这一方面涉及到使复杂模型对人类可理解。

+   数据隐私：保护用户数据并确保机器学习的道德使用应是一个高优先级。

机器学习是关于开发可以从数据中学习并基于数据做出决策的算法。大数据的兴起和计算能力的提升导致了机器学习（ML）的重大进步，使其成为现代技术解决方案的关键组成部分。

什么是 SCIKIT-LEARN？

Scikit-learn，通常简称为“sklearn”，是 Python 中流行的开源机器学习库。它提供了简单高效的数据分析和建模工具，使其成为机器学习领域初学者和专家的首选。

特性和功能

1. 算法：Scikit-learn 包括广泛的监督学习和无监督学习算法，例如：

+   分类：例如，支持向量机（SVMs）、随机森林、朴素贝叶斯

+   回归：例如，线性回归、岭回归、决策树

+   聚类：例如，k-means、层次聚类、DBSCAN

+   维度降低：例如，主成分分析（PCA）、t-SNE

2. 模型选择和评估：提供帮助分割数据集、网格搜索、交叉验证以及评估机器学习模型性能的各种度量工具

3. 数据预处理：提供数据预处理的函数，如归一化、标准化和编码分类变量

4. 特征提取：包含从图像和文本中提取特征的实用工具（例如，使用词袋方法）

5. 管道：提供按顺序应用一系列转换和最终估计器的工具。管道的中间步骤必须是转换器（例如，缩放器或 PCA），而最后一个估计器可以是任何对象（例如，分类器，回归器）

6. 兼容性：设计为与 Python 数值和科学库 NumPy 和 SciPy 互操作

优点

+   简单性：Scikit-learn 的 API 设计旨在保持一致性且易于使用。

+   完备的文档：详细的文档带有示例，使初学者易于理解

+   性能：流行算法的高效实现

+   社区支持：作为开源且受欢迎的库，拥有庞大的用户和贡献者社区，这导致定期更新和快速修复错误。

局限性

1. 神经网络：虽然 scikit-learn 确实有神经网络的基本工具，但它并不是专门为深度学习设计的。TensorFlow、Keras 或 PyTorch 等库更适合深度学习任务。

2. 可扩展性：对于非常大的数据集或分布式计算，Apache Spark 的 MLlib 或 Dask 等工具可能更为合适。

常规用法

Scikit-learn 通常用于传统机器学习任务，其中数据适合内存且不需要深度学习。它特别适合原型设计和构建端到端机器学习管道。

总结来说，scikit-learn 是 Python 中一个多才多艺且全面的机器学习库，其简单性和强大功能的结合使其成为许多数据科学家和研究人员的首选。

什么是 KNN 算法？

k 最近邻（kNN）算法是一种简单、直观且非参数的机器学习算法，用于分类和回归任务。以下是它是如何工作的。

基本概念

对于一个新的、未见过的观察值，kNN 在训练集中搜索与观察值最近的 k 个训练示例，并返回这些 k 个邻居中出现频率最高的输出值（类别或数值）。

步骤

1. 选择 k 的数量：确定你想要考虑的邻居数量。通常，k 是一个奇数，以防止平局情况（在分类的情况下）。

2. 距离度量：决定一个距离度量来衡量实例的“接近度”。最常用的度量是欧几里得距离，但根据数据的性质，也可以使用曼哈顿、闵可夫斯基和汉明距离等其他度量。

3. 搜索：对于新的数据点，计算它与训练集中所有点的距离，并识别出 k 个最近的点。

4. 聚合

+   对于分类：返回 k 个邻居中出现频率最高的类别

+   对于回归：返回 k 个邻居的输出值的平均值（或中位数）

优点

+   简单直观：对数据的分布或决策边界没有假设

+   多功能：适用于分类和回归

+   非参数：没有显式的训练阶段，它可以处理决策边界非常不规则的数据集。

缺点

+   计算密集型：它需要为每个预测计算所有训练样本的距离，对于大数据集来说可能会很慢。

+   内存使用：它存储整个数据集，因此内存消耗可能很高。

+   对无关特征敏感：距离度量可能受到对分类或回归不重要的特征的影响。

+   对数据规模敏感：具有较大规模的特性可能会主导距离度量，因此通常需要归一化或标准化数据。

用例

当以下情况成立时，kNN 特别有用：

+   数据被标记。

+   数据集不是太大（以避免计算效率低下）。

+   决策边界非常不规则。

尽管 kNN 很简单，但它可以出奇地有效，尤其是在基础决策边界复杂且不易被其他线性模型捕捉的情况下。在实践中，由于计算和内存需求，kNN 通常更多地用作基线或在较小的数据集中使用。

在 KNN 算法中选择 K 的值

确定 k 最近邻（kNN）算法的最佳 k 值至关重要，因为这个值可以显著影响模型的表现。特别是，k 的值可以影响预测的偏差和方差。以下是选择 kNN 算法中最佳 k 值时需要考虑的一些要点：

+   交叉验证

+   偏差-方差权衡

+   距离度量

+   平方根规则

+   领域知识

+   偶数 k 与奇数 k

+   计算效率

+   数据集的多样性

交叉验证

确定最优 k 的最常见方法是交叉验证，尤其是 k 折交叉验证。首先，将数据集分为训练集和验证集。对于每个潜在的 k 值，在训练集上训练 kNN 算法，并在验证集上进行验证。测量每个 k 在验证集上的准确度（或其他相关指标）。选择在验证集上表现最佳的 k。

偏差-方差权衡

k 的值较小（例如，k=1）意味着数据中的噪声将对结果有更大的影响，导致具有高方差但低偏差的模型。较大的 k 值具有平滑效果，可以减少方差但增加偏差。这可能会使算法对异常值更具抵抗力，但可能导致类别之间的边界不那么明显。

距离度量

距离度量的选择（例如，欧几里得、曼哈顿和闵可夫斯基）可以影响最优 k。在优化 k 的过程中尝试不同的距离度量。

平方根规则

一个常用的启发式方法，尤其是在开始搜索最优 k 时，是将 k 设置为训练数据集中数据点数量的平方根。这不是一个严格的规则，但可以作为起点。

领域知识

有时，领域知识或问题的具体背景可以指导 k 的选择。例如，在你知道数据点成对或成组相关的问题中，k=2 或 k=3 可能是一个合理的起点。

偶数与奇数 k

通常建议选择奇数 k 以避免平局，即两个类别具有相同数量的最近邻。然而，请注意，许多 kNN 实现都有平局解决机制。

计算效率

随着 k 的增加，计算可能会变得更加密集（因为你正在考虑更多的邻居）。然而，如果 k 太小，模型可能会对数据中的噪声过于敏感。

数据集的多样性

如果数据集有许多重叠的类别，较小的 k 可能更合适。如果类别更加明显，较大的 k 可以工作得很好。

在实践中，尝试一系列的 k 值，并对每个值进行性能验证。可视化工具，如显示验证准确度与不同 k 值的图表，可以帮助做出决策。

KNN 算法的“肘部方法”

如果你熟悉 k-means 聚类算法，你无疑知道用于确定 k 的最佳值的“肘部方法”。需要考虑的自然问题是，这种方法是否可以用于确定 kNN 算法中 k 的最佳值。

肘部方法主要与 k-means 聚类算法相关联，其中它被用来确定最佳聚类数量。在 k-means 的背景下，“肘部”是在簇内平方和（WCSS）与聚类数量之间的图表中的一个点。这个点代表了精度（更多聚类）和计算效率（较少聚类）之间的平衡。

对于 kNN 来说，主要目标是分类（或回归），而不是聚类。kNN 中的参数 k 代表在做出预测时考虑的邻居数量，而不是数据中的聚类数量。

然而，使用图表来识别收益递减点（“肘部”）的概念可以应用于 kNN 的参数调整中。

验证错误

你可以绘制一系列 k 值的验证错误（或准确率）。随着 k 的增加，模型可能会在减少方差的同时最初变得更加准确。然而，在某个点上，增加 k 可能会引入更多的偏差，导致错误增加或准确率下降。

在这种情况下，“肘部”将是增加 k 不再导致验证错误（或准确率）显著提高的点。

距离考虑

收益递减的概念也可以应用于 kNN 的距离度量。例如，可以检查不同 k 值下第 k 个最近邻的平均或中位数距离，以了解数据的密度和分布。

虽然在 kNN 超参数调整的背景下可以应用“肘部”的概念，但区分 k-means 中肘部方法的目的（确定聚类数量）与其在 kNN 中潜在应用（调整邻居数量以实现最佳预测）之间是至关重要的。

基于 kNN 算法的机器学习模型

本节包含了一个 GPT-4 使用 kNN 算法和 death.csv 数据集生成机器学习模型的示例。本节的前半部分包含了 GPT-4 执行的步骤解释，以及“标记”引用代码中的适当部分，随后是列表 6.1，其中包含 GPT-4 生成的基于 Python 的代码。

第一部分从以下提示开始，这是给 GPT-4 的，目的是生成一个使用 kNN 算法的机器学习模型的 Python 代码：

“请使用 kNN 算法和 death.csv 数据集生成一个机器学习模型。”

[注意：以下文本由 GPT-4 生成，并对格式进行了调整以改善可读性]

GPT-4 的响应如下所示。

在我们使用 kNN（k-Nearest Neighbors）算法创建机器学习模型之前，我将概述我们将遵循的步骤：

+   加载数据：读取 death.csv 数据集。

+   数据预处理：清理和预处理数据集，使其适合建模。

+   特征选择：选择用于训练模型的相关特征。

+   训练-测试集划分：将数据集划分为训练集和测试集。

+   模型训练：使用 kNN 算法在训练集上训练模型。

+   模型测试：在测试集上评估模型的性能。

+   性能指标：计算如准确度等指标，以了解模型的性能。

让我们先加载数据集并查看其前几行。

现在我们已经加载数据集，让我们继续进行数据预处理步骤：

+   处理缺失值：我们需要确保没有缺失值，或者如果存在，则处理它们。

+   编码分类特征：如果有任何分类特征，我们需要将它们编码为数值值以供 kNN 算法使用。

+   特征选择：我们将选择建模过程中的相关特征。

+   缩放：kNN 对特征缩放敏感，因此对数据集进行归一化或标准化很重要。

让我们先处理缺失值并检查每列的数据类型。数据集中没有缺失值，这是个好消息。然而，在检查数据类型时，我们可以看到应该为数值类型的几个列（如 age_adjusted_death_rate、average_deaths_per_year 等）被表示为对象。这表明这些列中可能存在非数值字符或符号。

要继续：

我将转换列到数值数据类型，并处理任何非数值字符。

+   编码分类特征。

+   选择建模的相关特征。

+   归一化数据集以准备 kNN 算法。

列已成功转换为适当的数值数据类型。

接下来，我们需要：

+   编码分类特征：将分类特征转换为数值值。

+   特征选择：决定使用哪些特征进行建模。

+   缩放：归一化数据集。

为了简化，让我们直接使用数值特征，并使用独热编码将分类特征 recent_trend_2 进行编码。然后我们将数据分为训练集和测试集，缩放特征，并继续进行 kNN 建模。

让我们从编码分类特征和分割数据开始。

数据已成功预处理并分为训练集和测试集。我们现在有 2512 个样本在训练集中，629 个样本在测试集中，每个集都有 12 个特征。

接下来，我们将继续进行：

+   模型训练：在训练数据上训练 kNN 分类器。

+   模型测试：使用训练好的 kNN 分类器在测试数据上预测目标变量。

+   性能指标：使用准确度评估模型的性能。

让我们从训练 kNN 分类器开始。

看起来数据集中有 NaN 值，这导致训练过程中出现问题。这很可能是由于将非数值字符转换为 NaN 所导致的。

为了处理这个问题，我将：

+   补充训练和测试数据集中的缺失值。

+   重新训练 kNN 分类器。

kNN 分类器在测试数据集上实现了约 98.09% 的准确率。这是一个很高的准确率，表明模型能够以很高的正确度预测给定数据集的目标变量 met_objective_of_45_5_1。

然而，必须记住，准确率只是一个指标。根据具体的应用或问题，其他指标（如精确度、召回率或 F1 分数）可能更相关。此外，kNN 中 k 的选择可以显著影响结果。我们使用了默认的 k=5，但不同的值可能会产生不同的结果。

前面的叙述（从本节开始）描述了 GPT-4 将遵循的过程，以使用 kNN 算法和 death.csv 数据集训练机器学习模型。

GPT-4 生成的实际 Python 代码显示在列表 6.1 中，其中包含 knn_gpt4.py 的代码。请注意，此文件名是手动选择的（不是由 GPT-4 本身选择），以反映此任务 Python 代码的内容。

列表 6.1: knn_gpt4.py

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p169.jpg)

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p170.jpg)

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p171.jpg)

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p172.jpg)

列表 6.1 中的代码描述（在代码列表之前）说明了 GPT-4 如何使用 kNN 算法执行机器学习任务。您可以将列表 6.1 中 GPT-4 生成的 Python 代码与用于解决机器学习任务的手写 Python 代码进行比较。运行列表 6.1 中的代码，您将看到以下输出：

=> 准确率：0.9809220985691574

基于决策树算法的机器学习模型

本节包含 GPT-4 使用 kNN 算法和 death.csv 数据集生成机器学习模型的示例。本节的前半部分包含对 GPT-4 执行的步骤的解释，以及“标记”引用代码中的适当部分，随后是列表 6.2，其中包含 GPT-4 生成的基于 Python 的代码。

以下提示被提供给 GPT-4 以生成使用决策树算法的模型的 Python 代码，随后是对代码的描述：

“请使用决策树算法和 death.csv 数据集生成一个机器学习模型。”

ChatGPT 的响应如下：

我将概述我们将遵循的步骤，以使用决策树算法生成机器学习模型：

+   加载数据：我们之前已经加载了 death.csv 数据集。

+   数据预处理：我们之前已经大部分预处理了数据集。我们将继续使用相同的预处理数据。

+   模型训练：使用决策树算法在训练集上训练模型。

+   模型测试：评估模型在测试集上的性能。

+   性能指标：计算准确率等指标，以了解模型的性能如何。

[注意：GPT-4 由于内部处理错误生成了以下语句。]

让我们从训练一个决策树分类器开始。

对于带来的不便，我深表歉意，但似乎出现了技术问题。

让我们重新训练决策树分类器，并计算其在测试集上的准确率。

对于疏忽，我深感抱歉。由于代码执行状态被重置，我需要重新导入必要的库并再次预处理数据。

我将快速浏览数据预处理步骤，然后训练决策树分类器。

对于带来的不便，我深表歉意。由于状态重置，需要重新上传数据集。

请您重新上传 death.csv 数据集，这样我们就可以继续进行决策树算法建模。

作者：“请继续。”

ChatGPT 的响应如下：

感谢您重新上传数据集。让我们继续进行数据预处理，然后训练决策树分类器。

[注意：GPT-4 遇到了以下一系列错误。]

对于疏忽，我深感抱歉。错误表明数据集中仍然存在我们在早期预处理步骤中遗漏的非数字字符。

让我们通过处理非数字字符来纠正数据预处理，然后再次训练决策树分类器。

对于疏忽，我深感抱歉。我忘记定义 cols_to_convert 列表，其中包含要处理的列。让我纠正这一点，并继续进行数据预处理和决策树分类器的训练。

对于重复的疏忽，我感到非常抱歉。看起来我在预处理数据集时犯了一个错误。我会纠正它，并确保在训练决策树分类器之前数据集被正确清理。

让我们处理非数字字符，然后继续模型训练。

对于重复的错误，我深表歉意。数据预处理步骤似乎仍然遇到了未适当处理的字符串值。

为了确保问题得到解决，我将采取不同的方法：

我将调查每一列的唯一值，以识别任何非数字字符。我将确保这些非数字字符得到适当的处理。然后，我将继续进行决策树分类器的训练。

看起来没有列包含非数字字符。这很令人费解，因为错误提示了相反的情况。

我将采取不同的方法：我将识别并删除特征集中包含非数字字符的任何行，然后继续进行决策树分类器的训练。

决策树分类器在测试数据集上达到了 100%的准确率。这表明模型能够完美地预测给定测试数据集的目标变量 met_objective_of_45_5_1。

然而，谨慎地对待这样的结果至关重要。100%的准确率可能表明模型已经过度拟合了训练数据，尤其是在像决策树这样的模型中，它们容易过度拟合。

验证这一点的办法之一是进行交叉验证或检查模型在不同、未见过的数据集上的性能。

[注意：这是 GPT-4 生成的文本的结尾。]

列表 6.2 显示了 decision_tree_gpt4.py 的内容，说明了如何使用决策树算法和 death.csv 数据集创建机器学习模型。

列表 6.2: decision_tree_gpt4.py

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p174.jpg)

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p175.jpg)

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p176.jpg)

列表 6.2（在代码列表之前）中代码的描述说明了 GPT-4 如何使用决策树分类器执行机器学习任务。列表 6.2 中的代码使您能够比较 GPT-4 生成的 Python 代码和手写的用于创建使用决策树算法的机器学习模型的 Python 代码。运行列表 6.2 中的代码，您将看到以下输出：

accuracy_dt: 1.0

使用随机森林算法的机器学习模型

本节包含了一个 GPT-4 使用随机森林算法和 death.csv 数据集生成机器学习模型的示例。本节的前半部分包含了 GPT-4 执行的步骤解释，以及“标记”引用代码中的适当部分，随后是列表 6.3，其中包含 GPT-4 生成的基于 Python 的代码。

为了生成使用随机森林算法的模型代码，向 GPT-4 提供的以下提示：

“请生成一个使用随机森林算法和 death.csv 数据集的机器学习模型。”

ChatGPT 的响应如下：

该数据集包含与美国不同县死亡率的多个相关列。以下是关键列：

county: 县的名称。

fips: 县的 FIPS 代码。

met_objective_of_45_5_1: 表示县是否达到某个目标（标题中未指定）。

age_adjusted_death_rate: 县的年龄调整死亡率。

lower_95_confidence_interval_for_death_rate: 死亡率的 95%置信区间的下限。

upper_95_confidence_interval_for_death_rate: 死亡率的 95%置信区间的上限。

average_deaths_per_year: 县每年平均死亡人数。

recent_trend_2: 死亡率的最近趋势。

recent_5_year_trend_2_in_death_rates: 死亡率的最近 5 年趋势。

lower_95_confidence_interval_for_trend: 趋势的 95%置信区间的下限。

upper_95_confidence_interval_for_trend: 趋势的 95%置信区间的上限。

要使用随机森林算法构建机器学习模型，我们需要确定目标变量和特征。目标变量可以是“age_adjusted_death_rate”或“average_deaths_per_year”这样的东西，而特征将是数据集中的其他列。

让我们继续预处理数据，然后构建随机森林模型。你能指定你想预测的变量吗？以及是否有任何特定的列你想用作或排除为特征？

作者：“请预测列变量 met_objective_of_45_5_1。”

ChatGPT 的响应如下：

随机森林模型被训练来预测你数据集中的“met_objective_of_45_5_1”变量。以下是模型评估的结果：

+   准确率：该模型达到了约 62.8% 的准确率。这意味着在测试集中，它在大约 62.8% 的情况下正确预测了该县是否达到了目标。

+   分类报告：报告提供了模型性能的详细分析：

+   精确率：它衡量阳性预测的准确性。例如，当模型预测一个县达到了目标时，对于某一类别，它在 78% 的时间是正确的。

+   召回率：它衡量模型通过将其标记为阳性来捕获的实际阳性病例的数量。例如，对于某一类别，模型正确识别了实际达到目标的 74% 的所有县。

+   F1 分数：这是精确率和召回率的加权平均值。对于表现最好的类别，F1 分数为 0.76，表明精确率和召回率之间的性能相对平衡。

+   支持度：这显示了指定数据集中每个类别的实际发生次数。例如，测试数据集中某一类别的实例有 407 个。

这些结果表明，虽然模型在预测“met_objective_of_45_5_1”变量方面表现合理，但仍有改进的空间，特别是在精确率和召回率分数较低的类别中。微调模型、选择不同的特征或甚至采用不同的建模方法可能会潜在地提高性能。

作者向 ChatGPT：请生成一个使用随机森林算法和 death.csv 数据集的机器学习模型的 Python 代码。

ChatGPT 的响应如下：

随机森林模型被训练来预测你数据集中的“met_objective_of_45_5_1”变量。以下是模型评估的结果：

+   准确率：该模型达到了约 62.8% 的准确率。这意味着在测试集中，它在大约 62.8% 的情况下正确预测了该县是否达到了目标。

+   分类报告：报告提供了模型性能的详细分析：

+   精确率：它衡量阳性预测的准确性。例如，当模型预测一个县达到了目标时，对于某一类别，它在 78% 的时间是正确的。

+   召回率：它衡量模型通过将其标记为阳性来捕获的实际阳性病例的数量。例如，对于某一类别，模型正确识别了实际达到目标的 74% 的所有县。

+   F1-Score：这是精确率和召回率的加权平均值。对于表现最好的类别，F1 分数为 0.76，表明精确率和召回率之间相对平衡。

+   支持度：这显示了指定数据集中每个类别的实际发生次数。例如，测试数据集中有一个类别的实例有 407 个。

这些结果表明，虽然模型在预测“met_objective_of_45_5_1”变量方面表现合理，但仍有改进空间，特别是在精确率和召回率分数较低的类别中。微调模型、选择不同的特征或甚至采用不同的建模方法可能会潜在地提高性能。

作者：“请生成一个使用随机森林算法和 death.csv 数据集的机器学习模型的 Python 代码。”

ChatGPT 的响应如下：

当然！以下是使用随机森林算法和 death.csv 数据集创建机器学习模型的 Python 代码。此代码包括数据预处理、将数据集分为训练集和测试集、构建随机森林模型以及评估其性能的步骤。

列表 6.3 显示了 random_forest_gpt4.py 的内容，该内容说明了如何使用随机森林算法和 death.csv 数据集创建机器学习模型。

列表 6.3：random_forest_gpt4.py

import pandas as pd

from sklearn.model_selection import train_test_split

from sklearn.ensemble import RandomForestClassifier

from sklearn.metrics import classification_report, accuracy_score

from sklearn.preprocessing import LabelEncoder

import numpy as np

# 加载数据集

data = pd.read_csv('/path/to/death.csv') # 替换为正确的文件路径

# 预处理

# 编码目标变量

le = LabelEncoder()

data['met_objective_of_45_5_1_encoded'] = le.fit_transform(data['met_objective_of_45_5_1'])

# 选择特征 - 排除目标变量和非数值列

features = data.select_dtypes(include=[np.number])

# 删除任何剩余的缺失值

features = features.dropna()

# 定义目标和特征变量

X = features.drop('met_objective_of_45_5_1_encoded', axis=1)

y = features['met_objective_of_45_5_1_encoded']

# 将数据集分为训练集和测试集

X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)

# 构建随机森林模型

rf_classifier = RandomForestClassifier(random_state=42)

rf_classifier.fit(X_train, y_train)

# 预测和评估模型

y_pred = rf_classifier.predict(X_test)

accuracy = accuracy_score(y_test, y_pred)

report = classification_report(y_test, y_pred)

# 输出结果

print("Accuracy:", accuracy)

print("Classification Report:\n", report)

记得将'/path/to/death.csv'替换为你的 death.csv 文件的实际路径。此代码假定你想要预测的目标变量是'met_objective_of_45_5_1'，并且它使用数据集中的所有数值列作为特征，排除任何包含非数值数据的列。根据你分析的具体要求可能需要进行调整。

ChatGPT 可能会出错。请考虑检查重要信息。

作者：“请解释你刚才生成的 Python 代码。”

ChatGPT 的响应如下：

当然，我会一步一步地带你通过 Python 代码：

1. 导入库

+   pandas 用于数据操作和分析。

+   sklearn.model_selection 的 train_test_split 函数用于将数据集分为训练集和测试集。

+   sklearn.ensemble 的 RandomForestClassifier 是用于分类任务的随机森林模型。

+   sklearn.metrics 包括用于评估模型性能的函数，如 classification_report 和 accuracy_score。

+   sklearn.preprocessing.LabelEncoder 用于将分类文本数据转换为模型可理解的数值格式。

+   numpy 用于数值运算。

2. 加载数据集

+   使用 pandas 的 read_csv 函数读取 death.csv 文件。你需要将“/path/to/death.csv”替换为你的数据集的实际路径。

3. 预处理

+   使用 LabelEncoder 将目标变量“met_objective_of_45_5_1”编码为数值格式，因为 sklearn 中的随机森林需要数值输入。

+   然后过滤数据集，只包含数值列，因为模型不能直接处理非数值数据。

4. 处理缺失值

+   数据集中任何剩余的缺失值都被删除，以确保模型接收到的数据是干净的。

5. 定义目标和特征变量

+   X（特征）被分配除了目标变量（“met_objective_of_45_5_1_encoded”）之外的所有列。

+   y（目标）被编码为“met_objective_of_45_5_1”列。

6. 分割数据集

+   使用 train_test_split 将数据集分为训练集（80%）和测试集（20%），并设置 random_state 以确保结果的重复性。

7. 构建随机森林模型

+   创建了一个 RandomForestClassifier 对象，并在训练数据（X_train 和 y_train）上进行了训练。

8. 预测和评估模型

+   使用模型对测试集（X_test）进行预测。

+   使用 accuracy_score（用于衡量整体准确率）和 classification_report（用于查看每个类的精确率、召回率、f1 分数和支持）评估预测。

9. 输出结果

+   最后，打印出准确率和分类报告，以查看模型的性能如何。

此代码提供了一个使用随机森林分类器的机器学习任务的基本框架。根据您的数据集的具体情况和问题的性质，可能需要额外的步骤，如更复杂的数据清理、特征工程或模型超参数调整，以获得最佳结果。

在 列表 6.3 中运行代码，您将看到以下输出：

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p182.jpg)

使用 SVM 算法的机器学习模型

本节包含 GPT-4 使用 SVM 算法和 death.csv 数据集生成机器学习模型的示例。本节的前半部分包含 GPT-4 执行的步骤解释，以及引用代码中适当部分的“标记”，随后是 列表 6.4，其中包含 GPT-4 生成的基于 Python 的代码。

为了生成使用 SVM 算法和 death.csv 数据集的模型 Python 代码，向 GPT-4 提供了以下提示：“请生成使用 SVM 算法和 death.csv 数据集的机器学习模型 Python 代码，并提供 Python 代码的解释。”

ChatGPT 的响应如下：

当然！下面是使用 death.csv 数据集创建机器学习模型的 SVM 算法 Python 代码。代码之后，我将提供解释。

列表 6.4 展示了 svm_gpt4.py 的内容，该内容说明了如何使用 SVM 算法和 death.csv 数据集创建机器学习模型。

列表 6.4: svm_gpt4.py

import pandas as pd

from sklearn.model_selection import train_test_split

from sklearn.svm import SVC

from sklearn.metrics import classification_report, accuracy_score

from sklearn.preprocessing import LabelEncoder, StandardScaler

import numpy as np

# 加载数据集

data = pd.read_csv('death.csv') # 替换为正确的文件路径

# 预处理

# 对目标变量进行编码

le = LabelEncoder()

data['met_objective_of_45_5_1_encoded'] = le.fit_transform(data['met_objective_of_45_5_1'])

# 选择特征 - 排除目标变量和非数值列

features = data.select_dtypes(include=[np.number])

# 删除任何剩余的缺失值

features = features.dropna()

# 定义目标和特征变量

X = features.drop('met_objective_of_45_5_1_encoded', axis=1)

y = features['met_objective_of_45_5_1_encoded']

# 特征缩放（对 SVM 很重要）

scaler = StandardScaler()

X_scaled = scaler.fit_transform(X)

# 将数据集划分为训练集和测试集

X_train, X_test, y_train, y_test = train_test_split(X_scaled, y, test_size=0.2, random_state=42)

# 构建 SVM 模型

svm_classifier = SVC(random_state=42)

svm_classifier.fit(X_train, y_train)

# 预测和评估模型

y_pred = svm_classifier.predict(X_test)

accuracy = accuracy_score(y_test, y_pred)

report = classification_report(y_test, y_pred)

# 输出结果

print("准确度:", accuracy)

print("分类报告:\n", report)

代码解释

1. 导入库：

2. 与随机森林模型中使用的库相同，增加了 sklearn.svm.SVC，这是 SVM 分类器，以及 sklearn.preprocessing.StandardScaler 进行特征缩放。

3. 加载数据集：

4. 数据集从 CSV 文件中加载。您需要将“/path/to/death.csv”替换为实际的文件路径。

5. 预处理：

6. 目标变量（“met_objective_of_45_5_1”）使用 LabelEncoder 编码成数值格式。

7. 排除非数值列，并删除任何缺失值。

8. 特征缩放：

9. 将 StandardScaler 应用于特征。这是 SVM 的一个重要步骤，因为它对输入特征的规模敏感。

10. 定义目标和特征：

11. X 是特征集，y 是目标变量。

12. 数据集分割：

13. 数据集被分为训练集和测试集。

14. 构建 SVM 模型：

15. 实例化 SVM 分类器（SVC）并在训练数据上训练。

16. 模型预测和评估：

17. 模型在测试集上进行预测，并使用准确率和分类报告来评估其性能。

18. 输出结果：

19. 打印准确率和分类报告以评估模型性能。

此代码提供了一个用于分类的 SVM 模型的基本实现。与任何机器学习模型一样，可能需要进行进一步的调整和验证，以优化其在特定数据集上的性能。

在列表 6.3 中运行代码，您将看到以下输出：

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p184.jpg)

[注意：这是由 GPT-4 生成的文本和输出的结束。]

逻辑回归算法

逻辑回归是一种统计方法和机器学习算法，用于对结果为分类的数据集进行建模和分析。虽然其名称包含“回归”，但它主要用于二元分类任务（即输出可以取两个可能结果时）。它也可以扩展以处理多类分类。

基本概念

逻辑回归模型预测给定实例属于特定类别的概率。它预测事件发生的概率的对数几率，而对数几率的转换给出概率。

数学表示

对于二元分类（标签为 0 和 1），概率 P(Y=1)的建模如下：

P(Y=1)=11+e−z

P(Y=1)=1+e−z1

其中：

e 是自然对数的底数。

z 是预测变量的线性组合：z=β0+β1X1+β2X2+...

步骤

1. 线性变换：计算输入特征的加权总和（加上一个偏置项）。

2. 逻辑变换：将步骤 1 的结果通过逻辑（Sigmoid）函数传递，以获得 P(Y=1)的概率。

3. 决策阈值：使用阈值将概率转换为二元结果（0 或 1），通常为 0.5。

参数估计

逻辑回归模型的系数（参数）通常使用最大似然估计（MLE）来估计。目标是找到最大化观察数据似然性的参数集。

优点

+   可解释性：系数可以用优势比来解释，这使得解释预测因子的影响变得容易。

+   效率：它不需要太多的计算资源

+   输出概率：它提供了一个概率框架，这对于理解预测的置信度很有用。

缺点

+   假设线性：它假设存在线性决策边界，这可能无法捕捉到没有特征工程的情况下更复杂的关系。

+   不适合复杂关系：对于高度非线性关系，其他算法（如决策树或神经网络）可能更合适。

+   容易过拟合：具有大量特征时，它可能会过拟合，尤其是在特征相关的情况下。

用例

逻辑回归在医学（疾病诊断）、金融（信用审批）、营销（客户流失预测）等多个领域被广泛应用，这些领域的输出结果都是二元的。

扩展

1. 多项式逻辑回归：当目标变量有超过两个类别时使用

2. 正则化逻辑回归：结合 L1（Lasso）或 L2（Ridge）正则化以防止过拟合

逻辑回归是二元分类任务的基础算法，它提供了良好的可解释性和预测的概率框架。

**朴素贝叶斯算法**

朴素贝叶斯是一种基于贝叶斯定理的概率机器学习算法，它假设预测因子之间相互独立（因此有“朴素”标签）。尽管算法简单且存在朴素假设，但在许多任务中，尤其是文本分类场景（如垃圾邮件过滤或情感分析）中，该算法非常有效。

贝叶斯定理提供了一种基于先验知识计算假设概率的方法。它如下公式化：

P(A∣B) = P(B∣A)×P(A)/P(B)

where

P(A∣B) 是给定数据 B 的假设 A 的后验概率。

P(A) 是 A 的先验概率。

P(B∣A) 是似然，即给定假设 A 的数据 B 的概率。

P(B) 是证据，即数据 B 的概率。

朴素贝叶斯分类

对于具有响应变量 Y 和预测因子 X1,X2,...,Xn 的分类问题，朴素贝叶斯分类器估计条件概率：

P(Y=k∣X1,X2,...,Xn)

P(Y=k∣X1,X2,...,Xn)

基于独立性假设，这可以简化为以下形式：

P(Y=k∣X1,X2,...,Xn)∝P(Y=k)×∏i=1nP(Xi∣Y=k)

P(Y=k∣X1,X2,...,Xn)∝P(Y=k)×i=1∏nP(Xi∣Y=k)

具有最高后验概率的类别 k 是给定输入的预测。

朴素贝叶斯类型

1. 高斯朴素贝叶斯：假设连续特征遵循高斯（正态）分布

2. 多项式朴素贝叶斯：适用于离散数据。常用于文本分类，其中数据通常表示为词计数或词频

3. 伯努利朴素贝叶斯：适用于二元/布尔特征

优点

+   效率：需要少量的训练数据来估计必要的参数

+   简单性：易于理解和实现

+   良好的性能：特别是在文本分类任务中

+   可扩展性：可以处理大型数据集和高维特征空间

缺点

+   独立性假设：在现实世界的应用中，预测变量独立性的假设通常被违反，这可能会影响性能。

+   数据分布：如果分布假设（例如高斯）与实际数据分布不匹配，模型的性能可能会受到影响。

应用场景

朴素贝叶斯在以下方面特别受欢迎：

1. 文本分类：例如垃圾邮件检测、情感分析和新闻文章的分类

2. 推荐系统：如建议新闻文章或音乐

3. 人脸识别：作为更大系统的一部分

朴素贝叶斯是一种多才多艺且计算效率高的分类算法。其优势在于其简单性、概率性质以及在许多场景中出人意料的鲁棒性能，尤其是在数据维度较高时。

支持向量机算法

支持向量机（SVM）是一种监督机器学习算法，主要用于分类任务，尽管它也可以用于回归。它以其鲁棒性和处理高维数据的能力而闻名。SVM 的主要目标是找到最优超平面，以最好地划分数据集为类别。

基本概念

对于二分类问题，想象一下在多维空间中绘制你的数据点。支持向量机（SVM）试图找到一个超平面（在 2D 中是一条线，在 3D 中是一个平面，等等），它能最好地分隔这两个类别。最优超平面是具有最大边界的那个，即两个类别数据点之间的最大距离。

重要组件

1. 支持向量：这些是位于超平面最近的数据点，有效地定义了它。如果移除这些数据点，它们会改变超平面的位置。

2. 边界：它是最近的数据点（任何类别）与超平面之间的距离。SVM 的目标是最大化这个边界。

3. 超平面：这是分隔类别的决策边界。在二维空间中，它是一条线。

类型

1. 线性 SVM：用于线性可分的数据。它找到一个超平面，以最好地分隔两个类别。

2. 非线性 SVM（核 SVM）：当数据不可线性分隔时，SVM 使用一种称为“核技巧”的技巧，将数据投影到一个更高维的空间，在那里它是线性可分的。常见的核包括多项式、径向基函数（RBF）和 Sigmoid。

优点

+   在高维空间中有效：即使特征数量大于样本数量，它也能很好地工作。

+   顽健：它最大化了边界，使其对异常值具有顽健性。

+   多功能性：核技巧可以使算法适应非线性数据。

缺点

+   不适用于大型数据集：由于其计算复杂性，它可能不是非常大的数据集的最佳选择。

+   对噪声敏感：少量错误标记的示例可以显著降低性能。

+   核的选择：性能可能对核及其参数的选择敏感。

用例

支持向量机被应用于各种应用中。

1. 文本分类：由于其处理高维数据的能力，支持向量机常用于文本分类。

2. 图像识别：作为图像分类管道的一部分

3. 生物信息学：用于蛋白质分类和癌症分类

4. 手写识别：用于识别手写字符

支持向量机为分类任务提供了一种强大的方法，尤其是在数据具有许多特征或类别无法线性分离时。适当的调整，尤其是在使用核支持向量机时，对于实现最佳性能至关重要。

决策树算法

决策树是一种类似于流程图的树结构算法，用于机器学习中的分类和回归任务。它在将数据集分解成更小的子集的同时，逐步并行地开发相关的决策树。

基本概念

决策树算法试图通过使用树结构来解决问题。树中的每个内部节点对应一个特征，每个叶节点对应一个响应或类别标签。

重要组件

1. 决策节点：由正方形表示，这些节点包含对单个属性的决策或测试。

2. 分支：表示测试的结果并连接节点

3. 叶节点：预测结果的终端节点

算法

1. 属性选择：根据指标（如信息增益或基尼不纯度）选择放置在决策节点上的属性。目标是选择提供最佳分割的属性。

2. 分支创建：对于所选属性的每个可能值，创建一个分支。

3. 递归分割：然后对每个分支重复步骤 1 和 2，使用与该分支关联的数据子集。

4. 终止：当满足停止条件之一时，例如达到最大树深度、达到最小节点大小或节点包含来自单个类别的数据时，递归停止。

类型

1. 分类树：当响应变量是分类变量时使用。结果是类别标签。

2. 回归树：当响应是数值或连续时使用。结果是实数值。

分割指标

1. 信息增益：衡量一个特征为我们关于类别的信息量。它基于熵。

2. Gini 不纯度：衡量一组元素的无序程度。它被 CART（分类和回归树）算法用于分类任务。

3. 方差减少：由 CART 用于回归树

优点

+   可解释性：树可以可视化，即使是非专家也容易理解。

+   最小数据准备：它不需要归一化或虚拟变量

+   处理连续和分类变量：它可以用于分类和回归任务。

+   非参数：它不对分布和分类器结构做出假设。

缺点

+   过拟合：如果没有适当的调整，树可能会记住训练数据，导致过拟合。

+   不稳定性：数据的小幅变化可能导致完全不同的树。

+   优化：找到一组数据的最佳树是 NP 难题。因此，使用贪婪算法等启发式方法，这有时会导致次优树。

用例

决策树是多功能的，可以用于各种应用，包括以下：

1. 医疗诊断：根据症状，预测疾病的可能性

2. 信用风险分析：决定是否批准或拒绝贷款

3. 营销：识别营销活动的潜在客户

扩展

1. 随机森林：决策树的集成，通过减少过拟合提供更好的预测性能

2. 梯度提升树：顺序构建决策树，其中每个树纠正其前一个树的错误

决策树提供了一种直观和可视化的决策过程方法。它们的简单性和易于解释使它们在各种领域成为流行的选择，但必须小心处理它们的局限性。

随机森林算法

随机森林是一种主要用于分类和回归任务的集成学习方法。它通过在训练期间构建多个决策树来运行，并输出由单个树产生的类别的众数（对于分类）或均值（对于回归）。

基本概念

1. 自举：随机森林首先从数据集中抽取多个自举样本（带替换的随机样本）。这引入了变异性，并确保森林中的每棵树都在数据集的不同子集上训练。

2. 特征随机性：在决策树的每个分割中，只考虑特征的一个随机子集。这进一步确保森林中树的多样性，使集成更少相关且更稳健。

3. 聚合：

+   对于分类，森林中的每棵树“投票”选择一个类别，得票最多的类别是随机森林的预测。

+   对于回归，所有树的平均预测是最终预测。

优点

+   高精度：它结合多个树来产生一个高精度的分类器。

+   过拟合控制：集成特性和在树构建中引入的随机性有助于控制过拟合。

+   处理大数据：它有效地处理具有更多特征和观察值的较大数据集。

+   特征重要性：它提供了关于不同特征在预测中的重要性的见解。

+   多功能性：它可以用于分类和回归任务。

+   处理缺失值：它可以处理包含缺失值的数据集。

缺点

+   复杂性：它比单个决策树计算量更大。

+   可解释性：虽然单个树是可解释的，但森林可能不那么直观易懂。

+   预测较慢：在森林中需要对所有树进行聚合以进行预测，这可能会比其他算法慢。

超参数

在调整随机森林时需要考虑的一些关键超参数包括以下内容：

1. 树的数量：森林中的树的数量

2. 最大深度：每棵树的最大深度

3. 分裂内部节点所需的最小样本数

4. 叶节点最小样本数：达到叶节点所需的最小样本数

用例

随机森林是多功能的，并在各个领域都有应用，包括以下内容：

+   银行：信用风险分析

+   医疗：疾病识别

+   电子商务：推荐系统

+   遥感：卫星图像分类

随机森林是一种强大且灵活的算法，它建立在决策树的优势之上，同时解决了一些弱点。通过聚合多个、多样化的树的结果，它实现了高精度和对抗过拟合的鲁棒性。在需要快速基线模型或解释性不是主要关注点的情况下，它特别有价值。

摘要

本章内容丰富，这是你用 GPT-4 生成的第二个关于分类器的完整章节。你简要介绍了 scikit-learn，然后讨论了 kNN 算法。

接下来，你学习了交叉验证、偏差-方差权衡和距离度量。此外，你还学习了在 kNN 算法中选择 k 的最佳值的肘部方法。

此外，你还看到了由 GPT-4 生成的涉及 kNN 算法、决策树算法、SVM 算法和逻辑回归算法的代码示例。

本章的最后部分包含了一个由 GPT-4 生成的高级描述，描述了以下算法：逻辑回归、朴素贝叶斯、SVG、决策树和随机森林。

第七章

使用 GPT-4 进行机器学习聚类

本章是第三个包含由 GPT-4 生成的 Python 代码示例的章节，其中包括三个流行的机器学习聚类任务的 Python 代码。

本章的第一部分介绍了机器学习中的聚类，随后列出了十个聚类算法。本节还描述了 k-means、层次聚类和 DBSCAN 算法的优点和缺点。

本章的第二部分包含三个基于 Python 的代码示例，用于 k-means、层次聚类和 DBSCAN 算法，使用合成数据集。所有代码示例都是通过向 GPT-4 提供合适的提示生成的。

什么是聚类？

聚类是机器学习中的一个基本概念，尤其是在无监督学习中。聚类是将数据集划分为多个组（称为簇）的任务，使得同一组中的项目彼此之间比与其他组的项目更相似。

重要要点

+   学习类型：聚类是一种无监督学习形式。这意味着您不需要标记数据来与聚类算法一起工作。相反，目标是发现数据中的隐藏模式。

+   目标：主要目标是分离具有相似特征的组并将它们分配到簇中。

应用

+   市场细分：根据购买历史分组客户

+   社交网络分析：识别网络中的社区

+   搜索结果分组：将搜索结果中的相似文档或网页分组

+   图像分割：根据像素相似性将图像划分为区域

+   异常检测：检测不符合预期行为的异常模式（异常值）

指标

+   簇内平方和（WCSS）：这衡量了簇内所有点到簇中心的平方平均距离。

+   轮廓分数：这衡量一个簇中的每个点到邻近簇中点的接近程度。

+   戴维斯-鲍尔丁指数：这是衡量每个簇与其最相似簇之间平均相似度的指标，其中相似度是簇内距离与簇间距离的比率。值越低越好。

流行的聚类算法

+   K-means：这种算法将数据划分为 kk 个互不重叠的子集（或簇）。它是通过最小化数据点和相应簇质心之间的平方距离之和来实现的。

+   层次聚类：这种算法生成一组嵌套簇，组织成层次树。这种聚类类型可以可视化为一棵树状图（树形图），展示了形成簇的顺序。

+   DBSCAN（基于密度的空间聚类应用噪声）：这种算法基于数据点的密度创建簇。它可以找到任意形状的簇，并且对于有噪声和异常值的数据很有用。

+   高斯混合模型（GMMs）：这些模型假设数据是由几个高斯分布的混合生成的。GMM 试图识别这些高斯分布。

+   聚类：与层次聚类类似，但通常更具可扩展性。它从每个项目作为一个单独的簇开始，并将它们合并成更大的簇。

挑战

+   簇的数量：聚类中的一个挑战是确定算法应该将数据分割成多少个簇。对于 k-means，一种流行的技术是“肘部方法”。

+   聚类的形状和大小：一些算法假设聚类是球形且大小相等的，这并不总是成立。

+   特征缩放：聚类算法，尤其是像 k 均值这样的基于距离的方法，对特征缩放敏感。你应该缩放特征，使它们具有相似的量级。

+   高维空间：在多维空间中进行聚类可能会出现问题，这被称为“维度诅咒”。可以使用 PCA（主成分分析）等技术来降低维度。

聚类提供了对数据分布、分类和结构的洞察。它是数据分析、异常检测和预处理步骤（如数据降维）的强大工具。

**TEN CLUSTERING ALGORITHMS**

本节包含机器学习中的十个聚类算法列表，以及它们的优缺点：

+   k 均值聚类

+   层次聚类

+   基于密度的空间聚类应用（DBSCAN）

+   聚类层次聚类

+   均值漂移聚类

+   高斯混合模型（GMM）

+   相似传播

+   谱聚类

+   聚类层次聚类

+   OPTICS（对聚类结构进行排序以识别点）

K 均值聚类

优点

+   简单且易于实现

+   对于球形且大小相等的聚类效果良好

+   对于大量变量来说速度快

缺点

+   它假设聚类是球形且大小相等的，这并不总是成立。

+   聚类的数量 k 必须事先指定。

+   对初始化敏感，因为不同的初始质心可能导致不同的聚类。

层次聚类

优点

+   它不需要指定聚类的数量。

+   它提供了一个树状图，这对于理解数据层次结构可能很有用。

缺点

+   它比 k 均值聚类计算上更昂贵。

+   对于非常大的数据集来说，它不具有可扩展性。

基于密度的空间聚类应用（DBSCAN）

优点

+   可以找到任意形状的聚类

+   不需要指定聚类的数量

+   可以识别噪声/异常值

缺点

+   可能难以处理密度不同的聚类

+   不总是确定性的：可以从多个聚类中到达的边界点可以是任一聚类的一部分。

聚类层次聚类

优点

+   适用于较小的数据集

+   不需要指定聚类的数量（尽管在实践中通常指定）

缺点

+   对于非常大的数据集来说不具有可扩展性

均值漂移聚类

优点

+   不假设关于聚类数量的任何先验知识

+   可以找到任意形状的聚类

缺点

+   计算上更昂贵

+   带宽参数需要仔细选择。

高斯混合模型（GMM）

优点

+   假设每个聚类遵循高斯分布

+   可以建模椭圆聚类

缺点

+   比 k 均值聚类计算上更密集

+   需要估计更多的参数

相似传播

优点

+   自动确定簇的数量

+   使用所有数据点作为潜在的示例

缺点

+   对于大数据集可能较慢且需要更多内存

+   可能会产生大量的簇

谱聚类

优点

+   可以捕捉复杂的簇结构

+   可以用来识别非凸簇

缺点

+   对于大数据集，可能计算成本较高

+   必须事先指定簇的数量

聚类

优点

+   提供了一种分层方法，导致簇的树状结构

+   适用于小数据集

缺点

+   不适用于大数据集

+   需要指定簇的数量。

OPTICS（按顺序排列点以识别聚类结构）

优点

+   不需要指定簇的数量

+   可以识别不同密度的簇

缺点

+   比像 k-means 这样的简单算法计算量更大

每个这些聚类算法都有自己的假设，适用于不同类型的数据和要求。算法的选择通常取决于数据的大小、维度和性质，以及具体问题的背景。

机器学习中最受欢迎的三个聚类算法是前述章节列表中的前三个算法。这些算法将在后续章节中描述，并附带基于 Python 的代码示例。

聚类算法的度量标准

本节包含了一组你可以用于评估聚类算法的度量标准。聚类算法的评估对于确定算法的性能至关重要。以下是常用评估聚类算法的度量标准列表，以及它们的优缺点：

+   影子分数

+   卡尔金斯-哈拉巴斯指数

+   戴维斯-鲍尔丁指数

+   邓恩指数

+   调整后的兰德指数 (ARI)

+   标准化互信息 (NMI)

+   福尔克斯-马洛斯指数

+   纯度

+   凝聚力

+   分离度

影子分数

优点

+   衡量一个对象与其簇的相似性相对于其他簇的相似性

+   值的范围从 -1 到 1，高值表示好的聚类

缺点

+   不适用于非凸簇或密度变化的簇

+   对于大数据集，计算成本可能很高

戴维斯-鲍尔丁指数

优点

+   衡量每个簇与其最相似簇的平均相似度

+   值越低表示聚类越好。

缺点

+   它假设簇是凸的和各向同性的，这并不总是成立。

卡尔金斯-哈拉巴斯指数

优点

+   计算簇间散布均值与簇内散布均值的比率

+   值越高表示聚类越好。

缺点

+   它假设簇是凸的和各向同性的。

邓恩指数

优点

+   考虑最小簇间距离与最大簇内距离之间的比率

+   邓恩指数越高表示聚类越好。

缺点

+   计算成本高

调整后的兰德指数 (ARI)

优点

+   测量两个聚类之间的相似度

+   考虑偶然性进行调整，提供更可靠的分数

缺点

+   需要了解真实情况

标准化互信息（NMI）

优点

+   测量两个聚类之间的互信息

+   标准化到[0, 1]的范围内

缺点

+   需要了解真实情况

Fowlkes-Mallows 指数

优点

+   测量精确率和召回率的几何平均值

+   值的范围从 0 到 1，1 表示完美的聚类

缺点

需要了解真实情况

纯度

优点

+   测量聚类包含单个类别的程度

+   简单易懂且易于计算

缺点

+   需要了解真实情况

+   不考虑聚类大小

聚合度

优点

+   测量同一聚类内实例之间的紧密程度

缺点

+   对聚类数量敏感

分离

优点

+   测量一个聚类与其他聚类之间的区别或分离程度

缺点

+   对聚类数量敏感

当评估聚类算法时，考虑数据的性质和具体用例至关重要。根据上下文，某些指标可能比其他指标更合适。使用多个指标以全面了解聚类性能也是有益的。

K-Means 聚类

优点

+   简单性：该算法简单且易于实现。

+   效率：它计算速度快，尤其是在 Elkan 算法等优化变体中。

+   可扩展性：K-means 在大数据集上表现良好，尤其是在使用 MiniBatch k-means 时。

+   流行：由于其简单性和适用性，它在实践中被广泛使用。

缺点

+   聚类数量：您需要事先指定聚类数量 k，这并不总是可行的。

+   球形假设：它假设聚类是球形且大小相等的。对于细长或不规则形状的聚类，它可能表现不佳。

+   初始化敏感性：算法的结果可能取决于初始质心位置。尽管 k-means++等技术有所帮助，但收敛到局部最小值仍然可能是一个问题。

+   对异常值敏感：异常值会严重影响质心的位置。

+   特征缩放：它对特征缩放敏感。特征需要缩放才能使算法正常工作。

层次聚类

优点

+   系谱图：层次聚类产生系谱图，这可以是一个理解数据层次结构的有用工具，也可以用于可视化。

+   无需指定 k：与 k-Means 不同，您不需要事先指定聚类数量。

+   灵活性：它可以产生多种多样的聚类结构，使其适用于各种应用。

+   确定性：给定相同的输入和参数，总是产生相同的聚类结果。

缺点

+   计算复杂性：标准算法的计算复杂性高，使其不太适合大型数据集。

+   敏感性：它可能对噪声和异常值敏感。

+   选择正确级别的困难：决定在层次结构中切割和形成聚类的级别可能很棘手。

DBSCAN（无噪声的基于密度的空间聚类应用）

优点

+   无需指定聚类数量：DBSCAN 根据数据自动确定聚类数量。

+   形状灵活性：它可以找到任意形状的聚类，这比 k-means 有显著优势。

+   噪声处理：它可以识别和处理噪声和异常值。

+   不假设聚类结构：它不假设聚类是球形的或任何特定的形状。

缺点

+   处理不同密度聚类的困难：当聚类具有显著不同的密度时，它很挣扎。

+   边界点：可以从多个聚类中到达的点可能会被分配到错误的聚类。

+   参数敏感性：它需要设置参数（如邻域半径和最小点数），这些参数可以极大地影响结果。

虽然这些是三种最受欢迎的聚类算法，但最佳算法通常取决于特定的数据集和问题要求。尝试多种算法并评估哪种算法最适合给定场景是一种常见做法。

现在你已经对机器学习中的聚类有了基本了解，让我们看看基于 k-means 算法的机器学习模型，这是下一节的主题。

什么是 K-Means 算法？

由于其简单性和效率，k-means 算法是最广泛使用的聚类方法之一。

K-means 聚类概述

K-means 是一种将数据集划分为 k 个不同、非重叠的子集（或聚类）的划分方法。k-means 算法的目标是找到数据中的组，组数由变量 k 表示。

算法

+   初始化：随机选择 k 个数据点（种子）作为初始聚类中心。

+   分配：将每个数据点分配到最近的聚类中心。分配给聚类中心的点构成一个聚类。

+   更新：计算每个聚类的新的平均值（聚类中心）。

+   迭代：重复步骤 2 和 3，直到聚类中心没有显著变化，或者达到预定的迭代次数。

重要概念

+   聚类中心：聚类的中心。在 k-Means 算法中，聚类中心是聚类中所有点的平均值。

+   WCSS（簇内平方和）：它衡量簇内所有点到簇中心的平方平均距离。k-Means 算法的目标是使这个指标最小化。

确定 k 的值

k-means 的一个挑战是选择合适的聚类数量 k。一种常见的技术是“肘部方法”。

1. 对不同的 k 值（例如，k 从 1 到 10）计算聚类算法。

2. 对于每个 k，计算总的 WCSS（加权平方聚类误差）。

3. 绘制 WCSS（加权平方聚类误差）与簇数 k 的曲线。

4. 图中弯曲点（“肘部”）的位置通常被认为是适当簇数的指标。

优点

+   简单且易于实现

+   在计算成本方面高效

+   适用于大型数据集

局限性

+   它假设簇是球形且大小相等的，但这并不总是如此。

+   必须事先设置簇数 k。

+   它对质心的初始化敏感。这个问题通常通过多次运行算法并选择最佳结果来解决。

+   它可能收敛到局部最优。这就是为什么通常需要多次运行整个过程，每次使用不同的起始条件。

+   它对特征缩放敏感。

变体

+   k-means++：这种变体旨在通过指定在执行标准 k-means 优化迭代之前初始化质心的过程来解决 k-means 随机初始化的弱点。

K-means 是一种基础聚类算法，已在各种应用中被广泛使用。虽然它功能强大且可扩展，但进行数据预处理和考虑其假设对于获得有意义的簇分配是必不可少的。

什么是层次聚类算法？

层次聚类算法是一种聚类算法，通过自底向上或自顶向下的方法构建簇的层次结构。层次聚类构建一个簇的树。这个树，称为树状图，有助于可视化簇合并或分裂的顺序。

层次聚类有两种主要策略：

1. 聚合（自底向上）：这是最常用的策略。它从将每个对象视为一个单例簇开始。成对的簇依次合并，直到所有簇都被合并成一个包含所有对象的单个大簇。

2. 分裂（自顶向下）：它从所有对象在一个单个簇开始。在后续步骤中，簇被分割成更小的簇，直到每个对象都有自己的单例簇。

聚合层次聚类算法

在这里，我们将重点关注更常用的聚合层次聚类。

1. 初始化：将每个数据点视为一个单独的簇，对于 nn 个数据点，将产生 nn 个簇。

2. 聚类

+   找到彼此最近的簇对。

+   将这两个簇合并成一个单一的簇。

+   更新距离矩阵（用于存储簇之间的距离）。

+   重复此过程，直到只剩下一个簇。

3. 完成阶段：上述过程的结果是一个树状图，称为树状图。树状图表示簇合并的顺序。

距离度量

距离度量的选择在层次聚类中至关重要。

+   欧几里得距离：欧几里得空间中两点之间的普通直线距离

+   曼哈顿距离：它们坐标绝对差之和

+   余弦相似度：衡量两个非零向量之间角度的余弦值

链接标准

当两个簇 S 和 T 合并成更大的簇时，如何定义簇之间的距离的选择由链接标准决定：

+   单链接：两个簇之间的距离定义为每个簇中两点之间的最短距离。

+   完全链接：两个簇之间的距离定义为簇中任意两点之间的最大距离。

+   平均链接：两个簇之间的距离定义为每个簇中每个点到另一个簇中每个点的平均距离。

+   瓦德方法：这种方法最小化了正在合并的簇之间的距离方差。

优点

+   系统发育树：提供了对数据层次结构的深入洞察

+   无需指定簇数量：与 k-means 不同，您不需要事先指定簇的数量。

+   灵活性：可以产生各种不同的簇结构，使其适用于各种应用

缺点

+   计算复杂性：对于非常大的数据集不可扩展

+   不可逆：一旦做出合并两个簇的决定，就不能撤销。

+   对噪声和异常值的敏感性：噪声数据可能导致簇被错误地合并。

+   链接选择：不同的链接方法可以产生不同的层次结构。选择正确的链接方法是至关重要的。

层次聚类在数据中存在层次结构时特别有用。它适用于较小的数据集，当系统发育树对分析或展示有益时。然而，对于大型数据集或当计算效率是一个关注点时，其他聚类方法，如 k-means 或 DBSCAN，可能更合适。

DBSCAN 算法是什么？

基于密度的空间聚类应用噪声（DBSCAN）是一种著名的聚类算法，以其能够检测任意形状的簇和对其输入数据排序的不敏感性而闻名。

原则

DBSCAN 根据距离测量（通常是欧几里得距离）和最小数据点数将彼此接近的数据点分组在一起。它还将位于低密度区域中的点标记为异常值。

步骤

1. 随机点选择：从一个尚未访问的任意数据点开始。

2. 邻域检查：检索该点的邻域（所有在预定义距离 εε 内的点）。

3. 扩展簇：

+   如果有足够多的邻居（大于阈值 minPts），将该点标记为核心点并形成一个簇。

+   将距离 εε 内的所有可达数据点（直接和间接）添加到该簇中。

+   对簇中的每个未访问的点重复此过程。

4. 标记噪声：如果一个点不属于任何簇且没有足够的邻居，则将其标记为噪声或异常值。

5. 迭代：重复此过程，直到所有点都被分配到簇中或被标记为噪声。

重要概念

+   核心点：如果一个数据点在 ε 距离内有超过 minPts 个点，则该数据点是一个核心点。

+   边界点：如果一个数据点在 ε 距离内有少于 minPts 个点，但位于核心点的 ε 距离内，则该数据点是一个边界点。

+   噪声/异常值：如果一个数据点既不是核心点也不是边界点，则该数据点是噪声。

+   直接密度可达：如果点 P 在 ε 距离内且 Q 是核心点，那么点 P 是从点 Q 直接密度可达的。

+   密度可达：如果存在一个点序列 P1,...,Pn，其中 P1=Q，Pn=P，且 Pi+1 是从 Pi 直接密度可达的，那么点 P 是从点 Q 密度可达的。

优点

+   任意形状的簇：与 k-means 不同，DBSCAN 可以找到任意形状的簇，而不仅仅是球形的。

+   噪声处理：它可以有效地处理噪声和异常值。

+   无需指定簇的数量：该算法不需要事先指定簇的数量。

缺点

+   参数敏感性：结果可能基于距离阈值 ε 和 minPts 的不同而变化。选择合适的值可能具有挑战性。

+   变化的密度：当簇具有显著不同的密度时，DBSCAN 可能会感到困难。

+   高维数据：随着数据维度的增加，算法的有效性会降低。

DBSCAN 是一种强大的算法，尤其是在簇形状各异且需要区分异常值时。它特别适用于空间数据和有噪声的数据。然而，参数调整和对数据本质的理解对于获得 DBSCAN 的最佳结果至关重要。

基于 k-means 算法的机器学习模型

本节包含 GPT-4 使用 k-means 算法和合成数据集生成机器学习模型的示例。本节的前半部分包含对 GPT-4 执行的步骤的解释，随后是列表 7.1，其中包含 GPT-4 生成的基于 Python 的代码。

这里是我们将要进行的概述：

1. 生成数据集：我们将使用 Scikit-learn 的 make_blobs 函数创建一个具有簇的合成数据集。

2. 可视化数据集：我们将绘制数据集以查看簇。

3. k-means 聚类：我们将使用 k-means 算法来识别簇。

4. 可视化簇：我们将再次绘制数据集，但这次将根据 k-means 识别的簇进行着色。

让我们生成合成数据集并可视化它。以下是生成的具有三个簇的数据集。颜色代表实际的簇（由于这是一个合成数据集，我们知道真实的簇分配）。

接下来，我们将使用 k-means 算法来识别数据集中的簇。我们将 kk（簇数）设置为 3，因为我们使用 3 个中心来生成数据集。聚类后，我们将可视化结果。

可视化显示了 k-means 聚类的结果。数据点根据 k-means 算法识别的簇进行着色。红色的“X”标记代表由 k-means 确定的簇中心。

如观察所示，k-means 算法已成功识别合成数据集中的簇。

列表 7.1 显示了 kMeans_GPT4.py 的内容，说明了如何使用 k-means 算法和 death.csv 数据集创建机器学习模型。

列表 7.1: kMeans_GPT4.py

从 sklearn.datasets 导入 make_blobs

导入 matplotlib.pyplot

# 生成包含 3 个簇的合成数据集

X, y = make_blobs(n_samples=300, centers=3, random_state=42, cluster_std=2.0)

# 可视化数据集

plt.figure(figsize=(8, 6))

plt.scatter(X[:, 0], X[:, 1], c=y, s=50, cmap='viridis')

plt.title("包含 3 个簇的生成数据集")

plt.xlabel("特征 1")

plt.ylabel("特征 2")

plt.show()

# 由于重置而重新导入必要的库

从 sklearn.datasets 导入 make_blobs

导入 matplotlib.pyplot

# 再次生成合成数据集

X, y = make_blobs(n_samples=300, centers=3, random_state=42, cluster_std=2.0)

# 可视化数据集

plt.figure(figsize=(8, 6))

plt.scatter(X[:, 0], X[:, 1], c=y, s=50, cmap='viridis')

plt.title("包含 3 个簇的生成数据集")

plt.xlabel("特征 1")

plt.ylabel("特征 2")

plt.show()

从 sklearn.cluster 导入 KMeans

# 应用 kMeans 聚类

kmeans = KMeans(n_clusters=3, random_state=42)

kmeans_labels = kmeans.fit_predict(X)

# 可视化识别的簇

plt.figure(figsize=(8, 6))

plt.scatter(X[:, 0], X[:, 1], c=kmeans_labels, s=50, cmap='viridis')

plt.scatter(kmeans.cluster_centers_[:, 0], kmeans.cluster_centers_[:, 1], s=200, c='red', marker='X', label='簇中心')

plt.title("kMeans 聚类结果")

plt.xlabel("特征 1")

plt.ylabel("特征 2")

plt.legend()

plt.show()

列表 7.1 以几个导入语句开始，接着调用 make_blobs()来创建一个合成数据集。接下来的代码块通过此代码片段生成并显示从生成的数据集中的数据生成的散点图：

plt.scatter(X[:, 0], X[:, 1], c=y, s=50, cmap='viridis')

列表 7.1 的下一部分实际上是多余的：代码中之前出现的成对导入语句再次被导入。此外，生成了相同的散点图，这也是多余的。

代码列表 7.1 的下一部分初始化变量 kmeans 为从 sklearn.cluster 导入的类 KMeans 的实例。接下来，变量 kmeans_labels 使用 kmeans 变量的 fit_predict()方法的结果进行初始化。在下一个代码块中，生成了一个额外的散点图，它通过这两段代码展示了每个聚类中心点的额外信息：

plt.scatter(X[:, 0], X[:, 1], c=kmeans_labels, s=50, cmap='viridis')

plt.scatter(kmeans.cluster_centers_[:, 0], kmeans.cluster_centers_[:, 1], s=200, c='red', marker='X', label='Cluster Centers')

运行代码列表 7.1 中的代码，你会看到生成两个图像。图 7.1 显示了三个聚类，而图 7.2 显示了带有红色中心点的三个聚类。

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p212-1.jpg)

图 7.1 三种聚类

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p212-2.jpg)

图 7.2 三种聚类及其中心

基于层次聚类算法的机器学习模型

本节包含了一个示例，展示了 GPT-4 使用层次聚类算法和合成数据集生成机器学习模型。本节的前半部分包含了 GPT-4 执行步骤的解释，随后是代码列表 7.2，其中包含了 GPT-4 生成的基于 Python 的代码。

让我们通过以下步骤在数据集上应用层次聚类算法：

1. 生成合成数据集：我们将使用 Scikit-learn 的 make_blobs 函数创建一个带有聚类的合成数据集。

2. 可视化数据集：绘制数据集以查看聚类。

3. 计算链接矩阵：使用 SciPy 中的链接函数，它将捕捉点之间的层次关系。

4. 树状图可视化：显示树状图以可视化聚类是如何逐步合并的。

5. 切割树状图：为了确定聚类的数量，我们将切割树状图并检索聚类标签。

6. 可视化聚类：我们将根据层次聚类识别的聚类对数据集进行着色绘图。

让我们再次通过生成合成数据集并对其应用层次聚类算法来继续。

这里是生成的包含三个聚类的数据集。

接下来，我们将使用 SciPy 库中的链接函数来计算链接矩阵。这个矩阵将捕捉数据点之间的层次关系。然后，我们将使用树状图来可视化这种关系。

这里是层次聚类产生的树状图。每条垂直线代表两个聚类的合并。垂直线的高度表示合并发生的距离。当你从树状图的底部移动到顶部时，聚类会依次合并，直到只剩下一个大聚类。

为了决定我们数据集的簇数量，我们将剪裁树状图。一种常见的做法是选择一个距离阈值，并在该距离处画一条水平线。水平线与垂直线相交的次数就是簇的数量。

在这个演示中，我们将剪裁树状图以检索三个簇（因为我们最初生成数据时创建了三个簇）。然后我们将可视化这些簇。

这是层次聚类算法在合成数据集上的结果。数据点根据剪裁树状图所识别的簇进行着色。

算法已成功识别并将数据点分组到三个不同的簇中，这与合成数据的生成方式相吻合。

列表 7.2(Listing 7.2)显示了 hierarchical_clustering_GPT4.py 的内容，展示了如何使用层次聚类算法和 death.csv 数据集创建机器学习模型。

列表 7.2: hierarchical_clustering_GPT4.py

# 导入必要的库

from sklearn.datasets import make_blobs

import matplotlib.pyplot as plt

import numpy as np

from scipy.cluster.hierarchy import dendrogram, linkage, fcluster

# 再次生成合成数据集

X_hc, y_hc = make_blobs(n_samples=150, centers=3, random_state=42, cluster_std=2.0)

# 可视化数据集

plt.figure(figsize=(8, 6))

plt.scatter(X_hc[:, 0], X_hc[:, 1], c=y_hc, s=50, cmap='viridis')

plt.title("具有 3 个簇的生成数据集")

plt.xlabel("特征 1")

plt.ylabel("特征 2")

plt.show()

# 计算连接矩阵

Z = linkage(X_hc, 'ward') # 使用'ward'方法作为连接标准

# 显示树状图

plt.figure(figsize=(10, 7))

dendrogram(Z)

plt.title("层次聚类树状图")

plt.xlabel("数据点")

plt.ylabel("欧几里得距离")

plt.show()

列表 7.2(Listing 7.2)开始于几个导入语句，随后调用 make_blobs()创建合成数据集。下一个代码块通过此代码片段生成并显示从生成数据集中的数据创建的散点图：

plt.scatter(X[:, 0], X[:, 1], c=y, s=50, cmap='viridis')

列表 7.2 的下一段代码通过调用 linkage()方法初始化变量 Z，以执行层次/聚合聚类，随后是一段代码调用 dendrogram(Z)来显示树状图。有关更详细的信息，请参阅 sklearn 文档中关于 linkage()方法的说明：

[`docs.scipy.org/doc/scipy/reference/generated/scipy.cluster.hierarchy.linkage.html#scipy.cluster.hierarchy.linkage`](https://docs.scipy.org/doc/scipy/reference/generated/scipy.cluster.hierarchy.linkage.html#scipy.cluster.hierarchy.linkage)

在 列表 7.2 中运行代码，你会看到生成三个图像。图 7.3 显示了三个簇，图 7.4 显示了一棵树状图（这是一种树状结构），它可视化 图 7.3 中显示的三个簇。

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p215.jpg)

图 7.3 三个簇

使用 DBSCAN 算法的机器学习模型

本节包含了一个示例，展示了 GPT-4 使用 DBSCAN 算法和合成数据集生成机器学习模型。本节的前半部分包含了 GPT-4 执行的步骤解释，随后是 列表 7.3，其中包含了 GPT-4 生成的基于 Python 的代码。

使用 DBSCAN 算法创建 ML 模型的过程涉及以下步骤：

1. 生成合成数据集：我们将重复使用我们之前创建的带有 blob 的数据集。

2. 可视化数据集：为了理解簇分布

3. 应用 DBSCAN：使用 DBSCAN 算法识别数据集中的簇。

4. 可视化结果：根据 DBSCAN 识别的簇来着色数据集。

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p216.jpg)

图 7.4 一棵树状图

让我们从可视化之前生成的合成数据集开始。

这里是我们将使用 DBSCAN 算法进行聚类的生成数据集。

现在，让我们应用 DBSCAN 算法来识别簇。

这里是 DBSCAN 算法在合成数据集上的结果。数据点根据 DBSCAN 识别的簇进行着色。

DBSCAN 已成功识别数据集中的簇。请注意，DBSCAN 可能会将一些点标记为噪声（通常标记为“-1”）。在这个可视化中，似乎所有点都已分配到簇中，这表明在这个特定实例中没有噪声。

列表 7.3 展示了 DBSCAN_GPT4.py 的内容，说明了如何使用 DBSCAN 算法和 death.csv 数据集创建机器学习模型。

列表 7.3: DBSCAN_GPT4.py

# 导入必要的库

from sklearn.datasets import make_blobs

import matplotlib.pyplot as plt

import numpy as np

from scipy.cluster.hierarchy import dendrogram, linkage, fcluster

# 再次生成合成数据集

X_hc, y_hc = make_blobs(n_samples=150, centers=3, random_state=42, cluster_std=2.0)

# 可视化之前生成的数据集

plt.figure(figsize=(8, 6))

plt.scatter(X_hc[:, 0], X_hc[:, 1], c=y_hc, s=50, cmap='viridis')

plt.title("生成的数据集")

plt.xlabel("特征 1")

plt.ylabel("特征 2")

plt.show()

from sklearn.cluster import DBSCAN

# 应用 DBSCAN 聚类

dbscan = DBSCAN(eps=2.5, min_samples=5)

dbscan_labels = dbscan.fit_predict(X_hc)

# 可视化 DBSCAN 识别的簇

plt.figure(figsize=(8, 6))

plt.scatter(X_hc[:, 0], X_hc[:, 1], c=dbscan_labels, s=50, cmap='viridis')

plt.title("DBSCAN 聚类结果")

plt.xlabel("特征 1")

plt.ylabel("特征 2")

plt.show()

列表 7.3 以几个导入语句开始，接着调用 make_blobs() 创建一个合成数据集。下一个代码块从生成的数据集中的数据生成并显示散点图。

列表 7.3 的下一部分初始化变量 dbscan 为从 sklearn.cluster 导入的类 DBSCAN 的一个实例。请注意，变量 dbscan_labels 使用变量 dbscan 的 fit_predict() 方法的结果进行初始化。dbscan_labels 的内容是一系列聚类标签，其中“噪声”样本被分配标签“-1”。此外，参数 eps 指定了两个样本之间的最大距离，一个样本被视为另一个样本的邻域。

列表 7.3 的最后一部分创建了一个散点图，显示了 DBSCAN 在数据集中识别出的聚类。运行 列表 7.3 中的代码，您将看到两个生成的图像。图 7.5 显示了三个聚类，而 图 7.6 显示了带有聚类标签的三个聚类。

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p218-1.jpg)

图 7.5 生成的数据集

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p218-2.jpg)

图 7.6 带有聚类标签的三个聚类

摘要

本章是您的第三个完整章节，其中包含由 GPT-4 生成的聚类材料。在简要概述聚类之后，您看到了十个聚类算法及其优缺点列表。此外，您还学习了聚类算法的度量标准。

最后，您看到了 GPT-4 生成的 Python 代码示例，包括 kMeans、层次聚类和 DBSCAN 聚类算法。

接下来，您看到了 k-means 算法的 Python 代码示例，这是机器学习中流行的聚类算法之一。然后您学习了层次聚类算法，接着是一个使用此算法的 Python 代码示例。此外，您还看到了 DBSCAN 算法的 Python 代码示例，这是机器学习中另一种流行的聚类算法。

第八章

CHATGPT 和数据可视化

本章包含使用 ChatGPT 和 GPT-4 进行数据可视化的示例，例如基于数据集（例如，泰坦尼克号数据集）的图表和图形。ChatGPT 通过高级数据分析插件生成了所有代码示例。ChatGPT 还为基于 Python 的代码示例生成了一些辅助文本。

本章的第一部分描述了在 ChatGPT 中上传数据集的过程，然后为解释给定数据集的特征、生成可视化以及下载精选数据集等任务提供提示。您还将学习如何提示 ChatGPT 创建和训练机器学习模型。

本章的第二部分包含使用 Matplotlib 进行数据可视化的示例，其中代码示例由 ChatGPT 生成。本章的第三部分包含使用 Seaborn 进行数据可视化的示例，其中代码示例由 ChatGPT 生成。

在你阅读本章内容之前，请记住，本章以及第五章、第六章和第七章中 GPT-4 生成的 AI 内容已经应用了一些格式。然而，额外的格式已经被保持在最低限度，以便你熟悉 GPT-4 的风格。

使用图表和图形

如果你已经与图表和图形工作过，那么你已经知道每种图表类型都有其独特的优势，并且最适合特定类型的数据和分析。图表的选择通常取决于数据的性质和想要得出的具体见解。本节包含多个小节，提供了关于各种图表和图形的信息，如下所示：

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

前面列表中的大多数图表和图形将在以下小节中进行讨论。

柱状图

柱状图用矩形条表示数据。条形的长度与它们代表的值成比例。它们可以是垂直的（柱状图）或水平的。一个使用示例涉及比较商店中不同产品的销售情况。

以下列出了一些柱状图的优点：

+   容易理解和广泛认可

+   可以比较单个或多个数据系列

+   适用于显示跨越多个类别的数据

以下列出了一些柱状图的缺点：

+   不适合显示随时间变化的模式或趋势

+   当比较太多类别时可能会变得杂乱

饼图

饼图以圆形格式表示数据，其中各个部分（切片）显示类别与整体的比例。一个使用示例涉及表示一个行业中不同公司的市场份额。

以下列出了一些饼图的优点：

+   简单的视觉展示，显示部分与整体的关系

+   清楚地表示比例

+   当有有限数量的类别时，效果良好

以下列出了一些饼图的缺点：

+   不适合比较单个类别

+   当切片过多时，可能会变得无效且难以解释

+   不显示绝对值，只显示比例

折线图

折线图通过直线连接数据点。它们主要用于可视化连续区间或时间段内的值。一个使用示例涉及跟踪一家公司在几年内的收入增长。

以下列出了一些折线图的优点：

+   适用于显示随时间变化的趋势

+   可以在一张图上比较多个数据系列

+   清晰地可视化数据点和区间

线形图的一些缺点如下：

+   不适合展示部分与整体的关系

+   当显示过多的数据系列时可能会变得杂乱

+   需要数据点的有意义顺序

热图

热图以矩阵格式表示数据，其中单个值以颜色表示。颜色强度通常表示值的幅度。一个使用示例是可视化网页不同部分的访问者活动。

热图的一些优点如下：

+   快速识别模式、相关性和集中区域

+   利用颜色有效地传达关于幅度的信息

热图的一些缺点如下：

+   不适合进行详细的数值分析

+   颜色选择至关重要；选择不当可能导致误解。

直方图

直方图是数据集分布的图形表示。它是连续变量概率分布的估计。一个使用示例是展示人口中年龄的分布。

直方图的一些优点如下：

+   通过指示位于值范围内的数据点数量，以提供数值数据的视觉解释

+   可以帮助识别数据分布模式

直方图的一些缺点如下：

+   不显示确切值

+   箱子的数量和宽度可以影响感知

箱线图

箱线图，或箱形图，通过四分位数来表示数据集的摘要。其中，“箱体”显示四分位距，而“须须”表示超出上下四分位数的变异。一个使用示例是对比不同团队的销售额表现。

箱线图的一些优点如下：

+   快速可视化数据的分布和偏度

+   识别异常值

箱线图的一些缺点如下：

+   不适合进行详细的分布分析

+   不显示数据的频率分布

帕累托图

帕累托图结合条形图和折线图来表示发生频率的累积频率。它识别数据集中的最重要因素。一个使用示例是确定哪些产品缺陷最频繁发生。

帕累托图的一些优点如下：

+   在大数据集中有效地突出最重要的因素

+   帮助优先考虑努力

帕累托图的一些缺点如下：

+   适用于排名和优先级相关的数据集

+   不适合展示数据点之间的关系

雷达图

雷达图是一种在二维图表中显示三个或更多定量变量的图形方法。数据点绘制在从中心开始的轴上。一个使用示例是对比产品的性能指标。

雷达图的一些优点如下：

+   可以比较多个定量变量

+   提供数据的视觉概述

下面列出了雷达图的一些缺点：

+   当比较太多数据集时可能会变得杂乱

+   当值相似时难以解释

树状图

树状图以嵌套矩形的形式显示层次数据。每个层次分支由彩色矩形表示。一个使用示例是可视化计算机上的存储使用情况。

下面列出了树状图的一些优点：

+   空间利用效率

+   可以使用大小和颜色表示多个维度

下面列出了树状图的一些缺点：

+   不适用于具有大量层次的数据集

+   当数据点过多时可能会变得难以解释

瀑布图

瀑布图表示依次发生的正或负值的累积效应。一个使用示例是可视化利润或收入如何受各种因素的影响。

下面列出了瀑布图的一些优点：

+   清晰地可视化正负顺序变化

+   帮助理解从一个数据点到另一个数据点的逐渐过渡

下面列出了瀑布图的一些缺点：

+   限于需要理解顺序变化的情况

+   当数据点过多时可能会变得难以理解

使用 MATPLOTLIB 的线图

以下提示被提供给 GPT-4 以生成用于简单线图的 Python 代码：“请生成用于绘制简单线图的 Python 代码，以便可视化趋势。”

列表 8.1 显示了 ChatGPT 生成的 line_plots.py 文件的内容，该文件用于使用 Matplotlib 渲染线图。

列表 8.1: line_plot.py

import matplotlib.pyplot as plt

def plot_line(x, y, title, x_label, y_label):

plt.plot(x, y)

plt.title(title)

plt.xlabel(x_label)

plt.ylabel(y_label)

plt.grid(True)

plt.show()

# 用法

x = [1, 2, 3, 4, 5]

y = [2, 4, 1, 3, 5]

plot_line(x, y, '样本线图', 'X 轴', 'Y 轴')

列表 8.1 从一个导入语句开始，然后定义了用于渲染线图的函数 plot_line()。Matplotlib 的 plot() 函数提供了一个简单的方式来创建线图。在这个函数中，我们在 x 和 y 轴上可视化趋势。

代码的下一部分初始化了 Python 列表 x 和 y，然后使用三个字符串调用 plot_line() 函数，这三个字符串分别是标题、横轴和纵轴的值。图 8.1 显示了在 列表 8.1 中启动代码的输出。

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p226.jpg)

图 8.1 使用 Matplotlib 创建的线图

使用 MATPLOTLIB 的饼图

饼图非常适合显示类别之间的比例数据。Matplotlib 的饼图函数提供了一个简单的方式来实现这一点。以下提示被提供给 GPT-4 以生成饼图的 Python 代码：“请生成用于显示简单饼图的 Python 代码。”

列表 8.2 显示了 ChatGPT 生成的 pie_chart1.py 文件的内容，该文件用于使用 Matplotlib 渲染饼图。

列表 8.2: pie_chart1.py

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p227-2.jpg)

列表 8.2 以与 列表 8.1 类似的方式开始，除了生成了用于生成饼图的 plot_pie() 函数。列表 8.2 的下一部分初始化了 Python 列表的标签和大小。使用这些列表以及一个作为饼图标题显示的字符串调用 plot_pie() 函数。图 8.2 显示了通过在 列表 8.2 中启动代码生成的饼图。

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p227-1.jpg)

图 8.2 使用 Matplotlib 创建的饼图

使用 MATPLOTLIB 绘制箱线图

箱线图，或箱线图，提供了数据分布的摘要，突出了中心趋势、变异性和异常值的存在。它们在比较不同组之间的分布时特别有用。它们可以根据最小值、第一四分位数、中位数、第三四分位数和最大值显示数据的分布。

以下提示被提供给 GPT-4 以生成用于箱图的 Python 代码：“请生成用于绘制箱图的 Python 代码。”

列表 8.3 显示了 ChatGPT 生成的 boxplot1.py 的内容，用于使用 Seaborn 绘制箱线图。

列表 8.3：boxplot1.py

import matplotlib.pyplot as plt

import seaborn as sns

import matplotlib.pyplot as plt

def plot_box(data, column):

plt.boxplot(data[column])

plt.show()

# 用法

data = sns.load_dataset("iris")

plot_box(data, "sepal_length")

列表 8.3 包含三个导入语句，随后是生成箱图的 plot_box() 函数。列表 8.3 的下一部分初始化变量 data 为 Seaborn 内置的 iris 数据集的内容，然后使用 data 和一个字符串调用 plot_box()，该字符串指定在绘制箱图时使用的特征（列）。图 8.3 显示了通过在 列表 8.3 中启动代码生成的箱图。

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p228.jpg)

图 8.3 使用 Matplotlib 创建的箱线图

使用 MATPLOTLIB 进行时间序列可视化

时间序列数据，其中观测值是在固定时间间隔内进行的，可以使用线图进行可视化。这使得分析师能够辨别趋势、模式和异常。以下提示被提供给 GPT-4 以生成用于时间序列数据的 Python 代码：“请生成用于绘制时间序列数据的 Python 代码。”

列表 8.4 显示了 ChatGPT 生成的 time_series.py 的内容，用于使用 Matplotlib 绘制时间序列。

列表 8.4：time_series.py

import matplotlib.pyplot as plt

import pandas as pd

def plot_time_series(dates, values, title):

plt.figure(figsize=(10, 5))

plt.plot(dates, values)

plt.title(title)

plt.xlabel('日期')

plt.ylabel('值')

plt.tight_layout()

plt.show()

# 用法

dates = pd.date_range(start="2021-01-01", periods=10, freq='D')

values = [x**1.5 for x in range(10)]

plot_time_series(dates, values, '样本时间序列数据')

Figure 8.4 displays the time series that is rendered by launching the code in Listing 8.4.

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p229.jpg)

FIGURE 8.4 A time series created with Matplotlib

STACKED BAR CHARTS WITH MATPLOTLIB

Stacked bar charts allow for the representation of subgroups in each category, giving a sense of the total size across categories and the subgroup distributions within them. The following prompt was supplied to GPT-4 to generate Python code for a stacked bar chart: “Please generate Python code to display a stacked bar chart.”

Listing 8.5 displays the content of stacked_bar_charts.py that ChatGPT generated to render stacked bar charts using Matplotlib.

LISTING 8.5: stacked_bar_charts.py

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p230-1.jpg)

Figure 8.5 displays the stacked bar charts that are rendered by launching the code in Listing 8.5.

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p230-2.jpg)

FIGURE 8.5 Stacked bar charts generated by ChatGPT

DONUT CHARTS USING MATPLOTLIB

Donut charts are a variation of pie charts. The hollow center can be used for additional annotations or just to provide a different aesthetic. They represent data proportionally among categories, and are similar to a pie chart but with a hollow center. The following prompt was supplied to GPT-4 to generate Python code for a donut chart: “Please generate Python code to plot a donut chart.”

Listing 8.6 displays the content of donut_charts.py that ChatGPT generated to render a donut chart using Matplotlib.

LISTING 8.6: donut_charts.py

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

plot_donut_chart(sizes, labels, ''Sample Donut Char'')

Figure 8.6 displays the donut chart that is rendered by launching the code in Listing 8.6.

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p231.jpg)

FIGURE 8.6 A donut chart created using Matplotlib

3D SURFACE PLOTS WITH MATPLOTLIB

Three-dimensional (3D) surface plots are used for visualizing functions with two variables. They can reveal intricate patterns and relationships in the data. The following prompt was supplied to GPT-4 to generate Python code for a 3D surface: “Please generate Python code to plot a 3D surface.”

Listing 8.7 displays the content of 3d_surface.py that ChatGPT generated to render a 3D surface using mpl_toolkits.

Incidentally, if you encounter issues with mpl_toolkits, please read the following post, which contains useful information:

[`stackoverflow.com/questions/37661119/python-mpl-toolkits-installation-issue`](https://stackoverflow.com/questions/37661119/python-mpl-toolkits-installation-issue)

LISTING 8.7: 3d_surface.py

import matplotlib.pyplot as plt

import numpy as np

def plot_3d_surface(x, y, z):

fig = plt.figure()

ax = fig.add_subplot(111, projection='3')

ax.plot_surface(x, y, z, cmap='viridi')

plt.show()

# 用法

x = np.linspace(-5, 5, 50)

y = np.linspace(-5, 5, 50)

x, y = np.meshgrid(x, y)

z = np.sin(np.sqrt(x**2 + y**2))

plot_3d_surface(x, y, z)

列表 8.7 从两个导入语句开始，然后是 plot_3d_surface()函数，用于渲染 3D 图。列表 8.7 的第二部分通过 NumPy 的 linspace()函数初始化变量 x 和 y，该函数将区间划分为一组等大小的子区间。

例如，代码片段 np.linspace(-5, 5, 50)将区间[-5,5]划分为 50 个等间距的点，这意味着有 49 个等宽的区间。你可以通过将 50 替换为 3 来证明这一点：结果是左端点-5、中点和右端点 5，这创建了 2（=3-1）个区间。

The next code snippet updates x and y with the result of invoking the meshgrid() function in NumPy, after which z is defined as the trigonometric sine function applied to the number that equals the distance of the point (x,y) from the origin. Although the latter number is monotonically increasing as the point (x,y) shifts away from the origin, and z is the sine of that distance, which is a periodic function: as a result, you will see a rolling wave-like effect.

列表 8.7 中的最后一个代码片段调用 plot_3d_surface()函数，使用变量 x、y 和 z 中的值。在列表 8.7 中运行代码，你将看到图 8.7 中显示的 3D 表面。

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p233.jpg)

图 8.7 使用 Matplotlib 创建的 3D 表面

使用 Matplotlib 的径向（或蜘蛛）图

径向（或蜘蛛）图用于以二维图表的形式可视化多维数据，其中包含三个或更多定量变量。每个变量都表示在从图表中心开始的单独轴上。以下提示被提供给 GPT-4 以生成用于显示径向图的 Python 代码：“请生成用于显示径向图的 Python 代码。”

列表 8.8 显示了 ChatGPT 生成的 radial_charts.py 的内容，该内容使用 Matplotlib 渲染径向图。

列表 8.8：radial_charts.py

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

ax.set_yticklabels([])

# 以下代码片段会导致错误：

# ax.set_xticks(angles)

# 以下代码片段是正确的：

ax.set_xticks(angles[:-1]) # Exclude the last angle since it’s cyclic

ax.set_xticklabels(categories)

plt.title(title, size=20, color="blue", y=1.1)

plt.show()

# 用法

categories = ["A", "B", "C", "D"]

values = [50, 30, 60, 40]

plot_spider_chart(values, categories, 'Sample Spider Chart')

列表 8.8 以两个导入语句开始，随后是 Python 函数 plot_spider_chart()，该函数用于渲染径向图。列表 8.8 的第二部分初始化变量 categories 和 values 为两个 Python 列表，然后使用变量 categories、values 和用于图表标题的文本字符串调用函数 plot_spider_chart()。图 8.8 显示了通过在列表 8.8 中启动代码生成的径向图。

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p234.jpg)

图 8.8 使用 Seaborn 创建的径向图

有一个额外的细节将帮助您调试 ChatGPT 为您生成的代码。让我们看看列表 8.8 中的加粗代码块：

# 以下代码片段会导致错误：

# ax.set_xticks(angles)

# 以下代码片段是正确的：

ax.set_xticks(angles[:-1]) # 排除最后一个角度，因为它具有循环性

如果您将这两个代码片段的顺序颠倒，代码将无法正确工作。以下是与 ChatGPT 的“对话”以寻求解决方案。

作者：“我上传了包含您为我编写的代码的 radial_charts.py。然而，这段代码导致以下错误：ValueError：固定定位器位置的数量（5），通常来自对 set_ticks 的调用，与刻度标签的数量（4）不匹配。您能提供解决方案吗？”

ChatGPT 的回复如下：

感谢您提供 radial_charts.py 文件。让我们首先读取其内容，以了解代码的结构和上下文。之后，我将分析提到的错误潜在原因并提供解决方案。

提供的 radial_charts.py 文件包含一个函数，plot_spider_chart，该函数旨在使用给定的值和类别绘制蜘蛛（或雷达）图。

根据您报告的错误和代码结构，问题可能源于刻度位置的数量（由 ax.set_xticks(angles) 设置）与刻度标签的数量（由 ax.set_xticklabels(categories) 设置）不匹配。

为了解决这个问题，我将确保刻度位置的数量与刻度标签的数量相匹配。让我们进行这个调整，并提供函数的修正版本。

作者：“现在工作正常了！感谢您的帮助！”

ChatGPT 的回复如下：

欢迎使用！很高兴听到它现在按预期工作。如果您将来有任何更多问题或需要进一步的帮助，请随时联系。祝您编码愉快！

MATPLOTLIB 的等高线图

等高线图有助于使用等高线在二维中可视化三维数据。以下提示被提供给 GPT-4 以生成绘制等高线的 Python 代码：“请生成绘制等高线的 Python 代码。”

列表 8.9 显示了 ChatGPT 生成的用于使用 Matplotlib 绘制等高线的 contour_lines.py 的内容。

列表 8.9: contour_lines.py

import matplotlib.pyplot as plt

import numpy as np

def plot_contour(x, y, z):

plt.contourf(x, y, z, 20, cmap='viridis')

plt.colorbar()

plt.show()

# 用法

x = np.linspace(-5, 5, 50)

y = np.linspace(-5, 5, 50)

x, y = np.meshgrid(x, y)

z = np.sin(np.sqrt(x**2 + y**2))

plot_contour(x, y, z)

列表 8.9 包含两个导入语句，然后定义了函数 plot_contour()，该函数为代码示例渲染等高线。请注意，列表 8.9 的第二部分与 列表 8.7 的后半部分代码几乎相同。图 8.9 显示了通过运行 列表 8.9 中的代码生成的等高线图。

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p236.jpg)

图 8.9 使用 Seaborn 创建的等高线图

向量场流线图

流线图用于显示向量场，如风向。它们提供了流动轨迹的快照，并且可以针对标量数据进行着色编码，以及将向量场可视化为流线。以下提示被提供给 GPT-4 以生成用于向量场的 Python 代码：“请生成用于显示向量场的 Python 代码。”

列表 8.10 显示了 ChatGPT 生成的用于使用 Seaborn 绘制流线图的 stream_plot.py 的内容。

列表 8.10: stream_plot.py

import matplotlib.pyplot as plt

import seaborn as sns

import numpy as np

def plot_streamplot(x, y, u, v):

plt.streamplot(x, y, u, v, density=1)

plt.show()

# 用法

x = np.linspace(-5, 5, 10)

y = np.linspace(-5, 5, 10)

# 这会导致错误：

#y, x = np.meshgrid(y, x)

# 这工作正常：

x, y = np.meshgrid(x, y)

u = -1 - x**2 + y

v = 1 + x - y**2

plot_streamplot(x, y, u, v)

图 8.10 显示了通过运行 列表 8.10 中的代码生成的流线图。

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p237.jpg)

图 8.10 使用 Seaborn 创建的流线图

ChatGPT 中的初始代码 列表 8.10 未能正确工作，因此我在与 ChatGPT 的以下“对话”中请求其提供解决方案。

作者：“我上传了包含你为我编写的代码的 stream_plot.py。这段代码导致以下错误：ValueError: 'x' 的行必须相等。你能提供解决方案吗？”

ChatGPT 的回复如下：

数组 x, y, u 和 v 的形状都是 (10,10)，这意味着它们在维度上是一致的。错误信息“ValueError: 'x' 的行必须相等”表明，问题可能出在 x 数组行内的值上，而不是其形状。

线 y, x = np.meshgrid(y, x) 交换了原始的 x 和 y 数组。这可能会导致 x 数组的行出现不一致。

为了解决错误，我将修改 meshgrid 的创建并确保 x 和 y 数组被正确初始化。让我们进行必要的调整。

作者：“这可行！谢谢你的帮助！”

ChatGPT 的回复如下：

欢迎使用！很高兴听到它现在按预期工作。如果您将来有任何更多问题或需要进一步的帮助，请随时联系。祝您编码愉快！

向量场箭头图

箭头图对于表示向量场非常有用，可以显示向量的方向和大小。例如，它们可以在物理学中用来显示电场或流体流动方向。以下提示被提供给 GPT-4 以生成用于箭头图的 Python 代码：“请生成用于绘制箭头图的 Python 代码。”

列表 8.11 显示了 ChatGPT 生成的用于绘制使用 Matplotlib 的箭头图的 quiver_plot.py 的内容。

列表 8.11：quiver_plot.py

导入 matplotlib.pyplot 库（import matplotlib.pyplot as plt）

导入 numpy 库（import numpy as np）

定义绘制箭头图的函数（def plot_quiver(x, y, u, v):）

绘制箭头图（plt.quiver(x, y, u, v, scale=20)）

显示图形（plt.show()）

# 使用方法

创建 x 和 y 的网格（x, y = np.meshgrid(np.arange(0, 2 * np.pi, .2), np.arange(0, 2 * np.pi, .2)）

计算 x 的正弦值（u = np.sin(x)）

计算 y 的余弦值（v = np.cos(y)）

绘制箭头图（plot_quiver(x, y, u, v)）

![图 8.11](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-#fig_8-11)显示了通过运行列表 8.11 中的代码生成的箭头图。

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p239.jpg)

![图 8.11](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-#fig_8-11)显示了使用 Seaborn 创建的箭头图。

极坐标图

极坐标图（或径向图）适合在二维图表中显示多变量数据，其中变量表示在同一起点开始的轴上。它们对于查看基于角度和幅度的模式非常有用。以下提示被提供给 GPT-4 以生成用于极坐标图的 Python 代码：“请生成用于显示极坐标图的 Python 代码。”

列表 8.12 显示了 ChatGPT 生成的用于使用 Seaborn 和 ChatGPT 生成绘制堆叠极坐标图的 polar_plots.py 的内容。

列表 8.12：polar_plots.py

导入 matplotlib.pyplot 库（import matplotlib.pyplot as plt）

导入 numpy 库（import numpy as np）

定义绘制极坐标图的函数（def plot_polar(theta, radii, title=""):）

创建一个大小为（8, 4）的图形（plt.figure(figsize=(8, 4)）

在极坐标投影中创建子图（ax = plt.subplot(111, projection='polar'）

绘制 theta 和 radii 的曲线（ax.plot(theta, radii)）

设置标题（ax.set_title(title)）

显示图形（plt.show()）

# 使用方法

计算 theta 的线性空间（theta = np.linspace(0, 2 * np.pi, 100)）

计算半径（radii = np.abs(np.sin(theta) * 2)）

绘制极坐标图（plot_polar(theta, radii, "Sample Polar Plot")）

![图 8.12](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-#fig_8-12)显示了通过运行列表 8.12 中的代码生成的极坐标图。

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p240.jpg)

![图 8.12](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-#fig_8-12)显示了使用 Matplotlib 创建的极坐标图。

使用 Seaborn 绘制条形图

Seaborn 为 Matplotlib 提供了一个高级接口，使得创建时尚的图表更加容易。此条形图有助于可视化不同类别中的数据。以下提示被提供给 GPT-4 以生成用于条形图的 Python 代码：“请生成用于渲染条形图的 Python 代码。”

注意：Seaborn 与 Pandas 集成时效果最佳。

列表 8.13 显示了 ChatGPT 生成的用于将条形图转换为使用 Seaborn 的 bar_chart1.py 的内容。

列表 8.13：bar_chart1.py

导入 matplotlib.pyplot 库（import matplotlib.pyplot as plt）

导入 seaborn 库（import seaborn as sns）

导入 pandas 库（import pandas as pd）

定义绘制条形图的函数（def plot_bar(data, x_col, y_col):）

使用 Seaborn 绘制条形图（sns.barplot(x=x_col, y=y_col, data=data)）

显示图形（plt.show()）

# 使用方法

data = pd.DataFrame({

'Category': ['A', 'B', 'C'],

'Values': [10, 20, 15]

})

plot_bar(data, 'Category', 'Values')

清单 8.13 从三个导入语句开始，接着是用于绘制柱状图的 plot_bar() 函数。清单 8.13 的后半部分初始化了 Pandas 数据帧 data，然后使用 data 和用于标记水平轴的字符串以及用于标记垂直轴的字符串调用 plot_bar()。图 8.13 显示了通过启动清单 8.13 中的代码生成的柱状图。

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p241.jpg)

图 8.13 ChatGPT 生成的柱状图

使用 SEABORN 绘制带有回归线的散点图

散点图显示数据点并利用回归线来帮助揭示关系。以下提示被提供给 GPT-4 以生成用于回归线的 Python 代码：“请生成用于绘制回归线的 Python 代码。”

清单 8.14 显示了 ChatGPT 生成的用于使用 Seaborn 绘制散点图的 scatter_plot.py 的内容。

清单 8.14: scatter_plot.py

import matplotlib.pyplot as plt

import pandas as pd

import seaborn as sns

def plot_scatter_with_regression(data, x_col, y_col):

sns.regplot(x=x_col, y=y_col, data=data)

plt.show()

# 用法

data = pd.DataFrame({

'X_Values': [10, 20, 30, 40, 50],

'Y_Values': [15, 25, 35, 45, 55]

})

plot_scatter_with_regression(data, 'X_Values', 'Y_Values')

散点图用于可视化两个变量之间的关系。Seaborn 的 regplot() 函数不仅绘制数据点，还拟合回归线。

清单 8.14 从三个导入语句开始，然后是用于绘制散点图的 plot_scattter_with_regression() 函数。清单 8.13 的后半部分初始化了 Pandas 数据帧 data，然后使用变量 data 调用 plot_scattter_with_regression()。图 8.14 显示了通过启动清单 8.14 中的代码生成的散点图。

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p242.jpg)

图 8.14 ChatGPT 生成的散点图

使用 SEABORN 绘制相关矩阵的热图

热图在表示数据矩阵方面非常强大，颜色表示大小。一个常见的用例是可视化相关矩阵，这有助于揭示不同变量之间的关系。以下提示被提供给 GPT-4 以生成用于简单折线图的 Python 代码：“请生成用于绘制热图的 Python 代码。”

清单 8.15 显示了 ChatGPT 生成的用于使用 Matplotlib 绘制线条的 heatmap1.py 的内容。

清单 8.15: heatmap1.py

import matplotlib.pyplot as plt

import pandas as pd

import seaborn as sns

def plot_heatmap(data):

correlation_matrix = data.corr()

sns.heatmap(correlation_matrix, annot=True, cmap='coolwarm')

plt.show()

# 用法

data = pd.DataFrame({

'A': [1, 2, 3, 4, 5],

'B': [5, 4, 3, 2, 1],

'C': [2, 3, 4, 5, 6]

})

plot_heatmap(data)

列表 8.15 从三个导入语句和用于渲染热图的 `plot_heatmap()` 函数开始。列表 8.15 的后半部分初始化 Pandas 数据框数据，然后使用变量 `data` 调用 `plot_heatmap()`。图 8.15 显示了通过运行列表 8.15 中的代码生成的渲染热图。

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p243.jpg)

图 8.15 使用 Matplotlib 创建的热图

使用 Seaborn 的直方图

直方图是可视化数据分布的强大工具。Seaborn 的 `histplot()` 函数提供了一种轻松生成具有额外功能（如核密度估计）的直方图的方法。以下提示被提供给 GPT-4 以生成用于直方图的 Python 代码：“请生成用于绘制直方图的 Python 代码。”

列表 8.16 显示了 ChatGPT 生成的用于使用 Seaborn 绘制直方图的 `histogram1.py` 的内容。

列表 8.16: histogram1.py

import matplotlib.pyplot as plt

import seaborn as sns

def plot_histogram(data, column, bins=10):

sns.histplot(data[column], bins=bins)

plt.show()

# 用法

data = sns.load_dataset("iris")

plot_histogram(data, "sepal_length")

列表 8.16 从两个导入语句和用于渲染直方图的 `plot_histogram()` 函数开始。列表 8.16 的后半部分使用 Seaborn 内置数据集 iris 的内容初始化 Pandas 数据框数据，然后使用变量 `data` 调用 `plot_histogram()`。图 8.16 显示了通过运行列表 8.16 中的代码生成的 iris 数据集的热图。

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p244.jpg)

图 8.16 ChatGPT 生成的直方图

使用 Seaborn 的小提琴图

小提琴图提供了对数据分布的更深入理解。它们结合了箱线图和直方图的特点，展示了数据在不同值处的概率密度。您可以将箱线图和直方图的方面结合起来，以提供对数据分布的更丰富描述。以下提示被提供给 GPT-4 以生成用于小提琴图的 Python 代码：“请生成用于绘制小提琴图的 Python 代码。”

列表 8.17 显示了 ChatGPT 生成的用于使用 Seaborn 绘制小提琴图的 `violin_plots.py` 的内容。

列表 8.17: violin_plots.py

import seaborn as sns

def plot_violin(data, x_col, y_col):

sns.violinplot(x=x_col, y=y_col, data=data)

plt.show()

# 用法

data = sns.load_dataset("iris")

plot_violin(data, "species", "sepal_length")

列表 8.17 从一个导入语句和用于渲染小提琴图的 `plot_violin()` 函数开始。列表 8.17 的后半部分使用 Seaborn 内置数据集 iris 的内容初始化 Pandas 数据框数据，并使用变量 `data` 调用 `plot_violin()`。图 8.17 显示了通过运行列表 8.17 中的代码生成的渲染小提琴图。

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p245.jpg)

图 8.17 使用 Seaborn 创建的小提琴图

使用 SEABORN 创建成对图

当处理具有多个特征的集合时，可视化特征之间的成对关系通常很有帮助。Seaborn 的 pairplot()函数可以生成散点图的矩阵，允许探索这种关系。以下提示被提供给 GPT-4 以生成用于成对图的 Python 代码：“请生成显示成对图的 Python 代码。”

列表 8.18 显示了 ChatGPT 生成的 pair_plots.py 的内容，用于使用 Matplotlib 绘制线条。

列表 8.18: pair_plots.py

import matplotlib.pyplot as plt

import seaborn as sns

def plot_pairplot(data):

sns.pairplot(data)

plt.show()

# 用法

data = sns.load_dataset("iris")

plot_pairplot(data)

列表 8.18 从两个导入语句和用于渲染成对图的 plot_pairplot()函数开始。列表 8.18 的第二部分使用 Seaborn 内置数据集 iris 的内容初始化 Pandas 数据帧 data，然后使用变量 data 调用 plot_pair()。图 8.18(#fig_8-18)显示了通过在列表 8.18(#lis_8-18)中运行代码生成的成对图。

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p247.jpg)

图 8.18 使用 Matplotlib 创建的成对图

使用 SEABORN 的面板网格

面板网格是一种根据分类变量在多个子图上可视化数据分布的方式。每个面板（子图）代表一个类别。以下提示被提供给 GPT-4 以生成用于面板网格的 Python 代码：“请生成绘制面板网格的 Python 代码。”

列表 8.19 显示了 ChatGPT 生成的 facet_grids.py 的内容，用于创建和渲染按类别分割的多个图。

列表 8.19: facet_grids.py

import matplotlib.pyplot as plt

import seaborn as sns

def plot_facetgrid(data, x_col, y_col, facet_col):

g = sns.FacetGrid(data, col=facet_col)

g.map(sns.scatterplot, x_col, y_col)

g.add_legend()

plt.show()

# 用法

data = sns.load_dataset("iris")

plot_facetgrid(data, "sepal_length", "sepal_width", "species")

列表 8.19 从两个导入语句和用于渲染面板的 plot_facetgrid()函数开始。列表 8.19 的第二部分使用 Seaborn 内置数据集 iris 的内容初始化 Pandas 数据帧 data，然后使用变量 data 调用 plot_pair()。图 8.19(#fig_8-19)显示了通过在列表 8.19(#lis_8-19)中运行代码生成的面板网格。

![image](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p248.jpg)

图 8.19 使用 Seaborn 创建的面板网格

层次聚类

Seaborn 的 clustermap 是一个二维矩阵数据集表示，其中行和列都是层次聚集的。这允许从复杂的数据集中出现模式。以热图格式可视化层次聚集关系。以下提示被提供给 GPT-4 以生成用于层次聚类的 Python 代码：“请生成用于显示层次聚类的 Python 代码。”

列表 8.20: cluster_map.py

导入 matplotlib.pyplot as plt

导入 seaborn as sns

def plot_clustermap(data):

sns.clustermap(data, method='average', cmap='coolwarm')

plt.show()

# 使用方法

data = sns.load_dataset("iris").drop("species", axis=1)

plot_clustermap(data)

列表 8.20 从两个导入语句和一个渲染聚类图的 plot_clustermap() 函数开始。列表 8.20 的第二部分使用 Seaborn 内置数据集 iris 的内容初始化 Pandas 数据帧 data，然后使用变量 data 调用 plot_pair()。图 8.20 显示了通过在列表 8.20 中启动代码生成的聚类图。

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p249.jpg)

图 8.20 使用 Seaborn 创建的聚类图

蜂窝图

蜂窝图将每个数据点放置在分类轴上，重叠最小，从而更好地表示值的分布。它创建了一个非重叠点的分类散点图。以下提示被提供给 GPT-4 以生成用于蜂窝图的 Python 代码：“请生成用于绘制蜂窝图的 Python 代码。”

列表 8.21 展示了 ChatGPT 生成的用于使用 Seaborn 绘制等高线的 swarm_plot.py 的内容。

列表 8.21: swarm_plot.py

导入 matplotlib.pyplot as plt

导入 seaborn as sns

def plot_swarm(data, x_col, y_col):

sns.swarmplot(x=x_col, y=y_col, data=data)

plt.show()

# 使用方法

data = sns.load_dataset("iris")

plot_swarm(data, "species", "sepal_length")

列表 8.21 从两个导入语句和一个渲染蜂窝图的 plot_swarm() 函数开始。列表 8.21 的第二部分使用 Seaborn 内置数据集 iris 的内容初始化 Pandas 数据帧 data，然后使用变量 data 调用 plot_swarm()。图 8.21 显示了通过在列表 8.21 中启动代码生成的蜂窝图。

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p250.jpg)

图 8.21 使用 Seaborn 创建的蜂窝图

二元数据的联合图

Seaborn 的 jointplot 显示了两个变量之间的关系。它结合了散点图、回归图，甚至与直方图一起的六边形图。它显示了两个变量之间的关系，以及它们的各自分布。以下提示被提供给 GPT-4 以生成用于二元数据的蜂窝图的 Python 代码：“请生成用于绘制二元数据的蜂窝图的 Python 代码。”

列表 8.22 展示了 ChatGPT 生成的用于使用 Seaborn 绘制联合图的 joint_plot.py 的内容。

列表 8.22: joint_plot.py

导入 matplotlib.pyplot 库

导入 seaborn 库

def plot_jointplot(data, x_col, y_col, kind='scatter'):

sns.jointplot(x=x_col, y=y_col, data=data, kind=kind)

plt.show()

# 使用方法

data = sns.load_dataset("iris")

plot_jointplot(data, "sepal_length", "sepal_width", "hex")

列表 8.22 从两个导入语句和用于渲染联合图的 plot_joint() 函数开始。列表 8.22 的第二部分使用 Seaborn 内置数据集 iris 的内容初始化 Pandas 数据帧 data，然后使用变量 data 调用 plot_pair()。图 8.22(#fig_8-22) 显示了通过运行列表 8.22(#lis_8-22) 中的代码所渲染的联合图。

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p251.jpg)

图 8.22 使用 Seaborn 创建的联合图

因子视图的点图

点图可以用来突出显示点之间的差异，尤其是在按因素（如使用示例中的性别）分类时。连接点的线条可以帮助强调任何趋势。用线条强调点之间的比较。以下提示被提供给 GPT-4 以生成用于点图的 Python 代码：“请生成用于显示点图的 Python 代码。”

列表 8.23 显示了 ChatGPT 生成的 point_plot.py 的内容，用于使用 Seaborn 渲染点图。

列表 8.23: point_plot.py

导入 matplotlib.pyplot 库

导入 seaborn 库

def plot_pointplot(data, x_col, y_col, hue=None):

sns.pointplot(x=x_col, y=y_col, hue=hue, data=data)

plt.show()

# 使用方法

data = sns.load_dataset("tips")

plot_pointplot(data, "day", "total_bill", "sex")

列表 8.23 从两个导入语句和用于渲染点图的 plot_pointplot() 函数开始。列表 8.23 的第二部分使用 Seaborn 内置数据集 tips 的内容初始化 Pandas 数据帧 data，然后使用变量 data 调用 plot_pointplot()。图 8.23(#fig_8-23) 显示了通过运行列表 8.23(#lis_8-23) 中的代码所渲染的点图。

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p252.jpg)

图 8.23 使用 Seaborn 创建的点图

SEABORN 的 KDE 图用于密度估计

核密度估计（KDE）图用于可视化连续变量的概率密度。它们可以被视为平滑的直方图，当想要辨别数据集的潜在分布时特别有用。以下提示被提供给 GPT-4 以生成用于 KDE 图的 Python 代码：“请生成用于渲染 KDE 图的 Python 代码。”

列表 8.24 显示了 ChatGPT 生成的 kde_plot.py 的内容，用于使用 Seaborn 渲染 KDE 图。

列表 8.24: kde_plot.py

导入 matplotlib.pyplot 库

导入 seaborn 库

def plot_kde(data, column):

sns.kdeplot(data[column], shade=True)

plt.show()

# 使用方法

data = sns.load_dataset("iris")

plot_kde(data, "sepal_length")

清单 8.24 从两个导入语句和用于渲染 KDE 图的 plot_kde() 函数开始。清单 8.23 的第二部分使用 Seaborn 内置数据集 iris 的内容初始化 Pandas 数据帧 data，然后使用变量 data 调用 plot_kde()。图 8.24 显示了通过启动清单 8.24 中的代码生成的点图。

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p253.jpg)

图 8.24 使用 Seaborn 创建的 KDE 图

SEABORN 的 RIDGE 图

岭图本质上是一系列重叠的 KDE 图，允许比较不同类别之间的分布。它们显示叠加的分布图，这对于可视化类别间的分布变化非常有用。以下提示被提供给 GPT-4 以生成用于岭图的 Python 代码：“请生成用于绘制岭图的 Python 代码。”

清单 8.25 展示了 ChatGPT 生成的 ridge_plot.py 的内容，用于使用 Seaborn 渲染岭图。

清单 8.25：ridge_plot.py

import matplotlib.pyplot as plt

import seaborn as sns

def plot_ridge(data, x_col, category_col):

g = sns.FacetGrid(data, row=category_col, hue=category_)

col, aspect=5)

g.map(sns.kdeplot, x_col, clip_on=False, shade=True,

alpha=1, lw=1.5, bw_method=0.2)

g.map(sns.kdeplot, x_col, clip_on=False, color="w",

lw=1, bw_method=0.2)

g.map(plt.axhline, y=0, lw=2, clip_on=False)

plt.show()

# 用法

data = sns.load_dataset("diamonds")

subset_data = data[data['cut'].isin(['Ideal', 'Fair', 'Good'])]

plot_ridge(subset_data, "price", "cut")

清单 8.25 从两个导入语句和用于渲染岭图的 plot_ridge() 函数开始。清单 8.25 的第二部分使用 Seaborn 内置数据集 diamonds 的内容初始化 Pandas 数据帧 data，然后使用变量 data 调用 plot_ridge()。图 8.25 显示了通过启动清单 8.25 中的代码生成的岭图。

![图片](img/oswald-campesato-python-3-and-machine-learning-using-chatgpt-p255.jpg)

图 8.25 使用 Seaborn 创建的岭图

摘要

本章包含了 ChatGPT 为各种任务生成的基于 Python 的解决方案。你了解了各种图表和图形的类型，何时使用它们，以及每种图表和图形类型的优缺点。

你学习了如何使用一个流行的开源 Python 库 Matplotlib 进行数据可视化，它可以渲染多种类型的图表和图形。

你还学会了如何渲染直方图、小提琴图和时间序列可视化。通过掌握这些技术，人们可以从数据中构建引人入胜的故事，帮助决策和洞察力的生成。精心制作的可视化胜过千行原始数据。

索引

A

准确率，46–47

激活函数，78–81

添加变量（部分回归）图，154

额外的模型诊断，155–156

调整的 R²，132–133

调整的兰德指数 (ARI)，201–202

高级数据分析，108

克劳德 2 对比，108–109

代码解析者，109

机器学习和 ChatGPT，115–116

相似性传播，199

聚类，196，198–199

聚类层次聚类算法，206–207

AI21，95

OpenAI 的基于 AI 的聊天机器人，102

Ajax，123

指数信息准则 (AIC)，132–133

亚马逊 Alexa，89

算法选择，39

AlphaGo，92

AlphaGo 100-0，92

AlphaGo Zero，92

AlphaStar，92

AlphaZero，92

ChatGPT 的替代方案，114–115

异常检测，37，196

人类学，96

苹果 GPT，123

艺术和音乐创作，88

人工智能 (AI)，159–160

属性选择，41

自相关，153

自动编码器，42

B

柱状图，222

与 Seaborn 一起，240–241

贝叶斯分类器，66，76–77

贝叶斯推理，74–76

贝叶斯定理，74–76

最大后验 (MAP) 假设，75–76

术语，75

贝叶斯信息准则 (BIC)，133

偏差-方差权衡，45，165

二元对多类分类，67

必应聊天，123

双变量分析，141，143

以及多元分析，146–148

布尔数据框，8–9

柱状图，224，228

使用 Matplotlib 绘制胡须图，228

C

Calinski-Harabasz 指数，201

标准相关分析（CCA），42

ChatBotX，98

ChatGPT，94，100，102–106，110–111，129

替代方案，114–115

自定义指令，104

以及数据可视化，221–256

教育者，110

生成与危险话题，110–111

Google “代码红色警报”，103

Google 搜索对比，103–104

以及 GPT-4，91–92，121–126

GPTBot，105–106

机器学习与，115–116

在移动设备和浏览器上，104–105

游戏场，106

插件，107

以及提示，105

样本查询和响应，112–113

优点和缺点，111

ChatGPT-3，92

ChatGPT-3.5，102

Chrome 扩展，102

分类，机器学习算法，37–38

机器学习中的分类器，66

激活函数，78–81

贝叶斯分类器，76–77

贝叶斯推理，74–76

二元对比多类分类，67

决策树，69–73

定义，66

评估，77–78

指数线性单元（ELU），82

hardmax 函数，83

kNN（k-最近邻）算法，68

线性分类器，68

逻辑回归，83–85

假设，84

线性可分数据，85

阈值值，84

多标签分类，67–68

随机森林，73

ReLU，81–82

Sigmoid 函数，83

softmax 激活函数，82

softmax 函数，83

softplus 激活函数，82

支持向量机，73–74

tanh 激活函数，83

在 kNN 中绑定，68–69

训练分类器，77

Claude 2，96，108–109，124

与高级数据分析相比，108–109

聚类，37–38

算法，197–200

应用，196

挑战，196–197

DBSCAN，204，208–209

定义，195

层次聚类，203–204

层次聚类算法，206–208

k-means 算法，205–206

k-means 聚类，203

机器学习模型

使用 DBSCAN 算法，215–218

使用层次聚类算法，213–215

使用 k-means 算法，209–212

度量，196，200–203

Code Whisperer，109

Codex，94，123

决定系数，131–132

Cohere，94

凝聚力，202

计算效率，165

条件数，155

混淆矩阵，46

等高线图，Matplotlib，235–236

对话式人工智能，89

评估，90

与生成式人工智能相比，89–90

在 Pandas 中将字符串转换为日期，18–20

卷积神经网络 (CNNs)，66–67，82

库克距离，155

CoPilot (OpenAI/Microsoft)，122–123

正确的模型指定，154

相关性分析，142

余弦相似度，207

反事实后悔最小化 (CFR)，93

反事实价值与策略网络（CVPN），93

协方差矩阵，42–43

创建与分类比较，88

交叉验证，164

维度诅咒，197

曲线拟合与线性回归比较，49

客户支持聊天机器人，89

D

DALL-E，90–91

DALL-E 2，96

Dask（用于分布式处理），3

数据

增强学习，89

清洗，39

生成，88

归一化与标准化比较，45

类型序列，2

数据框，1–3，6–8

以及数据清洗任务，3

特征，3

作为 HTML 网页，31–33

输入类型，1

使用 Numpy 示例，4–6

以及随机数，9–11

数据点，36

数据集，36

线性回归的准备过程，139–141

Datatable（Python 中的 R 数据表），3

数据可视化和 ChatGPT

层次聚类，248–249

双变量数据的联合图，250–251

核密度估计（KDE）密度估计图，252–253

Matplotlib

使用 3D 表面图，232–233

使用箱线图，228

等高线图，235–236

使用饼图，231

与之配合的线图，225–226

使用饼图，227

使用径向（或蜘蛛）图，23–235

使用堆叠条形图，230

使用时间序列可视化，229

因子视图的点图，251–252

极坐标图，239–240

向量场箭头图，238–239

岭图，254–255

Seaborn

使用条形图，240–241

与面网格，247–248

使用相关矩阵的热图，242–243

使用直方图，244

使用 pairplot() 函数，246–247

使用回归线绘制散点图，241–242

使用小提琴图，245

使用向量场流线图，236–238

蜂窝图，249–250

与图表和图形一起工作，222–225

Davies-Bouldin 指数，196，201

DBSCAN（基于密度的噪声应用空间聚类），196，198，204

算法，208–209

death.csv 数据集，线性回归

使用代码，150–153

详细 EDA，143–145

特征，138–139

决策树，38，66，69–73

算法，189–191

优缺点，191

算法，190

案例，191

概念和组件，189–190

扩展，191

使用机器学习模型，172–176

分割的度量，190

类型，190

DeepMind，92–93，95

分隔符属性，12

系统发育树，206，213

对话管理，90

维度降低，37，39，41–42

距离度量，165

分布分析，142–143

多样化的输出，88

数据集中的多样性，165

领域专家，40

领域知识，165

使用 Matplotlib 绘制饼图，231

药物发现，89

Dunn 指数，201

重复值，40

Durbin-Watson 统计量，132–133

E

肘部方法，196

对于 k 近邻（kNN）算法，165–166

嵌入策略，41

实体提取，90

错误矩阵，46

欧几里得距离，207

评估，77–78

even vs. odd k, 165

期望最大化，37–38

探索性数据分析 (EDA)，141–143

death.csv 数据集，线性回归，143–145

指数线性单元 (ELU)，80，82

F

F1 分数，48

使用 Seaborn 的面元网格，247–248

特征，36

工程学，40–41

提取，40–41

投影，40–41

缩放，197

选择，39–41

联邦信息处理标准 (FIPS) 代码，138，140

少样本学习，97

少样本提示，97

过滤策略，41

微调模型，39

修复错误值，39

Fowlkes-Mallows 指数，202

F 统计量，132–133

G

GANs，参见生成对抗网络 (GANs)

门控循环单元 (GRU)，82–83

高斯混合模型 (GMM)，196，199

双子星，122

广义判别分析 (GDA)，42

生成文本检测，109–110

生成对抗网络 (GANs)，88，90

生成式 AI

高级数据分析，108

AI21，95

ChatGPT 的替代方案，114–115

人类中心主义，96

ChatGPT，102–106，110–111

ChatGPT 和 GPT-4，91–92

Claude 2，108–109

代码轻语者，109

Cohere，94

对话式 AI 对比，89–90

DALL-E，90–91

DeepMind，92–93

特征，87–88

生成文本检测，109–110

生成模型，88–89

GPT-4，120–121

GPT-4 竞争对手，121–126

GPT-5，126–127

Hugging Face，94–95

inflectionAI，95

InstructGPT，117

机器学习与 ChatGPT，115–116

OpenAI，93–94

提示工程，96–102

ChatGPT 的示例查询和响应，112–113

相关技术，88

第三方 ChatGPT 插件，107

VizGPT 和可视化，117–120

生成模型，88–89

地理空间分析，142

巨型语言模型测试室 (GLTR)，110

GitHub CoPilot，122–123

Gmail，124

勒让德猜想，112–113

Google “代码红色警报”，103

Google Gemini，114，123

Google 搜索与 ChatGPT 对比，103–104

GPT2 检测器，109

GPT-3，92，94，96，100

应用，123

基于 LLM，123

GPT-4，92，94，100，120–121，125，129

竞争对手，121–126

微调，121

线性回归

使用数据集，137–138

使用随机数据，133–136

推荐内容，156–157

参数，121

以及考试成绩，120–121

基于转换器的 AR (自回归) 模型，121

GPT-5，126–127

基于 GPT 的模型，94

GPTBot，105–106

GPT-Index，121

GPT-x 系列的 LLM，93

基于图的核主成分分析（Kernel PCA），42

增长树 CFR（GT-CFR），93

H

hardmax 函数，83

hdate1，29

hdate2，29

热图，223

对于 Seaborn 中的相关矩阵，242–243

层次聚类分析（HCA），37–38

层次聚类，196，198，203–204，248–249

算法，206–208

高相关滤波器，39

技术，40

直方图，154，223–224

使用 Seaborn，244

保留法，77

同方差性，153–154

Pandas 中的 HTML 网页，30

Hugging Face，94–95，125

库，94–95

模型中心，95

假设生成，142–143

I

图像

生成，91

分割，196

综合，89

不朽，82

不完整信息，92

错误独立性，153

inflectionAI，95

影响图，155

信息增益，41

创新组合，91

InstructGPT，117

指令提示，98

Instruct 模型，94

意图识别，90

交互式语音响应（IVR）系统，89

iPhone，102

J

J1-Jumbo，92

JavaScript，102

双变量数据的联合图，250–251

Jurassic-1，95

K

Keras，162

基于 Keras 的代码，67–68

密度估计的核密度估计（KDE）图，252–253

核密度图，154

核主成分分析（Kernel PCA），37，42

k 折交叉验证技术，44，77

k-means，37–38，196，206

算法，65，205–206

聚类，197，203

k 近邻 (kNN)，38，42，66

算法，68，163–164

优缺点，163–164

案例分析，164

概念，163

肘部方法，165–166

机器学习模型，166–172

k 的值，164–165

L

L1 & L2 正则化，44

LangChain，121

语言模型，99

学习分布，88，91–92

线性分类器，66，68

线性判别分析 (LDA)，42，65

线性，154

假设，153

线性回归，37，48–49

额外的模型诊断，155–156

双变量和多变量分析，146–148

与曲线拟合比较，49

数据集，准备过程，139–141

death.csv 数据集

代码，150–153

详细的数据探索分析 (EDA)，143–145

特征，138–139

定义，130

探索性数据分析 (EDA)，141–143

GPT-4

数据集，137–138

随机数据，133–136

建议，156–157

与交互项，130

指标，131–133

模型诊断，153–155

模型选择过程，148–150

多变量分析，50

精确值解决方案，49–50

类型，130–131

线形图，223

使用 Matplotlib 的线形图，225–226

连接标准，207

Llama 2（大型语言模型 Meta AI），124–125

架构特征，125–126

微调，126

LlamaIndex，121

局部线性嵌入（LLE），37

Pandas 中的 loc()和 iloc()方法，12–13

逻辑回归，38，66，83–85

算法，185–186

假设，84

线性可分数据，85

阈值值，84

长短期记忆（LSTMs），65

低方差滤波，39

低方差滤波技术，40

M

机器学习

算法类型，37–39

偏差-方差权衡，45

与 ChatGPT 对比，115–116

使用 GPT-4 进行聚类，参见聚类

协方差矩阵，43

定义，35–36

维度约简，41–42

特征工程，选择和提取，40–41

使用 np.linspace()生成线性数据，60–61

线性回归，48–49

与曲线拟合对比，49

多变量分析，50

精确值解决方案，49–50

均方误差（MSE）

公式，58–59

手动，59–60

使用 np.linspace()API，61–63

测量模型的度量标准

准确率与精确率与召回率对比，46–47

混淆矩阵，46

接收者操作特征（ROC）曲线，47

R 平方值，46

Numpy 和 Matplotlib（1）

干扰技术，55

二次散点图，56–57

带有散点图的，54–55

主成分分析（PCA），42

回归类型，50–51

正则化

数据归一化与标准化对比，45

和特征缩放，44

统计术语

F1 分数，48

p 值，48

任务，39–40

类型，36–37

与数据集一起工作

交叉验证，44

训练数据与测试数据，43

在平面中处理线（可选），51–54

使用 GPT-4 的机器学习分类器

应用，160–161

挑战，161

概念，160

决策树算法，189–191

与机器学习模型，172–176

k 近邻（kNN）算法，163–164

用于的肘部方法，165–166

与机器学习模型，166–172

中的 k 值，164–165

逻辑回归算法，185–186

朴素贝叶斯算法，186–188

随机森林算法，177–182，191–193

Scikit-learn，161–162

SVM 算法与，182–184，188–189

类型，160

机器学习模型

聚类

使用 DBSCAN 算法，215–218

使用层次聚类算法，213–215

使用 k-means 算法，209–212

使用决策树算法，172–176

使用随机森林算法，177–182

使用 SVM 算法，182–184

曼哈顿距离，207

市场细分，196

在 Pandas 中匹配和拆分字符串，16–18

Matplotlib，133

使用 3D 表面图，232–233

使用箱线图，228

等高线图，235–236

使用饼图，231

使用线图，225–226

使用饼图，227

使用径向（或蜘蛛）图，23–235

使用堆叠条形图，230

使用其进行时间序列可视化, 229

矩阵合并, 78

均方绝对误差 (MAE), 58, 131–132

均值偏移, 38

聚类, 198

均方误差 (MSE), 131–132

定义, 35

公式, 58–59

手动操作, 59–60

使用 np.linspace()API, 61–63

均方误差 (MSE), 130

Med-PaLM 2, 124

在 Pandas 中合并和拆分列, 28–30

度量标准, 196, 200–203

对于线性回归, 131–133

微软, 93, 120, 122–123

微软 365 CoPilot, 122–123

微软 Bing AI, 123

MiniBatch k-means, 203

Pandas 中的缺失日期

检测, 21–22

插值, 22–24

“缺失”模式, 142

缺失值比率技术, 39–40

缺失值分析, 143

专家混合 (MoE) 架构, 120, 127

MNIST 数据集, 36, 38, 66

模型诊断，线性回归, 153–155

模型选择过程，线性回归, 148–150

Modin（性能更快）, 3

MT-NLG, 92

多重共线性, 154–155

多标签分类, 67–68

多项式分类器, 67

多棵独立树, 38

多元线性回归, 130

多变量分析, 37, 50, 141

N

简单贝叶斯, 38

算法, 186–188

分类器, 67, 76–77

自然语言处理 (NLP) 技术, 90, 92

神经网络, 162

非线性最小二乘法，58–59

非负矩阵分解（NMF），42

残差的正态性，153

标准化互信息（NMI），202

Numpy 和 Matplotlib（1）

干扰技术，55

二次散点图，56–57

带有散点图的，54–55

NumPy API，129

NumPy 数组，4–5

O

单次学习，97

单次提示，97

一对一（One-versus-One）技术，67

一对一（One-versus-One）技术，67

一对余者（One-versus-The-Rest），67

OpenAI，92–94

ChatGPT，123

Codex，123

开放式对话，117

Pandas 中的日期操作，24–28

OPTICS（按顺序排列点以识别聚类结构），200

异常值检测，143

异常值和杠杆点，154

P

使用 Seaborn 的 pairplot()函数，246–247

PaLM 2，122

PaLM-2，124

Pandas

替代方案，3–4

布尔数据帧，8–9

将分类数据转换为数值数据，13–16

在其中将字符串转换为日期，18–20

数据帧，2–3，6–8

和数据清洗任务，3

作为 HTML 网页，31–33

使用 NumPy 示例，4–6

和随机数，9–11

定义，1–2

包含 HTML 网页，30

在其中使用 loc()和 iloc()方法，12–13

在其中匹配和拆分字符串，16–18

在其中合并和拆分列，28–30

缺失的日期

检测，21–22

插值，22–24

中的日期操作，24–28

选项和设置，2

读取 CSV 文件，11–12

在其中处理日期范围，20–21

帕累托图，224

Pathways 语言模型，124

完美信息，92

π，115

饼图，222–223

使用 Matplotlib，227

游戏玩家（PoG），93

来自领英的 POE，115

因子视图的点图，251–252

极坐标图，239–240

多项式回归，130

精度，46–47

精度-召回（PR）曲线，78

预测误差，41

主成分分析（PCA），37，42，161，197

提示工程，96–102

和补全，97

DALL-E 2，96

定义，96

对于不同的 LLM，100–101

GPT-3，96

指令提示，98

提示和补全，97

提示模板，99–100

反向提示，98

系统提示与代理提示，98–99

模板，99–100

文本到图像生成，96

类型，97

文字提示，101–102

不同 LLM 的提示，100–101

纯度，202

p 值，48

PySpark（用于大型数据集），3

基于 Python 的代码，213

样本，159，200

Python 编码测试，96

PyTorch，162

Q

Q-Q（分位数-分位数）图，154–155

向量场的箭头图，238–239

R

雷达图，224–225

使用 Matplotlib 的径向（或蜘蛛）图，233–235

随机森林，38，66，73

算法，177–182，191–193

分类器，67

在 Pandas 中读取 CSV 文件，11–12

召回率，46–47

接收器操作特征（ROC）曲线，47，77–78

循环神经网络（RNNs），65，88

回归，37

系数，45–46，131

任务，36

类型，50–51

回归规格误差测试（RESET），154

正则化，44

和特征缩放，44

从人类反馈中进行强化学习（RLHF），115，117

相对误差，58–59

ReLU，81–82

偏差标准误差（RSE），132

解决重复值，39

解决缺失值，39

反向提示，98

Ridge plots，254–255

RMSPROP，58

RNNs，参见循环神经网络（RNNs）

鲁棒回归方法，156

根均方误差（RMSE），58，131–132

根均方层归一化（RMSNorm），126

R-squared，45–46

S

可扩展性，162

缩放指数线性单元（SELU），80

使用 Seaborn 绘制带有回归线的散点图，241–242

Scikit-learn，161–162

实现，38

Seaborn，数据可视化和 ChatGPT

使用条形图，240–241

使用 facet grids，247–248

使用热图绘制相关矩阵，242–243

使用直方图，244

使用 pairplot()函数，246–247

使用带有回归线的散点图，241–242

使用 Violin plots，245

搜索结果分组，196

二次多项式，131

半监督学习，36–37

分离，202–203

sep 参数，12

Shapiro-Wilk 测试，154

sigmoid 函数，83

影子分数，196，200–201

简单线性回归，130

Siri，89

社会网络分析，196

softmax 激活函数，82

softmax 函数，83

softplus 激活函数，82

精确值解，线性回归，49–50

SOTA（当前最佳水平）

AI21，95

性能，92

谱聚类，199

平方根规则，165

使用 Matplotlib 的堆叠条形图，230

标准化残差与杠杆作用图，154

星际争霸 II，93

向量场流图，236–238

风格迁移，89

摘要报告，142

监督学习技术，36–38

支持向量机（SVM）算法，38，66，73–74

优缺点，189

案例，189

组件，188

概念，188

与机器学习模型，182–184

类型，188

蜂群图，249–250

SwiGLU，126

综合，88

系统提示与代理提示，98–99

T

tanh 激活函数，83

T 属性，9

t 分布随机近邻嵌入（t-SNE），37，42

TensorFlow，130，162

API，65

测试模型，39

文本

生成，89，91

-相关任务，91

-图像生成，96

第三方 ChatGPT 插件，107

使用 Matplotlib 的 3D 表面图，232–233

阈值值，84

在 kNN 中绑定，68–69

使用 Matplotlib 的时间序列可视化，229

泰坦尼克号数据集，36

训练

分类器，77

模型，39

训练集与测试集，39

转换器，91

架构，91

树状图，225

趋势分析，142

t 统计量，132–133

280 GB 语言模型 Gopher，92

类型，97

TypeScript 和 CSS，110

U

UMAP，42

单变量分析，141，143

无监督学习，36–37，88，92

V

VAEs，参见变分自编码器（VAEs）

验证误差，166

变量选择，41

变量子集选择，41

方差膨胀因子（VIF），132–133，155

机器学习中的方差，45

变分自编码器（VAEs），88，90

使用 Seaborn 的小提琴图，245

Visual Studio Code 扩展，122–123

VizGPT 和数据可视化，117–120

“汽车数据集”行，118

“汽车数据集”可视化，119

语音操作虚拟助手，89

W

水流图，225

聚类内平方和（WCSS），166，196，205

文字提示，101–102

工作

带图表和图形，222–225

带数据集

交叉验证，44

训练数据与测试数据，43

在 Pandas 中的日期范围，20–21

在平面中带线（可选），51–54

包装策略，41

Y

YouChat，115

YouTube，124

Z

零概率问题，76

零样本，97

学习，97

提示，97

Z 分数，142
