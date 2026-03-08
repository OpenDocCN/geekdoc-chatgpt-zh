# 人类 VS ChatGPT：美容产品广告中的广告语言

> 原文：[Human vs ChatGPT – Language of Advertising in Beauty Products Advertisements  ](https://annas-archive.org/md5/1e75f52d1c47fee804fa5e861ac2f2e6)
> 
> 译者：[飞龙](https://github.com/wizardforcel)
> 
> 协议：[CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-cover.jpg)

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-halftitleimg.jpg)

前言

本书旨在弥合 Python 编程、机器学习和在数据科学中创新使用 ChatGPT 领域中理论与实践之间的差距。它旨在为那些希望深化对这些快速发展的领域理解和技能的人提供全面指南。

这种动机源于对实用、深入的资源日益增长的需求，这些资源满足学生、数据科学家和希望利用高级技术和工具的人工智能研究人员的需求。随着这些领域在重要性和影响力上的持续增长，熟练地操作数据、理解机器学习算法以及应用人工智能的最新进展变得至关重要。

本书结构旨在促进对几个核心主题的深入理解：

■   Pandas 简介：我们首先详细介绍 Pandas，这是数据操作和分析的基石 Python 库。本节旨在帮助您掌握数据框并高效地执行复杂的数据清理和准备任务。

■机器学习分类器：接下来，我们将探索各种机器学习分类器，为您提供选择和实施适合您项目正确算法的知识。从 kNN 到 SVMs，您将通过实际示例了解每种方法的细节。

■GPT-4 和线性回归：当我们探索 GPT-4 的能力时，我们讨论了其在增强传统线性回归分析中的应用。本节展示了 GPT-4 如何以推动传统数据分析边界的方式执行和解释回归。

■使用 ChatGPT 进行数据可视化：最后，本书涵盖了 ChatGPT 在数据可视化方面的创新应用。本部分重点介绍 AI 如何将数据转化为引人入胜的视觉故事，使复杂的结果易于理解和访问。它包括材料 AI 应用、GANs 和 DALL-E。

每一章都是基于前几节的知识构建的，确保了连贯和全面的学习体验。为了满足广泛的 学习风格，本书包括逐步教程、现实世界应用，以及基于实际示例的理论概念部分。这种方法不仅巩固了理解，还增强了您在实际场景中应用这些技术的 能力。

本书特色

■涵盖最新的 Python 库：您将掌握使用现代数据科学家必需的尖端库的技能。

■现实世界问题解决：这本书挑战您将技能应用于真实数据，为您在专业成功方面做好准备。

■与源代码、数据集和图表配套的文件可通过向出版社（需提供购买证明）发送电子邮件至 info@merclearning.com 下载。

这本书不仅仅是一个学习工具；它是一本您在职业生涯中会反复查阅的参考书。无论您是希望在学习编程和数据科学方面有一个稳固起步的初学者，还是希望探索 AI 新进展的资深专业人士，“Python 3 和 ChatGPT/GPT-4 机器学习”都是一项宝贵的资产。

我们希望您会发现这本书是一个有价值的资源，它能激发您进一步探索并应用您的知识来解决复杂问题。生成式 AI 的未来既令人兴奋又充满可能性。

O. Campesato

2024 年 4 月

第一章

PANDAS 简介

本章向您介绍 Pandas，并提供了一些代码示例，展示了其一些有用的功能。如果您熟悉这些主题，可以快速浏览材料并查看代码示例，以防它们包含您未知的信息。

第一部分简要介绍了 Pandas。本节包含了一些代码示例，展示了 Pandas DataFrame 的一些功能，并对序列进行了简要讨论，这两者都是 Pandas 的主要功能。

本章的第二部分讨论了您可以创建的各种数据框类型，例如数值型和布尔型数据框。此外，我们还讨论了使用 NumPy 函数和随机数创建数据框的示例。

注意：本章中的几个代码示例引用了 NumPy 库来处理数组和生成随机数，您可以从在线文章中学习这些内容。

什么是 Pandas？

Pandas 是一个与 NumPy 和 Matplotlib 等其他 Python 库兼容的 Python 库。通过打开命令行并调用以下命令安装 Pandas（适用于 Python 3.x）：

pip3 install pandas

在许多方面，Pandas 库中 API 的语义类似于电子表格，同时支持 XSL、XML、HTML 和 CSV 文件类型。Pandas 提供了一个名为数据框的数据类型（类似于 Python 字典），具有极其强大的功能。

Pandas 数据框支持多种输入类型，如 ndarray、列表、字典或序列。

数据类型序列是另一种管理数据的方式。除了在线搜索更多关于序列的详细信息外，以下文章包含了一个很好的介绍：

[`towardsdatascience.com/20-examples-to-master-pandas-series-bc4c68200324`](https://towardsdatascience.com/20-examples-to-master-pandas-series-bc4c68200324)

Pandas 选项和设置

您可以更改环境变量的默认值，以下是一个示例：

import pandas as pd

display_settings = {

'max_columns': 8,

'expand_frame_repr': True, # Wrap to multiple pages

'max_rows': 20,

'precision': 3,

'show_dimensions': True

}

for op, value in display_settings.items():

pd.set_option("display.{}".format(op), value)

如果您想让 Pandas 显示最多 20 行和 8 列，并且浮点数以三位小数显示，请在自己的代码中包含前面的代码块。如果要将输出“环绕”到多页，请将 expand_frame_rep 设置为 True。前面的 for 循环遍历 display_settings，并将选项设置为相应的值。

此外，以下代码片段显示您代码中的所有 Pandas 选项及其当前值：

print(pd.describe_option())

您可以使用选项及其值执行各种其他操作（例如，使用 pd.reset()方法重置值），如 Pandas 用户指南中所述：

[`pandas.pydata.org/pandas-docs/stable/user_guide/options.html`](https://pandas.pydata.org/pandas-docs/stable/user_guide/options.html)

Pandas 数据框

简而言之，Pandas 数据框是一个二维数据结构，并且方便将数据结构视为行和列。数据框可以进行标记（包括行和列），并且列可以包含不同的数据类型。Pandas 数据框的数据集来源可以是数据文件、数据库表或 Web 服务。数据框的功能包括：

+   数据框方法

+   数据框统计信息

+   分组、交叉和重塑

+   处理缺失数据

+   连接数据框

本章中的代码示例几乎展示了上述列表中的所有功能。

数据框和数据清洗任务

你需要执行的具体任务取决于数据集的结构和内容。通常，你将按照以下步骤执行工作流程，不一定总是按照这个顺序（某些步骤可能是可选的）。以下所有步骤都可以使用 Pandas 数据框完成：

+   将数据读入数据框

+   显示数据框的顶部

+   显示列数据类型

+   显示缺失值

+   用一个值替换 NA

+   遍历列

+   每列的统计信息

+   查找缺失值

+   总缺失值

+   缺失值的百分比

+   排序表格值

+   打印摘要信息

+   缺失值超过 50% 的列

+   重命名列

本章包含说明如何执行上述列表中许多步骤的章节。

Pandas 的替代方案

在深入研究代码示例之前，有一些提供非常有用功能的 Pandas 替代方案，其中一些如下所示：

+   PySpark（用于大型数据集）

+   Dask（用于分布式处理）

+   Modin（更快性能）

+   Datatable（Python 中的 R data.table）

包含这些替代方案的目的不是要贬低 Pandas。实际上，你可能不需要上述列表中的任何功能。然而，如果你将来需要此类功能，那么现在了解这些替代方案是值得的（未来可能还有更强大的替代方案）。 

一个使用 NUMPY 的 PANDAS 数据框示例

列表 1.1 展示了 pandas_df.py 的内容，说明了如何定义几个数据框并显示其内容。

列表 1.1：pandas_df.py

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

列表 1.1 从 Pandas 和 NumPy 的标准导入语句开始，接着是定义两个一维 NumPy 数组和二维 NumPy 数组。每个 NumPy 变量后面都跟着一个相应的 Pandas 数据框（mydf1、mydf2 和 mydf3）。现在运行 列表 1.1 中的代码，以查看以下输出，并比较 NumPy 数组与 Pandas 数据框：

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

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-img_5a.jpg)

mydf3:

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-img_5.jpg)

相比之下，以下代码块说明了如何定义两个 Pandas Series，这两个 Series 是 Pandas 数据框定义的一部分：

names = pd.Series(['SF', 'San Jose', 'Sacramento'])

sizes = pd.Series([852469, 1015785, 485199])

df = pd.Data frame({ 'Cities': names, 'Size': sizes })

print(df)

使用前面的代码（以及所需的导入语句）创建一个 Python 文件，当你运行该代码时，你会看到以下输出：

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-img_6.jpg)

描述 PANDAS 数据框

列表 1.2 展示了 pandas_df_describe.py 的内容，它说明了如何定义一个包含 3x3 整数值 NumPy 数组的 Pandas 数据框，其中数据框的行和列都有标签。数据框的其他方面也显示了出来。

列表 1.2：pandas_df_describe.py

import numpy as np

import pandas as pd

myarray = np.array([[10,30,20], [50,40,60],[1000,2000,3000]])

rownames = ['apples', 'oranges', 'beer']

colnames = ['January', 'February', 'March']

mydf = pd.Data frame(myarray, index=rownames, columns=colnames)

print("contents of df:")

print(mydf)

print()

print("January 的内容:")

print(mydf['January'])

print()

print("行数：")

print(mydf.shape[0])

print()

print("列数：")

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

列表 1.2 从两个标准的导入语句开始，接着是变量 myarray，它是一个 3x3 的数字 NumPy 数组。变量 rownames 和 colnames 分别为 Pandas 数据框 mydf 的行和列提供名称，mydf 是初始化为包含指定数据源（即 myarray）的 Pandas 数据框。

下面的输出第一部分需要一个单独的 print() 语句（它只是显示 mydf 的内容）。输出第二部分是通过调用任何 Pandas 数据框都有的 describe() 方法生成的。describe() 方法很有用：你会看到各种统计量，如均值、标准差、最小值和最大值，这些统计量是针对列（而不是行）进行的，还包括 25^(th)、50^(th) 和 75^(th) 分位数。列表 1.2 的输出如下：

df 的内容：

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-img_7.jpg)

January 的内容：

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-img_7a.jpg)

Name: January, dtype: int64

行数：

3

列数：

3

行数和列数：

(3, 3)

Column Names:

Index(['January', 'February', 'March'], dtype='object')

列类型：

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-img_7b.jpg)

dtype: object

描述：

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-img_8.jpg)

PANDAS 布尔数据框

Pandas 支持数据框上的布尔运算，例如逻辑或、逻辑与和一对数据框的逻辑否定。列表 1.3 展示了 pandas_boolean_df.py 的内容，该内容说明了如何定义一个 Pandas 数据框，其行和列是布尔值。

列表 1.3：pandas_boolean_df.py

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

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-img_8a.jpg)

Pandas 数据框的转置

T 属性（以及转置函数）允许您生成 Pandas 数据框的转置，类似于 NumPy 稀疏数组。转置操作将行转换为列，列转换为行。例如，以下代码片段定义了一个 Pandas 数据框 df1，然后显示 df1 的转置：

df1 = pd.DataFrame({'a': [1, 0, 1], 'b': [0, 1, 1]}, dtype=int)

print("df1.T:")

print(df1.T)

上述代码片段的输出如下：

df1.T:

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-img_9.jpg)

以下代码片段定义了 Pandas 数据框 df1 和 df2，然后显示它们的和：

df1 = pd.DataFrame({'a': [1, 0, 1], 'b': [0, 1, 1]}, dtype=int)

df2 = pd.DataFrame({'a': [3, 3, 3], 'b': [5, 5, 5]}, dtype=int)

print("df1 + df2:")

print(df1 + df2)

输出如下：

df1 + df2:

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-img_9a.jpg)

PANDAS 数据框和随机数

列表 1.4 展示了 pandas_random_df.py 的内容，该内容说明了如何创建一个包含随机整数的 Pandas 数据框。

列表 1.4：pandas_random_df.py

import pandas as pd

import numpy as np

df = pd.DataFrame(np.random.randint(1, 5, size=(5, 2)), columns=['a', 'b'])

df = df.append(df.agg(['sum', 'mean']))

print("数据框的内容：")

print(df)

列表 1.4 定义了由 5 行和 2 列的 1 到 5 之间的随机整数组成的数据框 df。请注意，df 的列标记为“a”和“b”。此外，下一个代码片段附加了包含两列数字总和和平均值的两行。列表 1.4 的输出如下：

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-img_10.jpg)

列表 1.5 展示了 pandas_combine_df.py 的内容，该内容说明了如何组合 Pandas 数据框。

列表 1.5：pandas_combine_df.py

import pandas as pd

import numpy as np

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-img_10a.jpg)

print("df2 的内容：")

print(df)

print("foo1 的内容：")

print(df.foo1)

print("foo2 的内容：")

print(df.foo2)

列表 1.5 定义了 Pandas 数据框 df，它由 5 行和 2 列（标记为“foo1”和“foo2”）的随机实数（介于 0 和 5 之间）组成。 列表 1.5 的下一部分显示了 df 和 foo1 的内容。 列表 1.5 的输出如下：

df 的内容：

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-img_11.jpg)

在 Pandas 中读取 CSV 文件

Pandas 提供了 read_csv() 方法来读取 CSV 文件的内容。例如，列表 1.6 显示了包含标记数据（垃圾邮件或垃圾邮件）的 sometext.csv 的内容，列表 1.7 显示了 read-csv-file.py 的内容，该内容说明了如何读取 CSV 文件的内容。

列表 1.6：sometext.csv

| 类型 | 文本 |
| --- | --- |
| 垃圾邮件 | 今天可用 |
| 垃圾邮件 | 我在和你开玩笑 |
| 垃圾邮件 | 在每周竞赛中免费入场 |
| 垃圾邮件 | 你说得太早了 |
| 垃圾邮件 | 我认为他不会去我们这里 |
| 垃圾邮件 | 免费消息，你好 |
| 垃圾邮件 | 我的兄弟没有生病 |
| 垃圾邮件 | 按您的要求，Melle |
| 垃圾邮件 | 获胜者！！作为一位尊贵的客户 |

列表 1.7：read-csv-file.py

导入 pandas 库

导入 numpy 库

df = pd.read_csv('sometext.csv', delimiter='\t')

打印("=> 前五行：")

打印(df.head(5))

列表 1.7 读取 sometext.csv 的内容，其列由制表符（"\t"）分隔。运行 列表 1.7 中的代码以查看以下输出：

=> 前五行：

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-img_12.jpg)

head() 方法的默认值是 5，但您可以使用代码片段 df.head(n) 显示数据框 df 的前 n 行。

在文本文件中指定分隔符和列集

前一节向您展示了如何使用 delimiter 属性在文本文件中指定分隔符。您还可以使用 sep 参数指定不同的分隔符。此外，您还可以将 names 参数分配给您想要读取的数据中的列名。使用 delimiter 和 sep 的一个示例如下：

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-img_12a.jpg)

Pandas 还提供了 read_table() 方法来读取 CSV 文件的内容，它使用与 read_csv() 方法相同的语法。

在文本文件中指定索引

假设您知道文本文件中的某一列包含文本文件行索引值。例如，包含关系型表数据的文本文件通常包含索引列。

幸运的是，Pandas 允许你指定文本文件中的第 k 列作为索引，如下所示：

df = pd.read_csv('myfile.csv', index_col=k)

Pandas 中的 LOC() 和 ILOC() 方法

如果您想显示 Pandas 数据框中记录的内容，请在 loc() 方法中指定行的索引。例如，以下代码片段通过特征名称在数据框 df 中显示数据：

df.loc[feature_name]

选择数据框中 "height" 列的第一行：

df.loc([0], ['height'])

以下代码片段使用 iloc() 函数通过此代码片段显示名称列的前 8 条记录：

df.iloc[0:8]['name']

将分类数据转换为数值数据

机器学习中一个常见的任务是将包含字符数据的特征转换为包含数值数据的特征。列表 1.8 展示了 cat2numeric.py 的内容，说明了如何将文本字段替换为相应的数值字段。

列表 1.8: cat2numeric.py

导入 pandas as pd

导入 numpy as np

df = pd.read_csv('sometext.csv', delimiter='\t')

print("=> 前五行（之前）：")

print(df.head(5))

print("-------------------------")

print()

# 将 ham/spam 映射到 0/1 值：

df['type'] = df['type'].map( {'ham':0 , 'spam':1} )

print("=> 前五行（之后）:")

print(df.head(5))

print("-------------------------")

列表 1.8 使用 sometext.csv 文件的 内容初始化数据框 df，然后通过调用 df.head(5) 显示前五行内容，这也是默认显示的行数。

列表 1.8 中的下一个代码片段调用 map() 方法，将 ham 替换为 0，将 spam 替换为 1，如以下所示：

df['type'] = df['type'].map( {'ham':0 , 'spam':1} )

列表 1.8 的最后部分再次调用 head() 方法来显示在重命名类型列的内容后数据集的前五行。运行 列表 1.8 中的代码以查看以下输出：

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-img_13.jpg)

-------------------------

例如，列表 1.9 展示了 shirts.csv 的内容，列表 1.10 展示了 shirts.py 的内容；这些示例说明了将分类数据转换为数值数据的四种技术。

列表 1.9: shirts.csv

类型,ssize

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

列表 1.10: shirts.py

导入 pandas as pd

shirts = pd.read_csv("shirts.csv")

print("shirts 之前：")

print(shirts)

print()

# 技巧 #1:

#shirts.loc[shirts['ssize']=='xxlarge','size'] = 4

#shirts.loc[shirts['ssize']=='xlarge', 'size'] = 4

#shirts.loc[shirts['ssize']=='large', 'size'] = 3

#shirts.loc[shirts['ssize']=='medium', 'size'] = 2

#shirts.loc[shirts['ssize']=='small', 'size'] = 1

#shirts.loc[shirts['ssize']=='xsmall', 'size'] = 1

# 技巧 #2:

#shirts['ssize'].replace('xxlarge', 4, inplace=True)

#shirts['ssize'].replace('xlarge', 4, inplace=True)

#shirts['ssize'].replace('large', 3, inplace=True)

#shirts['ssize'].replace('medium', 2, inplace=True)

#shirts['ssize'].replace('small', 1, inplace=True)

#shirts['ssize'].replace('xsmall', 1, inplace=True)

# 技巧 #3:

#shirts['ssize'] = shirts['ssize'].apply({'xxlarge':4, 'xlarge':4, 'large':3, 'medium':2, 'small':1, 'xsmall':1}.get)

# 技巧 #4:

shirts['ssize'] = shirts['ssize'].replace(regex='xlarge', value=4)

shirts['ssize'] = shirts['ssize'].replace(regex='large', value=3)

shirts['ssize'] = shirts['ssize'].replace(regex='medium', value=2)

shirts['ssize'] = shirts['ssize'].replace(regex='small', value=1)

print("shirts 之后：")

print(shirts)

列表 1.10 以六个语句的代码块开始，这些语句使用字符串的直接比较来进行数值替换。例如，以下代码片段将所有 xxlarge 字符串替换为值 4：

shirts.loc[shirts['ssize']=='xxlarge','size'] = 4

第二个代码块由六个语句组成，这些语句使用 replace()方法执行相同的更新，以下是一个示例：

shirts['ssize'].replace('xxlarge', 4, inplace=True)

第三个代码块由一个语句组成，该语句使用 apply()方法执行相同的更新，如下所示：

shirts['ssize'] = shirts['ssize'].apply({'xxlarge':4, 'xlarge':4, 'large':3, 'medium':2, 'small':1, 'xsmall':1}.get)

第四个代码块由四个语句组成，这些语句使用正则表达式执行相同的更新，以下是一个示例：

shirts['ssize'] = shirts['ssize'].replace(regex='xlarge', value=4)

由于前面的代码片段同时匹配 xxlarge 和 xlarge，我们只需要四个语句而不是六个语句。（如果你不熟悉正则表达式，可以在网上找到讨论正则表达式的文章。）现在启动列表 1.10 中的代码，以查看以下输出：

shirts 之前

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p16.jpg)

PANDAS 中的字符串匹配和分割

列表 1.11 显示了 shirts_str.py 的内容，它说明了如何匹配具有初始字符串的列值以及如何根据字母分割列值。

列表 1.11：shirts_str.py

import pandas as pd

shirts = pd.read_csv("shirts2.csv")

print("shirts：")

print(shirts)

print()

print("以 xl 开头的 shirts：")

print(shirts[shirts.ssize.str.startswith('xl')])

print()

print("排除'xlarge'衬衫：")

print(shirts[shirts['ssize'] != 'xlarge'])

print()

print("前三个字母：")

shirts['sub1'] = shirts['ssize'].str[:3]

print(shirts)

print()

print("在字母'a'上分割 ssize：")

shirts['sub2'] = shirts['ssize'].str.split('a')

print(shirts)

print()

print("第 3 行到第 5 行和第 2 列：")

print(shirts.iloc[2:5, 2])

print()

列表 1.11 使用 CSV 文件 shirts.csv 的内容初始化数据帧 df，然后显示 df 的内容。在列表 1.11 中的下一个代码片段使用 startswith()方法匹配以字母 xl 开头的衬衫类型，随后是一个显示尺寸不等于字符串 xlarge 的短裤的代码片段。

下一个代码片段使用 str[:3]构造来显示衬衫类型的第一个三个字母，随后是一个使用 split()方法根据字母“a”分割衬衫类型的代码片段。

最终的代码片段调用 iloc[2:5,2] 来显示第 3 行至第 5 行（包括第 5 行）的内容，以及仅第二列。列表 1.11 的输出如下：

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p17.jpg)

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p18.jpg)

在 PANDAS 中将字符串转换为日期

列表 1.12 展示了 string2date.py 的内容，该内容说明了如何将字符串转换为日期格式。

列表 1.12：string2date.py

import pandas as pd

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-img_19.jpg)

df1 = pd.DataFrame(bdates1, columns = ['strdates','people'])

df1['dates'] = pd.to_datetime(df1['strdates'], format='%Y%m%d')

print("=> 数据框 df1 的内容：")

print(df1)

print()

print(df1.dtypes)

print()

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-img_19a.jpg)

df2 = pd.DataFrame(bdates2, columns = ['strdates','people'])

df2['dates'] = pd.to_datetime(df2['strdates'], format='%d%b%Y')

print("=> 数据框 df2 的内容：")

print(df2)

print()

print(df2.dtypes)

print()

列表 1.12 初始化数据框 df1，包含 bdates1 的内容，然后使用 %Y%m%d 格式将 strdates 列转换为日期。列表 1.12 的下一部分初始化数据框 df2，包含 bdates2 的内容，然后使用 %d%b%Y 格式将 strdates 列转换为日期。现在运行列表 1.12 中的代码，以查看以下输出：

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p19.jpg)

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p20.jpg)

在 PANDAS 中处理日期范围

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

print("DATES BETWEEN",start_d,"AND",end_d,":")

print(df.loc[start_d:end_d])

print()

print("DATES BEFORE",start_d,":")

print(df.loc[df.index < start_d])

years = ['2020','2021','2022']

for year in years:

year_sum = df.loc[year].sum()[0]

print("SUM OF VALUES FOR YEAR",year,":",year_sum)

列表 1.13 首先初始化变量 df，包含 CSV 文件 multiple_dates.csv 的内容，然后显示其内容。接下来的代码片段将日期列设置为索引列，然后初始化变量 start_d 和 end_d，分别包含起始日期和结束日期。

列表 1.13 的下一部分显示 start_d 和 end_d 之间的日期，然后显示在 start_d 之前的日期列表。最后的代码块遍历年份列表，然后计算列表中每个年份的值字段中的数值总和。现在运行列表 1.13 中的代码，以查看以下输出：

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p21.jpg)

2020 年数值总和：141.0

2021 年数值总和：235.0

2022 年数值总和：160.0

在 PANDAS 中检测缺失日期

列表 1.14 展示了 pandas_missing_dates.py 的内容，该内容说明了如何在 CSV 文件中检测缺失的日期值。

列表 1.14：pandas_missing_dates.py

import pandas as pd

# 从列表字典创建数据框

data = {'Date': ['2021-01-18', '2021-01-20', '2021-01-21', '2021-01-24'],

'Name': ['Joe', 'John', 'Jane', 'Jim']}

df = pd.Data frame(data)

# 将日期值设置为索引：

df = df.set_index('Date')

# to_datetime()将字符串格式转换为 DateTime 对象：

df.index = pd.to_datetime(df.index)

start_d="2021-01-18"

end_d="2021-01-25"

# 显示不按顺序的日期：

print("从",start_d,"到",end_d,"之间缺失的日期：")

dates = pd.date_range(start=start_d, end=end_d).difference(df.index)

for date in dates:

print("日期：",date)

print()

列表 1.14 初始化字典 data，包含日期字段和名称字段的值列表，之后变量 df 被初始化为一个数据框，其内容来自 data 变量。

下面的代码片段将数据框 df 的日期字段设置为索引，之后基于字符串的日期被转换为 DateTime 对象。另一对代码片段分别初始化变量 start_d 和 end_d 为起始日期和结束日期。

列表 1.14 的最后部分初始化变量 dates，包含 start_d 和 end_d 之间的缺失日期列表，之后显示 dates 的内容。现在运行列表 1.14 中的代码，可以看到以下输出：

2021 年 1 月 18 日至 2021 年 1 月 25 日之间缺失的日期：

date: 2022-01-19 00:00:00

date: 2022-01-22 00:00:00

date: 2022-01-23 00:00:00

date: 2022-01-25 00:00:00

PANDAS 中插值缺失日期

列表 1.15 展示了 missing_dates.csv 的内容，列表 1.16 展示了 pandas_interpolate.py 的内容，该内容说明了如何以多种方式计算插值值来替换 NaN 值。

列表 1.15：missing_dates.csv

"dates","values"

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

注意列表 1.15 中的值 140（粗体显示）：这个值是一个异常值，它将影响插值值的计算，并可能生成额外的异常值。

列表 1.16：pandas_interpolate.py

import pandas as pd

df = pd.read_csv("missing_dates.csv")

# 使用线性插值填充 NaN 值：

df1 = df.interpolate()

# 使用二次多项式插值填充 NaN 值：

df2 = df.interpolate(method='polynomial', order=2)

# 使用三次多项式插值填充 NaN 值：

df3 = df.interpolate(method='polynomial', order=3)

print("原始数据框：")

print(df)

print()

print("线性插值：")

print(df1)

print()

print("二次插值：")

print(df2)

print()

print("三次插值：")

print(df3)

print()

列表 1.16 使用 CSV 文件 missing_dates.csv 的内容初始化 df，然后通过 interpolate() 方法分别使用线性、二次和三次插值初始化基于线性、二次和三次插值的数据框 df1、df2 和 df3。现在运行 列表 1.16 中的代码以查看以下输出：

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p23.jpg)

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p24.jpg)

OTHER OPERATIONS WITH DATES IN PANDAS

列表 1.17 展示了 pandas_misc1.py 的内容，说明了如何从一个数据框的列中提取年份列表。

LISTING 1.17: pandas_misc1.py

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

列表 1.17 使用 CSV 文件 multiple_dates.csv 的内容初始化 df，然后显示其内容。列表 1.17 的下一部分初始化 year_list 为 df 的日期列。

下一个代码块包含一个循环，遍历 year_list 中的元素，提取前四个字符（即年份值）并将该子字符串追加到 NumPy 数组 arr1 中。最后一个代码块将变量 unique_arr 初始化为包含字典 unique_years 中唯一年份的 NumPy 数组。现在运行 列表 1.17 中的代码以查看以下输出：

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p25.jpg)

unique_years:

{'2022', '2020', '2021'}

unique_arr:

[['2022']

['2020']

['2021']]

列表 1.18 展示了 pandas_misc2.py 的内容，说明了如何遍历数据框的行。请注意，不建议按行迭代，因为它可能导致大数据集中的性能问题。

LISTING 1.18: pandas_misc2.py

import pandas as pd

df = pd.read_csv('multiple_dates.csv', parse_dates=['dates'])

print("df:")

print(df)

print()

print("=> 遍历行:")

for idx,row in df.iterrows():

print("idx:",idx," year:",row['dates'])

print()

列表 1.18 初始化 Pandas 数据框 df，打印其内容，然后循环处理 df 的行。在每次迭代中，显示当前索引和行内容。现在运行 列表 1.18 中的代码以查看以下输出：

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p26.jpg)

列表 1.19 展示了 pandas_misc3.py 的内容，说明了如何显示介于开始日期和结束日期之间的周日期集。

列表 1.19: pandas_misc3.py

import pandas as pd

start_d="01/02/2022"

end_d="12/02/2022"

weekly_dates=pd.date_range(start=start_d, end=end_d, freq='W')

print("从",start_d,"到",end_d,"的周日期：")

print(weekly_dates)

Listing 1.19 starts with initializing the variable start_d and end_d that contain a start date and an end date, respectively, and then initializes the variable weekly_dates with a list of weekly dates between the start date and the end date. Now launch the code in Listing 1.19 to see the following output:

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p27.jpg)

MERGING AND SPLITTING COLUMNS IN PANDAS

Listing 1.20 shows the contents of employees.csv and Listing 1.21 shows the contents of emp_merge_split.py. These examples illustrate how to merge columns and split columns of a CSV file.

LISTING 1.20: employees.csv

name,year,month

Jane-Smith,2015,Aug

Dave-Smith,2020,Jan

Jane-Jones,2018,Dec

Jane-Stone,2017,Feb

Dave-Stone,2014,Apr

Mark-Aster,,Oct

Jane-Jones,NaN,Jun

LISTING 1.21: emp_merge_split.py

import pandas as pd

emps = pd.read_csv("employees.csv")

print("emps:")

print(emps)

print()

emps['year'] = emps['year'].astype(str)

emps['month'] = emps['month'].astype(str)

# separate column for first name and for last name:

emps['fname'],emps['lname'] = emps['name'].str.split("-",1).str

# concatenate year and month with a "#" symbol:

emps['hdate1'] = emps['year'].

astype(str)+"#"+emps['month'].astype(str)

# concatenate year and month with a "-" symbol:

emps['hdate2'] = emps[['year','month']].agg('-'.join, axis=1)

print(emps)

print()

Listing 1.21 initializes the data frame df with the contents of the CSV file employees.csv, and then displays the contents of df. The next pair of code snippets invoke the astype() method to convert the contents of the year and month columns to strings.

The next code snippet in Listing 1.21 uses the split() method to split the name column into the columns fname and lname that contain the first name and last name, respectively, of each employee's name:

emps['fname'],emps['lname'] = emps['name'].str.split("-",1).str

The next code snippet concatenates the contents of the year and month string with a "#" character to create a new column called hdate1:

emps['hdate1'] = emps['year'].

astype(str)+"#"+emps['month'].astype(str)

The final code snippet concatenates the contents of the year and month string with a “-” to create a new column called hdate2, as shown here:

emps['hdate2'] = emps[['year','month']].agg('-'.join, axis=1)

Now launch the code in Listing 1.21 to see the following output:

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p29.jpg)

There is one other detail regarding the following commented-out code snippet:

#emps['fname'],emps['lname'] = emps['name'].str.split("-",1).str

The following deprecation message is displayed if you uncomment the preceding code snippet:

#FutureWarning: Columnar iteration over characters

#will be deprecated in future releases.

READING HTML WEB PAGES IN PANDAS

列表 1.22 显示了 HTML 网页 abc.html 的内容。列表 1.23 展示了 read_html_page.py 的内容，该内容说明了如何从 Pandas 中读取 HTML 网页的内容。请注意，此代码仅适用于包含至少一个 HTML `<table>` 元素的网页。

列表 1.22：abc.html

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p30.jpg)

列表 1.23：read_html_page.py

import pandas as pd

file_name="abc.html"

with open(file_name, "r") as f:

dfs = pd.read_html(f.read())

print("HTML 网页中的 HTML 表格内容:")

print(dfs)

列表 1.23 以导入语句开始，随后初始化变量 file_name 为 abc.html，该文件在 列表 1.22 中显示。下一个代码片段初始化变量 dfs 为包含 HTML 网页 abc.html 内容的数据帧。列表 1.23 的最后部分显示了数据帧 dsf 的内容。现在运行 列表 1.23 中的代码以查看以下输出：

HTML 网页中的 HTML 表格内容：

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p30-1.jpg)

有关 Pandas read_html() 方法的更多信息，请访问此 URL：

[`pandas.pydata.org/pandas-docs/stable/reference/`](https://pandas.pydata.org/pandas-docs/stable/reference/)

将 Pandas 数据帧保存为 HTML 网页

列表 1.24 展示了 read_html_page.py 的内容，该内容说明了如何从 Pandas 中读取 HTML 网页的内容。请注意，此代码仅适用于包含至少一个 HTML `<table>` 元素的网页。

列表 1.24：read_html_page.py

import pandas as pd

emps = pd.read_csv("employees.csv")

print("emps:")

print(emps)

print()

emps['year'] = emps['year'].astype(str)

emps['month'] = emps['month'].astype(str)

# 分离用于姓氏和名字的列：

emps['fname'],emps['lname'] = emps['name'].str.split("-",1).str

# 使用“#”符号连接年份和月份：

emps['hdate1'] = emps['year']

.astype(str)+"#"+emps['month'].astype(str)

# 使用“-”符号连接年份和月份：

emps['hdate2'] = emps[['year','month']].agg('-'.join, axis=1)

print(emps)

print()

html = emps.to_html()

print("数据帧作为 HTML 网页:")

print(html)

列表 1.24 将数据帧 temps 填充为 employees.csv 的内容，然后将年份和月份属性转换为字符串类型。接下来的代码片段使用“-”符号作为分隔符拆分名称字段的内容。因此，此代码片段将新字段 fname 和 lname 分别填充为拆分字段的前缀和姓氏。

列表 1.24 中的下一个代码片段将年份和月份字段转换为字符串，然后使用“#”作为分隔符将它们连接起来。另一个代码片段将 hdate2 字段填充为年份和月份字段的连接。

在显示数据框 emps 的内容后，最后的代码片段通过调用 Pandas 的 to_html() 方法，将数据框 emps 转换为 HTML 网页的结果赋值给变量 html。现在运行 列表 1.24 中的代码，可以看到以下输出：

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p32.jpg)

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p33.jpg)

概述

本章向您介绍了 Pandas，用于创建带标签的数据框并显示数据框的元数据。然后您学习了如何从各种数据源创建数据框，例如随机数和硬编码的数据值。此外，您还看到了如何在 Pandas 数据框中执行基于列和行的操作。

您还学习了如何读取 Excel 工作表并对这些工作表中的数据进行数值计算，例如数值列中的最小值、平均值和最大值。然后，您看到了如何从存储在 CSV 文件中的数据创建 Pandas 数据框。

第二章

机器学习简介

本章介绍了机器学习中的许多概念，例如特征选择、特征工程、数据清洗、训练集和测试集。

本章的第一部分简要讨论了机器学习以及准备数据集通常所需的步骤序列。这些步骤包括可以使用各种算法执行的“特征选择”或“特征提取”。

第二部分描述了您可能会遇到的数据类型，数据集中可能出现的问题以及如何纠正这些问题。当您执行训练步骤时，您还将了解“保留”和“k 折”之间的区别。

本章的第三部分简要讨论了线性回归中涉及的基本概念。尽管线性回归是在 200 多年前开发的，但这项技术仍然是解决（尽管简单）统计学和机器学习问题核心技术之一。事实上，用于在二维平面（或更高维度的超平面）上找到最佳拟合线的均值平方误差（MSE）技术，在 Python 中实现以最小化后面讨论的损失函数。

本章的第四部分包含使用 NumPy 标准技术进行线性回归任务的额外代码示例。因此，如果您熟悉这个主题，您可能可以快速浏览本章的前两节。

什么是机器学习？

从高层次来说，机器学习是人工智能的一个子集，可以解决传统编程语言难以实现或过于繁琐的任务。电子邮件垃圾邮件过滤器是机器学习的早期例子。机器学习通常优于旧算法的准确性。

尽管机器学习算法种类繁多，但数据可能比选定的算法更重要。数据可能会出现许多问题，例如数据不足、数据质量差、数据错误、数据缺失、数据不相关和数据值重复。在本章的后面部分，你将看到解决许多这些数据相关问题的技术。

如果你对机器学习术语不熟悉，数据集是一组数据值，可以是 CSV 文件或电子表格的形式。每一列称为特征，每一行是一个数据点，包含每个特征的特定值集合。如果一个数据集包含有关客户的信息，那么每一行都与一个特定客户相关。

机器学习的类型

你会遇到三种主要的机器学习类型（这些类型的组合也是可能的）：

+   监督学习

+   无监督学习

+   半监督学习

监督学习意味着数据集中的数据点都有一个标签来标识其内容。例如，MNIST 数据集包含 28x28 的 PNG 文件，每个文件包含一个手绘的数字（即 0 到 9 的数字）。每个包含数字 0 的图像都有标签“0”，每个包含数字 1 的图像都有标签“1”，所有其他图像都根据图像中显示的数字进行标记。

作为另一个例子，泰坦尼克号数据集中的列是关于乘客的特征，例如他们的性别、船舱等级、票价以及乘客是否幸存。每一行包含关于单个乘客的信息，包括如果乘客幸存则值为 1。MNIST 数据集和泰坦尼克号数据集涉及分类任务：目标是训练一个模型，然后预测测试数据集中每一行的类别（MNIST）或幸存（泰坦尼克号）。

通常，用于分类任务的数据集具有少量可能的值：0 到 9 范围内的九个数字之一，四种动物之一（狗、猫、马、长颈鹿），或两个值之一（幸存与死亡，购买与未购买）。通常，如果结果的数量可以在下拉列表中合理地显示，那么它可能是一个分类任务。

在包含房地产数据的数据集中，每一行包含关于特定房屋的信息，例如卧室数量、房屋平方英尺、浴室数量和房屋价格。在这个数据集中，房屋价格是每一行的标签。请注意，可能的房价范围太大，无法合理地适合下拉列表。房地产数据集涉及回归任务：目标是基于训练数据集训练模型，然后预测测试数据集中每一所房屋的价格。

无监督学习涉及未标记数据，这通常是聚类算法的情况（将在后面讨论）。以下是一些涉及聚类的无监督学习的重要算法：

+   k-means

+   层次聚类分析（HCA）

+   期望最大化

一些涉及降维（将在后面更详细地讨论）的重要无监督学习算法如下：

+   PCA（主成分分析）

+   核 PCA

+   LLE（局部线性嵌入）

+   t-SNE（t-分布随机邻域嵌入）

还有一个非常重要的无监督任务称为异常检测。这项任务与欺诈检测和检测异常值（将在后面更详细地讨论）相关。

半监督学习是监督学习和无监督学习的结合：一些数据点被标记，一些未被标记。一种技术是使用标记数据来分类（即标记）未标记的数据，之后你可以应用分类算法。

机器学习算法类型

机器学习算法主要有三种类型：

+   回归（例如：线性回归）

+   分类（例如：k 最近邻）

+   聚类（例如：k-means）

回归是一种监督学习技术，用于预测数值。回归任务的一个例子是预测特定股票的价值。请注意，这项任务与预测特定股票的价值是否会明天（或某个其他未来时间段）增加或减少是不同的。另一个回归任务的例子是预测房地产数据集中房屋的损失。这两个任务都是回归任务的例子。

机器学习中的回归算法包括线性回归和广义线性回归（在传统统计学中也称为多元分析）。

分类也是一种监督学习技术，但它用于预测分类量。分类任务的一个例子是检测垃圾邮件、欺诈或确定 PNG 文件中的数字（如 MNIST 数据集）。在这种情况下，数据已经被标记，因此你可以将预测与分配给给定 PNG 的标签进行比较。

机器学习中的分类算法包括以下算法列表（它们将在下一章中更详细地讨论）：

+   决策树（单一树）

+   随机森林（多棵树）

+   kNN（k-最近邻）

+   逻辑回归（尽管其名称）

+   简单贝叶斯

+   SVM（支持向量机）

一些机器学习算法（如 SVMs、随机森林和 kNN）支持回归和分类。在 SVM 的情况下，该算法的 scikit-learn 实现提供了两个 API：SVC 用于分类和 SVR 用于回归。

前面的每个算法都涉及在数据集上训练的模型，之后使用该模型进行预测。相比之下，随机森林由多个独立的树组成（数量由你指定），每棵树对特征的值进行预测。如果特征是数值型的，取平均值或众数（或执行其他计算）以确定“最终”预测。如果特征是分类的，使用众数（即最频繁出现的类别）作为结果；在平局的情况下，你可以随机选择其中之一。

顺便提一下，以下 URL 包含有关用于分类和回归的 kNN 算法的更多信息：

[`saedsayad.com/k_nearest_neighbors_reg.htm`](http://saedsayad.com/k_nearest_neighbors_reg.htm)

聚类是一种无监督学习技术，用于将相似数据分组在一起。聚类算法将数据点放入不同的簇中，而不了解数据点的性质。数据被分离到不同的簇之后，你可以使用 SVM 算法进行分类。

机器学习中的聚类算法包括以下内容（其中一些是彼此的变体）：

+   k-means

+   均值漂移

+   层次聚类分析（HCA）

+   期望最大化

请记住以下要点。首先，k-means 中的 k 值是一个超参数，通常是一个奇数，以避免两个类别之间的平局。接下来，均值漂移算法结合了 k-means 算法，不需要你指定 k 的值。实际上，均值漂移算法确定最佳聚类数量。然而，这个算法在大数据集上扩展性不好。

机器学习任务

除非你已经有一个已经被清洗过的数据集，否则你需要检查数据集中的数据，以确保它们处于合适的状态。数据准备阶段包括检查行（“数据清洗”）以确保它们包含有效数据（可能需要特定领域的知识）以及检查列（特征选择或特征提取）以确定你是否可以仅保留最重要的列。

以下列出了机器学习任务序列的高级列表（其中一些可能不是必需的）：

+   获取数据集

+   数据清洗

+   特征选择

+   维度降低

+   算法选择

+   训练集与测试集

+   训练模型

+   测试模型

+   微调模型

+   获取模型的度量

首先，显然你需要为你的任务获取一个数据集。在理想情况下，这个数据集已经存在；否则，你需要从一个或多个数据源（例如，CSV 文件、关系数据库、No-SQL 数据库和 Web 服务）中提取数据。

其次，你需要进行数据清洗，你可以通过以下技术来完成：

+   缺失值比率

+   低方差滤波器

+   高相关滤波器

通常，数据清理涉及检查数据集中的数据值，以解决以下一个或多个问题：

+   修复不正确的值

+   解决重复值

+   解决缺失值

+   决定如何处理异常值

如果数据集有太多缺失值，请使用缺失值比率技术。在极端情况下，您可能能够删除具有大量缺失值的特征。使用低方差过滤器技术来识别并从数据集中删除具有常数值的特征。使用高相关性过滤器技术来查找高度相关的特征，这些特征会增加数据集中的多重共线性：可以从数据集中删除这些特征（但在这样做之前请咨询您的领域专家）。

根据您的背景和数据集的性质，您可能需要与领域专家合作，该专家是对数据集内容有深入了解的人。

例如，您可以使用统计值（平均值、众数等）用合适的值替换不正确的值。重复值可以以类似的方式处理。您可以用零、最小值、平均值、众数或数值列中的最大值替换缺失的数值值。您可以用分类列的众数替换缺失的分类值。

如果数据集中的一行包含一个异常值，您有三个选择：

+   删除该行

+   保留该行

+   用其他值（例如平均值）替换异常值

当数据集中包含异常值时，您需要根据特定数据集的领域知识做出决定。

假设一个数据集包含与股票相关的信息。如您所知，1929 年发生了股市崩盘，您可以将其视为异常值。这种事件很少发生，但它可能包含有意义的信息。顺便提一下，20 世纪一些家庭的财富来源是基于大萧条期间以非常低的价格购买大量股票。

特征工程、选择和提取

除了创建数据集和“清理”其值之外，您还需要检查该数据集中的特征，以确定您是否可以减少数据集的维度（即特征的数目）。这样做的过程涉及三个主要技术：

+   特征工程

+   特征选择

+   特征提取（也称为“特征投影”）

特征工程是确定一组基于现有特征组合的新特征的过程，以创建针对给定任务的有意义的数据集。即使是在相对简单的数据集的情况下，这个过程通常也需要领域专业知识。特征工程可能既繁琐又昂贵，在某些情况下，您可能考虑使用自动特征学习。在创建数据集之后，执行特征选择或特征提取（或两者兼而有之）以确保您有一个高质量的数据集是一个好主意。

特征选择也称为“变量选择”、“属性选择”或“变量子集选择”。特征选择涉及在数据集中选择相关特征的一个子集。本质上，特征选择涉及选择数据集中最重要的特征，这提供了以下优势：

+   减少训练时间

+   更简单、更容易解释的模型

+   避免维度灾难

+   由于减少过拟合（“方差减少”）而获得更好的泛化

特征选择技术通常用于具有许多特征和相对较少样本（或数据点）的领域。请记住，低价值特征可能是冗余的或不相关的，这两个概念是不同的。例如，当与另一个强相关特征结合时，一个相关特征可能是冗余的。

特征选择可以使用三种策略：过滤器策略（例如，信息增益）、包装器策略（例如，由准确度引导的搜索）和嵌入式策略（在开发模型时使用预测误差来确定特征是否包含或排除）。另一个有趣的观点是，特征选择对于回归任务以及分类任务也可能很有用。

特征提取通过组合原始特征生成新的特征。相比之下，特征选择涉及确定现有特征的一个子集。

特征选择和特征提取都会导致给定数据集的维度降低，这是下一节的主题。

维度降低

维度降低指的是减少数据集中特征数量的算法。正如您将看到的，有许多技术可用，它们涉及特征选择或特征提取。

使用特征选择进行维度降低的算法如下：

+   后向特征消除

+   前向特征选择

+   因子分析

+   独立成分分析 (ICA)

使用特征提取进行维度降低的算法如下：

+   主成分分析 (PCA)

+   非负矩阵分解 (NMF)

+   核主成分分析 (kernel PCA)

+   基于图的核主成分分析 (graph-based kernel PCA)

+   线性判别分析 (LDA)

+   广义判别分析 (GDA)

+   自动编码器

以下算法结合了特征提取和维度降低：

+   主成分分析 (PCA)

+   线性判别分析 (LDA)

+   均值相关分析 (CCA)

+   非负矩阵分解 (NMF)

这些算法可以在使用聚类或其他算法（如 kNN）对数据集进行处理之前作为预处理步骤使用。另一组算法包括基于投影的方法，其中包括 t-Distributed Stochastic Neighbor Embedding (t-SNE) 以及 UMAP。

本章讨论了 PCA，您可以通过在线搜索找到有关其他算法的更多信息。

主成分分析 (PCA)

主成分是数据集中初始特征的新组合。此外，这些成分是不相关的，并且最有意义或最重要的信息包含在这些新成分中。

PCA 有两个优点：由于特征数量大大减少，计算时间减少，并且当组件最多有三个时，可以绘制组件图。如果你有四个或五个组件，你将无法从视觉上显示它们，但你可以选择三个组件的子集进行可视化，并可能对数据集有更深入的了解。

PCA 使用方差作为信息的度量：方差越高，成分越重要。实际上，PCA 确定协方差矩阵（稍后讨论）的特征值和特征向量，并构建一个新的矩阵，其列是特征向量，从左到右按最左侧列的最大特征值排序，直到最右侧的特征向量也有最小的特征值。

协方差矩阵

作为提醒，随机变量 X 的统计量称为方差，定义为以下：

variance(x) = [SUM (x – xbar)*(x-xbar)]/n

协方差矩阵 C 是一个 n x n 矩阵，其主对角线上的值是变量 X1, X2, . . ., Xn 的方差。C 的其他值是每对变量 Xi 和 Xj 的协方差值。

变量 X 和 Y 的协方差公式是变量方差的推广，公式如下所示：

covariance(X, Y) = [SUM (x – xbar)*(y-ybar)]/n

注意，你可以反转项的乘积顺序（乘法是交换律的），因此协方差矩阵 C 是一个对称矩阵：

covariance(X, Y) = covariance(Y,X)

PCA 计算协方差矩阵 A 的特征值和特征向量。

**处理数据集**

除了数据清洗之外，你还需要执行几个其他步骤，例如选择训练数据与测试数据，以及在训练过程中决定是否使用“保留”或交叉验证。更多细节将在后续章节中提供。

训练数据与测试数据

在你完成了本章前面描述的任务（即数据清洗以及可能的降维）之后，你就可以将数据集分成两部分。第一部分是训练集，用于训练模型，第二部分是测试集，用于“推理”（预测的另一种说法）。确保你的测试集符合以下指南：

1. 集合足够大，可以产生具有统计意义的成果。

2. 它代表了整个数据集。

3. 永远不要在测试数据上训练。

4. 永远不要在训练数据上测试。

什么是交叉验证？

交叉验证的目的是使用非重叠的测试集来测试模型，其执行方式如下：

步骤 1）将数据分成 k 个大小相等的子集。

步骤 2）选择一个子集用于测试，其余的用于训练。

步骤 3）对其他 k-1 个子集重复步骤 2。

这个过程被称为 k 折交叉验证，总体误差估计是误差估计的平均值。一种标准的评估方法涉及十折交叉验证。大量实验表明，使用十个子集是获得准确估计的最佳选择。实际上，你可以重复十折交叉验证十次，并计算结果的平均值，这有助于减少方差。

下一节将讨论正则化，这是本书中一个重要但可选的主题。如果你计划精通机器学习，你需要了解正则化。

**什么是正则化**？

正则化有助于解决过拟合问题，当模型在训练数据上表现良好但在验证或测试数据上表现不佳时，就会发生过拟合问题。正则化通过向损失函数添加惩罚项来解决此问题，从而通过此惩罚项控制模型复杂度。正则化通常对以下情况是有用的：

+   变量数量众多

+   观察数与变量数的低比率

+   高多重共线性

正则化主要有两种类型：L1 正则化（与 MAE，即差异的绝对值相关）和 L2 正则化（与 MSE，即差异的平方相关）。一般来说，L2 的性能优于 L1，且 L2 在计算效率方面是有效的。

机器学习与特征缩放

特征缩放将数据的特征范围标准化。这一步骤在数据预处理步骤中执行，部分原因是因为梯度下降从特征缩放中受益。

假设数据符合标准正态分布，标准化涉及从每个数据点减去均值并除以标准差，从而得到 N(0,1) 的正态分布。

数据归一化与标准化比较

数据归一化是一种线性缩放技术。假设一个数据集具有值 {X1, X2, . . . , Xn} 以及以下术语：

Minx = Xi 值的最小值

Maxx = Xi 值的最大值

现在按照以下方式计算一组新的 Xi 值：

Xi = (Xi – Minx)/[Maxx – Minx]

新的 Xi 值现在已缩放，使其介于 0 和 1 之间。

**偏差-方差权衡**

机器学习中的偏差可能源于学习算法中错误假设的错误。高偏差可能导致算法错过特征与目标输出之间的相关关系（欠拟合）。预测偏差可能由于“噪声”数据、不完整的特征集或有偏的训练样本而出现。

由于偏差引起的错误是模型预期的（或平均）预测值与想要预测的正确值之间的差异。重复模型构建过程多次，每次都收集新的数据，并执行分析以生成新的模型。由于基础数据集具有一定的随机性，因此生成的模型具有一系列预测值。偏差衡量这些模型的预测值与正确值的偏差程度。

机器学习中的方差是平方偏差的期望值。高方差可能导致算法对训练数据中的随机噪声进行建模，而不是预期的输出（过拟合）。

向模型添加参数会增加其复杂性，增加方差，并减少偏差。处理偏差和方差就是处理欠拟合和过拟合。

由于方差引起的错误是针对给定数据点的模型预测的变异性。与之前一样，重复整个模型构建过程，方差是针对给定点的预测在不同“实例”的模型中变化的程度。

衡量模型的指标

线性回归模型使用 R 平方值，该值衡量数据与拟合回归线（回归系数）的接近程度。R 平方值始终是介于 0%和 100%之间的百分比。0%的值表示模型无法解释响应数据围绕其均值的任何变异性。100%的值表示模型可以解释响应数据围绕其均值的全部变异性。一般来说，R 平方值越高，表示模型越好。

R 平方的局限性

虽然高 R 平方值是首选的，但它们并不一定是始终好的值。同样，低 R 平方值也不一定是坏的。例如，预测人类行为的 R 平方值通常小于 50%。此外，R 平方无法确定系数估计和预测是否存在偏差。此外，R 平方值并不表示回归模型是否充分。因此，对于好的模型，可能有一个低 R 平方值，或者对于拟合不良的模型，可能有一个高 R 平方值。将 R 平方值与残差图、其他模型统计量和领域知识一起评估。

混淆矩阵

分类算法使用混淆矩阵（也称为“错误矩阵”），这是一个包含错误正例、错误负例、真正例和真负例数量的方形列联表。2x2 混淆矩阵中的四个条目可以如下标记：

TP：真正例

FP：假正例

TN：真负例

FN：假负例

混淆矩阵的对角线值是正确预测，而离对角线值是不正确预测。一般来说，FP 值比 FN 值低更好。例如，FP 表示一个健康的人被错误地诊断为疾病，而 FN 表示一个不健康的人被错误地诊断为健康。

准确率与精确率与召回率

一个 2x2 的混淆矩阵有四个条目，代表正确和错误分类的各种组合。根据前面章节的定义，精确率、准确率和召回率的定义如下公式：

精确率 = TP/(TP + FP)

准确率 = (TP + TN)/[TP + FP + FN + TN]

召回率 = TP/[TP + FN]

准确率可能是一个不可靠的指标，因为它在数据不平衡的情况下会产生误导性的结果。当不同类别的观察数量显著不同时，它会给错误阳性分类和错误阴性分类同等的重要性。例如，宣布癌症为良性比错误地告知患者他们正在遭受癌症更糟糕。不幸的是，准确率无法区分这两种情况。

请记住，混淆矩阵可以是一个 nxn 矩阵，而不仅仅是 2x2 矩阵。例如，如果一个类别有 5 个可能的值，那么混淆矩阵是一个 5x5 矩阵，而对角线上的数字是“真正”结果。

ROC 曲线

接收者操作特征（ROC）曲线是一条曲线，它绘制了真正阳性率（TPR，即召回率）与假阳性率（FPR）的关系。请注意，真正阴性率（TNR）也称为特异性。

以下网页包含一个使用 sklearn 和 Iris 数据集的 Python 代码示例，以及绘制 ROC 曲线的代码：

[`scikit-learn.org/stable/auto_examples/model_selection/plot_roc.html`](https://scikit-learn.org/stable/auto_examples/model_selection/plot_roc.html)

以下网页包含用于绘制 ROC 曲线的 Python 代码示例的集合：

[`stackoverflow.com/questions/25009284/how-to-plot-roc-curve-in-python`](https://stackoverflow.com/questions/25009284/how-to-plot-roc-curve-in-python)

其他有用的统计术语

机器学习依赖于许多统计量来评估模型的有效性，其中一些列在这里：

+   RSS

+   TSS

+   R²

+   F1 分数

+   p-value

RSS、TSS 和 R² 的定义如下，其中 y^是最佳拟合线上一点的 y 坐标，y_ 是数据集中点的 y 值平均值：

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p47.jpg)

什么是 F1 分数？

*F1 分数*是测试准确度的衡量指标，它被定义为精确率和召回率的调和平均数。以下是相关公式，其中 p 是精确率，r 是召回率：

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p48.jpg)

F1 分数的最佳值是 0，最差值也是 0\. F1 分数通常用于分类问题，而 R² 值通常用于回归任务（如线性回归）。

p 值是什么？

如果 p 值足够小（< 0.005），则使用 p 值来拒绝零假设，这表明更高的显著性。回想一下，零假设表明一个因变量（如 y）和一个自变量（如 x）之间没有相关性。p 的阈值通常是 1%或 5%。

计算 p 值没有直接的公式，p 值总是在 0 和 1 之间。实际上，p 值是用于评估“零假设”的统计量，它们是通过 p 值表或电子表格/统计软件计算得出的。

什么是线性回归？

线性回归的目标是找到最佳拟合线，该线“代表”数据集。请记住两个关键点。首先，最佳拟合线不一定通过数据集中的所有（甚至大多数）点。最佳拟合线的目的是最小化该线与数据集中点的垂直距离。其次，线性回归并不确定最佳拟合的多项式：后者涉及找到通过数据集中许多点的更高次多项式。

此外，平面上的数据集可以包含两个或更多位于同一直线上的点，也就是说这些点的 x 值相同。然而，一个函数不能穿过这样的点对：如果两个点(x1,y1)和(x2,y2)具有相同的 x 值，那么它们必须具有相同的 y 值（即 y1=y2）。一个函数可以有多个位于同一直线上的点。

现在考虑一个在平面上有许多点，这些点在某种程度上“聚集”成一种拉长的云状形状的散点图：最佳拟合线可能只会与有限数量的点相交（实际上，最佳拟合线可能不会与任何点相交）。

考虑另一种场景：假设一个数据集包含一组位于同一直线上的点。例如，假设 x 的值在集合{1,2,3,...,10}中，而 y 的值在集合{2,4,6,...,20}中。那么最佳拟合线的方程是 y=2*x+0\. 在这种情况下，所有点都是共线的，也就是说它们位于同一直线上。

线性回归与曲线拟合的比较

假设一个数据集由 n 个形式为 (x, y) 的数据点组成，并且这些数据点中没有两个具有相同的 x 值。那么，根据数学中的一个已知结果，存在一个次数小于或等于 n-1 的多项式可以穿过这 n 个点（如果你真的感兴趣，你可以在在线文章中找到这个陈述的数学证明）。例如，一条直线是一个次数为一的多项式，它可以与平面上的任意一对非垂直点相交。对于平面上的任意三个不在同一直线上的点，存在一个二次方程可以穿过这些点。

此外，有时可以使用低次多项式。例如，考虑一组 100 个点，其中 x 值等于 y 值：在这种情况下，直线 y = x（这是一个次数为一的多项式）穿过所有 100 个点。

然而，一条直线“代表”平面上一组点的程度取决于这些点可以通过直线近似到何种程度，这由点的方差（方差是一个统计量）来衡量。点越线性，方差越小；相反，点越“分散”，方差越大。

解何时为精确值？

尽管基于统计的解决方案为线性回归提供了封闭形式解，但神经网络提供近似解。这是因为线性回归的机器学习算法涉及一系列近似，这些近似“收敛”到最优值，这意味着机器学习算法产生对精确值的估计。例如，对于二维平面上的一组点，最佳拟合线的斜率 m 和 y 截距 b 在统计学中有一个封闭形式解，但它们只能通过机器学习算法进行近似（虽然存在例外，但它们是罕见的情况）。

尽管对于“传统”线性回归的封闭形式解提供了 m 和 b 的精确值，但有时你只能使用这些精确值的近似值。例如，假设最佳拟合线的斜率 m 等于 3 的平方根，而 y 截距 b 是 2 的平方根。如果你计划在源代码中使用这些值，你只能处理这两个数字的近似值。在相同的情况下，神经网络计算 m 和 b 的近似值，无论 m 和 b 的精确值是有理数、无理数还是整数。然而，机器学习算法更适合复杂、非线性、多维数据集。

作为简单的例子，假设线性回归问题的封闭形式解为 m 和 b 产生整数或有理数值。具体来说，让我们假设封闭形式解为最佳拟合线的斜率和 y 截距分别产生 2.0 和 1.0 的值。这条直线的方程看起来像这样：

y = 2.0 * x + 1.0

然而，通过训练神经网络得到的相应解可能会产生斜率 m 和 y 截距 b 的最佳拟合线对应的值分别为 2.0001 和 0.9997。始终牢记这一点，尤其是在训练神经网络时。

什么是多元分析？

多元分析将欧几里得平面上的直线方程推广到更高维度，并被称为超平面而不是直线。推广后的方程具有以下形式：

y = w1*x1 + w2*x2 + ... + wn*xn + b

在二维线性回归的情况下，你只需要找到斜率（m）和 y 截距（b）的值，而在多元分析中，你需要找到 w1、w2、...、wn 的值。请注意，多元分析是统计学中的一个术语，在机器学习中通常被称为“广义线性回归”。本书中涉及线性回归的大多数代码示例都涉及欧几里得平面中的二维点。

其他类型的回归

线性回归找到最佳拟合线来“代表”数据集，但如果平面上的直线不适合数据集怎么办？当你处理数据集时，这是一个相关的问题。

线性回归的一些替代方案包括二次方程、三次方程或更高次的多项式。然而，这些替代方案涉及权衡，我们将在后面讨论。

另一种可能性是一种混合方法，它涉及到分段线性函数，由一系列线段组成。如果连续的线段是连接的，那么它是一个分段线性连续函数；否则，它是一个分段线性不连续函数。

因此，给定平面上的点集，回归涉及到解决以下问题：

1. 哪种类型的曲线最适合数据？我们如何知道？

2. 另一种类型的曲线是否更适合数据？

3. “最佳拟合”是什么意思？

检查直线是否适合数据的一种方法是通过视觉检查，但这种方法不适用于高于二维的数据点。此外，这是一个主观的决定，本章后面将展示一些样本数据集。通过数据集的视觉检查，你可能会决定二次或三次（甚至更高次）多项式有可能是更好的拟合。然而，视觉检查可能仅限于二维平面或三维空间中的点。

让我们先不考虑非线性情况，假设一条直线对于数据集来说是一个很好的拟合。有一种已知的技术可以找到此类数据集的“最佳拟合”线，它涉及到最小化均方误差（MSE，我们将在本章后面讨论）。

下一个部分将简要回顾平面上的线性方程，并附有一些说明线性方程示例的图像。

在平面上的直线处理（可选）

本节简要回顾了欧几里得平面中的线，如果您对这个主题感到舒适，可以跳过这一节。一个常被忽视的细微之处是，欧几里得平面中的线具有无限长度。如果您选择一条线上的两个不同点，那么这两个选定点之间的所有点都构成一条线段。射线是一条“半无限”线：当您选择一个点作为端点时，那么直线一侧的所有点构成一条射线。

例如，平面上 y 坐标为 0 的点是一条线，同时也是 x 轴，而 x 轴上(0,0)和(1,0)之间的点形成一条线段。此外，x 轴上位于(0,0)右侧的点形成一条射线，而 x 轴上位于(0,0)左侧的点也形成一条射线。

为了简洁和方便，在这本书中，我们将“线”和“线段”这两个术语交替使用。现在让我们深入了解欧几里得平面中线的细节。以下是欧几里得平面中一条（非垂直）线的方程：

y = m*x + b

m 的值是直线的斜率，b 的值是 y 轴截距（即直线与 y 轴相交的点）。

如果需要，您可以使用一个更通用的方程来表示垂直线，如下所示：

a*x + b*y + c = 0

然而，我们不会处理垂直线，因此我们将使用第一个公式。

图 2.1 显示了三条水平线，其方程（从上到下）分别是 y = 3，y = 0 和 y = -3。

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p52-1.jpg)

图 2.1 三条水平线段。

图 2.2 显示了两条斜率线，其方程分别是 y = x 和 y = -x。

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p52-2.jpg)

图 2.2 展示了两条对角线段。

图 2.3 显示了两条斜率平行的线，其方程分别是 y = 2*x 和 y = 2*x + 3。

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p53-1.jpg)

图 2.3 两条斜率平行线段。

图 2.4 显示了一个由连接线段组成的分段线性图。

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p53-2.jpg)

图 2.4 展示了由连接线段组成的分段线性图。

让我们将注意力转向使用 NumPy API 生成准随机数据，然后我们将使用 Matplotlib 绘制数据。

使用 NumPy 和 Matplotlib 绘制散点图（1）

代码清单 2.1 展示了 np_plot1.py 的内容，该内容说明了如何使用 NumPy 的 randn() API 生成数据集，然后使用 Matplotlib 的 scatter() API 绘制数据集中的点。

需要注意的一个细节是，所有相邻的水平值都是等间距的，而垂直值是基于一个线性方程加上一个“扰动”值。这种“扰动技术”（这不是一个标准术语）在本章的其他代码示例中用于在绘制点时添加一个轻微的随机效果。这种技术的优点是，m 和 b 的最佳拟合值是事先已知的，因此我们不需要猜测它们的值。

列表 2.1: np_plot1.py

import numpy as np

import matplotlib.pyplot as plt

x = np.random.randn(15,1)

y = 2.5*x + 5 + 0.2*np.random.randn(15,1)

print("x:",x)

print("y:",y)

plt.scatter(x,y)

plt.show()

列表 2.1 包含两个导入语句，然后使用 15 个介于 0 和 1 之间的随机数初始化数组变量 x。

接下来，数组变量 y 在两部分定义：第一部分是一个线性方程 2.5*x + 5，第二部分是基于随机数的“扰动”值。因此，数组变量 y 模拟了一组接近线段的一组值。

这种技术在模拟线段的代码示例中使用，然后训练部分近似最佳拟合线的 m 和 b 的值。显然，我们已经知道最佳拟合线的方程：这种技术的目的是比较训练得到的斜率 m 和 y 截距 b 的值与已知值（在这种情况下，是 2.5 和 5）进行比较。以下是 列表 2.1 的部分输出：

x: [[-1.42736308]

[ 0.09482338]

[-0.45071331]

[ 0.19536304]

[-0.22295205]

// 省略值以节省空间

y: [[1.12530514]

[5.05168677]

[3.93320782]

[5.49760999]

[4.46994978]

// 省略值以节省空间

图 2.5 显示了基于 x 和 y 值的点散点图。

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p55.jpg)

图 2.5 线段的点散点图

为什么扰动技术是有用的

你已经看到了如何使用扰动技术，为了比较，考虑以下数据集，这些点定义在 Python 数组变量 X 和 Y 中：

X = [0,0.12,0.25,0.27,0.38,0.42,0.44,0.55,0.92,1.0]

Y = [0,0.15,0.54,0.51, 0.34,0.1,0.19,0.53,1.0,0.58]

如果你需要找到前面数据集的最佳拟合线，你会如何猜测斜率 m 和 y 截距 b 的值？在大多数情况下，你可能无法猜测它们的值。然而，扰动技术使你能够稍微移动一条线的点，这条线的斜率 m（以及可选的 y 截距 b）的值是事先指定的。

当你引入小的随机值，而这些值不会导致 m 和 b 的值不同时，扰动技术才起作用。

使用 NumPy 和 Matplotlib 的散点图（2）

列表 2.1（前一个章节中的代码）为变量 x 分配了随机值，而斜率 m 被分配了一个硬编码的值。y 值是 x 值的硬编码倍数，加上通过扰动技术计算出的随机值。因此，我们不知道 y 截距 b 的值。

在本节中，trainX 的值基于 np.linspace() API，而 trainY 的值涉及前一个章节中描述的扰动技术。

此示例中的代码简单地打印了 trainX 和 trainY 的值，它们对应于欧几里得平面中的数据点。列表 2.2 显示了 np_plot2.py 的内容，说明了如何在 NumPy 中模拟线性数据集。

列表 2.2: np_plot2.py

import numpy as np

trainX = np.linspace(-1, 1, 11)

trainY = 4*trainX + np.random.randn(*trainX.shape)*0.5

print("trainX: ",trainX)

print("trainY: ",trainY)

列表 2.2 通过 NumPy linspace() API 初始化 NumPy 数组变量 trainX，然后是定义在两部分的数组变量 trainY。第一部分是线性项 4*trainX，第二部分涉及扰动技术，这是一个随机生成的数字。列表 2.2 的输出如下：

trainX: [-1\. -0.8 -0.6 -0.4 -0.2 0\. 0.2 0.4 0.6 0.8 1\. ]

trainY: [-3.60147459 -2.66593108 -2.26491189 -1.65121314 -0.56454605 0.22746004 0.86830728 1.60673482 2.51151543 3.59573877 3.05506056]

下一个部分包含一个类似于列表 2.2 的示例，使用相同的扰动技术生成一组近似二次方程的点，而不是线段。

使用 NumPy 和 Matplotlib 绘制二次散点图

列表 2.3 显示了 np_plot_quadratic.py 的内容，说明了如何在平面上绘制二次函数。

列表 2.3: np_plot_quadratic.py

import numpy as np

import matplotlib.pyplot as plt

#查看这个值集会发生什么：

#x = np.linspace(-5,5,num=100)

x = np.linspace(-5,5,num=100)[:,None]

y = -0.5 + 2.2*x +0.3*x**2 + 2*np.random.randn(100,1)

print("x:",x)

plt.plot(x,y)

plt.show()

列表 2.3 使用 np.linspace() API 生成的值初始化数组变量 x，在这种情况下，是一个介于 -5 和 5 之间等距的 100 个十进制数的集合。注意 x 初始化中的 [:,None] 片段，它导致每个元素都是一个只包含单个数字的数组。 

数组变量 y 定义在两部分：第一部分是一个二次方程 -0.5 + 2.2*x +0.3*x**2，第二部分是一个基于随机数的“扰动”值（类似于列表 2.1 中的代码）。因此，数组变量 y 模拟了一组近似二次方程的值。列表 2.3 的输出如下：

x:

[[-5\. ]

[-4.8989899 ]

[-4.7979798 ]

[-4.6969697 ]

[-4.5959596 ]

[-4.49494949]

// 省略值以节省篇幅

[ 4.8989899 ]

[ 5\. ]]

图 2.6 展示了基于 x 和 y 值的点散点图，这些点的大致形状类似于二次方程。

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p57.jpg)

图 2.6 二次方程的点散点图

均方误差（MSE）公式

MSE 是实际 y 值与预测 y 值之间差异的平方和，除以点的数量。请注意，预测 y 值是如果该点实际上位于最佳拟合线上，每个点将具有的 y 值。

虽然 MSE 在线性回归中很受欢迎，但还有其他类型的误差可用，其中一些将在下一节中简要讨论。

错误类型列表

尽管我们将在本书中仅讨论线性回归的 MSE，但还有其他类型的公式可用于线性回归，其中一些列在这里：

+   MSE

+   RMSE

+   RMSPROP

+   MAE

MSE 是前面误差类型的基础。例如，RMSE 是均方根误差，它是 MSE 的平方根。

MAE 是平均绝对误差，它是 y 项差异的绝对值之和（而不是 y 项差异的平方），然后除以项的数量。

RMSPROP 优化器利用最近梯度的幅度来归一化梯度。具体来说，RMSPROP 维护一个 RMS（均方根）梯度的移动平均值，然后将其除以当前梯度。

虽然计算 MSE 的导数更容易，但 MSE 也更容易受到异常值的影响，而 MAE 则不太容易受到异常值的影响。原因很简单：平方项可以显著大于项的绝对值。例如，如果差异项是 10，则将 100 添加到 MSE 中，而 MAE 只添加 10（-20 的绝对值）。同样，如果差异项是 -20，则将 400 添加到 MSE 中，而 MAE 只添加 20（-20 的绝对值）。

非线性最小二乘法

在预测房价时，数据集包含广泛的价值范围，线性回归或随机森林等技术可能导致模型过度拟合具有最高值的样本，以减少如平均绝对误差等数量。

在这种情况下，你可能需要一个误差度量，如相对误差，以减少拟合最大值样本的重要性。这种技术称为非线性最小二乘法，它可能使用基于标签和预测值的对数变换。

下一节包含几个代码示例，第一个示例涉及手动计算 MSE，随后是一个使用 NumPy 公式进行计算的示例。

手动计算 MSE

本节包含两个线形图，每个图都包含一条近似散点图中一组点的线。

图 2.7 展示了一条线段，该线段近似表示了一组点的散点图（其中一些点与线段相交）。图 2.7 中线的均方误差（MSE）计算如下（仅比较分子）：

MSE = (1*1 + (-1)*(-1) + (-1)*(-1) + 1*1)/9 = 4/9

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p59.jpg)

图 2.7 一个近似表示散点图点的线图

图 2.8 展示了一组点和一条可能是最佳拟合线的线。图 2.8 中线的均方误差（MSE）计算如下：

MSE = ((-2)*(-2) + 2*2)/7 = 8/7

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p60.jpg)

图 2.8 一个近似表示散点图点的线图

因此，图 2.7 中的线比图 2.8 中的线具有更小的 MSE，这可能会让你感到惊讶（或者你猜对了？）。

在这两个图中，我们轻松快速地计算了 MSE，但在一般情况下，这要困难得多。例如，如果我们在一个欧几里得平面上绘制 10 个点，这些点不紧密地拟合一条线，并且涉及非整数值的各个项，我们可能需要计算器。

一个更好的解决方案涉及 NumPy 函数，例如 np.linspace() API，如下一节所述。

使用 np.linspace()近似线性数据

代码列表 2.4 展示了 np_linspace1.py 的内容，该内容说明了如何结合扰动技术使用 np.linspace() API 生成一些数据。

代码列表 2.4: np_linspace1.py

import numpy as np

trainX = np.linspace(-1, 1, 6)

trainY = 3*trainX + np.random.randn(*trainX.shape)*0.5

print("trainX: ", trainX)

print("trainY: ", trainY)

这个代码示例的目的是生成并显示一组随机生成的数字。在本章的后面部分，我们将使用这个代码作为实际线性回归任务的起点。

代码列表 2.4 从定义通过 np.linspace() API 初始化的数组变量 trainX 开始。接下来，通过在之前的代码示例中使用的扰动技术定义数组变量 trainY。代码列表 2.4 的输出如下：

trainX: [-1\. -0.6 -0.2 0.2 0.6 1\. ]

trainY: [-2.9008553 -2.26684745 -0.59516253 0.66452207 1.82669051 2.30549295]

trainX: [-1\. -0.6 -0.2 0.2 0.6 1\. ]

trainY: [-2.9008553 -2.26684745 -0.59516253 0.66452207 1.82669051 2.30549295]

现在我们知道了如何生成线性方程的(x,y)值，接下来让我们学习如何计算 MSE，这将在下一节中讨论。下一个示例使用 np.linspace()方法和 np.random.randn()方法生成一组数据值，以在数据点中引入一些随机性。

使用 np.linspace() API 计算 MSE

本节中的代码示例与本章中许多早期的代码示例不同：它使用硬编码的 X 和 Y 的值数组，而不是扰动技术。因此，你将不知道斜率和 y 截距的正确值（你可能甚至无法猜测它们的正确值）。列表 2.5 显示了 plain_linreg1.py 的内容，该内容说明了如何使用模拟数据计算均方误差。

列表 2.5：plain_linreg1.py

import numpy as np

import matplotlib.pyplot as plt

X = [0,0.12,0.25,0.27,0.38,0.42,0.44,0.55,0.92,1.0]

Y = [0,0.15,0.54,0.51, 0.34,0.1,0.19,0.53,1.0,0.58]

losses = []

# 步骤 1：参数初始化

W = 0.45

b = 0.75

for i in range(1, 100):

# 步骤 2：计算损失

Y_pred = np.multiply(W, X) + b

Loss_error = 0.5 * (Y_pred - Y)**2

loss = np.sum(Loss_error)/10

# 步骤 3：计算 dW 和 db

db = np.sum((Y_pred - Y))

dw = np.dot((Y_pred - Y), X)

losses.append(loss)

# 步骤 4：更新参数：

W = W - 0.01*dw

b = b - 0.01*db

if i%10 == 0:

print("第", i,"次迭代的损失 = ", loss)

# 步骤 5：通过 for 循环重复 1000 次迭代

# 绘制损失与迭代次数的关系图

print("W = ", W,"& b = ", b)

plt.plot(losses)

plt.ylabel('损失')

plt.xlabel('迭代次数（每十次）')

plt.show()

列表 2.5 使用硬编码的值初始化数组变量 X 和 Y，然后初始化标量变量 W 和 b。列表 2.5 的下一部分包含一个循环，循环 100 次。循环的每次迭代后，都会计算 Y_pred、Loss_error 和 loss 的值。接下来，根据 Y_pred-Y 数组中项的和以及 Y_pred-y 和 X 的内积，分别计算 dw 和 db 的值。

注意 W 和 b 的更新方式：它们的值分别减去 0.01*dw 和 0.01*db 的项。这个计算应该看起来很熟悉：代码正在程序化地计算 W 和 b 的梯度的近似值，W 和 b 都乘以学习率（硬编码的值 0.01），然后从 W 和 b 的当前值中减去这个结果项，以产生 W 和 b 的新近似值。尽管这个技术很简单，但它确实计算了 W 和 b 的合理值。

列表 2.5 的最后一部分显示了 W 和 b 的中间近似值，以及损失（垂直轴）与迭代次数（水平轴）的图表。列表 2.5 的输出如下：

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

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p63.jpg)

图 2.9 线性回归的均方误差值

代码示例 plain-linreg2.py 与列表 2.5 中的代码相似：不同之处在于，它不是 100 次迭代的单个循环，而是一个外循环，执行 100 次，而在外循环的每次迭代中，内循环也执行 100 次。

概述

本章介绍了机器学习以及诸如特征选择、特征工程、数据清洗、训练集和测试集等概念。接下来，你学习了监督学习、无监督学习和半监督学习。然后你学习了回归任务、分类任务和聚类，以及准备数据集通常所需的步骤。这些步骤包括“特征选择”或“特征提取”，可以使用各种算法执行。然后你学习了数据集中可能出现的与数据相关的问题以及如何纠正这些问题。

此外，你还学习了线性回归，以及如何计算欧几里得平面上值数据集的最佳拟合线的一个简要描述。你看到了如何使用 NumPy 初始化数据值数组来执行线性回归，以及一种“扰动技术”，该技术为 y 值引入了一些随机性。这种技术是有用的，因为你知道最佳拟合线的斜率和 y 截距的正确值，然后你可以将它们与训练值进行比较。

第三章

机器学习中的分类器

本章介绍了机器学习中的许多分类算法。这包括 kNN（k-最近邻）算法、逻辑回归（尽管其名称如此，但它是一种分类器）、决策树、随机森林、SVMs 和贝叶斯分类器。对算法的强调旨在让你了解机器学习，其中包括一个基于树的代码示例，该示例依赖于 scikit-learn。

由于篇幅限制，本章没有涵盖其他知名算法，如线性判别分析和 k-means 算法（该算法用于无监督学习和聚类）。然而，有许多在线教程讨论了这些以及其他机器学习算法。

考虑到前面的要点，本章的第一节简要讨论了引言段落中提到的分类器。本章的第二节概述了激活函数，如果你决定学习深度神经网络，这将非常有用。你将了解它们在神经网络中是如何以及为什么被使用的。本节还包含了一个 TensorFlow API 激活函数列表，随后是对其中一些优点的描述。

第三节介绍了逻辑回归，它依赖于 Sigmoid 函数，也用于 RNNs（循环神经网络）和 LSTMs（长短期记忆）。

为了给你一些背景信息，分类器是三种主要类型的算法之一：回归算法（例如，线性回归和第四章中的 GPT-4），分类算法（本章讨论），以及聚类算法（如 k-means，本书未讨论）。

关于激活函数的部分确实涉及到了神经网络中隐藏层的基本理解。根据你的经验水平，在阅读这一部分之前，你可能需要阅读一些预备材料（网上有很多相关文章）。

什么是分类？

给定一个包含已知类别成员资格的观察值的数据集，分类是确定新数据点所属类别的任务。类别指的是类别，也称为“目标”或“标签”。例如，电子邮件服务提供商中的垃圾邮件检测涉及二元分类（只有两个类别）。MNIST 数据集包含一系列图像，其中每个图像都是一个单独的数字，这意味着有十个标签。分类的一些应用包括信用批准、医疗诊断和目标营销。

什么是分类器？

在上一章中，你了解到线性回归结合了监督学习和数值数据。目标是训练一个模型，使其能够做出数值预测（例如，明天股票的价格，系统的温度或其气压）。相比之下，分类器结合了监督学习和非数值类别的数据：目标是训练一个模型，使其能够做出分类预测。

例如，假设数据集的每一行都是一种特定的葡萄酒，每一列都涉及一种特定的葡萄酒特征（单宁、酸度等等）。进一步假设数据集中有五种葡萄酒类别：为了简单起见，让我们将它们标记为 A、B、C、D 和 E。给定一个新的数据点，也就是说，新的数据行，这个数据集的分类器试图确定这种葡萄酒的标签。

本章中的一些分类器不仅可以执行分类，还可以进行数值预测（即，它们既可以用于回归，也可以用于分类）。

常见分类器

这里列出了机器学习中一些最流行的分类器（不分先后顺序）：

+   线性分类器

+   kNN

+   逻辑回归

+   决策树

+   随机森林

+   SVMs

+   贝叶斯分类器

+   CNNs（深度学习）

不同的分类器有不同的优缺点，这通常涉及到复杂性和准确性之间的权衡，类似于人工智能领域之外的领域的算法。

在深度学习的情况下，卷积神经网络（CNNs）执行图像分类，这使得它们成为分类器（它们也可以用于音频和文本处理）。

下面的部分简要介绍了上一列表中列出的机器学习分类器。

二分类与多分类分类

二分类器与具有两个类别的数据集一起工作，而多分类器（有时称为多项式分类器）可以区分超过两个类别。随机森林分类器和朴素贝叶斯分类器支持多类别，而 SVMs 和线性分类器只能用作二分类器。

此外，还有基于二分类器的多分类技术：一对多（OvA）和一对一（OvO）。

OvA 技术（也称为“一对多”）涉及多个等于类别数的二分类器。例如，如果一个数据集有五个类别，那么 OvA 使用五个二分类器，每个二分类器检测五个类别中的一个。为了在这个特定数据集中对数据点进行分类，选择输出最高分数的二分类器。

OvO 技术也涉及多个二分类器，但在这个情况下，使用一个二分类器来训练一对类别。例如，如果类别是 A、B、C、D 和 E，那么需要十个二分类器：一个用于 A 和 B，一个用于 A 和 C，一个用于 A 和 D，以此类推，直到最后一个用于 D 和 E 的二分类器。

通常，如果有 n 个类别，则需要 n*(n-1)/2 个二分类器。尽管 OvO 技术需要的二分类器（例如，对于 20 个类别需要 190 个）比 OvA 技术（例如，对于 20 个类别只需要 20 个）多得多，但 OvO 技术的优势在于每个二分类器只在其两个选择的类别相关的数据集部分上训练。

多标签分类

多标签分类涉及将多个标签分配给数据集中的实例。因此，多标签分类是多分类分类（在上一节中讨论）的推广，后者涉及将单个标签分配给属于具有多个类别的数据集的实例。一篇涉及多标签分类并包含基于 Keras 的代码的文章可在网上找到：

[使用 Keras-imagedatagenerator 的多标签图像分类教程](https://medium.com/@vijayabhaskar96/multi-label-image-classification-tutorial-with-keras-imagedatagenerator-cd541f8eaf24)

您还可以在线搜索涉及 SKLearn 或 PyTorch 的多标签分类任务的文章。

什么是线性分类器？

线性分类器将数据集分为两类。线性分类器是二维点的线，三维点的平面，以及更高维度的超平面（平面的推广）。

线性分类器通常是速度最快的分类器，因此当分类速度非常重要时经常被使用。线性分类器通常在输入向量稀疏（即大部分为零值）或维度数量很大时表现良好。

什么是 kNN？

kNN（k-最近邻）算法是一种分类算法。简而言之，彼此“靠近”的数据点被归类为属于同一类。当引入一个新点时，它会被添加到其最近邻大多数点的类别中。例如，假设 k 等于 3，并引入一个新数据点。查看其 3 个最近邻的类别：假设它们是 A、A 和 B。然后通过多数投票，新数据点被标记为类别 A 的数据点。

kNN 算法本质上是一种启发式方法，而不是具有复杂数学基础的技巧，尽管如此，它仍然是一个有效且有用的算法。

如果你想要使用一个简单的算法，或者当你认为你的数据集性质高度无结构时，尝试 kNN 算法。kNN 算法可以产生高度非线性的决策，尽管它非常简单。你可以在搜索应用中使用 kNN 来搜索“相似”的项目。

通过创建项目的向量表示来衡量相似度，然后使用适当的距离度量（如欧几里得距离）比较向量。

kNN 搜索的一些具体例子包括搜索语义相似的文档。

如何处理 kNN 中的平局

k 的值为奇数时，不太可能导致平局投票，但这并非不可能。例如，假设 k 等于 7，当引入一个新数据点时，其 7 个最近邻属于集合{A,B,A,B,A,B,C}。如你所见，没有多数投票，因为类别 A 有 3 个点，类别 B 有 3 个点，类别 C 有 1 个点。

在 kNN 中处理平局有多种技术，如下所示：

+   给予较近的点更高的权重。

+   增大 k 的值，直到确定一个赢家。

+   减小 k 的值，直到确定一个赢家。

+   随机选择一个类别。

如果你将 k 减小到 1，仍然可能存在平局投票：可能有两个点与新的点距离相等，因此你需要一种机制来决定选择这两个点中的哪一个作为 1-邻居。

如果类别 A 和类别 B 之间存在平局，那么随机选择类别 A 或类别 B。另一种变体是跟踪“平局”投票，并轮流确保更均匀的分布。

什么是决策树？

决策树是另一种涉及树形结构的分类算法。在“通用”树中，数据点的放置由简单的条件逻辑决定。作为一个简单的说明，假设一个数据集包含一组代表人们年龄的数字，并且假设第一个数字是 50。这个数字被选为树的根，所有小于 50 的数字都添加到树的左分支，而所有大于 50 的数字都添加到树的右分支。

例如，假设我们有一个如下数字序列：{50, 25, 70, 40}。然后我们可以构建如下树：50 是根节点；25 是 50 的左子节点；70 是 50 的右子节点；40 是 20 的右子节点。我们将添加到这个数据集的每个附加数值都经过处理，以确定在树的每个节点处应向哪个方向前进（“左或右”）。

列表 3.1 显示了 sklearn_tree2.py 的内容，该内容定义了欧几里得平面上的二维点集及其标签，然后预测了欧几里得平面上的其他几个二维点的标签（即类别）。

列表 3.1: sklearn_tree2.py

from sklearn import tree

# X = 2D 点的对和 Y = 每个点的类别

X = [[0, 0], [1, 1], [2,2]]

Y = [0, 1, 1]

tree_clf = tree.DecisionTreeClassifier()

tree_clf = tree_clf.fit(X, Y)

#predict the class of samples:

print("predict class of [-1., -1.]:")

print(tree_clf.predict([[-1., -1.]]))

print("predict class of [2., 2.]:")

print(tree_clf.predict([[2., 2.]]))

# 训练样本中相同类别的百分比

# 在叶子节点中等于每个类别的概率

print("probability of each class in [2.,2.]:")

print(tree_clf.predict_proba([[2., 2.]]))

列表 3.1 从 sklearn 导入树类，然后使用数据值初始化数组 X 和 y。接下来，变量 tree_clf 被初始化为 DecisionTreeClassifier 类的实例，然后通过调用 fit() 方法使用 X 和 y 的值进行训练。

现在运行 列表 3.1 中的代码，你将看到以下输出：

predict class of [-1., -1.]:

[0]

predict class of [2., 2.]:

[1]

[2.,2.] 中每个类别的概率：

[[0. 1.]]

如你所见，点 [-1,-1] 和 [2,2] 分别被正确标记为值 0 和 1。

列表 3.2 显示了 sklearn_tree3.py 的内容，该内容通过添加第三个标签并预测欧几里得平面上的三个点而不是两个点来扩展 列表 3.1 中的代码，修改内容以粗体显示。

列表 3.2: sklearn_tree3.py

from sklearn import tree

# X = pairs of 2D points and Y = the class of each point

X = [[0, 0], [1, 1], [2,2]]

Y = [0, 1, 2]

tree_clf = tree.DecisionTreeClassifier()

tree_clf = tree_clf.fit(X, Y)

#predict the class of samples:

print("predict class of [-1., -1.]:")

print(tree_clf.predict([[-1., -1.]]))

print("predict class of [0.8, 0.8]:")

print(tree_clf.predict([[0.8, 0.8]]))

print("predict class of [2., 2.]:")

print(tree_clf.predict([[2., 2.]]))

# 相同类别的训练样本百分比

# 在叶子节点中的值等于每个类别的概率

print("probability of each class in [2.,2.]:")

print(tree_clf.predict_proba([[2., 2.]]))

现在运行 列表 3.2，你将看到以下输出：

预测 [-1., -1.] 的类别：

[0]

预测 [0.8, 0.8] 的类别：

[1]

预测 [2., 2.] 的类别：

在 [2.,2.] 中每个类别的概率：

[2]

[[0\. 0\. 1.]]

如您所见，点 [-1,-1]，[0.8, 0.8] 和 [2,2] 分别被正确标记为值 0，1 和 2。

列表 3.3 显示了数据集 partial_wine.csv 的一部分，该数据集包含两个特征和标签列（有三个类别）。此数据集的总行数为 178。

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

import numpy as np

import matplotlib.pyplot as plt

import pandas as pd

# 导入数据集

dataset = pd.read_csv('partial_wine.csv')

X = dataset.iloc[:, [0, 1]].values

y = dataset.iloc[:, 2].values

# 将数据集拆分为训练集和测试集

from sklearn.model_selection import train_test_split

X_train, X_test, y_train, y_test = train_test_split(X, y, test_size = 0.25, random_state = 0)

# 特征缩放

from sklearn.preprocessing import StandardScaler

sc = StandardScaler()

X_train = sc.fit_transform(X_train)

X_test = sc.transform(X_test)

# ====> 在此处插入您的分类器代码 <====

from sklearn.tree import DecisionTreeClassifier

classifier = DecisionTreeClassifier(criterion='entropy',rand om_state=0)

classifier.fit(X_train, y_train)

# ====> 在此处插入您的分类器代码 <====

# 预测测试集结果

y_pred = classifier.predict(X_test)

# 生成混淆矩阵

from sklearn.metrics import confusion_matrix

cm = confusion_matrix(y_test, y_pred)

print("confusion matrix:")

print(cm)

列表 3.4 包含一些导入语句，然后使用 CSV 文件 partial_wine.csv 的内容填充 Pandas 数据帧 dataset。接下来，变量 X 被初始化为 dataset 的前两列（以及所有行），变量 y 被初始化为 dataset 的第三列（以及所有行）。

接下来，使用 75/25 的比例将 X 和 y 的数据填充到变量 X_train、X_test、y_train 和 y_test 中。注意，变量 sc（StandardScaler 类的实例）对 X_train 和 X_test 变量执行缩放操作。

在列表 3.4 中用粗体显示的代码块是我们创建 DecisionTreeClassifier 类的实例，然后使用变量 X_train 和 X_test 中的数据训练该实例。

列表 3.4 的下一部分将变量 y_pred 填充为从 X_test 变量中的数据生成的预测集。列表 3.4 的最后一部分基于 y_test 中的数据和 y_pred 中的预测数据创建一个混淆矩阵。

记住，混淆矩阵的所有对角线元素都是正确预测（例如真正例和真负例）；所有其他单元格包含一个数值，指定了错误预测的数量（例如假正例和假负例）。

现在运行列表 3.4 中的代码，你将看到以下混淆矩阵的输出，其中包含 36 个正确预测和 9 个错误预测（准确率为 80%）：

混淆矩阵：

[[13 1 2]

[ 0 17 4]

[1 1 6]]

from sklearn.metrics import confusion_matrix

在前面的 3x3 矩阵中总共有 45 个条目，对角线条目是正确识别的标签。因此，准确率为 36/45 = 0.80。

什么是随机森林？

随机森林是决策树的推广：这个分类算法涉及多个树（数量由你指定）。如果数据涉及进行数值预测，则计算树的预测平均值。如果数据涉及进行分类预测，则确定树的预测众数。

通过类比，随机森林以类似于金融投资组合多元化的方式运行：目标是平衡损失与更高的收益。随机森林使用“多数投票”来做出预测，这基于这样的假设，即选择多数投票比任何单个树的预测更有可能正确（并且更频繁）。

你可以轻松修改列表 3.4 中的代码以使用随机森林，只需将显示的粗体两行代码替换为以下代码：

from sklearn.ensemble import RandomForestClassifier

classifier = RandomForestClassifier(n_estimators = 10, criterion='entropy', random_state = 0)

进行此代码更改，运行代码，并检查混淆矩阵以比较其准确率与列表 3.4 中决策树的准确率。

什么是 SVMs？

支持向量机涉及监督机器学习算法，可用于分类或回归问题。SVMs 可以处理非线性可分数据以及线性可分数据。SVMs 使用一种称为“核技巧”的技术来转换数据，然后找到最优边界。这种转换涉及更高的维度。这种技术导致转换后的数据分离，之后可以找到一个超平面将数据分为两类。

SVM 在分类任务中比回归任务更常见。SVM 的一些用例包括以下：

+   文本分类任务：类别分配

+   检测垃圾邮件/情感分析

+   用于图像识别：基于方面的识别、基于颜色的分类

+   手写数字识别（邮政自动化）

SVM 的权衡

尽管 SVM 非常强大，但其中涉及权衡。SVM 的一些优点如下：

+   高准确度

+   在较小的更干净的数据集上表现良好

+   可以更高效，因为它使用训练点的子集

+   在数据集有限的情况下是 CNN 的替代品

+   捕获数据点之间更复杂的关系

尽管 SVM 很强大，但也有一些缺点，如下所示：

+   不适合大型数据集：训练时间可能很高

+   在噪声数据集和重叠类上效果较差

SVM 涉及比决策树和随机森林更多的参数

一个可以考虑的建议是修改列表 3.4，使用 SVM，通过将以下加粗的两行替换为以下加粗的两行：

from sklearn.svm import SVC

classifier = SVC(kernel = 'linear', random_state = 0)

您现在有一个基于 SVM 的模型，只需通过更新之前的代码即可。修改代码，然后运行代码并检查混淆矩阵，以比较其准确性与本章前面提到的决策树模型和随机森林模型的准确性。

什么是贝叶斯推断？

贝叶斯推断是统计学中的一个重要技术，它涉及统计推断和贝叶斯定理，随着更多信息的出现来更新假设的概率。贝叶斯推断通常被称为“贝叶斯概率”，它在序列数据的动态分析中非常重要。

贝叶斯定理

给定两个集合 A 和 B，让我们定义以下数值（它们都在 0 和 1 之间）：

P(A) = 在集合 A 中存在的概率

P(B) = 在集合 B 中存在的概率

P(Both) = 在 A 和 B 中存在的概率

P(A|B) = 在 B 中存在的概率（假设你在 B 中）

P(B|A) = 在 A 中存在的概率（假设你在 A 中）

然后，以下公式也是正确的：

P(A|B) = P(Both)/P(B) (#1)

P(B|A) = P(Both)/P(A) (#2)

将前面的一对等式乘以分母中出现的项，我们得到以下等式：

P(B)*P(A|B) = P(Both) (#3)

P(A)*P(B|A) = P(Both) (#4)

现在将等式#3 和#4 的左侧设置为相等，这样就得到了以下等式：

P(B)*P(A|B) = P(A)*P(B|A) (#5)

将等式#5 的两边除以 P(B)，我们得到这个著名的等式：

P(A|B) = P(A)*P(A|B)/P(B) (#6)

一些贝叶斯术语

在上一节中，我们推导了以下关系：

P(h|d) = (P(d|h) * P(h)) / P(d)

前面的等式中的四个项都有名称，如下所述。

首先，后验概率是 P(h|d)，这是在数据 d 给定的情况下假设 h 的概率。

第二，P(d|h) 是在假设 h 为真的条件下数据 d 的概率。

第三，h 的先验概率是 P(h)，这是假设 h 为真的概率（无论数据如何）。

最后，P(d) 是数据的概率（无论假设如何）

我们对从先验概率 p(h) 通过 P(D) 和 P(d|h) 计算后验概率 P(h|d) 感兴趣。

什么是 MAP？

最大后验假设（MAP）是概率最高的假设，即最可能的假设。这可以表示如下：

MAP(h) = max(P(h|d))

或者：

MAP(h) = max((P(d|h) * P(h)) / P(d))

或者：

MAP(h) = max(P(d|h) * P(h))

为什么使用贝叶斯定理？

贝叶斯定理描述了基于与事件可能相关条件先验知识的事件概率。如果我们知道条件概率，我们可以使用贝叶斯规则来找出反向概率。前面的陈述是贝叶斯规则的一般表示。

什么是贝叶斯分类器？

朴素贝叶斯分类器是一种受贝叶斯定理启发的概率分类器。NB 分类器假设属性是条件独立的，即使假设不成立，它也能很好地工作。这个假设大大降低了计算成本，并且它是一个简单的算法，只需要线性时间。此外，NB 分类器可以轻松扩展到更大的数据集，并且在大多数情况下都能获得良好的结果。NB 分类器的其他优点包括以下内容：

+   可以用于二进制和多类分类

+   提供不同类型的 NB 算法

+   是文本分类问题的良好选择

+   是垃圾邮件分类的一个流行选择

+   可以轻松地在小型数据集上训练

如您所料，NB 分类器确实有一些缺点，如下所示：

+   假设所有特征都是无关的。

+   它无法学习特征之间的关系。

+   它可能会遭受“零概率问题”。

零概率问题指的是当属性的条件下概率为零时的情况，它无法给出有效的预测。然而，可以使用拉普拉斯估计器明确地修复。

基于朴素贝叶斯分类器的类型

有三种主要的 NB 分类器：

+   高斯朴素贝叶斯

+   多项式朴素贝叶斯（多项式 NB）

+   伯努利朴素贝叶斯

这些分类器的详细信息超出了本章的范围，但您可以通过在线搜索获取更多信息。

训练分类器

常见的训练分类器的技术如下：

+   保留法

+   k 折交叉验证

保留法是最常见的方法，它首先将数据集分为两个部分，称为训练集和测试集（分别为 80% 和 20%）。训练集用于训练模型，测试数据用于测试其预测能力。

k 折交叉验证技术用于验证模型没有过拟合。数据集被随机划分为 k 个互斥的子集，其中每个子集的大小相等。一个子集用于测试，其他子集用于训练。在整个 k 个折中迭代。

评估分类器

每次为数据集选择分类器时，显然重要的是评估该分类器的准确性。以下列出了一些评估分类器的常见技术：

+   精确度和召回率

+   ROC 曲线（接收者操作特征）

精确度和召回率在第二章中讨论，并在此处重现以供方便。让我们定义以下变量：

TP = 真阳性结果的数量

FP = 错误阳性结果的数量

TN = 真阴性结果的数量

FN = 错误阴性结果的数量

然后给出了精确度、准确度和召回率的定义，如下公式所示：

精确度 = TP / (TN + FP)

准确度 = (TP + TN) / [TP + FP + FN + TN]

召回率 = TP / [TP + FN]

ROC 曲线用于对分类模型进行可视化比较，显示了真正阳性率和错误阳性率之间的权衡。ROC 曲线下的面积是模型准确性的度量。当模型接近对角线时，其准确性较低，完美准确的模型将有一个面积为 1.0。

ROC 曲线绘制了真正阳性率与错误阳性率的关系。另一种类型的曲线是 PR 曲线，它绘制了精确度与召回率的关系。当处理高度倾斜的数据集（强类别不平衡）时，精确度-召回率（PR）曲线给出更好的结果。

这部分章节关于统计术语和测量数据集有效性的技术就到这里结束。现在让我们来看看机器学习中的激活函数，这是下一节的主题。

什么是激活函数？

激活函数（通常）是一个非线性函数，它将非线性引入神经网络中，从而防止神经网络中隐藏层的“巩固”。具体来说，假设神经网络中每对相邻层仅涉及矩阵变换而没有激活函数。这样的网络是一个线性系统，这意味着其层可以被合并成一个更小的系统。

首先，连接输入层和第一隐藏层的边的权重可以用一个矩阵表示：让我们称它为 W1。接下来，连接第一隐藏层和第二隐藏层的边的权重也可以用一个矩阵表示：让我们称它为 W2。重复此过程，直到我们达到连接最终隐藏层和输出层的边：让我们称这个矩阵为 Wk。由于我们没有激活函数，我们可以简单地乘以矩阵 W1、W2、…、Wk，并产生一个矩阵：让我们称它为 W。现在，我们已经用包含一个输入层、一个权重矩阵 W 和一个输出层的等效神经网络替换了原始神经网络。换句话说，我们不再有原来的多层神经网络了！

幸运的是，当我们指定每对相邻层之间的激活函数时，我们可以防止上述情况发生。换句话说，每层的激活函数防止了这种“矩阵合并”。因此，我们可以在训练神经网络的整个过程中保持所有中间隐藏层。

为了简单起见，让我们假设每对相邻层之间都有相同的激活函数（我们很快就会去掉这个假设）。在神经网络中使用激活函数的过程涉及几个步骤，如下所述：

1. 从一个数字输入向量 x1 开始。

2. 将 x1 乘以权重矩阵 W1，该矩阵表示连接输入层和第一隐藏层的边。结果是新的向量 x2。

3. “应用”激活函数到 x2 的每个元素，以创建另一个向量 x3。

现在重复步骤 2 和 3，但这次我们使用“起始”向量 x3 和权重矩阵 W2 来表示连接第一隐藏层和第二隐藏层（如果只有一个隐藏层，则为输出层）的边。

完成前面的过程后，我们“保留”了神经网络，这意味着它可以在数据集上训练。你不必在每一步都使用相同的激活函数，你可以用不同的激活函数来替换每个激活函数（选择权在你）。

我们为什么需要激活函数？

前一节概述了将输入向量从输入层通过隐藏层直到达到输出层的过程。神经网络中激活函数的作用至关重要，因此在这里重复一遍：激活函数“维持”神经网络的结构，防止它们被简化为输入层和输出层。换句话说，如果我们指定每对连续层之间的非线性激活函数，那么神经网络就不能被替换为包含较少层的神经网络。

没有非线性激活函数，我们只是将给定连续层的权重矩阵与从前一连续层产生的输出向量相乘。我们重复这个简单的乘法，直到达到神经网络的输出层。达到输出层后，我们实际上用单个“连接”输入层和输出层的矩阵替换了多个矩阵。

激活函数是如何工作的？

如果你第一次遇到激活函数的概念，可能会感到困惑，所以这里有一个可能有帮助的类比。假设你在深夜开车，高速公路上没有其他人。在没有障碍物（如停车标志和交通灯）的情况下，你可以以恒定的速度行驶。然而，假设你开进了一个大型杂货店的停车场。当你接近减速带时，你必须减速，通过减速带，然后再次加速，并重复这个过程，直到每个减速带。

将神经网络中的非线性激活函数想象成减速带的对立面：你无法保持恒定的速度，这（通过类比）意味着你不能首先将所有权重矩阵相乘并将它们“折叠”成一个单一的权重矩阵。另一个类比涉及一个有多个收费站的道路：你必须减速，支付通行费，然后继续驾驶，直到到达下一个收费站。这些只是不完美的类比，帮助你理解非线性激活函数的需求。

常见激活函数

尽管存在许多激活函数（如果你知道如何定义，你也可以定义自己的），以下是一些常见的激活函数列表，后面跟着简要描述：

+   sigmoid

+   tanh

+   ReLU

+   ReLU6

+   ELU

+   SELU

sigmoid 激活函数基于欧拉常数 e，其值域在 0 和 1 之间，其公式如下：

1/[1+e^(-x)]

tanh 激活函数也是基于欧拉常数 e，其公式如下：

[e^x – e^(-x)]/[e^x+e^(-x)]

记忆前面公式的 一种方法是注意分子和分母有相同的成对项：它们在分子中由“-”符号分隔，在分母中由“+”符号分隔。tanh 函数的值域在 -1 和 1 之间。

ReLU（修正线性单元）激活函数非常直接：如果 x 是负数，那么 ReLU(x) 是 0；对于 x 的所有其他值，ReLU(x) 等于 x。ReLU6 是 TensorFlow 特有的，它是 ReLU(x) 的一个变体：额外的约束是当 x >= 6 时，ReLU(x) 等于 6（因此得名）。

ELU 是指数线性单元，它是 ReLU 的指数“外壳”，用对所有 x 值（包括 x = 0）可微分的指数激活函数替换了 ReLU 的两个线性段。

SELU 是缩写，代表缩放指数线性单元，它比其他激活函数稍微复杂一些（并且使用频率较低）。要详细了解这些以及其他激活函数（以及描述它们形状的图表），请访问以下维基百科网页：

[激活函数](https://en.wikipedia.org/wiki/Activation_function)

前面的链接提供了一个包含激活函数及其导数的长列表。

Python 中的激活函数

列表 3.5 显示了包含各种激活函数公式的文件 activations.py 的内容。

列表 3.5：activations.py

导入 numpy 库：`import numpy as np`

# Python 中的 sigmoid 示例：

z = 1/(1 + np.exp(-np.dot(W, x)))

# Python 中的 tanh 示例：

z = np.tanh(np.dot(W,x))

# Python 中的 ReLU 示例：

z = np.maximum(0, np.dot(W, x))

列表 3.5 包含使用 NumPy 方法定义 sigmoid 函数、tanh 函数和 ReLU 函数的 Python 代码。请注意，你需要指定 x 和 W 的值来运行列表 3.5 中的代码。

RELU 和 ELU 激活函数

目前 ReLU 通常是“首选”的激活函数；之前，首选的激活函数是 tanh（在 tanh 之前是 sigmoid）。ReLU 由两条线段组成（一条斜率为零，另一条斜率为 1），在二维欧几里得平面的原点相交，并提供最佳的训练准确率和验证准确率。

ReLU 就像线性性的开关：不需要时它是“关闭”的，当它激活时，其导数为 1，这使得 ReLU 成为所有当前激活函数中最简单的。请注意，函数的二阶导数在所有地方都是 0：它是一个非常简单的函数，简化了优化。此外，梯度对于大值是恒定的，它永远不会“饱和”（即，它不会在正水平轴上缩小到零）。

矩形线性单元及其推广版本基于线性模型更容易优化的原则。ReLU 激活函数或其相关替代方案（稍后讨论）在许多情况下是推荐的激活函数。

ReLU 的优缺点

以下列表包含了 ReLU 激活函数的优点：

+   在正区域不会饱和

+   在计算效率方面非常高效

+   使用 ReLU 的模型通常比使用其他激活函数的模型收敛得更快

然而，ReLU 确实存在一个缺点，那就是当 ReLU 神经元的激活值为 0 时：在反向传播过程中，该神经元的梯度也将为 0。你可以通过明智地分配初始权重和学习率来减轻这种情况。

ELU

指数线性单元（ELU）基于 ReLU：主要区别在于 ELU 在原点处是可微的（ReLU 是一个连续函数，但在原点处不可微）。然而，请注意以下几点。首先，ELUs 以“不朽”（对“死亡”的免疫力）为代价换取计算效率。阅读以下论文以获取更多详细信息：[arxiv.org/abs/1511.07289](http://arxiv.org/abs/1511.07289)。其次，ReLU 仍然很受欢迎，并且比 ELU 更受欢迎，因为 ELU 的使用引入了一个额外的新的超参数。

SIGMOID、SOFTMAX 和 HARDMAX 的相似性

Sigmoid 激活函数的范围在(0,1)之间，它会饱和并“杀死”梯度。与 tanh 激活函数不同，sigmoid 的输出不是零中心的。此外，sigmoid 和 softmax 在 vanilla 前馈实现中都不被鼓励使用。然而，sigmoid 激活函数仍然用于 LSTMs（特别是遗忘门、输入门和输出门）、GRUs（门控循环单元）和概率模型。此外，一些自动编码器有额外的要求，这阻止了分段线性激活函数的使用。

Softmax

Softmax 激活函数将数据集中的值映射到另一组介于 0 和 1 之间的值，且这些值的总和等于 1。因此，softmax 创建了一个概率分布。在卷积神经网络（CNNs）进行图像分类的情况下，softmax 激活函数“映射”了最终隐藏层中的值到输出层的 10 个神经元。包含最大概率的位置索引与输入图像的一热编码中数字 1 的索引相匹配。如果索引值相等，则表示图像已被分类，否则被认为是错配。

Softplus

Softplus 激活函数是 ReLU 激活函数的平滑（即可微）近似。回想一下，ReLU 函数的唯一不可微点是原点，它通过 softmax 激活函数被“平滑”，其方程如下：

f(x) = ln(1 + e^x)

Tanh

Tanh 激活函数的范围在(-1,1)之间，而 sigmoid 函数的范围在(0,1)之间。这两个激活函数都会饱和，但与 sigmoid 神经元不同，tanh 的输出是零中心的。因此，在实践中，tanh 非线性总是比 sigmoid 非线性更受欢迎。

Sigmoid 和 tanh 激活函数出现在 LSTMs（sigmoid 用于三个门，tanh 用于内部细胞状态）以及 GRUs（门控循环单元）在涉及输入门、遗忘门和输出门的计算中。

SIGMOID、SOFTMAX 和 HARDMAX 的区别

本节简要讨论了这三个函数之间的一些差异。首先，sigmoid 函数在逻辑回归模型中用于二元分类，以及在 LSTMs 和 GRUs 中的门控。在构建神经网络时，sigmoid 函数用作激活函数，但请注意，概率之和不一定等于 1。

其次，softmax 函数是对 sigmoid 函数的推广：它用于逻辑回归模型中的多分类。softmax 函数是 CNN 中“全连接层”的激活函数，这是最右侧的隐藏层和输出层。与 sigmoid 函数不同，概率之和必须等于 1。对于二元（n=2）分类，你可以使用 sigmoid 函数或 softmax 函数。

第三，hardmax 函数将 0 或 1 分配给输出值（类似于阶跃函数）。例如，假设我们有三个类别{c1, c2, c3}，其分数分别为[1, 7, 2]。hardmax 概率为[0, 1, 0]，而 softmax 概率为[0.1, 0.7, 0.2]。请注意，hardmax 概率之和为 1，softmax 概率之和也是如此。然而，hardmax 概率是全有或全无的，而 softmax 概率类似于获得“部分分数”。

逻辑回归是什么？

尽管名为逻辑回归，但它是一种具有二元输出的分类器和线性模型。逻辑回归与多个自变量一起工作，并涉及 sigmoid 函数来计算概率。逻辑回归本质上是将 sigmoid 激活函数应用于线性回归以执行二元分类的结果。

逻辑回归在许多无关的领域中都有用。这些领域包括机器学习、各种医学领域和社会科学。逻辑回归可以根据患者的各种观察特征来预测患某种疾病的风险。使用逻辑回归的其他领域包括工程、营销和经济学。

逻辑回归可以是二项式（因变量的结果只有两种），多项式（因变量的结果有三个或更多），或有序的（因变量是有序的）。例如，假设一个数据集包含属于类别 A 或类别 B 的数据。如果你得到一个新的数据点，逻辑回归会预测该新数据点属于类别 A 还是类别 B。相比之下，线性回归预测一个数值，例如股票的次日价值。

设置阈值值

阈值是一个数值，用于确定哪些数据点属于类别 A，哪些点属于类别 B。例如，及格/不及格的阈值可能是 0.70。在加利福尼亚州通过书面驾驶员考试及格的阈值是 0.85。

作为另一个例子，假设 p = 0.5 是“截止”概率。那么我们可以将概率大于 0.5 的数据点分配给类别 A，将概率小于等于 0.5 的数据点分配给类别 B。由于只有两个类别，我们确实有一个分类器。

类似的场景涉及抛掷一个平衡良好的硬币。我们知道抛出正面的概率是 50%（让我们将这个结果标记为“类别 A”），抛出反面的概率也是 50%（让我们将这个结果标记为“类别 B”）。如果我们有一个包含标记结果的数据库，那么我们期望大约 50%的结果是类别 A 和类别 B。

然而，我们无法提前确定有多少比例的人会通过书面驾驶考试，或者有多少人将通过他们的课程。包含这些类型场景结果的数据库需要训练，逻辑回归可以是一个适合进行此操作的技术。

逻辑回归：重要假设

逻辑回归要求观测值彼此独立。此外，逻辑回归要求独立变量之间几乎没有多重共线性。逻辑回归处理数值、分类和连续变量，并假设独立变量和 log odds 的线性关系，这在此处定义：

odds = p/(1-p) 和 logit = log(odds)

这种分析不需要因变量和自变量之间存在线性关系；然而，另一个要求是独立变量与 log odds 线性相关。

逻辑回归用于在存在多个解释变量的情况下获得 odds ratio。该过程与多元线性回归非常相似，只是响应变量是二项式的。结果是每个变量对观察到的感兴趣事件的 odds ratio 的影响。

线性可分数据

线性可分数据是指可以通过一条线（在二维中）、一个平面（在三维中）或超平面（在更高维度中）进行分离的数据。线性不可分数据是指无法通过线或超平面进行分离的数据（例如聚类）。例如，XOR 函数涉及无法通过线进行分离的数据点。如果你为具有两个输入的 XOR 函数创建一个真值表，那么点（0,0）和（1,1）属于类别 0，而点（0,1）和（1,0）属于类别 1（在二维平面上绘制这些点以说服自己）。解决方案涉及在更高维度中转换数据，使其成为线性可分，这是 SVMs 中使用的技巧。

摘要

本章从分类和分类器的解释开始，然后简要介绍了机器学习中常用的分类器。

然后我们讨论了激活函数，如果你决定学习深度神经网络，这将非常有用。你还收到了关于激活函数的高级介绍，包括 sigmoid、tanh、ReLU、ReLU6、ELU 和 SELU。

接下来，你学习了逻辑回归，它依赖于 sigmoid 函数，以及逻辑回归的潜在假设。最后，你看到了一个涉及逻辑回归和 MNIST 数据集的代码示例。

第四章

CHATGPT AND GPT-4

本章包含有关 ChatGPT 和 GPT-4 的主要特性以及它们的一些竞争对手的信息。

本章的第一部分从 ChatGPT 关于生成式 AI 和对话式 AI 与生成式 AI 本质的信息开始。根据 ChatGPT 的说法，ChatGPT 本身、GPT-4 和 DALL-E 确实包含在生成式 AI 中。本节还讨论了 ChatGPT 的一些特性，以及 ChatGPT 的替代品。

本章的第三部分讨论了 GPT-4 的一些特性，这些特性为 ChatGPT 提供了动力。你将了解 GPT-4 的一些竞争对手，例如 Llama 2（Meta）和 Bard（更名为 Google Gemini）。

什么是生成式 AI？

生成式 AI 是指人工智能模型和技术的子集，旨在生成与给定输入数据在本质上相似的新数据样本。目标是生成原本不属于原始训练集的内容或数据，但内容连贯、上下文相关，并且具有相同的风格或结构。

生成式 AI 的独特之处在于其创造和创新的能力，而不是仅仅分析或分类。该领域的进步导致了创意领域和实际应用的突破，使其成为人工智能研究和开发的前沿领域。

生成式 AI 的重要特性

以下列表包含生成式 AI 的关键特性，每个条目后面都有简要描述：

+   数据生成

+   综合合成

+   学习分布

数据生成指的是创建新的数据点的能力，这些数据点不是训练数据的一部分，但与它们相似。这可能包括文本、图像、音乐、视频或任何其他形式的数据。

综合意味着生成模型可以混合各种输入以生成包含每个输入特征的输出，例如合并两张图片的风格。

学习分布意味着生成式 AI 模型旨在学习训练数据的概率分布，以便它们可以从该分布中生成新的样本。

生成式 AI 中的流行技术

生成对抗网络（GANs）：GANs 由两个网络组成，一个生成器和一个判别器，它们同时训练。生成器试图生成假数据，而判别器试图区分真实数据和假数据。随着时间的推移，生成器在生成逼真数据方面变得越来越好。

变分自编码器（VAEs）：VAEs 是概率模型，它们学习以编码和解码数据的方式，使得编码表示可以用来生成新的数据样本。

循环神经网络（RNNs）：主要用于序列生成，如文本或音乐。

生成式 AI 的独特之处

创作与分类：虽然大多数传统 AI 模型旨在将输入数据分类到预定义的类别中，但生成模型旨在创建新的数据。

无监督学习：许多生成模型，尤其是 GANs 和 VAEs，以无监督的方式运行，这意味着它们在训练时不需要标记数据。

多样化的输出：生成模型可以根据学习到的分布产生各种各样的输出，这使得它们非常适合艺术生成、风格迁移等任务。

挑战：生成式 AI 带来了独特的挑战，例如 GANs 中的模式坍塌或确保生成内容的连贯性。

有许多涉及生成式 AI 应用的领域，其中一些如下列出：

+   艺术和音乐创作

+   数据增强

+   风格迁移

+   文本生成

+   图像合成

+   药物发现

艺术和音乐创作包括生成画作、音乐或其他形式的艺术。

数据增强涉及为训练模型创建额外的数据，尤其是在原始数据集有限的情况下。

风格迁移是指将一个图像的风格应用到另一个图像的内容上。

文本生成是生成式 AI 的一个非常流行的应用，它涉及创建连贯且与上下文相关的文本。

图像合成是生成式 AI 的另一个流行领域，它涉及生成逼真的图像、面部，甚至为视频游戏创建场景。

药物发现是生成式 AI 的一个重要方面，涉及为新潜在药物生成分子结构。

对话式 AI 与生成式 AI

对话式 AI 和生成式 AI 都是人工智能更广泛领域中的突出子领域。然而，这两个子领域在主要目标、使用的技术和应用程序方面有不同的重点。

[`medium.com/@social_65128/differences-between-conversational-ai-and-generative-ai-e3adca2a8e9a`](https://medium.com/@social_65128/differences-between-conversational-ai-and-generative-ai-e3adca2a8e9a)

两个子领域的主要差异如下：

+   主要目标

+   应用

+   使用的技术

+   训练与交互

+   评估

+   数据需求

主要目标

对话式 AI 的主要目标是促进机器与人类之间类似人类的交互。这包括聊天机器人、虚拟助手以及其他与用户进行对话的系统。

生成式 AI 的主要目标是创建新的内容或数据，这些内容或数据不在训练集中，但在结构和风格上相似。这可以从生成图像、音乐和文本到更复杂的任务，如视频合成。

应用

对话式 AI 的常见应用包括客户支持聊天机器人、语音操作虚拟助手（如 Siri 或 Alexa）以及交互式语音响应 (IVR) 系统。

生成式 AI 的常见应用包括创作艺术或音乐、生成逼真的视频游戏环境、合成声音以及生成逼真的图像甚至深度伪造。

使用的技术

对话式 AI 通常依赖于自然语言处理 (NLP) 技术来理解和生成人类语言。这包括意图识别、实体提取和对话管理。

生成式 AI 通常使用生成对抗网络 (GANs)、变分自编码器 (VAEs) 和其他生成模型来生成新内容。

训练与交互

虽然训练可以是监督的、半监督的或无监督的，但对话式 AI 的主要交互模式是通过来回对话或交谈。

生成式 AI 的训练过程，特别是对于 GANs 等模型，涉及迭代过程，其中模型通过试图欺骗判别器相信生成数据是真实的来学习生成数据。

评估

对话式 AI 的评估指标通常围绕理解与响应准确性、用户满意度以及生成响应的流畅性展开。

对于像 GANs 这样的生成式 AI 模型的评估指标可能具有挑战性，可能需要结合使用定量指标和人类判断来评估生成内容的品质。

数据需求

对话式 AI 的数据需求通常涉及对话数据，包括人与人之间的对话或人与机器人之间的对话。

生成式 AI 的数据需求涉及大量它应该生成的内容的数据集，如图像、文本和音乐。

尽管对话式 AI 和生成式 AI 都涉及生成输出，但它们的主要目标、应用和方法可能存在显著差异。对话式 AI 用于与用户的交互式通信，而生成式 AI 则专注于生成新的、原创的内容。

IS DALL-E PART OF GENERATIVE AI?

DALL-E 和类似工具，它们可以从文本生成图形，是生成式 AI 的例子。事实上，DALL-E 是图像合成领域最突出的生成式 AI 例子之一。

以下是 DALL-E 的生成特性列表，随后是每个项目的简要描述：

+   图像生成

+   学习分布

+   创新组合

+   广泛应用

+   Transformer 架构

图像生成是 DALL-E 的一个关键特性，它被设计成根据文本描述生成图像。给定一个提示，如“一个双头火烈鸟”，DALL-E 可以生成一个符合描述的新颖图像，即使它在训练数据中从未见过这样的图像。

学习分布：与其他生成模型一样，DALL-E 学习其训练数据的概率分布。当它生成图像时，它会从这个学习到的分布中采样，以产生基于其训练数据的合理视觉。

创新组合：DALL-E 可以生成代表全新或抽象概念的图像，展示了其能够以创新方式组合和重新组合学习元素的能力。

除了图像合成之外，DALL-E 还在艺术生成、风格融合以及创建具有特定属性或主题的图像等领域提供了广泛的应用支持，突显了其作为生成工具的多样性。

DALL-E 利用与 GPT-3 等模型类似的转换器架构变体，但针对图像生成任务进行了调整。

其他基于输入数据（无论是文本、另一张图像还是任何其他形式的数据）生成图形、艺术或任何形式视觉内容的工具，并且可以产生其训练数据中未明确呈现的输出，也被认为是生成式 AI。它们展示了 AI 模型不仅能够分析和分类，还能够创造和创新。

ChatGPT 和 GPT-4 是否属于生成式 AI？

ChatGPT 和 GPT-4 都被认为是生成式 AI 的例子，它们是被称为“转换器”的模型类别的一部分，这些模型特别擅长处理数据序列，例如与文本相关的任务。

以下列表提供了各种原因，说明为什么这些大型语言模型被认为是生成式的，随后对每个项目进行了简要描述：

+   文本生成

+   学习分布

+   广泛应用

+   无监督学习

文本生成：这些模型可以根据给定的提示生成连贯、上下文相关且通常非常复杂的文本序列。它们生成的响应在它们的训练数据中并未明确呈现，但基于它们在训练期间学习的模式和结构构建。

学习分布：GPT-3、GPT-4 以及类似模型学习其训练数据的概率分布。在生成文本时，它们实际上是从这个学习到的分布中进行采样，以产生基于其训练数据的可能序列。

广泛应用：除了基于文本的聊天或对话之外，这些模型还可以用于各种生成任务，如故事写作、代码生成、诗歌，甚至创建特定风格或模仿某些作者的内容，展示了它们的生成能力。

无监督学习：虽然它们可以使用特定数据集进行微调，但像 GPT-3 这样的模型主要是以无监督方式在大量文本上进行训练，学习生成内容，而不需要为每个可能的响应提供显式的标记数据。

OpenAI 的 ChatGPT-3、GPT-4 以及类似模型是自然语言处理和生成领域中生成式人工智能的典范。

下几节简要介绍一些在人工智能领域具有强大影响力的公司。

DEEPMIND

DeepMind 在人工智能领域做出了重大贡献，包括创建了各种人工智能系统。DeepMind 成立于 2010 年，并于 2014 年成为谷歌的子公司。其主页位于 [`deepmind.com/`](https://deepmind.com/)。

DeepMind 创建了 280 GB 的语言模型 Gopher，其性能显著优于其竞争对手，包括 GPT-3、J1-Jumbo 和 MT-NLG。DeepMind 还开发了 AlphaFold，它解决了研究人员十年未能解决的蛋白质折叠任务。DeepMind 于 2021 年 7 月将 AlphaFold 免费提供给每个人。DeepMind 在世界级人工智能游戏系统的发展中做出了重大贡献，其中一些将在下一节中讨论。

DeepMind 和游戏

DeepMind 是 AlphaStar 和 AlphaGo 人工智能系统的幕后力量，这些系统击败了围棋（比国际象棋难得多）的最佳人类玩家。这些游戏提供了“完美信息”，而具有“不完美信息”（如扑克）的游戏对机器学习模型构成了挑战。

AlphaGo Zero（AlphaGo 的继任者）通过自我对弈在更短的时间内和更少的计算能力下掌握了游戏。AlphaGo Zero 通过以 100-0 的成绩击败 AlphaGo 展现了非凡的性能。另一个强大的系统是 AlphaZero，它使用自我对弈学习技术来玩围棋、国际象棋和将棋，并实现了 SOTA（最先进技术）性能结果。

相比之下，使用树搜索的机器学习模型非常适合具有完美信息的游戏。相比之下，具有不完美信息（如扑克）的游戏涉及隐藏信息，可以利用这些信息制定反策略来对抗对手的策略。AlphaStar 能够与星际争霸 II 的最佳玩家对战，并成为第一个在需要“在信息不完整的世界中的战略能力”的游戏中实现 SOTA（最先进技术）成果的人工智能。

游戏玩家（PoG）

谷歌的 DeepMind 团队设计了基于以下技术的通用 PoG（游戏玩家）算法：

+   CFR（反事实后悔最小化）

+   CVPN（反事实价值与策略网络）

+   GT-CFT（增长树 CFR）

+   CVPN

反事实价值与策略网络（CVPN）是一个神经网络，它计算游戏中每个状态信念的反事实。这在评估任何给定时间点的游戏的不同变体时至关重要。

Growing tree CFR (GT-CFR) 是一种针对随时间增长的博弈树优化的 CFR 变体。GT-CFR 基于两个基本阶段，更多详细信息可在网上找到：

[`medium.com/syncedreview/deepminds-pog-excels-in-perfect-and-imperfect-information-games-advancing-research-on-general-9dbad5c04221`](https://medium.com/syncedreview/deepminds-pog-excels-in-perfect-and-imperfect-information-games-advancing-research-on-general-9dbad5c04221)

OPENAI

OpenAI 是一家对 AI 做出重大贡献的人工智能研究公司，包括 DALL-E 和 ChatGPT，其主页在这里：[`openai.com/api/`](https://openai.com/api/)。

OpenAI 由埃隆·马斯克和山姆·奥特曼（以及其他一些人）在旧金山创立，其声明的目标之一是开发对人类有益的 AI。鉴于微软对该组织的大量投资和深度联盟，OpenAI 可能被视为微软的一部分。OpenAI 是 GPT-x 系列大型语言模型（LLM）以及 ChatGPT 的创造者，ChatGPT 于 2022 年 11 月 30 日公开发布。

OpenAI 通过 API 以按字计费的方式将 GPT-3 商业化，用于各种应用。GPT-3 于 2020 年 7 月宣布，并通过测试计划提供。然后，在 2021 年 11 月，OpenAI 将 GPT-3 向所有人开放。更多详细信息可在网上找到：

[`openai.com/blog/api-no-waitlist/`](https://openai.com/blog/api-no-waitlist/)。

此外，OpenAI 开发了 DALL-E，它可以从文本生成图像。OpenAI 最初不允许用户上传包含真实人脸的图像。后来，在 2022 年第四季度，OpenAI 改变了其政策，允许用户将其人脸上传到其在线系统中。（请查看 OpenAI 网页以获取更多详细信息。）顺便提一下，扩散模型已经取代了 DALL-E 的基准。

OpenAI 还发布了一个公开测试版的 Embeddings，这是一种适合各种机器学习（ML）任务的格式，具体描述如下：

[`beta.openai.com/docs/guides/embeddings`](https://beta.openai.com/docs/guides/embeddings)

OpenAI 是 Codex 的创造者，Codex 提供了一组使用自然语言处理（NLP）训练的模型。Codex 的初始发布处于私有测试版，更多信息可在[`beta.openai.com/docs/engines/instruct-series-beta`](https://beta.openai.com/docs/engines/instruct-series-beta)找到。

OpenAI 提供了四种模型，统称为他们的指令模型，这些模型支持 GPT-3 生成自然语言的能力。这些模型将在 2024 年初被弃用，并替换为 GPT-3、ChatGPT 和 GPT-4 的更新版本。

如果你想了解更多关于 OpenAI 提供的功能和服务，请访问以下网页：[`platform.openai.com/overview`](https://platform.openai.com/overview)。

COHERE

Cohere 是一家初创公司，也是 OpenAI 的竞争对手，其主页在这里：[`cohere.ai/`](https://cohere.ai/)。

Cohere 开发的是商业上可用的尖端 NLP 技术，服务于多个行业。Cohere 专注于执行文本分析而不是文本生成模型（如基于 GPT 的模型）。Cohere 的创始团队令人印象深刻：CEO Aidan Gomez 是 transformer 架构的共同发明人之一，而 CTO Nick Frosst 是 Geoff Hinton 的弟子。

HUGGING FACE

Hugging Face 是一个流行的基于社区的开放源代码 NLP 技术仓库，其主页在[`github.com/huggingface`](https://github.com/huggingface)。

与 OpenAI 或 Cohere 不同，Hugging Face 不构建自己的 NLP 模型。相反，Hugging Face 是一个平台，管理着大量的开源 NLP 模型，客户可以对这些模型进行微调，然后部署这些微调后的模型。实际上，Hugging Face 已经成为人们协作开发 NLP 模型的重要场所，有时也被称为“机器学习和 NLP 的 GitHub。”

Hugging Face 库

Hugging Face 提供了三个重要的库：datasets、tokenizers 和 transformers。Accelerate 库支持 PyTorch 模型。datasets 库提供了各种 NLP 库。tokenizers 库使您能够将文本数据转换为数值。

可能最令人印象深刻的库是 transformers 库，它提供了一整套预训练的基于 BERT 的模型，可以执行各种 NLP 任务。GitHub 仓库在这里：[`github.com/huggingface/transformers`](https://github.com/huggingface/transformers)。

Hugging Face 模型中心

Hugging Face 提供了一个模型中心，提供大量可在线访问的模型。此外，该网站支持其模型的在线测试，包括以下任务：

+   使用 BERT 进行掩码词完成

+   使用 Electra 进行命名实体识别

+   使用 RoBERTa 进行自然语言推理

+   使用 DistilBERT 进行问答

+   使用 BART 进行摘要

+   使用 GPT-2 进行文本生成

+   使用 T5 进行翻译

导航到以下网页以查看“使用 transformer 进行写作”的文本生成能力：[`transformer.huggingface.co`](https://transformer.huggingface.co)。

在下一章中，您将看到 Python 代码示例，展示如何列出所有可用的 Hugging Face 数据集以及如何加载特定数据集。

AI21

AI21 是一家通过 API 提供专有大型语言模型的公司，以支持其客户的各项应用。AI21 当前的 SOTA 模型称为 Jurassic-1（与 GPT-3 大小大致相同），AI21 还在 Jurassic-1 和其他模型之上创建了其自己的应用。AI21 当前的应用套件包括增强阅读和写作的工具。

Primer 是这个领域的老对手，比 transformer 的发明早两年成立。该公司主要服务于政府和防务行业的客户。

INFLECTIONAI

在 AI 领域较新的公司是 InflectionAI，其令人印象深刻的创始团队包括：

+   Reid Hoffman（LinkedIn）

+   DeepMind 联合创始人 Mustafa Suleyman

+   DeepMind 研究员 Karen Simonyan

InflectionAI 致力于一项具有挑战性的任务：使人类能够以与人类相互沟通相同的方式与计算机交互。

ANTHROPIC

Anthropic 是由 OpenAI 的前员工于 2021 年创建的，其主页如下：[`www.anthropic.com/`](https://www.anthropic.com/)。

Anthropic 从包括 Google 和 Salesforce 在内的一系列公司获得了重要的财务支持。该公司发布了 Claude 2 作为 ChatGPT 的竞争对手。

Claude 2 能够总结多达 75,000 个单词的基于文本的内容，而 ChatGPT 目前限制在 3,000 个单词。此外，Claude 2 在部分律师资格考试中获得了 76.5% 的分数，在 Python 编码测试中获得了 71% 的分数。Claude 2 在向用户查询提供“干净”的回复方面也比 ChatGPT 有更高的比率。

这部分章节关于在人工智能领域做出重要贡献的 AI 公司的内容到此结束。下一节将提供一个关于大型语言模型（LLMs）的高级介绍。

什么是提示工程？

你已经了解了来自 OpenAI 的文本生成器，如 GPT-3 和 DALL-E 2，以及来自 AI21 的 Jurassic，以及 Midjourney 和 Stable Diffusion，它们可以执行文本到图像的生成。提示工程是指设计基于文本的提示，使基于 AI 的系统能够改进生成的输出，这意味着输出更接近用户从 AI 系统中想要产生的结果。通过类比，将提示视为类似教练的角色：他们提供建议和意见，以帮助人们在特定任务中表现更好。

由于提示是基于文字的，挑战在于学习不同的单词如何影响生成的输出。此外，预测系统对给定提示的反应是困难的。例如，如果你想生成一幅风景画，暗色调的风景和亮色调的风景之间的区别是直观的。然而，如果你想生成一幅美丽的风景，AI 系统将如何生成相应的图像？正如你可以推测的，对于从文本生成图像的 AI 系统来说，具体词汇比抽象或主观词汇更容易。仅为了增加更多内容到之前的例子，你将如何可视化以下内容？

+   一幅美丽的风景

+   一首美丽的歌曲

+   一部美丽的电影

尽管提示工程始于文本到图像的生成，但还有其他类型的提示工程，例如基于音频的提示，它解释了在语音中检测到的强调文本和情绪，以及基于草图生成图像的提示。最近关注的焦点是用于生成视频的基于文本的提示，这为艺术家和设计师提供了令人兴奋的机会。以下网页提供了一个图像到图像处理的示例：

[`huggingface.co/spaces/fffiloni/stable-diffusion-color-sketch`](https://huggingface.co/spaces/fffiloni/stable-diffusion-color-sketch)

提示和完成

提示是用户提供给 LLMs 的文本字符串，而完成是用户从 LLMs 收到的文本。提示帮助 LLMs 完成请求（任务），并且它们的长度可以不同。尽管提示可以是任何文本字符串，包括随机字符串，但提示的质量和结构会影响完成的质量。

将提示视为向 LLMs 提供“指导”的机制，或者甚至将其视为“教练”LLMs 以提供所需答案的方式。提示中的标记数加上完成中的标记数最多为 2,048 个标记。

提示类型

以下列表包含 LLMs 已知类型的提示：

+   零样本提示

+   单样本提示

+   少样本提示

+   指令提示

零样本提示包含对任务的描述，而单样本提示则包含完成任务的单一示例。少样本提示由多个示例（通常在 10 到 100 个之间）组成。在所有情况下，建议提供对任务或任务的清晰描述：更多的任务可以为 GPT-3 提供更多信息，从而可能导致更准确的完成。

T0（代表“零样本”）是一个有趣的 LLM：尽管 T0 比 GPT-3 小 16 倍（11 GB），但 T0 在语言相关任务上超过了 GPT-3。T0 可以在未见过的 NLP 任务上表现良好（即对 T0 来说是新任务），因为它是在包含多个任务的数据集上训练的。

以下网址提供了 T0 的 GitHub 仓库，其中包含模型训练和评估的信息：

[`github.com/bigscience-workshop/t-zero`](https://github.com/bigscience-workshop/t-zero)

T0++基于 T0，并且它训练了超出 T0 训练任务集的额外任务。

作为旁注，前面列表中的前三个提示也分别被称为“零样本学习”、“单样本学习”和“少样本学习”。

指令提示

指令提示用于微调 LLMs，并指定 LLMs 在响应中应遵守的格式（由您确定）。您可以准备自己的指令提示，或者可以访问包含不同任务的不同模板以及不同数据集的提示模板库。各种提示指令模板公开可用，例如以下链接提供了 Llama 的提示模板：

[`github.com/devbrones/llama-prompts`](https://github.com/devbrones/llama-prompts)

[`pub.towardsai.net/llama-gpt4all-simplified-local-chatgpt-ab7d28d34923`](https://pub.towardsai.net/llama-gpt4all-simplified-local-chatgpt-ab7d28d34923)

反向提示

另一种技术使用的是反向顺序：输入提示是答案，而响应是与答案相关的提问（类似于一个流行的游戏节目）。例如，给定一个法语句子，你可能会问模型，“什么英语文本可能导致了这个法语翻译？”

系统提示与代理提示的比较

在对话式人工智能系统和聊天机器人设计的情况下，系统提示和代理提示之间的区别经常被提及。

系统提示通常是系统给出的初始消息或提示，用于指导用户可以做什么，或设定对交互的期望。它通常作为介绍或指导用户如何继续的方式。以下是一些系统提示的例子：

+   “欢迎来到 ChatBotX！你可以问我关于天气、新闻或体育的问题。今天我能帮你什么？”

+   “你好！按 1 键获取账户详情，按 2 键获取技术支持。”

+   “你好！输入‘order’跟踪你的包裹或输入‘help’寻求帮助。”

相比之下，代理提示是在交互过程中，AI 模型或代理对用户输入的响应生成的消息。它是对话中来回交流的一部分。代理提示引导用户提供更多信息，澄清歧义，或引导用户采取特定行动。以下是一些代理提示的例子：

用户：“我在找鞋子。”

代理提示：“太好了！你在找男士鞋还是女士鞋？”

用户：“我无法登录。”

代理提示：“很抱歉听到这个。你能具体说明是密码还是用户名有问题吗？”

用户：“给我讲一个笑话。”

代理提示：“为什么鸡加入了乐队？因为它有鸡腿！”

两者之间的基本区别在于它们的目的和在交互中的位置。系统提示通常在交互开始时，为对话设定场景。代理提示发生在对话过程中，根据用户输入引导对话的方向。

这两种类型的提示对于为用户提供流畅直观的对话体验至关重要。它们指导用户，并有助于确保系统有效地理解和解决用户的需求。

提示模板

提示模板是预定义的格式或结构，用于指导模型或系统执行特定任务。它们是生成提示的基础，其中模板的某些部分可以填充或定制，以产生各种特定的提示。通过类比，提示模板类似于在某些文本编辑器中可以定义的宏。

提示模板在与语言模型一起工作时特别有用，因为它们提供了一种在多个任务或数据点查询模型的一致方式。特别是，提示模板可以更容易地：

+   确保在多次查询模型时的一致性

+   促进批量处理或自动化

+   减少提问方式中的错误和变化

例如，假设你正在与一个 LLM 合作，你想将英文句子翻译成法语。相关的提示模板可能是以下内容：

“将以下英文句子翻译成法语：{sentence}”

注意，{sentence}是一个占位符，你可以用任何英文句子替换它。

你可以使用前面的提示模板来生成特定的提示：

+   “将以下英文句子翻译成法语：‘你好，你好吗？’”

+   “将以下英文句子翻译成法语：‘我爱冰淇淋。’”

正如你所见，提示模板使你能够轻松地为不同的句子生成各种提示，而无需每次都重写整个指令。实际上，这个概念可以扩展到更复杂的任务，并可以包含多个占位符或更复杂的结构，具体取决于应用。

不同 LLM 的提示词

GPT-3、ChatGPT 和 GPT-4 都是基于 Transformer 架构的 LLM，在底层机制上本质上是相似的。ChatGPT 基本上是 GPT 模型的一个版本，专门针对对话交互进行了微调。GPT-4 在规模和能力方面是 GPT-3 的演变或改进。

这些模型提示词的差异主要源于特定的用例和上下文，而不是模型之间的固有差异。以下是一些基于用例的提示词差异。

GPT-3 可以用于广泛的任务，而不仅仅是对话，从内容生成到代码编写。以下是 GPT-3 的一些提示词示例：

+   “将以下英文文本翻译成法语：‘你好，你好吗？’”

+   “编写一个计算数字阶乘的 Python 函数。”

ChatGPT 专门针对对话交互进行了微调。以下是一些 ChatGPT 的提示词示例：

用户：“你能帮我做家庭作业吗？”

ChatGPT: “当然！你需要帮助哪个科目或主题？”

用户：“告诉我一个笑话。”

ChatGPT: “为什么鸡穿过操场？为了到达另一边的滑梯！”

GPT-4 提供了更大规模和改进，因此提示词在本质上与 GPT-3 相似，但可能产生更准确或更细腻的输出。以下是 GPT-4 的一些提示词示例：

+   “提供关于量子力学与广义相对论之间关系的详细分析。”

+   “基于末世世界和希望主题写一个短篇故事。”

这三个模型接受自然语言提示并产生自然语言输出。与它们交互的基本方式保持一致。

主要差异来自模型被使用的上下文以及任何应用的微调。例如，ChatGPT 被设计成更具对话性，因此虽然你可以使用 GPT-3 进行聊天，但 ChatGPT 可能会产生更多上下文相关的对话输出。

当直接与这些模型交互，尤其是通过 API 时，您可能还可以控制诸如“温度”（控制随机性）和“最大令牌数”（控制响应长度）等参数。调整这些参数可以塑造响应，无论您使用的是哪种 GPT 变体。

虽然底层模型在规模和特定训练/微调方面存在差异，但您提示它们的方式在很大程度上保持一致：清晰、具体的自然语言提示会产生最佳结果。

不当措辞的提示

在构建提示时，尽可能清晰和具体至关重要，以便引导响应朝期望的方向发展。含糊或模糊的提示可能导致各种响应，其中许多可能对用户的实际意图没有帮助或不相关。

此外，措辞不当的提示通常模糊、含糊或过于宽泛，可能导致 AI 模型产生混淆、误解或非具体响应。以下是一些示例列表：

+   “告诉我那件事。”

    问题：过于模糊。正在指代什么“事物”？

+   “为什么会发生这样的事？”

    问题：没有上下文。正在讨论的事件或情况是什么？

+   “解释一些东西。”

    问题：过于宽泛。应该解释哪些具体的“东西”？

+   “做你需要做的事。”

    问题：含糊。需要采取什么具体行动？

+   “我想了解信息。”

    问题：不具体。需要什么类型的信息？

+   “你能从那个地方帮我拿到那个东西吗？”

    问题：两者“事物”和“地方”都不清楚。

+   “你能告诉我那个人的书是什么吗？”

    问题：含糊的引用。谁是“他”？ 

+   “你怎么做这个过程？”

    问题：指的是哪个“过程”？

+   “描述这个主题的重要性。”

    问题：“主题”未指定。

+   “为什么它是好是坏？”

    问题：没有上下文。这是什么“它”？

+   “帮助解决这个问题。”

    问题：模糊。面临的具体问题是什么？

+   “考虑这个任务的注意事项。”

    问题：歧义。正在讨论的“任务”是什么？

+   “这是怎么工作的？”

    问题：缺乏具体性。这是什么“这”？ 

什么是 ChatGPT？

“聊天机器人战争”正在加剧，主要竞争对手的长期价值仍有待确定。一个竞争对手是 ChatGPT-3.5（ChatGPT），这是来自 OpenAI 的基于 AI 的聊天机器人。ChatGPT 通过提供对话式响应来响应用户的查询，并且可以通过以下链接访问：[`chat.openai.com/chat`](https://chat.openai.com/chat)。

ChatGPT 注册用户的增长率非常惊人。最接近的竞争对手是 iPhone，它在 2.5 个月内达到了一百万用户，而 ChatGPT 在六天内就突破了百万用户。ChatGPT 的用户量峰值约为 18 亿，然后下降到大约 15 亿，您可以在以下链接中的图表中看到这一点：

[`decrypt.co/147595/traffic-dip-hits-openais-chatgpt-first-times-hardest`](https://decrypt.co/147595/traffic-dip-hits-openais-chatgpt-first-times-hardest)

注意，尽管 Meta 的 Threads 在会员数量方面超过了 ChatGPT，但 Threads 的日活跃用户数量下降了约 50%。以下是六个知名公司/产品与 ChatGPT 达到一百万会员所需时间框架的比较：[`www.syntheticmind.io/p/01`](https://www.syntheticmind.io/p/01)。

前一个网页还包含有关 Will Hobick 的信息，他使用 ChatGPT 编写了一个用于电子邮件相关任务的 Chrome 扩展程序，尽管他没有 JavaScript 或 Chrome 扩展程序编程经验。Will Hobick 在此处提供了关于他的 Chrome 扩展的更多详细信息：

[`www.linkedin.com/posts/will-hobick_gpt3-chatgpt-ai-activity-7008081003080470528-8QCh`](https://www.linkedin.com/posts/will-hobick_gpt3-chatgpt-ai-activity-7008081003080470528-8QCh)

ChatGPT

ChatGPT 的付费版本可能是世界上最好的聊天机器人。确实，ChatGPT 可以执行多种任务，其中一些如下所示：

+   写诗

+   写文章

+   写代码

+   角色扮演

+   拒绝不适当的要求

此外，它对自然语言查询的回答质量超过了其前辈 GPT-3 的能力。另一个有趣的特性包括能够承认自己的错误。ChatGPT 还提供“提示回复”，这是你可以向 ChatGPT 提出的问题的示例。ChatGPT 的一个有趣用途是生成一条结束关系的短信：

[`www.reddit.com/r/ChatGPT/comments/zgpk6c/breaking_up_with_my_girlfriend/`](https://www.reddit.com/r/ChatGPT/comments/zgpk6c/breaking_up_with_my_girlfriend/)

ChatGPT 生成的圣诞歌词可在此处获取：

[`www.cnet.com/culture/entertainment/heres-what-it-sounds-like-when-ai-writes-christmas-lyrics`](https://www.cnet.com/culture/entertainment/heres-what-it-sounds-like-when-ai-writes-christmas-lyrics)

ChatGPT 的一个可能不会让有小孩的父母感到亲切的方面是，ChatGPT 告诉孩子们圣诞老人不存在：

[`futurism.com/the-byte/openai-chatbot-santa`](https://futurism.com/the-byte/openai-chatbot-santa)

[`www.forbes.com/sites/lanceeliot/2022/12/21/pointedly-asking-generative-ai-chatgpt-about-whether-santa-claus-is-real-proves-to-be-eye-opening-for-ai-ethics-and-ai-law`](https://www.forbes.com/sites/lanceeliot/2022/12/21/pointedly-asking-generative-ai-chatgpt-about-whether-santa-claus-is-real-proves-to-be-eye-opening-for-ai-ethics-and-ai-law)

ChatGPT：谷歌“红色代码”

2022 年 12 月，谷歌的 CEO 就 ChatGPT 作为谷歌搜索引擎竞争对手的潜在威胁发布了“红色代码”，这在此处简要讨论：

[`www.yahoo.com/news/googles-management-reportedly-issued-code-190131705.html`](https://www.yahoo.com/news/googles-management-reportedly-issued-code-190131705.html)

根据前文，谷歌正在投资资源开发基于 AI 的产品，预计是为了提供能够成功与 ChatGPT 竞争的功能。其中一些基于 AI 的产品也可能生成与 DALL-E 图形效果相当的图形。确实，争夺 AI 主导权的竞赛仍在继续，并且无疑将在可预见的未来持续下去。

ChatGPT 与谷歌搜索的比较

鉴于经常有人猜测 ChatGPT 注定要取代谷歌搜索，让我们简要比较一下谷歌和 ChatGPT 对给定查询的回应方式。首先，谷歌是一个使用 PageRank 算法（由拉里·佩奇开发，是一个严格保密的秘密）的搜索引擎。谷歌使用这个算法对网站进行排名，并为给定查询生成搜索结果。然而，搜索结果中包括付费广告，这些广告可能会“扰乱”链接列表。

相比之下，ChatGPT 不是一个搜索引擎：它会对给定的查询提供直接回应。用通俗的话说，ChatGPT 会直接“切入正题”并消除任何提及多余链接的内容。ChatGPT 也可能产生错误的结果，其后果可能从无害到严重不等。

因此，谷歌搜索和 ChatGPT 都有优点和缺点，并且它们在不同类型的查询中表现出色：前者适用于具有多方面答案的查询（例如，关于法律问题的问题）和后者适用于直接了当的查询（例如，编码问题）。显然，它们在许多其他类型的查询中也表现出色。

根据玛格丽特·米切尔的说法，ChatGPT 不会取代谷歌搜索。她提供了一些关于谷歌搜索和 PageRank 的有趣细节，您可以在以下链接中阅读：[`twitter.com/mmitchell_ai/status/1605013368560943105`](https://twitter.com/mmitchell_ai/status/1605013368560943105)。

ChatGPT 自定义指令

ChatGPT 增加了对自定义指令的支持，这使您可以在 ChatGPT 回应您的查询时指定一些偏好。

ChatGPT Plus 用户可以通过访问 ChatGPT 网站并执行以下步骤来启用自定义指令：

设置 > 测试功能 > 选择自定义指令

以一个简单的例子来说，您可以指定您更喜欢看到除 Python 以外的语言中的代码。通过自定义指令，您还可以在 ChatGPT 中指定一组常见的初始要求，用于常规任务。设置自定义指令的详细步骤可在以下 URL 在线访问：

[`artificialcorner.com/custom-instructions-a-new-feature-you-must-enable-to-improve-chatgpt-responses-15820678bc02`](https://artificialcorner.com/custom-instructions-a-new-feature-you-must-enable-to-improve-chatgpt-responses-15820678bc02)

自定义指令的一个有趣例子来自杰里米·豪沃德，他准备了一套详尽且详细的自定义指令，可在以下链接中访问：

[`twitter.com/jeremyphoward/status/1689464587077509120`](https://twitter.com/jeremyphoward/status/1689464587077509120)

当这本书印刷时，只有注册了 ChatGPT Plus 的用户才能获得定制指令。

移动设备和浏览器上的 ChatGPT

ChatGPT 在 2023 年首先对 iOS 设备开放，然后是对 Android 设备。您可以从以下网页下载 ChatGPT 到 iOS 设备：

[`www.macobserver.com/tips/how-to/how-to-install-and-use-the-official-chatgpt-app-on-iphone/`](https://www.macobserver.com/tips/how-to/how-to-install-and-use-the-official-chatgpt-app-on-iphone/)

或者，如果您拥有安卓设备，您可以从以下网页下载 ChatGPT：

[`play.google.com/store/apps/details?id=com.openai.chatgpt`](https://play.google.com/store/apps/details?id=com.openai.chatgpt)

如果您想从微软的 Bing 浏览器安装 ChatGPT，请导航到以下网页：

[`chrome.google.com/webstore/detail/chatgpt-for-bing/pkkmgcildaegadhngpjkklnbfbmhpdng`](https://chrome.google.com/webstore/detail/chatgpt-for-bing/pkkmgcildaegadhngpjkklnbfbmhpdng)

ChatGPT 和提示

尽管 ChatGPT 擅长生成对查询的响应，但有时您可能对结果并不完全满意。一个选择是输入单词“重写”，以便从 ChatGPT 获得另一个版本。

尽管这是最简单的提示之一，但在有效性方面有限。如果您想要更多有意义的提示列表，以下仅限会员的文章包含了 31 个可能比使用“重写”这个词更好的提示（而不仅仅是 ChatGPT）：

[`medium.com/the-generator/31-ai-prompts-better-than-rewrite-b3268dfe1fa9`](https://medium.com/the-generator/31-ai-prompts-better-than-rewrite-b3268dfe1fa9)

GPTBot

GPTBot 是网站的爬虫。幸运的是，您可以通过将 GPTBot 添加到网站的 robots.txt 文件中来禁止 GPTBot 访问网站：

用户代理：GPTBot

禁止：/

您还可以通过将 GPTBot 令牌添加到网站的类似 robots.txt 的文件中，仅对网站的一部分进行 GPTBot 访问的定制：

用户代理：GPTBot

允许：/youcangohere-1/

禁止：/dontgohere-2/

作为旁注，Stable Diffusion 和 LAION 都通过 Common Crawl 抓取互联网。然而，您可以通过在 robots.txt 文件中指定以下片段来防止您的网站被抓取：

用户代理：CCBot

禁止：/

更多关于 GPTBot 的信息可以在以下网站获取：[`platform.openai.com/docs/gptbot`](https://platform.openai.com/docs/gptbot) [`platform.openai.com/docs/gptbot`](https://platform.openai.com/docs/gptbot)

[`www.yahoo.com/finance/news/openai-prepares-unleash-crawler-devour-020628225.html`](https://www.yahoo.com/finance/news/openai-prepares-unleash-crawler-devour-020628225.html)

ChatGPT 游乐场

ChatGPT 有一个自己的游乐场，您会发现它与可在此处访问的 GPT-3 游乐场在实质上有所不同：[`chat.openai.com/chat`](https://chat.openai.com/chat)。

为了您的方便，GPT-3 游乐场的链接在此重现：

[`beta.openai.com/playground`](https://beta.openai.com/playground)。

OpenAI 定期为 ChatGPT 添加新功能，包括以下内容：

+   用户可以查看（并继续）之前的对话

+   减少 ChatGPT 不会回答的问题数量

+   用户登录时间超过两周

另一个不错的增强功能包括对键盘快捷键的支持：当与代码一起工作时，您可以使用序列⌘ (Ctrl) + Shift +（对于 Mac）来复制最后一个代码块，以及序列⌘ (Ctrl) + /来查看完整的快捷键列表。

关于 ChatGPT 以及如何编写提示以从 ChatGPT 中提取您想要的详细信息有许多文章。其中一篇文章如下：

[`www.tomsguide.com/features/7-best-chatgpt-tips-to-get-the-most-out-of-the-chatbot`](https://www.tomsguide.com/features/7-best-chatgpt-tips-to-get-the-most-out-of-the-chatbot)

插件、高级数据分析和 Code Whisperer

除了回答用户的大量查询外，ChatGPT 通过提供以下支持来扩展其功能：

+   第三方 ChatGPT 插件

+   高级数据分析

+   Code Whisperer

上述主题将在以下子节中进行简要讨论，以及一个讨论高级数据分析与 Claude 2 的短节。

插件

目前有数百个 ChatGPT 插件可供使用，一些流行插件的列表可以在以下网站上找到：

[`levelup.gitconnected.com/5-chatgpt-plugins-that-will-put-you-ahead-of-99-of-data-scientists-4544a3b752f9`](https://levelup.gitconnected.com/5-chatgpt-plugins-that-will-put-you-ahead-of-99-of-data-scientists-4544a3b752f9)

[`www.zdnet.com/article/the-10-best-chatgpt-plugins-of-2023/`](https://www.zdnet.com/article/the-10-best-chatgpt-plugins-of-2023/)

“最佳”ChatGPT 插件的列表经常变化，因此请进行在线搜索以了解有关较新 ChatGPT 插件的信息。以下链接还包含有关高度评价插件的详细信息：

[`www.tomsguide.com/features/i-tried-a-ton-of-chatgpt-plugins-and-these-3-are-the-best`](https://www.tomsguide.com/features/i-tried-a-ton-of-chatgpt-plugins-and-these-3-are-the-best)

下面展示的另一组推荐插件（当然，取决于您的需求）：

+   AskYourPDF

+   ChatWithVideo

+   Noteable

+   Upskillr

+   Wolfram

如果您担心 ChatGPT 抓取您网站的内容，OpenAI 的浏览器插件支持一个名为 ChatGPT-User 的用户代理令牌，该令牌遵守许多网站提供的 robots.txt 文件中指定的内容，以限制对内容的访问。

如果您想为 ChatGPT 开发插件，请访问此网站获取更多信息：[`platform.openai.com/docs/plugins/introduction`](https://platform.openai.com/docs/plugins/introduction)。

除了开发 ChatGPT 插件的详细信息外，前面的 OpenAI 网站还提供了有关插件的有用信息，如下所示：

+   认证

+   示例

+   插件审查

+   插件策略

OpenAI 不控制您添加到 ChatGPT 中的任何插件：它们将 ChatGPT 连接到外部应用程序。此外，ChatGPT 根据您在 ChatGPT 账户中启用的特定插件，在您的会话期间确定要使用哪个插件。

高级数据分析

ChatGPT 高级数据分析使 ChatGPT 能够生成图表和图形，创建和训练机器学习模型，包括深度学习模型。ChatGPT 高级数据分析提供了一套广泛的功能，并且对支付每月 20 美元订阅费的 ChatGPT 用户开放。然而，这个功能可能很快就会对所有用户开放。

[`towardsdatascience.com/chatgpt-code-interpreter-how-it-saved-me-hours-of-work-3c65a8dfa935`](https://towardsdatascience.com/chatgpt-code-interpreter-how-it-saved-me-hours-of-work-3c65a8dfa935)

OpenAI 的模型可以访问一个限制在沙盒和防火墙执行环境中的 Python 解释器。在评估 Python 代码期间，解释器插件还可以访问一些临时磁盘空间。尽管临时磁盘空间是有限的，但在同一会话中的多次查询可能会在代码和执行环境方面产生累积效应。

此外，ChatGPT 可以根据请求生成数据的下载链接。高级数据分析现在可以一次性分析多个文件，包括 CSV 文件和 Excel 工作表。

高级数据分析可以执行各种有趣的任务，以下列出了一些：

+   解决数学任务

+   执行数据分析和可视化

+   在不同格式之间转换文件

+   与 Excel 工作表一起工作

+   在 PDF 中读取文本内容

以下文章讨论了您可以使用高级数据分析的各种方法：

[`mlearning.substack.com/p/the-best-88-ways-to-use-chatgpt-code-interpreter`](https://mlearning.substack.com/p/the-best-88-ways-to-use-chatgpt-code-interpreter)

高级数据分析与 Claude 2 对比

Anthropic 的 Claude 2 是 ChatGPT 的另一个竞争对手。除了响应用户的提示外，Claude 2 还可以生成代码和“摄取”整本书。Claude 2 也受到幻觉的影响，这是基于大型语言模型（LLM）的聊天机器人的共同特点。有关 Claude 2 的更详细信息，请在此处获取：

[`medium.com/mlearning-ai/claude-2-vs-code-interpreter-gpt-4-5-d2e5c9ee00c3`](https://medium.com/mlearning-ai/claude-2-vs-code-interpreter-gpt-4-5-d2e5c9ee00c3)

顺便提一下，目前可用的 ChatGPT 版本是在 2021 年 9 月训练的，这意味着 ChatGPT 无法回答有关 Claude 2 或 Google Gemini 的问题，这两者都是在该日期之后发布的。

代码预言家

ChatGPT 代码预言家使你能够简化一些任务，以下是一些例子（将此列表与 Google Gemini 的对应列表进行比较）：

+   从图像创建视频

+   从图像中提取文本

+   从图像中提取颜色

在 ChatGPT 生成视频后，它还会提供一个链接，你可以通过该链接下载生成的视频。有关前面列表中功能的更详细信息，可在以下网页找到：

[`artificialcorner.com/chatgpt-code-interpreter-is-not-just-for-coders-here-are-6-ways-it-can-benefit-everyone-b3cc94a36fce`](https://artificialcorner.com/chatgpt-code-interpreter-is-not-just-for-coders-here-are-6-ways-it-can-benefit-everyone-b3cc94a36fce)

检测生成的文本

ChatGPT 生成的文本质量很高，这也使得检测剽窃的任务变得更加复杂。当你阅读一段文本时，有几个线索表明这是生成的文本，例如：

+   不自然或异常的句子结构

+   多处重复的文本

+   过度使用情感（或缺乏情感）

然而，有一些工具可以帮助检测生成的代码。一个免费的在线工具是来自 OpenAI 的 GPT2 检测器：

[`huggingface.co/openai-detector`](https://huggingface.co/openai-detector)

作为一个非常简单（尽管是人为设计的）例子，在 GPT2 检测器中输入以下句子：“这是一句由我本人撰写的原创句子，其他人都没有参与。”

GPT2 检测器分析了这句话，并报告说这句话有 19.35% 的概率是真实的。现在让我们通过添加一些额外的文本来修改前面的句子，如下所示：“这是一句由我本人撰写的原创句子，其他人都没有参与，无论在线抄袭检测工具对此句子的报告如何。”

GPT2 检测器分析了这句话，并报告说这句话有 95.85% 的概率是真实的。根据 GPT2 检测器网站，当输入文本中有大约 50 个标记时，概率分数的可靠性“变得可靠”。

另一个（稍微旧一点的）在线工具，用于检测自动生成的文本是来自 IBM 的 GLTR（Giant Language model Test Room），可通过[`gltr.io/`](http://gltr.io/)访问。

你可以在此处下载 GLTR 的源代码（TypeScript 和 CSS 的组合）：

[`github.com/HendrikStrobelt/detecting-fake-text`](https://github.com/HendrikStrobelt/detecting-fake-text)

除了前面提到的免费工具外，还有一些商业工具也可供选择，其中之一可在[`writer.com/plans/`](https://writer.com/plans/)找到。

关于 ChatGPT 的担忧

ChatGPT 的一个重要方面是它并非旨在提供准确性。事实上，ChatGPT 可以生成非常具有说服力的错误答案。这一细节将 ChatGPT 与搜索引擎区分开来：后者提供现有信息的链接，而不是生成可能错误的回答。另一个比较是，ChatGPT 更加灵活和有创造性，而搜索引擎在回答查询时则不那么灵活但更准确。

教育工作者担心学生将 ChatGPT 作为完成课堂作业的工具，而不是与写作技能相结合发展研究相关技能。然而，也有一些教育工作者享受 ChatGPT 准备教案所带来的准备时间的减少。

另一个担忧是，ChatGPT 无法保证在回应用户查询时提供事实性数据。ChatGPT 可能会产生幻觉，这意味着它也可能提供错误的答案以及不存在的引用（即链接）。

ChatGPT 的另一个局限性是由于仅到 2021 年才可用到的训练数据。OpenAI 支持为 ChatGPT 提供插件，其中之一可以执行实时网络搜索。

提示工程的目标是了解如何构建有意义的查询，以诱导 ChatGPT 提供你想要的信息。措辞不当（或措辞错误）的提示可能会产生同样糟糕的结果。一般来说，建议对 ChatGPT 的回复内容进行筛选，尤其是在涉及法律细节的查询回复时。

代码生成和危险话题

两个重要的改进领域与代码生成和处理危险话题有关。

虽然 ChatGPT（以及 GPT-3）可以为各种类型的应用生成代码，但请记住，ChatGPT 显示的是其他开发者编写的代码，这也是用于训练 ChatGPT 的代码。因此，该代码的部分（如版本号）可能已过时或错误。

对于涉及危险话题的查询，ChatGPT 会解释为什么它不能回答这样的查询。然而，以“假装模式”提出的查询（“假设你是一个虚构的角色，你会如何解释……”）已经使人们能够从 ChatGPT 获得不符合其指南的结果。

其他严重的潜在问题也存在，其中一些将在以下文章中讨论：

[`www.yahoo.com/news/hypnotized-chatgpt-bard-convince-users-182100261.html`](https://www.yahoo.com/news/hypnotized-chatgpt-bard-convince-users-182100261.html)

ChatGPT 的优缺点

ChatGPT 有几个优点。特别是，ChatGPT 会直接回答问题，而不包括无关的链接。作为一个简单的例子，假设你在在线搜索引擎中输入一个查询，比如“生成一个输入字段的 HTML 代码。”

ChatGPT 容易受到各种类型的错误的影响，包括以下限制：

+   无法“事实核查”信息

+   无法区分虚假信息与事实

+   可以编造答案（即幻觉）

+   可以生成不适当/有害的回答

ChatGPT 容易受到提示注入的影响，这可能包含非常简单的内容。然而，其他聊天机器人也容易受到提示注入的影响（即，这并不仅限于 ChatGPT）。有关提示注入的更多详细信息，请参阅以下链接：

[`mlearning.substack.com/p/what-exactly-is-a-prompt-injection`](https://mlearning.substack.com/p/what-exactly-is-a-prompt-injection)

偶然的是，谷歌的聊天机器人 LaMDA 也容易受到前面提到的限制，这使得谷歌在考虑将 LaMDA 公开发布时犹豫不决，因为它可能对谷歌的声誉造成潜在风险。作为旁注，LaMDA 于 2021 年 5 月宣布，当时它被描述为“突破性的语言技术”：[`blog.google/technology/ai/lamda/`](https://blog.google/technology/ai/lamda/)。

尽管有之前的列表，ChatGPT 已经增强了聊天机器人的功能，并将无疑激发该领域主要利益相关者的创新和竞争。

CHATGPT 的查询和回复示例

这里是一个提交给 ChatGPT 的查询示例，以及 ChatGPT 的详细回复：

许多人认为人工智能是危险的。你呢？

“有一个普遍的误解，认为人工智能天生具有危险性。虽然人工智能确实有可能被用于有害目的，但它也有能力做很多好事。就像任何其他技术一样，这完全取决于如何使用。在合适的人手中，人工智能可以用来解决世界上一些最紧迫的问题，例如治愈疾病和改善农业。在不合适的人手中，它可能会被用来造成伤害。对我们来说，负责任和道德地使用人工智能，并确保以最小化潜在危害的方式对其进行监管和控制，是非常重要的。”

这里是提交给 ChatGPT-3 的一些查询示例，以及相应的详细回复：

1. 你有哪些方法可以提高你对查询的回答的准确性？

“提高我对查询的回答准确性的方法有几个。一种方法是用更多的数据来训练我的算法。我拥有的数据越多，我可以处理的信息就越多，我的回答就越准确。提高准确性的另一种方法是使用更先进的算法和技术，例如机器学习和自然语言处理。这些方法使我能够更好地理解语言的细微差别，并提供更准确的查询回答。此外，定期的测试和评估可以帮助识别可以提高准确性的领域，并使我能够专注于这些领域以改进我的回答。”

2. 你能给出一个奇完全数的例子吗？

“据我们所知，目前没有发现奇完全数。虽然人们相信奇完全数存在，但至今尚未找到，也不知道是否存在。事实上，目前完全不清楚是否存在任何奇完全数。如果发现了一个奇完全数，那将是数学领域的重大突破。”

3. 你能提供哥德巴赫猜想的证明吗？

“很抱歉，我无法提供哥德巴赫猜想的证明。哥德巴赫猜想是数学中一个著名的未解问题，它断言每个大于 2 的偶数都可以表示为两个素数之和。尽管多年来数学家们付出了巨大努力，但该猜想的证明尚未找到。它被认为是数学中最具挑战性的未解问题之一。由于我是一个由 OpenAI 训练的大型语言模型，我没有能力证明数学猜想。我的能力仅限于基于我所训练的信息提供答案。”

4. 死后有生命吗？与地球上的生活相比如何？

“没有科学证据支持死后有生命的观点。这是一个争论了几个世纪的话题，不同的文化和信仰体系对死后发生的事情有自己的看法。有些人相信来世，而另一些人则不相信。由于没有科学证据支持来世的存在，因此无法比较其与地球上的生活。这最终是一个个人信仰问题。”

5. 请提供一份关于乌克兰与俄罗斯战争的四段分析，并给出你对结果的预测

“乌克兰与俄罗斯之间的战争是一场复杂的冲突，其根源可追溯到 2014 年俄罗斯吞并克里米亚。自那时起，冲突不断升级，俄罗斯支持的乌克兰东部分离主义者与乌克兰政府军交战。战斗已导致数千人伤亡，并使许多人流离失所。

冲突的核心问题在于乌克兰的主权问题。俄罗斯长期以来将乌克兰视为其势力范围的一部分，吞并克里米亚被许多人视为对乌克兰主权的侵犯。另一方面，乌克兰决心维护其独立，并得到了许多西方国家的支持。

预测战争的结果是困难的。尽管乌克兰军队近年来在对抗分离主义者方面取得了一些进展，但俄罗斯继续向叛军提供支持，冲突仍未解决。从长远来看，可能需要通过外交解决方案来结束战斗。然而，这样的解决方案能否达成以及何时达成，目前尚不确定。

同时，战争继续对乌克兰人民造成巨大损失。许多人陷入交火，持续的暴力和不稳定对国家的经济和整体发展产生了重大影响。国际社会继续支持乌克兰维护其主权和结束冲突的努力至关重要。”

如前所述的示例所示，ChatGPT 以超越许多近年来聊天机器人的方式提供了令人印象深刻且准确的查询响应。然而，仍然有可能使这个聊天机器人困惑：

[`www.theverge.com/23488017/openai-chatbot-chatgpt-ai-examples-web-demo`](https://www.theverge.com/23488017/openai-chatbot-chatgpt-ai-examples-web-demo)

CHATGPT 的替代品

有几种 ChatGPT 的替代品提供了类似的功能集，以下列出了一些：

+   Google Gemini

+   Bing Chat

+   Gemini（Google）

+   Jasper

+   PaLM（Google）

+   Pi

+   POE（LinkedIn）

+   Replika

+   WriteSonic

+   YouChat

下面的子节讨论了前面列表中的一些（但不是全部）ChatGPT 替代品。

Google Gemini

Google Gemini 是一个具有与 ChatGPT 类似功能的人工智能聊天机器人，例如生成代码以及生成文本/文档。以下展示了 Bard 支持的功能子集：

+   内置互联网搜索支持

+   内置语音识别支持

+   基于“PaLM 2（Google）”构建

+   支持 20 种编程语言

+   阅读并总结 PDF 内容

+   提供信息链接

根据以下文章，Gemini 增加了对 40 种额外语言的支持以及文本到语音的支持：

[`www.extremetech.com/extreme/google-bard-updated-with-text-to-speech-40-new-languages`](https://www.extremetech.com/extreme/google-bard-updated-with-text-to-speech-40-new-languages)

此外，Gemini 支持包含图像的提示（由 Google Lens 解释）并可以根据图像生成字幕。

以下文章建议，Google 可以通过利用 PaLM 与 ChatGPT 保持竞争力：

[`analyticsindiamag.com/googles-palm-is-ready-for-the-gpt-challenge/`](https://analyticsindiamag.com/googles-palm-is-ready-for-the-gpt-challenge/)

YouChat

ChatGPT 的另一个替代品是 YouChat，它是搜索引擎[you.com](http://you.com)的一部分，并且可以在[`you.com/`](https://you.com/)访问。

在机器学习社区因众多贡献而广为人知的理查德·索科尔（Richard Socher）是[you.com](http://you.com)的创造者。根据理查德·索科尔的说法，YouChat 是一个搜索引擎，它可以提供通常的搜索相关功能，以及搜索网络以获取更多信息以响应用户查询的能力。

另一个竞争对手是来自 LinkedIn 的 POE，你可以在[`poe.com/login`](https://poe.com/login)创建免费账户。

Inflection 的 Pi

Pi 是由 InflectionAI 开发的聊天机器人，该公司由 Mustafa Suleyman 创立，他也是 DeepMind 的创始人。Pi 可在 [`pi.ai/talk`](https://pi.ai/talk) 访问

以及更多信息可以在以下网页找到：

[`medium.com/@ignacio.de.gregorio.noblejas/meet-pi-chatgpts-newest-rival-and-the-most-human-ai-in-the-world-367b461c0af1`](https://medium.com/@ignacio.de.gregorio.noblejas/meet-pi-chatgpts-newest-rival-and-the-most-human-ai-in-the-world-367b461c0af1)

开发团队使用了基于人类反馈的强化学习（RLHF）来训练这个聊天机器人：

[`medium.com/@ignacio.de.gregorio.noblejas/meet-pi-chatgpts-newest-rival-and-the-most-human-ai-in-the-world-367b461c0af1`](https://medium.com/@ignacio.de.gregorio.noblejas/meet-pi-chatgpts-newest-rival-and-the-most-human-ai-in-the-world-367b461c0af1)

机器学习与 ChatGPT：高级数据分析

OpenAI 支持一个名为高级数据分析的功能，该功能使 ChatGPT 能够根据数据集的数据生成生成图表和图形的 Python 代码。此外，高级数据分析可以生成可以在数据集上训练的机器学习模型。例如，图 4.1 显示了基于泰坦尼克号数据集的图表截图。

顺便说一句，如果您想查看 ChatGPT 生成用于机器学习模型的 Python 代码以及图表和图形的示例，您可以在几本即将出版的书中学习如何做到这一点：

+   机器学习、Python 3 和 ChatGPT”

+   Python 和 ChatGPT/GPT-4

+   使用 ChatGPT 进行 Python 和数据可视化

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p116.jpg)

图 4.1 泰坦尼克号图表和图形

什么是 InstructGPT？

InstructGPT 是由 OpenAI 开发的一种语言模型，它是 ChatGPT 的一个兄弟模型。InstructGPT 被设计为遵循提示中给出的指令以生成详细响应。以下列出了关于 InstructGPT 的一些关键点：

+   指令遵循

+   训练

+   应用

+   局限性

指令遵循：与专注于开放式对话的 ChatGPT 不同，InstructGPT 被设计为在提示中遵循用户指令。这使得它适合用户通过给出明确的指令来获取特定信息或输出的任务。

训练：InstructGPT 使用与 ChatGPT 类似的基于人类反馈的强化学习（RLHF）进行训练。一个初始模型是通过监督微调训练的，其中人类 AI 训练师提供了用户和 AI 助手两边的对话。然后，这个新的对话数据集与 InstructGPT 数据集混合，并转换为对话格式。

应用：InstructGPT 可以在需要更详细解释、逐步指南或基于提供的指令的具体输出的场景中非常有用。

局限性：与其他模型一样，InstructGPT 有其局限性。它可能会产生不正确或无意义的答案。输出取决于提示的措辞。它对输入措辞也很敏感，可能会根据轻微的改写给出不同的回答。

随着 AI 模型及其应用的快速发展，InstructGPT 在 2021 年之后可能已经进行了进一步的发展或迭代。请始终参考 OpenAI 的官方出版物和更新以获取最新信息。有关 InstructGPT 的更多信息可在[`openai.com/blog/instruction-following/`](https://openai.com/blog/instruction-following/)找到。

VIZGPT 和数据可视化

VizGPT 是一个在线工具，允许您指定基于英语的提示以可视化数据集的各个方面，并且可以在[`www.vizgpt.ai/`](https://www.vizgpt.ai/)访问。

选择默认的“汽车数据集”，然后点击“数据”按钮以显示数据集的内容，如图图 4.2 所示。

接下来，选择默认的“汽车数据集”，然后点击“与可视化聊天”按钮以显示数据集的可视化，如图图 4.3 所示。

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p118.jpg)

图 4.2 VizGPT “汽车数据集”行

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p119.jpg)

图 4.3 VizGPT “汽车数据集”可视化

您可以使用 VizGPT 进行进一步实验。例如，您可以通过点击“上传 CSV”按钮上传自己的数据集，并使用该数据集获得类似的结果。

什么是 GPT-4？

GPT-4 于 2023 年 3 月中旬发布，并且仅通过向现有 ChatGPT 账户付费升级（每月 20 美元）才能获得。根据用户的各种在线轶事故事，GPT-4 在性能上显著优于 ChatGPT。此外，微软有一个 GPT-4 版本，为 Bing 浏览器提供动力，该浏览器对公众免费提供。

GPT-4 是一个大型多模态模型，可以处理基于图像的输入以及基于文本的输入，然后生成文本输出。目前，基于图像的输出对公众不可用，但它确实有内部支持图像生成。

GPT-4 支持 25,000 个单词的输入文本：相比之下，ChatGPT 的限制为 4,096 个字符。尽管 GPT-4 的参数数量未公开，但以下文章声称 GPT-4 是由 8 个 220 亿参数模型混合而成的，这是 MoE（专家混合）架构的一个例子：

[`thealgorithmicbridge.substack.com/p/gpt-4s-secret-has-been-revealed`](https://thealgorithmicbridge.substack.com/p/gpt-4s-secret-has-been-revealed)

GPT-4 和测试成绩

改进准确性的一个有趣例子与律师资格考试有关，ChatGPT 的成绩在倒数 10%之内。相比之下，GPT-4 在相同的律师资格考试中得分在顶部 10%之内。更多详情请见此处：

[`www.abajournal.com/web/article/latest-version-of-chatgpt-aces-the-bar-exam-with-score-in-90th-percentile`](https://www.abajournal.com/web/article/latest-version-of-chatgpt-aces-the-bar-exam-with-score-in-90th-percentile)

此外，GPT-4 显然能够以 3.34 的 GPA 通过哈佛大学一年级。更多详情请在此处查看：

[`www.businessinsider.com/chatgpt-harvard-passed-freshman-ai-education-GPT-4-2023-7?op=1`](https://www.businessinsider.com/chatgpt-harvard-passed-freshman-ai-education-GPT-4-2023-7?op=1)

GPT-4 在多项其他测试中表现良好，其中一些如下所示：

+   AP 考试

+   SAT

+   GRE

+   医疗测试

+   律师考试

+   商学院考试

+   宾夕法尼亚大学沃顿商学院考试

+   美国生物学奥林匹克半决赛考试

+   葡萄酒师（酒保）考试

您可以从以下网页了解更多关于前面测试的详细信息：

[`www.businessinsider.com/list-here-are-the-exams-chatgpt-has-passed-so-far-2023-1`](https://www.businessinsider.com/list-here-are-the-exams-chatgpt-has-passed-so-far-2023-1)

以下网页包含有关 GPT-4 测试分数、基准和其他结果的更多详细信息：[`openai.com/research/gpt-4`](https://openai.com/research/gpt-4).

GPT-4 参数

本节包含有关一些 GPT-4 参数的信息，其中一些是最佳猜测近似值。

由于 GPT-4 是基于 Transformer 的 AR（自回归）模型，它被训练来进行下一个标记预测。以下论文“GPT-4 技术报告”于 2023 年 3 月发布，其中包含了对 GPT-4 能力的详细分析：

[`arxiv.org/abs/2303.08774`](https://arxiv.org/abs/2303.08774)

GPT-4 微调

尽管 OpenAI 允许您微调四个基础模型，但目前（目前）无法对 ChatGPT 3.5 或 GPT-4 进行微调。相反，您可以通过 LangChain 或 LlamaIndex（之前称为 GPT-Index）将 OpenAI 模型与您自己的数据源集成。它们都使您能够将 OpenAI 模型与现有的数据源连接。

LlamaIndex 介绍可在以下网页找到：

[`www.pinecone.io/learn/series/langchain/langchain-intro/`](https://www.pinecone.io/learn/series/langchain/langchain-intro/)

LlamaIndex 介绍可在以下网页找到：

[`zilliz.com/blog/getting-started-with-llamaindex`](https://zilliz.com/blog/getting-started-with-llamaindex)

[`stackoverflow.com/questions/76160057/openai-chat-completions-api-how-do-i-customize-answers-from-gpt-3-5-or-gpt-4-mo?noredirect=1&lq=1`](https://stackoverflow.com/questions/76160057/openai-chat-completions-api-how-do-i-customize-answers-from-gpt-3-5-or-gpt-4-mo?noredirect=1&lq=1)

CHATGPT 和 GPT-4 竞争对手

在 2022 年 11 月 30 日 ChatGPT 发布后不久，各家公司纷纷推出 ChatGPT 的竞争对手，以下是一些例子：

+   Google Gemini

+   CoPilot（微软）

+   Codex（OpenAI）

+   Apple GPT (苹果)

+   PaLM 2 (谷歌和 GPT-4 竞争对手)

+   Claude 2 和 Claude 3 (Anthropic)

+   Llama 2（Meta）

以下小节包含有关前面列表中 LLM 的更多详细信息。

Gemini

Gemini 是谷歌的一个 AI 聊天机器人，是 ChatGPT 的竞争对手。通过比较，Gemini 由 PaLM 2（稍后讨论）提供动力，而 ChatGPT 由 GPT-4 提供。最近，Gemini 在对用户查询的回答中增加了对图像的支持，而 ChatGPT 的这一功能尚未向公众发布。更多信息可以在以下网页找到：

[`artificialcorner.com/google-bards-new-image-recognition-means-serious-competition-to-chatgpt-here-are-6-best-use-cases-55d69eae1b27`](https://artificialcorner.com/google-bards-new-image-recognition-means-serious-competition-to-chatgpt-here-are-6-best-use-cases-55d69eae1b27)

Bard（在成为 Google Gemini 之前）在一场备受瞩目的发布中遇到了与詹姆斯·韦伯太空望远镜相关的问题，这导致字母表的市值大幅下降。然而，谷歌一直在努力修复问题并增强 Bard 的功能。您可以通过 [`bard.google.com/`](https://bard.google.com/) 访问 Bard。

大约在 2023 年中旬，Bard 获得了 GPT-4 在同一时间期间没有的一些功能，其中一些如下所示：

+   生成图像

+   从图像生成 HTML/CSS

+   从图像生成移动应用程序

+   从图像创建 LaTeX 公式

+   从图像中提取文本

据推测，这些功能将促使 OpenAI 提供相同的功能集（其中一些已在 GPT-4 中实现，但尚未公开提供）。

CoPilot (OpenAI/微软)

Microsoft CoPilot 是一个由 GPT-4 驱动的 Visual Studio Code 扩展。GitHub CoPilot 已因其能够在程序上下文中生成代码块的能力而闻名。此外，微软还在开发 Microsoft 365 CoPilot，截至 2023 年中旬尚未公布其可用日期。

然而，微软已经提供了早期演示，展示了 Microsoft 365 Copilot 的一些功能，包括自动化以下任务：

+   写电子邮件

+   概括会议

+   制作 PowerPoint 演示文稿

Microsoft 365 Copilot 可以分析 Excel 工作表中的数据，在 PowerPoint 中插入 AI 生成的图像，并生成求职信草稿。微软还将 Microsoft 365 Copilot 集成到其一些现有产品中，例如 Loop 和 OneNote。

根据以下文章，微软计划每月收取 30 美元为 Office 365 Copilot 收费：

[`www.extremetech.com/extreme/microsoft-to-charge-30-per-month-for-ai-powered-office-apps`](https://www.extremetech.com/extreme/microsoft-to-charge-30-per-month-for-ai-powered-office-apps)

Copilot 在 2022 年晚些时候被逆向工程，详情如下：

[`thakkarparth007.github.io/copilot-explorer/posts/copilot-internals`](https://thakkarparth007.github.io/copilot-explorer/posts/copilot-internals)

以下文章展示了如何创建一个使用 NextJS、React 和 CoPilot 的 GPT-3 应用程序：

[`github.blog/2023-07-25-how-to-build-a-gpt-3-app-with-nextjs-react-and-github-copilot/`](https://github.blog/2023-07-25-how-to-build-a-gpt-3-app-with-nextjs-react-and-github-copilot/)

Codex (OpenAI)

OpenAI Codex 是一个基于 GPT-3 的微调大型语言模型（LLM），可以从文本生成代码。实际上，Codex 为 GitHub Copilot 提供动力。Codex 在超过 150 GB 的 Python 代码上进行了训练，这些代码来自超过 5000 万个 GitHub 仓库。

根据 OpenAI 的说法，Codex 的主要目的是加速人类编程，它可以完成近 40% 的请求。Codex 在生成用于解决简单任务的代码方面表现得相当不错。访问 Codex 主页以获取更多信息：[`openai.com/blog/openai-codex`](https://openai.com/blog/openai-codex)。

Apple GPT

到 2023 年中旬，苹果公司宣布了 Apple GPT，这是 OpenAI 的 ChatGPT 的竞争对手。实际发布日期预计将在 2024 年。目前“Apple GPT”是旨在与 Google Gemini、OpenAI ChatGPT 和 Microsoft Bing AI 竞争的产品名称。

简而言之，LLM PaLM 2 为 Google Gemini 提供动力，而 GPT-4 则为 ChatGPT 以及 Bing Chat 提供动力，Ajax 则是 Apple GPT 的动力来源。Ajax 基于 Google 的 Jax，而 Ajax 这个名字是一个巧妙的组合（可能是“Apple Jax”吗？）。

PaLM-2

PaLM-2，即路径语言模型（Pathways Language Model）的缩写，是 PaLM（约 2022 年）的继任者。PaLM-2 为 Gemini 提供动力，并且也是 GPT-4 的直接竞争对手。相比之下，PaLM 由 5400 亿个参数组成，PaLM-2 可能是一个更大的 LLM（后者的详细信息尚未公开）。

PaLM-2 提供了四个子模型，称为 Gecko、Otter、Bison 和 Unicorn（从小到大）。PaLM-2 在超过 100 种人类语言以及 Fortran 等编程语言上进行了训练。此外，PaLM-2 已部署到包括 Gmail 和 YouTube 在内的众多 Google 产品中。

Med-PaLM M

除了上述四个子模型之外，Med-PaLM 2（Med-PaLM 的继任者）是一个提供医疗问题答案的 LLM，可在以下链接访问：[`sites.research.google/med-palm/`](http://sites.research.google/med-palm/)。

Med-PaLM 的继任者是 Med-PaLM M，有关此 LLM 的详细信息可在以下链接找到：[`arxiv.org/abs/2307.14334`](https://arxiv.org/abs/2307.14334)。

提供了 PaLM 2 和 GPT-4 性能基准直接比较的文章可在以下链接找到：

[`www.makeuseof.com/google-palm-2-vs-openai-gpt-4/`](https://www.makeuseof.com/google-palm-2-vs-openai-gpt-4/)

PaLM-2 拥有一套强大的功能，并且是 GPT-4 的一个重要竞争对手。

Claude 2

Anthropic 创建了 LLM Claude 2，它可以回答关于特定主题的问题。它还可以执行涉及多个文档的搜索，可以总结文档、创建文档和生成代码。

Claude 2 是其前身 Claude 1.3 的改进，它可以“吞噬”整本书，并根据用户的提示生成代码。Claude 2 在竞争功能方面似乎与 ChatGPT 和 GPT-4 等竞争对手相当。

此外，Claude 2 支持 100,000 个 token 的上下文窗口。它是在 2023 年初的数据上训练的，而 ChatGPT 是在 2021 年之前的数据上训练的。然而，Claude 2 无法搜索网络（与竞争对手 GPT-4 不同）。Anthropic 可能会在该领域做更多重要的工作。

LLAMA 2

Llama 2（大型语言模型 Meta AI）是 Meta 开源的微调 LLM，它仅使用公开可用的数据进行训练；它在 AI 社区中引起了很大的兴奋。Llama 2 提供了三个模型（7B、13B 和 70B 参数），在预训练步骤中使用的比许多其他 LLM 更多。Llama 2 被优化以提供比其他 LLM 更快的推理和更长的上下文长度（4K）。

此外，Llama 2 聊天 LLM 的表现出人意料地好：在某些情况下，其质量接近 ChatGPT 和 GPT-4 等高性能 LLM 的质量。与 GPT-4 相比，Llama 2 更易于使用，在撰写文本方面提供更好的结果。然而，GPT-4 在生成代码等任务上更为擅长。

如何下载 Llama 2

Llama 2 为社区使用和商业使用提供了许可协议，Meta 已将代码以及预训练模型和微调模型公开。

您可以通过多种方式下载 Llama 2，从以下网页开始（在您提供一些信息，如姓名、国家、隶属机构后）：[`ai.meta.com/llama/`](https://ai.meta.com/llama/)。

您可以在以下网址访问 7B、13B 和 70B 模型的演示：

[`huggingface.co/spaces/huggingface-projects/Llama 2-7b-chat`](https://huggingface.co/spaces/huggingface-projects/Llama2-7b-chat)

[`huggingface.co/spaces/huggingface-projects/Llama 2-13b-chat`](https://huggingface.co/spaces/huggingface-projects/Llama2-13b-chat)

[`huggingface.co/spaces/ysharma/Explore_llamav2_with_TGI`](https://huggingface.co/spaces/ysharma/Explore_llamav2_with_TGI)

您也可以从以下网页访问 Hugging Face 上的 Llama 2：[`huggingface.co/blog/llama2`](https://huggingface.co/blog/llama2)

[`github.com/facebookresearch/llama`](https://github.com/facebookresearch/llama)

[`ai.meta.com/research/publications/llama-2-open-foundation-and-fine-tuned-chat-models/`](https://ai.meta.com/research/publications/llama-2-open-foundation-and-fine-tuned-chat-models/)

如果你感兴趣在笔记本电脑上训练 Llama 2，更多细节请在此处获取：[`blog.briankitano.com/llama-from-scratch/`](https://blog.briankitano.com/llama-from-scratch/).

Llama 2 架构特性

本节仅包含一些 Llama 2 的重要区分特征的概述，如下所示：

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

大多数 LLM 包含原始 transformer 架构中的层归一化。相比之下，LlaMa 使用了一种简化的替代方案，涉及根均方层归一化（RMSNorm）。RMSNorm 在训练稳定性和泛化方面都取得了改进的结果。

尽管 SwiGLU 在计算上比原始 transformer 架构中的 ReLU 激活函数更昂贵，但 SwiGLU 实现了更好的性能。

注意，RLHF 在第五章中进行了讨论，其中还包括了 TRPO 和 PPO 的简要描述。有关如何在三个任务上微调 Llama 2 的详细描述，请访问以下网页：

[`www.anyscale.com/blog/fine-tuning-llama-2-a-comprehensive-case-study-for-tailoring-models-to-unique-applications`](https://www.anyscale.com/blog/fine-tuning-llama-2-a-comprehensive-case-study-for-tailoring-models-to-unique-applications)

微调 Llama 2

虽然 Llama 2 在其前辈 Llama 的基础上有所改进，但你可以通过对这种 LLM 进行一些微调来进一步提高 Llama 2 的性能。

[`medium.com/@murtuza753/using-llama-2-0-faiss-and-langchain-for-question-answering-on-your-own-data-682241488476`](https://medium.com/@murtuza753/using-llama-2-0-faiss-and-langchain-for-question-answering-on-your-own-data-682241488476)

以下文章展示了如何在 Google Colaboratory 笔记本中微调 Llama 2：

[`towardsdatascience.com/fine-tune-your-own-llama-2-model-in-a-colab-notebook-df9823a04a32`](https://towardsdatascience.com/fine-tune-your-own-llama-2-model-in-a-colab-notebook-df9823a04a32)

以下文章描述了如何使用 MonsterAPI（文章中也进行了讨论）通过五个步骤微调 Llama 2：[`blog.monsterapi.ai/how-to-fine-tune-llama-2-llm/`](https://blog.monsterapi.ai/how-to-fine-tune-llama-2-llm/).

以下网页描述了如何在 Google Colaboratory 中访问 Llama 2：

[`levelup.gitconnected.com/harnessing-the-power-of-llama-2-using-google-colab-2e1dedc2d1d8`](https://levelup.gitconnected.com/harnessing-the-power-of-llama-2-using-google-colab-2e1dedc2d1d8)

GPT-5 何时可用？

当这本书准备印刷时，关于 GPT-5 的状态没有官方信息可用，也就是说，一切都是推测性的。在 2023 年初，OpenAI 的首席执行官 Sam Altman 表示，“没有关于 GPT-5 的官方计划”。

然而，在 2023 年中，OpenAI 为 GPT-5 申请了专利，其中包含了一些关于 GPT-5 特性的高级细节。有些人推测 GPT-5 将是 GPT-4 的更强大版本，而其他人则认为申请专利可能只是 OpenAI 确保 GPT-5 名称的举措。

无论申请专利的动机如何，来自各个公司的 GPT-4 竞争非常激烈。因此，OpenAI 可能会在 2024 年底之前发布 GPT 4.5 或 GPT-5。关于模型大小，回想一下，GPT-3 有 1750 亿个参数，有些人推测 GPT-4 有 100 万亿个参数，这意味着 GPT-4 大约是 GPT-3 的 60 倍。GPT-5 规模增加的相同幅度似乎是不可能的，因为 GPT-5 将包含 600 万亿个参数。

另一种可能性是，GPT-4 基于 MoE（专家混合）方法，该方法涉及多个组件。例如，GPT-4 可能是 8 个组件的组合，每个组件包含 2.2 亿个参数，因此 GPT-4 将包含 1.76 万亿个参数。

训练 LLM（如 GPT-4）非常昂贵，并且需要大量的数据集进行预训练步骤。无论 GPT-5 最终的大小如何，训练过程都可能涉及巨大的成本。

摘要

本章从 OpenAI 的 ChatGPT 及其一些特性开始讨论。此外，你还了解了一些 ChatGPT 的竞争对手，例如 Anthropic 的 Claude 2。

接下来，你学习了 OpenAI 的 GPT-4，它是 ChatGPT 的驱动力，以及它的一些特性。然后，你学习了 GPT-4 的一些竞争对手，例如 Meta 的 Llama 2 和 Google Gemini。

第五章

使用 GPT-4 的线性回归

本章介绍了线性回归，并包含了使用 NumPy API 生成的 GPT-4 代码示例。这些代码示例采用“增量”方法，从涉及 Python 和 NumPy 代码（通常使用 NumPy linspace() API）的简单示例开始。

本章的第一部分简要讨论了各种类型的线性回归，包括简单线性回归、多元线性回归、多项式回归以及带有交互项的线性回归的示例。

本章的第二部分包含了一些使用 NumPy 标准技术的线性回归任务的额外代码示例。因此，如果你对这个主题感到舒适，你可能会快速浏览本章的前两节。

在阅读本章之前，请记住，大部分（大约 90%）的内容是由 ChatGPT 生成的。本章材料的编辑过程涉及以下变更：

+   添加章节标题

+   包含项目符号列表

+   移除无关紧要的细节

+   斜体标题

正如你很快就会看到的，本章的细节展示了 ChatGPT 提供全面详细响应用户提出任务时的惊人能力。此外，ChatGPT 还拥有非常有用的调试功能，可以帮助调试它为你生成的代码，因为该代码并不总是完美的。

现在我们来看看 GPT-4 生成的内容，以下部分作为起点。

什么是线性回归？

尽管线性回归是在 200 多年前开发的，但这种方法仍然是解决（尽管是简单的）统计学和机器学习问题的“核心”技术之一。用于在二维平面（或更高维度的超平面）上的数据点找到最佳拟合线的均值平方误差（MSE）技术，在 Python 和 TensorFlow 中实现，以最小化后面讨论的成本函数。

线性回归的目标是找到最佳拟合线，该线“代表”数据集。请记住两个关键点。首先，最佳拟合线不一定通过数据集中的所有（甚至大多数）点。最佳拟合线的目的是最小化该线与数据集中点的距离。其次，线性回归并不确定最佳拟合的多项式：后者涉及找到一个高阶多项式，它通过数据集中的许多点。

线性回归的示例

线性回归是一种统计方法，用于建模因变量与一个或多个自变量之间的关系。线性回归最简单的形式是简单线性回归，它涉及一个因变量和一个自变量。相比之下，多元线性回归涉及一个因变量和两个或更多的自变量。我们将讨论以下类型回归的示例：

+   简单线性回归

+   多元线性回归

+   多项式回归

+   具有交互项的线性回归

选择使用哪种类型的线性回归取决于数据的性质和你要尝试回答的具体问题。例如，简单线性回归的一个例子是根据一个人的身高预测其体重。假设你有一组人的身高和体重数据。你想要根据身高（自变量）预测体重（因变量）。体重和身高的数学表示如下所示：

重量=β0+β1×身高

多元线性回归的一个例子是根据房屋的大小和年龄预测其价格。在这种情况下，你正在根据两个自变量预测房价（因变量）：房屋的大小（以平方英尺计）和房屋的年龄（以年计）。价格、大小和年龄的数学表示如下所示：

价格=β0+β1×尺寸+β2×年龄

第三个例子涉及带有交互项的线性回归，例如根据产品的价格和广告量预测产品销量，同时考虑价格和广告之间的交互作用。

除了价格和广告对销量的直接影响之外，你还考虑了这两个的组合（它们的交互作用）可能如何影响销量。以下是销量、价格、广告以及价格和广告的乘积的数学表示：

销量=β0+β1×价格+β2×广告+β3×(价格×广告)

除了前面的例子之外，还可以执行多项式回归（一种线性回归），例如根据时间预测抛物线的轨迹。尽管它被称为“多项式”，但它仍然是一种线性回归，因为回归系数（贝塔）是线性的。非线性在于自变量。以下是一个二次多项式的数学表示（示例）：

身高=β0+β1×时间+β2×时间²

另一个例子涉及带有分类预测因子的线性回归，涉及根据个人的教育水平（例如，高中、学士或硕士）预测一个人的薪水。这涉及到使用虚拟变量来表示分类预测因子。以下是数学表示（假设“高中”是参考类别）：

薪资=β0+β1×学士+β2×硕士

虚拟变量的系数（即，β1 和β2）表示相对于参考类别的平均薪资的差异。

线性回归的指标

评估线性回归模型的性能对于理解模型如何拟合数据以及与其他模型进行比较至关重要。

没有单一的指标可以提供一个完整的模型性能图景。考虑多个指标并理解你正在解决的问题的上下文是至关重要的。以下是一些常用于评估线性回归模型的指标：

+   决定系数 (R²)

+   均方误差 (MSE)

+   根均方误差 (RMSE)

+   均方绝对误差 (MAE)

+   残差标准误差 (RSE)

+   F-统计量

+   T-统计量

+   调整后的 R²

+   AIC（赤池信息准则）

+   杜宾-沃森统计量

+   方差膨胀因子 (VIF)

下面的子节包含对前面列表中主题的简要描述。

决定系数 (R²)

R²（R-平方）表示回归模型中由自变量解释的因变量变差的比例。其值范围从 0 到 1，1 表示模型解释了响应数据围绕其均值的所有变异性。以下是公式：

R²=1−(残差平方和 (RSS))/(总平方和 (TSS))

均方误差 (MSE) 表示误差或偏差的平方的平均值（即估计值与估计值之间的差异）。以下是公式：

MSE = (∑(yi−y^i)²)/n

在前面的公式中，yi 是实际值，y^i 是预测值，n 是观测数。

RMSE 表示 MSE 的平方根。它提供了与原始数据相同单位的误差幅度。

MAE 表示观测实际结果与预测之间的平均绝对差异。公式如下：

MAE = (∑∣yi−y^i∣)/n

RSE 表示残差的均方根。它给出了残差围绕最佳拟合线的分散程度的度量。以下是公式：

RSE = sqrt((∑(yi−y^i)²)/df)

在前面的公式中，yi 是观测值，y 是预测值，df 是自由度（观测值的总数）。RSE 的值越小，表示拟合模型越好，因为数据点将更紧密地“聚集”在回归线周围。

F 统计量用于 ANOVA（方差分析）测试的上下文中，它提供了对因变量和自变量之间是否存在显著关系的统计检验。它比较了包含预测因子的完整模型与没有预测因子的模型。

t 统计量涉及测试一个给定的系数是否与 0 不同（无效应）。大的 t 统计量（或远离零的 t 统计量）和小的 p 值表明系数在统计上显著。

调整后的 R² 考虑了模型中的预测因子数量。与 R² 不同，它惩罚了额外预测因子的添加。当比较具有不同预测因子数量的模型时很有用。

阿卡伊克信息准则 (AIC) 和贝叶斯信息准则 (BIC) 用于模型选择。它们在模型的拟合优度和模型的复杂性之间取得平衡。具有最低 AIC 或 BIC 的模型更受欢迎。

杜宾-沃森统计量涉及对残差自相关的测试，并在时间序列数据中很有用。

方差膨胀因子 (VIF) 衡量当你的预测因子相关时，估计回归系数的方差增加的程度。如果没有因素相关，VIF 将等于 1。

使用 GPT-4 的随机数据线性回归

列表 5.1 展示了 linreg_gpt4.py 的内容，该内容说明了如何使用 NumPy 的 randn() API 生成数据集，然后使用 Matplotlib 的 scatter() API 绘制数据集中的点。

注意：列表 5.1 中的代码描述是由作者准备的，而不是由 ChatGPT 准备的。

列表 5.1: linreg_gpt4.py

"""

使用 Python 的 scikit-learn 库的一个简单线性回归示例。

1. 生成样本数据

首先，让我们生成一些合成数据。假设我们正在尝试建模经验年数与薪水之间的关系。

"""

import numpy as np

import matplotlib.pyplot as plt

# 生成合成数据

np.random.seed(0) # for reproducibility

# 随机经验年数在 0 到 2.5 年之间

X = 2.5 * np.random.rand(100, 1)

# Salary = base + 3*Experience + noise

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

我们假设基本薪水为 5，并且对于每增加一年经验，薪水增加 3 个单位。此外，还有一些随机噪声。

"""

"""

2. 训练线性回归模型

让我们拟合一个线性回归模型到这些数据。

"""

from sklearn.linear_model import LinearRegression

# 创建线性回归模型

reg = LinearRegression()

# 将模型拟合到数据

reg.fit(X, y)

# 获取回归系数

intercept = reg.intercept_[0]

slope = reg.coef_[0][0]

print(f"截距（基本薪水）：{intercept:.2f}")

print(f"斜率（每年经验增加的薪水）：{slope:.2f}")

"""

在上面的代码中：

使用 scikit-learn 的 LinearRegression() 进行线性回归模型。

fit 方法使用我们的合成数据训练模型。

intercept_ 提供了基本薪水（y 截距），coef_ 提供了每增加一年经验薪水增加的量（斜率）。

3. 可视化回归线

让我们绘制数据点和回归线。

"""

# 预测值

y_pred = reg.predict(X)

plt.scatter(X, y)

plt.plot(X, y_pred, color='red')

plt.xlabel("经验年数")

plt.ylabel("薪水")

plt.title("带有回归线的经验与薪水")

plt.show()

"""

在可视化中，数据点以蓝色点表示。

红线是线性回归模型的预测。

4. 评估模型

最后，让我们计算 RMSE（均方根误差）以评估我们模型的性能。

"""

from sklearn.metrics import mean_squared_error

rmse = np.sqrt(mean_squared_error(y, y_pred))

print(f"均方根误差：{rmse:.2f}")

"""

在这一步：

使用 scikit-learn 中的 mean_squared_error 函数计算均方误差。

均方误差的平方根给出了 RMSE，它表示模型预测误差与目标变量的相同单位。

整个过程使我们能够理解经验和薪水之间的关系，使用线性回归对其进行建模，并评估模型的性能。

"""

列表 5.1 从两个导入语句开始，接着是 X 和 y 的公式，这些公式基于 X 的值生成 y 的准随机值。接下来，基于 X 和 y 的值显示散点图。

列表 5.1 的下一部分初始化变量 reg 为 LinearRegression 类的实例，然后调用 fit() 方法将模型拟合到 CSV 文件 death.csv 中的数据。现在我们可以使用以下代码片段初始化变量 intercept 和 slope：

intercept = reg.intercept_[0]

slope = reg.coef_[0][0]

启动 列表 5.1 中的代码，你将看到两个图表显示。![图 5.1](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-#fig_5-1) 显示数据点，图 5.2 显示最佳拟合线。

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p136-1.jpg)

图 5.1 数据点集

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p136-2.jpg)

图 5.2 最佳拟合线

使用 GPT-4 对数据集进行线性回归

本节中的示例使用从以下网页下载的 death.csv 数据集进行线性回归：

[`data.world/nrippner/cancer-linear-regression-model-tutorial`](https://data.world/nrippner/cancer-linear-regression-model-tutorial)

为了方便起见，列表 5.2 显示了 CSV 文件 death.csv 的一部分内容。

列表 5.2: death.csv

县,县代码,met_objective_of_45_5_1,年龄调整后的死亡率,

死亡率下 95% 置信区间,死亡率上 95% 置信区间,

死亡率置信区间，平均死亡人数,

年份,最近两年趋势,最近五年死亡趋势,

趋势下 95% 置信区间,趋势上 95% 置信区间

趋势置信区间

美国,0,No,46,45.9,46.1,"157,376",下降,-2.4,-2.6,-2.2

"Perry County, Kentucky",21193,No,125.6,108.9,144.2,43,稳定,-0.6,-2.7,1.6

"Powell County, Kentucky",21197,No,125.3,100.2,155.1,18,稳定,1.7,0,3.4

"North Slope Borough, Alaska",2185,No,124.9,73,194.7,5,**,**,**,**

// 省略细节以节省篇幅

"Yakutat City and Borough, Alaska³",2282,*,*,*,*,*,**,**,**,**

"Yukon-Koyukuk Census Area, Alaska",2290,*,*,*,*,*,**,**,**,**

"Zapata County, Texas",48505,*,*,*,*,*,**,**,**,**

"Zavala County, Texas",48507,*,*,*,*,*,**,**,**,**

"Ziebach County, South Dakota",46137,*,*,*,*,*,**,**,**,**

让我们使用 GPT-4 对此数据集进行线性回归，从上传 death.csv 数据集开始。您可以在 ChatGPT 中通过选择“GPT-4”然后在屏幕底部点击“+”符号来完成此步骤，之后从您的笔记本电脑上传数据集。

到目前为止，我们已经准备好执行一系列多步骤操作来分析和准备 death.csv 数据集以进行线性回归，如下所示：

1. 描述 death.csv 数据集的特征。

2. 描述 death.csv 数据集的准备过程。

3. 描述探索性分析。

4. 描述模型选择。

5. 描述模型诊断。

上述列表中的每个步骤将在以下子节中进行讨论。请注意，某些子节相当长，因此您可能更有效地先快速浏览这些部分，然后再返回进行深入阅读。

DEATH.CSV 数据集特征描述

根据提供的数据集内容，以下是每个加粗特征的详细描述。

1. 县

描述：县或地区的名称

类型：分类（名义）

示例值：“美国”，“肯塔基州佩里县”，“肯塔基州鲍威尔县”

用法：可作为每个数据点的标识符

2. 县代码

描述：联邦信息处理标准（FIPS）代码，美国每个县的唯一标识符

类型：数值型（尽管用作分类标识符）

示例值：0（对于整个美国），21193，21197

用途：可作为唯一标识符，特别是用于与其他使用 FIPS 代码的数据集进行连接

3. Met_objective_of_45_5_1

描述：指示是否达到了特定的目标（可能是 45.5 的目标死亡率）

类型：分类型（二元）

示例值：“是”，“否”

用途：可用于评估和比较不同县与一个标准或目标的表现

4. age_adjusted_death_rate

描述：调整年龄的死亡率，以便在不同年龄分布的地区之间进行比较

类型：数值型

示例值：46，125.6，125.3

用途：理解总体死亡率的关键指标，独立于年龄分布。

5. lower_95_confidence_interval_for_death_rate & upper_95_confidence_interval_for_death_rate

描述：调整年龄的死亡率的 95%置信区间的下限和上限。给出了估计死亡率的不确定性或变异性。

类型：数值型

示例值：对于下限：45.9，108.9，100.2；对于上限：46.1，144.2，155.1

用途：有助于理解估计死亡率的可靠性和范围

6. average_deaths_per_year

描述：每年发生的平均死亡人数

类型：数值型

示例值：157,376，43，18

用途：提供死亡人数的绝对度量，可用于进一步分析或规划

7. recent_trend_2

描述：指示死亡率的最近趋势

类型：分类型（有序）

示例值：“下降”，“稳定”，“**”（可能表示缺失或未定义的数据）

用途：提供关于最近一段时间死亡率是增加、减少还是保持稳定的见解

8. recent_5_year_trend_2_in_death_rates

描述：最近五年死亡率的变动

类型：数值型

示例值：-2.4，-0.6，1.7

用途：指示死亡率的变动率，这对于预测或理解最近模式可能很有用

9. lower_95_confidence_interval_for_trend & upper_95_confidence_interval_for_trend

描述：最近五年死亡率的 95%置信区间的下限和上限

类型：数值型

示例值：对于下限：-2.6，-2.7，0；对于上限：-2.2，1.6，3.4

用途：提供趋势估计的范围，提供对其可靠性和变异性的见解

这些特征提供了与不同县死亡率相关的绝对和相对指标，允许进行综合分析、比较，并理解随时间变化的模式和趋势。

数据集的准备工作

为了描述 death.csv 数据集的准备过程，我们首先检查数据集的内容。我们检查其结构、前几行和总体统计信息。这将给我们一个关于我们正在处理的内容以及可能涉及到的准备工作的概念。

让我们从加载数据集并检查其结构开始，该结构如下：

行：3141 个条目（包括整个美国的条目）

列：11 列

每个字段的描述如下：

+   county: 县的名称（或“美国”表示全国平均水平）

+   fips: 县的联邦信息处理标准（FIPS）代码

+   met_objective_of_45_5_1: 表示是否达到某个目标（值似乎为“是”或“否”）

+   age_adjusted_death_rate: 调整年龄后的死亡率

+   lower_95_confidence_interval_for_death_rate: 死亡率 95%置信区间的下限

+   upper_95_confidence_interval_for_death_rate: 死亡率 95%置信区间的上限

+   average_deaths_per_year: 每年死亡的平均数

+   recent_trend_2: 死亡的近期趋势

+   recent_5_year_trend_2_in_death_rates: 死亡率的五年趋势

+   lower_95_confidence_interval_for_trend: 趋势 95%置信区间的下限

+   upper_95_confidence_interval_for_trend: 趋势 95%置信区间的上限

观察：

大多数列都是对象数据类型，这表明可能存在非数值值或用特殊字符（如 recent_trend_2 和 recent_5_year_trend_2_in_death_rates 列中的“**”）表示的缺失值。一些数值，如 average_deaths_per_year 列中的数值，用逗号表示，这就是为什么它们被视为对象数据类型。

准备过程：

根据数据集结构和观察结果，以下是 death.csv 数据集可能的准备过程。

1. 数据收集：

2. 数据可能来自各个县级行政区和国家级数据库或卫生组织。

3. 数据清洗：

4. 这包括处理缺失值。特殊字符如“**”可能被用来表示缺失或不可用数据。

5. 格式化：为了可读性，数字可能已被格式化，包括逗号。

特征工程：

置信区间的计算：死亡率趋势的 95%置信区间表明在数据收集后进行了统计计算。

年龄调整：死亡率已根据年龄进行调整，表示某种形式的标准化。

数据转换：数据可能已被转换或汇总，以表示县级行政区的平均值、趋势和其他指标。

数据标注：如 met_objective_of_45_5_1 之类的列表明，数据集中评估并标注了某些指标或目标。

数据验证：确保 FIPS 代码与正确的县匹配，并且数据集中没有重复或不一致。

为了进一步理解和提出改进建议，我们可以进行更深入的探索性数据分析（EDA）和质量检查，这些将在下一节中展示。

探索性分析

探索性数据分析（EDA）是一种分析数据集的方法，通常在正式建模或假设检验之前进行。EDA 的主要目标是了解数据、其结构、异常值和模式，并识别潜在的异常或特殊性。以下是针对 death.csv 数据集的 EDA 过程的详细描述：

1. 单变量分析

一次分析一个变量。对于数值变量，描述集中趋势（均值、中位数）和离散程度（范围、方差、标准差）。直方图、箱线图和密度图可能很有用。对于分类变量，使用条形图来了解每个类别的频率或比例。

2. 双变量分析

分析两个变量之间的关系。对于连续-连续对，使用散点图。对于分类-连续对，使用箱线图。对于分类-分类对，使用堆积柱状图或错综图。

3. 多变量分析

同时分析超过两个变量。使用相关矩阵或热图来了解连续变量之间的关系。使用配对图或三维散点图来直观表示关系。

4. 检查缺失值

识别有缺失值的列。分析“缺失”的模式。是随机缺失还是有某种模式？

5. 异常值检测

检测异常或可疑的值。使用视觉方法（例如，箱线图或散点图）或统计方法（例如，四分位数范围或 Z 分数）。

6. 特征工程

从现有变量创建新变量。例如，从数据集中，可以推导出一个特征，表示一个县的死亡率是否高于或低于全国平均水平。

7. 数据质量检查

确保数据是一致的、准确的和可靠的。例如，FIPS 代码应每个县唯一。

8. 相关性分析

这有助于我们了解不同连续变量之间的关系。对于连续变量，使用皮尔逊相关系数；对于分类变量，使用卡方 V 值。

9. 趋势分析

这对于我们的数据集中最近 5 年趋势 2 死亡率特征特别相关。这种分析有助于展示数据随时间的变化趋势。

10. 分布分析

这允许我们检查关键指标（例如，年龄调整死亡率）的分布。这允许我们检查正态性、偏度和峰度。

11. 地理空间分析

由于数据集包含县信息，因此（在附加的地理数据支持下）可以在地图上可视化指标，突出感兴趣的区域。

12. 汇总报告

这允许我们总结发现，可能以仪表板或报告的形式，突出数据中的重要见解。

13. 假设生成

根据发现，这使我们能够生成后续分析或建模中要测试的假设。在 EDA 之后，分析师应该对数据集的特征及其潜在局限性有更深入的了解。它提供了可以指导后续建模过程的见解，并确保建模过程中做出的假设是有效的。

DETAILED EDA ON THE DEATH.CSV DATASET

让我们对 death.csv 数据集进行详细的数据探索分析（EDA）。我们将采取以下步骤：

+   单变量分析 – 用于理解个体特征

+   双变量分析 – 用于理解特征对之间的关系

+   缺失值分析 – 用于识别和理解任何缺失数据

+   异常值检测 – 用于识别数据集中的潜在异常值

+   分布分析 – 用于理解重要指标的分布

让我们从单变量分析开始，以更深入地理解基于数值特征的单变量分析中的个体特征。

1. age_adjusted_death_rate

大多数县的人口调整死亡率在 20 到 60 之间。有几个县的死亡率非常高，这可以被认为是异常值。

2. lower_95_confidence_interval_for_death_rate & upper_95_confidence_interval_for_death_rate

死亡率上下 95%置信区间的分布与年龄调整死亡率的分布相似。这是预期的，因为它们提供了围绕死亡率的估计范围。

3. recent_5_year_trend_2_in_death_rates

死亡率的五年趋势似乎集中在零点，这表明对于许多县来说，死亡率保持稳定。有些县呈现上升趋势，有些县呈现下降趋势。

4. lower_95_confidence_interval_for_trend & upper_95_confidence_interval_for_trend:

这些分布代表了五年趋势死亡率的估计范围。它们提供了趋势估计的变异性和可靠性的背景。

接下来，让我们分析分类特征并了解它们的分布

来自分类特征的单一变量分析。

1. met_objective_of_45_5_1:

有相当数量的县没有达到目标（用“否”表示），而较少的部分已经达到目标（用“是”表示）。

2. recent_trend_2:

大多数县最近的趋势是“稳定”的。相当多的县呈现“下降”趋势。较少的县呈现死亡率的“上升”趋势。一些条目被标记为“**”，这很可能表示缺失或未定义的数据。

让我们使用双变量分析来探索特征对之间的关系。我们将首先通过热图分析数值特征之间的相关性。

从数值特征的关联热图中，我们发现以下信息。年龄调整后的死亡率与 lower_95_confidence_interval_for_death_rate 和 upper_95_confidence_interval_for_death_rate 高度相关。这是预期的，因为置信区间提供了死亡率的不确定性范围。同样，recent_5_year_trend_2_in_death_rates 与 lower_95_confidence_interval_for_trend 和 upper_95_confidence_interval_for_trend 高度相关。其他变量对之间的相关性相对较低。

接下来，让我们分析数据集中的缺失值，以了解是否存在任何缺失数据，并决定如何处理它。

1. recent_5_year_trend_2_in_death_rates, lower_95_confidence_interval_for_trend, and upper_95_confidence_interval_for_trend:

所有这些都有相同的缺失值数量，为 447（或约 14.23%的数据）。这表明当趋势数据缺失时，其对应的置信区间也缺失。

2. age_adjusted_death_rate, lower_95_confidence_interval_for_death_rate, and upper_95_confidence_interval_for_death_rate:

所有这些都有相同的缺失值数量，为 328（或约 10.44%的数据）。这与趋势列相似：当死亡率数据缺失时，其对应的置信区间也缺失。

接下来，让我们检查异常值检测。我们将使用箱线图来直观地识别数值列中的潜在异常值：

1. age_adjusted_death_rate:

有几个数据点位于上级须之上，可以被认为是潜在的异常值。这些代表死亡率异常高的县。

2. lower_95_confidence_interval_for_death_rate & upper_95_confidence_interval_for_death_rate:

这两个特征在其各自的上级须上显示出潜在的异常值，与年龄调整后的死亡率中的异常值一致。

3. recent_5_year_trend_2_in_death_rates:

数据点既在须上也在须下，表明最近五年死亡率趋势异常高或低的县。

4. lower_95_confidence_interval_for_trend & upper_95_confidence_interval_for_trend:

这两个特征显示出潜在的异常值，与最近五年趋势中的异常值一致。

接下来，让我们分析一些关键指标的分布，重点关注它们的偏度和峰度。偏度可以提供关于分布对称性的见解，而峰度揭示了其“尾部”特征。

1. age_adjusted_death_rate

偏度（0.55）：分布适度右偏斜，意味着右侧有一个尾巴。这表明有一些县死亡率异常高。

偏度（1.29）：此值表明分布的尾部比正态分布更重，表明存在异常值。

2. lower_95_confidence_interval_for_death_rate & upper_95_confidence_interval_for_death_rate

两者都具有偏斜值，表明分布呈右偏态，上置信区间更为偏斜。它们的峰度值表明比正态分布更重的尾部。

3. 最近 5 年趋势 2 的死亡率

偏斜（-2.35）：分布显著左偏斜，意味着左侧有一个尾部。这表明许多县的死亡率呈下降趋势。

峰度（58.03）：这个高值表明分布中存在极端异常值或尖锐的峰值。

4. 趋势下 95%置信区间 & 趋势上 95%置信区间

这两个特征都表现出高度偏斜和峰度值，表明存在非正态分布，尾部明显且可能存在异常值。

这些从分布分析中获得的见解可以指导进一步的统计分析、假设检验和建模工作。在 EDA 的下一步中，我们将深入双变量和多变量分析，以了解特征之间的关系。

双变量和多变量分析

让我们通过双变量和多变量分析来探索特征之间的关系。

双变量分析

+   使用连续变量之间的散点图来可视化关系。

+   使用箱线图来查看分类-连续变量对，以了解连续变量在不同类别中的变化。

+   使用交叉表或堆叠条形图来理解不同组别中类别的分布。

多元分析

+   使用成对图来同时查看多个连续变量之间的关系。

+   使用相关热图来理解连续变量之间的线性关系。

让我们从双变量分析开始。我们将创建年龄调整死亡率和其他连续特征之间的散点图，以了解它们之间的关系。散点图提供了年龄调整死亡率和其他连续特征之间关系的见解。

1. 年龄调整死亡率与死亡率下 95%置信区间 & 年龄调整死亡率与死亡率上 95%置信区间

这些图显示出强烈的线性关系，这是预期的，因为置信区间提供了年龄调整死亡率的界限。

2. 年龄调整死亡率与最近 5 年趋势 2 的死亡率

这里的关系似乎不是线性的。虽然许多县在零点附近有一个稳定的趋势，但不同死亡率的数据点分布较广，表明总体死亡率不一定能预测最近的趋势。

3. 年龄调整死亡率与趋势下 95%置信区间 & 年龄调整死亡率与趋势上 95%置信区间

这些图显示出分散的模式，表明趋势的置信区间与年龄调整死亡率之间没有直接的线性关系。

接下来，让我们使用箱线图分析分类特征最近趋势 2 和连续特征年龄调整死亡率之间的关系。这将帮助我们了解年龄调整死亡率在不同最近趋势（上升、下降、稳定）中的变化情况。箱线图说明了年龄调整死亡率在不同最近趋势中的分布。

1. 下降

死亡率趋势下降的县往往有较高的死亡率中位数，但分布范围较广，表明这些县之间减少的程度存在差异。

2. 稳定

死亡率趋势稳定的县与死亡率趋势下降的县相比，死亡率中位数较低，四分位距（IQR）也更窄，表明这些县之间的变异性较小。

3. 上升

死亡率呈上升趋势的县与死亡率呈下降趋势的县相比，中位数较低，但高于死亡率稳定的县。分布看起来更紧凑，异常值更少。

4. **（未定义或缺失数据）

这个类别似乎与稳定趋势有类似的分布，但重要的是要调查和理解这些未定义条目的含义或原因。

接下来，对于多元分析，让我们为连续特征的子集创建一个配对图，以可视化成对关系和分布。我们将关注年龄调整死亡率、最近 5 年趋势 2 在死亡率中的变化，以及它们各自的置信区间。配对图提供了所选特征的成对关系和个体分布的概述。

1. 对角线核密度图

这些图显示了单个特征的分布。如前所述，年龄调整死亡率呈中等右偏斜，而最近 5 年趋势 2 在死亡率中呈左偏斜。

2. 对角线散点图

年龄调整死亡率和其置信区间（上下）之间的散点图显示出预期的强线性关系。年龄调整死亡率和最近 5 年趋势 2 在死亡率中的关系没有显示出明显的趋势，这证实了我们的早期观察。

现在，为了进一步探索多元关系，让我们使用更广泛的连续特征集创建一个相关性热图。这将使我们能够了解这些特征之间的线性关系。扩展的相关性热图加强了我们的一些早期观察，并提供了额外的见解。

1. 年龄调整死亡率和其置信区间

如前所述，年龄调整死亡率和其上下 95%置信区间之间存在高度相关性。这是预期的，因为这些区间提供了主要指标的范围。

2. 最近 5 年趋势 2 在死亡率中的变化及其置信区间

同样，最近 5 年趋势 2 在死亡率中的变化也与其相应的置信区间表现出高度相关性。

3. 年龄调整死亡率和最近 5 年趋势 2 在死亡率中的变化

这两个之间的相关性相对较低，这表明总体死亡率与最近五年死亡率的趋势不是强线性相关的。

置信区间

死亡率和趋势的置信区间在一定程度上是相关的，这是有道理的，因为它们是从相同的基本数据中得出的。我们已经对 death.csv 数据集进行了全面的 EDA。我们研究了单个特征，分析了双变量关系，并探索了多元关联。从这次 EDA 中获得的认识可以指导后续的建模、假设检验和进一步的分析。

模型选择过程

模型选择过程涉及为特定数据集和问题选择最佳的机器学习或统计模型。这个过程至关重要，因为你的预测或推理的成功很大程度上取决于你选择的模型。以下是模型选择过程的详细描述。

1. 定义问题

明确定义目标：是分类、回归、聚类还是其他类型的问题？确定评估指标。例如，对于平衡的分类问题，准确率可能适用，但精确率、召回率或 F1 分数可能更适合不平衡的数据集。对于回归问题，你可能需要考虑如 RMSE 或 MAE 等指标。

2. 基准模型

从一个简单的模型开始，作为基准。这可能是一个用于回归问题的线性回归或用于分类任务的逻辑回归。你应该有一个基本的性能度量，可以用来比较更复杂的模型。

3. 选择候选模型

根据问题类型和数据特征，筛选出一组已知适用于此类问题的算法。例如，对于结构化表格数据，可以考虑决策树、随机森林、梯度提升机器和 SVMs 等算法。对于如图像这样的非结构化数据，你可能需要考虑深度学习模型。

4. 数据准备

不同的算法可能需要不同的数据预处理步骤。对于 SVMs 或神经网络等算法，需要对数据进行归一化或标准化。使用如独热编码等技术处理分类变量，特别是对于不原生处理分类数据的算法。确保数据被分成训练集、验证集（以及可能的测试集）。

5. 超参数调优

几乎每个算法都有需要设置的超参数，这些参数可以极大地影响性能。使用网格搜索、随机搜索或贝叶斯优化等技术来找到每个候选模型的最佳超参数。

6. 交叉验证

为了确保你的模型性能稳健且不过度乐观，请使用交叉验证。K 折交叉验证是一种常见技术。交叉验证为模型在未见数据上的性能提供了一个更通用的指标。

7. 模型评估

使用你选择的指标在验证集上评估每个模型。将不同模型与基线模型和彼此的性能进行比较。

8. 集成

如果单个模型表现不够好，考虑结合多个模型。像 bagging、boosting 或 stacking 这样的技术通常会比单个模型有更好的性能。

9. 模型可解释性

并非总是关于获得最高的准确率；有时理解模型为何做出某些决策是至关重要的。根据领域（如医疗保健或金融），你可能会优先考虑更简单、更可解释的模型，即使后者有稍微更好的性能。

10. 最终模型选择

根据验证性能、可解释性和业务目标选择最终模型。在这个模型上训练结合的训练和验证集，以在测试集上做出最终预测。

11. 部署和监控

一旦最终模型被选定并评估，它就可以在生产环境中部署。持续监控模型在现实世界中的性能。随着时间的推移，数据的变化，模型可能需要重新训练或微调。

12. 反馈循环

随着模型的使用和预测的收集，这些数据可以反馈到训练数据集中，以用于未来模型的改进。

模型选择过程的目标并不总是找到具有最高性能指标的模型。它是找到一个满足业务目标、可靠、可解释（如果需要）并且对未见数据泛化良好的模型。

使用 DEATH.CSV 数据集进行线性回归的代码

让我们使用 death.csv 数据集来实现线性回归。以下是我们将遵循的步骤：

1. 数据预处理：处理缺失值并准备数据以进行建模。

2. 特征选择：选择我们将用于预测因变量的自变量（特征）。

3. 数据拆分：将数据集拆分为训练集和测试集。

4. 模型训练：在训练集上训练一个线性回归模型。

5. 模型评估：评估模型在测试集上的性能。

6. 模型解释：解释模型的系数。

在这个演示中，让我们使用年龄调整死亡率作为因变量，最近 5 年死亡率趋势 _2 作为自变量。

让我们从数据预处理开始。线性回归模型在测试数据上的性能如下：

均方误差 (MSE)：145.22

R 平方 (R²) 值：0.1114

R2R2 值表明，大约 11.14%的年龄调整死亡率变异性可以通过最近 5 年死亡率趋势 _2 来解释。这个值并不高，表明仅使用最近五年趋势的线性模型可能不足以捕捉死亡率的全部变异性。

最后，让我们通过检查模型的系数来继续进行模型解释。线性回归模型可以用以下方程表示：

age_adjusted_death_rate = 1.5506*recent_5_year_trend_2_in_death_rates + 54.9239

解释系数得出以下结果：

最近 5 年死亡率趋势 _2 的系数等于 1.5506。对于最近 5 年死亡率趋势 _2 每增加一个单位，年龄调整死亡率增加约 1.5506 个单位，保持其他所有因素不变。

截距（54.9239）：

当最近 5 年死亡率趋势 _2 为零时，预测的年龄调整死亡率约为 54.9239。

考虑到 R2 值适中，如果需要提高预测能力，考虑其他特征或更高级的建模技术是必要的。此线性模型提供了两个变量之间基本理解和关系的理解。

列表 5.3 显示了 linreg2_gpt4.py 的内容，说明了如何使用死亡.csv 数据集的行子集执行线性回归。

列表 5.3：linreg2_gpt4.py

import pandas as pd

from sklearn.linear_model import LinearRegression

from sklearn.model_selection import train_test_split

from sklearn.metrics import mean_squared_error, r2_score

# CSV 文件 death_clean.csv 将在后面描述：

death_df = pd.read_csv('death_clean.csv')

# 第一步：数据预处理

# 删除感兴趣列中的缺失值行

processed_data = death_df.dropna(subset=["age_adjusted_death_rate", "recent_5_year_trend_2_in_death_rates"])

# 第二步：特征选择

X = processed_data[["recent_5_year_trend_2_in_death_rates"]] # 自变量

y = processed_data["age_adjusted_death_rate"] # 因变量

# 第三步：数据拆分

X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)

# 第四步：模型训练

linear_reg = LinearRegression()

linear_reg.fit(X_train, y_train)

# 第五步：模型评估

y_pred = linear_reg.predict(X_test)

mse = mean_squared_error(y_test, y_pred)

r2 = r2_score(y_test, y_pred)

# 作者添加的代码片段：

print("mse:",mse,"r2:",r2)

列表 5.3 以几个导入语句开始，随后使用 CSV 文件 death_clean.csv 的内容初始化 Pandas 数据框 death_df。请注意，此 CSV 文件是由作者创建的，通过删除包含一个或多个星号的死亡 _clean.csv 中的数据点。

列表 5.3 的下一段初始化了 Pandas 数据框 processed_data，该数据框通过以下代码片段从 Dataframe death_df 中删除了两列：

processed_data = death_df.dropna(subset=["age_adjusted_death_rate", "recent_5_year_trend_2_in_death_rates"])

现在我们已经有一个验证过的数据集，我们可以使用以下代码片段初始化自变量 X 和因变量 y：

X = processed_data[["recent_5_year_trend_2_in_death_rates"]]

y = processed_data["age_adjusted_death_rate"]

接下来，对数据集执行标准的训练/测试分割，其中 80%的数据用于训练，20%的数据集用于测试，如下代码片段所示：

X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)

第四步涉及将 linear_reg 初始化为 LinearRegression 类的实例，之后我们可以将此实例拟合到数据上。列表 5.3 的最后一部分通过调用训练模型 linear_reg 的 predict()方法进行模型评估。此时，我们可以将 use 初始化为均方误差（MSE）和 R² 分数，然后打印它们的值。现在运行列表 5.3 中的代码，你将看到以下输出：

mse：145.2243931078172 r2：0.11141880352501743

描述模型诊断

模型诊断在识别回归模型中的潜在问题以及确保线性回归的基本假设得到满足方面起着至关重要的作用。以下是线性回归的主要诊断和相关的检查：

1.线性

2.误差独立性

3. 同方差性

4. 残差的正态性

5. 多重共线性

6. 异常值和杠杆点

7. 模型指定

线性的假设意味着独立变量与因变量之间的关系应该是线性的。

诊断工具：

残差与拟合值图：如果此图中存在模式（如曲线），则表明存在非线性。观测值与预测值的散点图。

误差独立性的假设意味着残差（误差）应该是独立的。

诊断工具：

杜宾-沃森检验检测残差中是否存在自相关（即存在给定时间滞后值之间的关系）。

假设同方差性意味着残差的方差应该在独立变量（s）的所有水平上保持恒定。

诊断工具：

+   残差与拟合值图：如果存在漏斗形状，则表明存在异方差性（非恒定方差）。布雷斯-帕甘或怀特检验用于统计检验异方差性。

假设残差的正态性意味着残差应该近似服从正态分布。

诊断工具：

+   直方图或核密度图：用于检查正态性。

+   Q-Q（分位数-分位数）图：如果残差位于 45 度参考线上，则它们近似服从正态分布。

+   Shapiro-Wilk 检验：一个正式的正态性检验。

假设多重共线性意味着独立变量之间不应高度相关。

诊断工具：

+   VIF：VIF 值大于 10 表示存在高度多重共线性。

+   相关矩阵或热图：用于检查变量之间的相关性。

检测异常值和杠杆点很重要，因为异常值可能会过度影响模型，导致不可靠的估计。

诊断工具：

+   标准化残差与杠杆作用图：有助于识别对回归线有高杠杆作用的点。

+   库克距离：衡量删除给定观测值的影响。

正确的模型指定意味着没有遗漏变量偏差，也没有包含不必要的变量。

诊断工具：

+   添加变量（部分回归）图：有助于检查变量是否向模型添加信息。

+   RESET（回归指定误差测试）：测试模型是否指定不当。

对于我们使用 death.csv 数据集的线性回归模型，让我们进行一些这些诊断，从检查线性、同方差性和残差的正态性开始。根据诊断图，我们有以下结果：

残差与拟合值图：

线性：残差与拟合值之间似乎没有明显的模式，这表明线性假设并未被强烈违反。

同方差性：残差的分布似乎在整个拟合值范围内相对均匀，这表明同方差性假设并未被强烈违反。

残差直方图：

直方图显示了残差的分布。虽然它不是完美的正态分布，但分布没有极端的偏离正态性。

Q-Q 图：

Q-Q 图显示了残差分布与正态分布的匹配程度。残差大体上遵循 45 度参考线，尤其是在中心区域。有一些偏差，尤其是在尾部，表明与完美的正态性存在一些小的偏差。

为了进一步确保模型的可靠性，还应考虑额外的诊断，如检查多重共线性（对于具有多个预测因子的模型更相关）、异常值和高杠杆点。对于这个只有一个预测因子的简单线性模型，多重共线性不是问题。

描述额外的模型诊断

在提示 ChatGPT 深入探讨我们线性回归的额外模型诊断后，ChatGPT 回复了以下列表项之后的文本：

+   影响图

+   库克距离

+   VIF（方差膨胀因子）

+   条件数

影响图有助于识别对回归方程有高度影响的点。

库克距离衡量删除给定观测值的影响。库克距离大的数据点可能具有影响力。

VIF：虽然对于只有一个预测因子的简单模型来说，多重共线性不是问题，但在未来扩展模型时，了解这一诊断是有好处的。

条件数：高条件数可能表明多重共线性以及回归中的潜在数值不稳定性。

让我们从影响图和 Cook 距离开始。影响图提供了观测值对回归影响的视觉表示。点的尺寸与 Cook 距离成正比，而更靠右的点具有更高的杠杆作用。大多数观测值聚集在左侧，表明杠杆作用低。然而，一些点，尤其是那些尺寸较大的点，可能具有影响力。

Cook 距离：

我们已经识别出 73 个 Cook 距离大于阈值“4nn4”的观测值，其中“nn”是观测值的数量。这些可能是对模型拟合产生不当影响的潜在重要点。

存在重要观测值表明有几项可能的行动方案：

+   调查重要点：在考虑删除任何数据点之前，了解它们为什么可能具有影响力是至关重要的。它们是错误，还是代表真正的极端情况？

+   稳健回归：如果数据集有重要点或异常值，考虑使用降低异常值影响力的稳健回归方法。

GPT-4 的更多推荐

根据使用 death.csv 数据集进行的线性回归模型的结果和诊断，以下是一些建议。

1. 处理异常值

调查在诊断过程中识别出的潜在异常值。确定它是否是数据错误或实际极端值。如果是错误，则更正或删除它。如果是真实的，可以根据上下文及其对模型可能产生的影响来决定是否保留它。

2. 扩展模型

当前模型只使用一个预测因子。考虑添加数据集中其他相关的预测因子以提高模型的可解释性。在添加更多预测因子时，注意多重共线性，并确保再次运行诊断。

替代模型：

考虑到适中的 R2 值，可以考虑使用更复杂的回归模型，如多项式回归、岭回归或 Lasso 回归，甚至非线性模型。

值得探索的集成方法，如随机森林或梯度提升机。

3. 特征工程

探索创建新特征或转换现有特征。例如，如果某些关系不是线性的，非线性变换（例如，对数）可能会有所帮助。

4. 更有策略地处理缺失值

我们为了简单起见删除了包含缺失值的行。根据缺失数据的性质，考虑使用插补技术以利用更多数据。

5. 模型验证

使用如 k 折交叉验证等技术确保稳健的验证。这提供了对未见数据上模型性能的更可靠估计。

6. 领域知识

与领域专家合作，更好地理解特征，验证模型的发现，并可能识别出新的相关特征。

7. 模型可解释性

如果目标是理解影响死亡率的因素，可以考虑使用决策树或 SHAP 值与集成方法相结合的模型，以获得更好的可解释性。

8. 定期更新

根据数据随时间的变化情况，模型可能需要定期更新或微调。设置一个监控机制。

9. 数据质量和收集

确保数据质量。如果数据收集中存在系统性错误或偏差，即使是最好的模型也可能产生误导性的结果。

总结来说，虽然最初的线性回归模型提供了基础理解，但仍有很大的改进和精炼空间。最佳的方法是迭代式地进行：精炼模型，验证它，解释结果，并在必要时进行调整。

**摘要**

本章是这本书的第一章，其中包含了由 GPT-4 生成的材料。你看到了 GPT-4 如何描述数据集的准备过程以及探索性分析。

然后你看到了对 death.csv 数据集的详细 EDA 分析，模型选择过程以及该数据集的实际线性回归代码。

此外，你学习了 GPT-4 生成的模型诊断，随后是 GPT-4 生成的推荐列表。

**第六章**

**使用 GPT-4 的机器学习分类器**

本章包含 GPT-4 基于 Python 的代码示例，涵盖了众多机器学习分类算法。

本章的前一部分向 GPT-4 请求有关机器学习分类器的信息。本节还包含由 GPT-4 生成的高层次 scikit-learn 描述。

本章的第二部分向 GPT-4 请求描述著名的机器学习算法，如 kNN、逻辑回归、支持向量机（SVM）、决策树、随机森林和朴素贝叶斯。本节还包含每个这些机器学习算法的 Python 代码示例。

本章包括 GPT-4 生成的用于各种算法（包括 kNN、决策树、随机森林和 SVMs）的机器学习模型的 Python 代码。你还将看到一些关于相同算法的内容，所有这些内容都是由 GPT-4 生成的。然而，首先，我们将从讨论这些算法开始；然后你可以检查包含 GPT-4 生成的 Python 代码的部分。

在阅读本章内容时，请记住，为了提高 GPT-4 生成的材料的可读性，偶尔会包含一些额外的注释。例如，在 GPT-4 的文本部分之后，你可能会看到以下内容：“注意：这是由 GPT-4 生成的文本的结束。”

**根据 GPT-4 的机器学习**

机器学习（ML）是人工智能（AI）的一个子集，专注于构建可以从数据中学习和基于数据做出决策的系统。与被明确编程执行任务不同，机器学习算法使用统计技术来学习数据中的模式，并根据它做出预测或决策。以下是一个更深入的讨论。

重要概念

+   学习：

+   机器学习涉及训练算法使用数据集识别模式。数据的数量和质量越好，算法的学习效果越好。

+   模型：

+   一旦算法从数据中学习，它就会形成一个模型。然后可以使用该模型进行预测或决策，而无需明确编程执行任务。

+   预测：

+   这涉及使用模型为新输入确定输出。例如，在垃圾邮件检测中，预测将是新电子邮件是否为垃圾邮件。

机器学习的类型

+   监督学习：

+   算法在标记数据集上训练，这意味着数据集中的每个示例都与正确的输出配对。目标是学习从输入到输出的映射。

+   例子：回归、分类

+   无监督学习：

+   算法在未标记数据集上训练，试图学习数据的潜在结构。

+   例子：聚类、降维

+   半监督学习：

+   这种方法使用标记和未标记数据训练。当获取完整标记数据集昂贵或耗时时，通常使用。

+   强化学习：

+   算法通过与环境交互并接收关于奖励或惩罚的反馈来学习。

+   例子：训练机器人穿越迷宫

机器学习应用

机器学习有广泛的应用，包括以下内容：

+   图像和语音识别：这用于面部识别或语音激活助手。

+   医疗诊断：根据症状或医学影像协助医生诊断疾病是一个重要的应用。

+   财务预测：机器学习可用于预测股市趋势。

+   推荐系统：这些系统可以根据用户偏好建议产品、电影或音乐。

+   自然语言处理：NLP 常用于聊天机器人和翻译服务。

+   自动驾驶汽车：机器学习使汽车能够在没有人为干预的情况下导航。

机器学习中的挑战

+   过拟合：当模型学习训练数据过于“紧密”时，会在新的、未见过的数据上表现不佳。

+   欠拟合：当模型过于简单，无法捕捉数据的潜在结构时发生。

+   偏见与公平性：确保机器学习模型不会持续或放大数据中存在的偏见对于应用的有用性至关重要。

+   可解释性：这一方面涉及使复杂模型对人类可理解。

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

2. 模型选择和评估：提供工具帮助分割数据集、网格搜索、交叉验证以及各种指标来评估机器学习模型的性能

3. 数据预处理：提供数据预处理的函数，如归一化、标准化和编码分类变量

4. 特征提取：包含从图像和文本中提取特征的工具（例如，使用词袋方法）

5. 管道：提供了一种按顺序应用一系列转换和最终估计器的工具。管道的中间步骤必须是转换器（例如，缩放器或 PCA），而最后的估计器可以是任何对象（例如，分类器，回归器）

6. 兼容性：设计用于与 Python 数值和科学库 NumPy 和 SciPy 互操作

优势

+   简单性：Scikit-learn 的 API 设计旨在保持一致性且易于使用。

+   完备的文档：详细的文档带有示例，使初学者易于理解

+   性能：流行算法的高效实现

+   社区支持：作为开源且受欢迎的库，拥有庞大的用户和贡献者社区，这导致定期更新和快速修复错误。

局限性

1. 神经网络：虽然 scikit-learn 确实有基本的神经网络工具，但它并不是专门用于深度学习的。像 TensorFlow、Keras 或 PyTorch 这样的库更适合深度学习任务。

2. 可扩展性：对于非常大的数据集或分布式计算，Apache Spark 的 MLlib 或 Dask 等工具可能更合适。

典型用法

Scikit-learn 通常用于传统机器学习任务，其中数据适合内存且不需要深度学习。它特别适合原型设计和构建端到端机器学习管道。

总结来说，scikit-learn 是 Python 中一个功能丰富且全面的机器学习库，其简单性和强大功能的结合使其成为许多数据科学家和研究人员的首选。

**什么是 kNN 算法？**

k-最近邻（kNN）算法是一种简单、直观且非参数的机器学习算法，用于分类和回归任务。以下是它是如何工作的。

基本概念

给定一个新的、未见过的观察值，kNN 在训练集中搜索与观察值最近的 k 个训练示例，并返回这些 k 个邻居中具有最高代表性的输出值（类别或数值）。

步骤

1. 选择 k 的数值：确定你想要考虑的邻居数量。通常，k 是一个奇数，以防止平局情况（在分类的情况下）。

2. 距离度量：确定一个距离度量来衡量实例的“接近度”。最常用的度量是欧几里得距离，但根据数据的性质，还可以使用曼哈顿、闵可夫斯基和汉明距离等其他度量。

3. 搜索：对于新的数据点，计算它与训练集中所有点的距离，并识别最近的 k 个点。

4. 聚合

+   对于分类：返回 k 个邻居中出现频率最高的类别

+   对于回归：返回 k 个邻居的输出值的平均值（或中位数）

优点

+   简单直观：对数据的分布或决策边界没有假设

+   多功能：适用于分类和回归

+   非参数：没有显式的训练阶段，并且可以处理决策边界非常不规则的数据集。

缺点

+   计算密集型：它需要为每个预测计算所有训练样本的距离，对于大数据集来说可能很慢。

+   内存使用：它存储整个数据集，因此内存消耗可能很高。

+   对无关特征敏感：距离度量可能会受到对分类或回归不重要的特征的影响。

+   对数据规模敏感：具有较大尺度的特征可能会主导距离度量，因此通常需要归一化或标准化数据。

用例

当以下情况成立时，kNN 特别有用：

+   数据已标记。

+   数据集不是太大（以避免计算效率低下）。

+   决策边界非常不规则。

尽管简单，kNN 可以非常有效，尤其是在潜在的决策边界复杂且不易被其他线性模型捕获的情况下。在实践中，由于其计算和内存需求，kNN 通常更多地用作基线或在较小的数据集中使用。

**KNN 算法中 K 值的选取**

在 k-最近邻（kNN）算法中确定 k 的最佳值至关重要，因为这个值可以显著影响模型的表现。特别是，k 的值可以影响预测的偏差和方差。以下是一些在选择 kNN 算法中 k 的最佳值时需要考虑的点：

+   交叉验证

+   偏差-方差权衡

+   距离度量

+   平方根规则

+   领域知识

+   偶数 k 与奇数 k

+   计算效率

+   数据集的多样性

交叉验证

确定最优 k 值最常见的方法是通过交叉验证，尤其是 k 折交叉验证。首先，将数据集分为训练集和验证集。对于每个潜在的 k 值，在训练集上训练 kNN 算法，并在验证集上进行验证。测量每个 k 在验证集上的准确度（或其他相关指标）。选择在验证集上表现最佳的 k 值。

偏差-方差权衡

小的 k 值（例如，k=1）意味着数据中的噪声将对结果有更大的影响，导致模型具有高方差但低偏差。大的 k 值具有平滑效应，可以减少方差但增加偏差。这可能会使算法对异常值更具抵抗力，但可能产生更不明显的类别边界。

距离度量

距离度量（例如，欧几里得、曼哈顿和闵可夫斯基）的选择可以影响最优 k 值。在优化 k 的过程中，尝试不同的距离度量。

平方根规则

一个常见的启发式方法，尤其是在开始寻找最优 k 值时，是将 k 设置为训练数据集中数据点数量的平方根。这不是一个严格的规则，但可以作为起点。

领域知识

有时，领域知识或问题的具体背景可以指导 k 的选择。例如，在你知道数据点对或三元组通常相关的问题中，k=2 或 k=3 可能是一个合理的起点。

偶数 k 与奇数 k

通常建议选择奇数 k 以避免平局，即两个类别具有相同数量的最近邻。然而，请注意，许多 kNN 实现都有平局解决机制。

计算效率

随着 k 的增加，计算可能会变得更加密集（因为你正在考虑更多的邻居）。然而，如果 k 太小，模型可能会对数据中的噪声过于敏感。

数据集的多样性

如果数据集有许多重叠的类别，较小的 k 可能更合适。如果类别更加明显，较大的 k 可以工作得很好。

在实践中，尝试 k 的一系列值，并对每个值进行性能验证。可视化工具，如显示验证准确度与不同 k 值关系的图表，有助于做出决策。

KNN 算法的“肘部方法”

如果你熟悉 k 均值聚类算法，你无疑知道用于确定 k 最优值的“肘部方法”。需要考虑的自然问题是，这种方法是否可以用于确定 kNN 算法中 k 的最优值。

肘部方法主要与 k-means 聚类算法相关联，其中它用于确定最佳簇数量。在 k-means 的上下文中，“拐点”是在簇内平方和（WCSS）与簇数量之间的图表中的点。这一点代表了精度（更多簇）和计算效率（较少簇）之间的平衡。

对于 kNN，主要目标是分类（或回归），而不是聚类。kNN 中的参数 k 代表在做出预测时考虑的邻居数量，而不是数据中的簇数量。

然而，使用图表来识别衰减收益（“拐点”）的概念可以应用于 kNN 的超参数调整上下文中。

验证错误

您可以绘制一系列 k 值的验证错误（或准确率）。随着 k 的增加，模型可能会在减少方差的同时最初变得更加准确。然而，在某个点上，增加 k 可能会引入更多偏差，导致错误增加或准确率下降。

在这种情况下，“拐点”将是增加 k 后不再导致验证错误（或准确率）显著提高的点。

距离考虑

衰减收益的概念也可以应用于 kNN 的距离度量。例如，可以检查不同 k 值下到第 k 个最近邻的平均或中位数距离，以了解数据的密度和分布。

虽然“拐点”的概念可以应用于 kNN 超参数调整的上下文中，但区分 k-means（确定簇数量）中肘部方法的用途与其在 kNN（调整邻居数量以实现最佳预测）中的潜在应用是至关重要的。

基于 kNN 算法的机器学习模型

本节包含 GPT-4 使用 kNN 算法和 death.csv 数据集生成机器学习模型的示例。本节的前半部分包含 GPT-4 执行的步骤解释，以及“标记”引用代码中的适当部分，随后是列表 6.1，其中包含 GPT-4 生成的基于 Python 的代码。

前半部分从以下提示开始，这是给 GPT-4 的，以便生成使用 kNN 算法的机器学习模型的 Python 代码：

“请生成一个使用 kNN 算法和 death.csv 数据集的机器学习模型。”

[注意：以下文本由 GPT-4 生成，并对格式进行了调整以提高可读性]

GPT-4 的响应如下。

在我们使用 kNN（k-最近邻）算法创建机器学习模型之前，我将概述我们将遵循的步骤：

+   加载数据：读取 death.csv 数据集。

+   数据预处理：清理和预处理数据集，使其适合建模。

+   特征选择：选择将用于训练模型的有关特征。

+   训练-测试集划分：将数据集划分为训练集和测试集。

+   模型训练：使用 kNN 算法在训练集上训练模型。

+   模型测试：评估模型在测试集上的性能。

+   性能指标：计算如准确率等指标，以了解模型的性能表现如何。

让我们先加载数据集并查看其前几行。

现在我们已经加载数据集，让我们继续进行数据预处理步骤：

+   处理缺失值：我们需要确保没有缺失值，或者如果存在，则处理它们。

+   编码分类特征：如果有任何分类特征，我们需要将它们编码为数值，以便 kNN 算法使用。

+   特征选择：我们将选择建模过程中相关的特征。

+   缩放：kNN 对特征缩放敏感，因此对数据集进行归一化或标准化很重要。

让我们先处理缺失值并检查每一列的数据类型。数据集中没有缺失值，这是个好消息。然而，在检查数据类型时，我们可以看到几个本应表示为数值的列（如 age_adjusted_death_rate、average_deaths_per_year 等）被表示为对象。这表明这些列中可能存在非数值字符或符号。

继续进行：

我将转换这些列为数值数据类型，并处理任何非数值字符。

+   编码分类特征。

+   选择建模相关的特征。

+   归一化数据集，为 kNN 算法做准备。

列已经成功转换为适当的数值数据类型。

接下来，我们需要：

+   编码分类特征：将分类特征转换为数值。

+   特征选择：决定使用哪些特征进行建模。

+   缩放：归一化数据集。

为了简单起见，我们将直接使用数值特征，并使用独热编码将分类特征 recent_trend_2 编码。然后我们将数据分为训练集和测试集，缩放特征，并继续进行 kNN 建模。

让我们先对分类特征进行编码并分割数据。

数据已经成功预处理并分为训练集和测试集。现在训练集中有 2512 个样本，测试集中有 629 个样本，每个集中有 12 个特征。

接下来，我们将继续进行：

+   模型训练：在训练数据上训练一个 kNN 分类器。

+   模型测试：使用训练好的 kNN 分类器在测试数据上预测目标变量。

+   性能指标：使用准确率评估模型的性能。

让我们先从训练 kNN 分类器开始。

看起来数据集中有 NaN 值，这导致训练过程中出现问题。这很可能是由于将非数值字符转换为 NaN 所导致的。

为了处理这个问题，我将：

+   补充训练集和测试集中的缺失值。

+   重新训练 kNN 分类器。

kNN 分类器在测试数据集上实现了约 98.09%的准确度。这是一个很高的准确度，表明模型能够以高正确度预测给定数据集的目标变量 met_objective_of_45_5_1。

然而，重要的是要记住，准确度只是一个指标。根据具体的应用或问题，其他指标（如精确度、召回率或 F1 分数）可能更相关。此外，kNN 中 k 的选择可以显著影响结果。我们使用了默认的 k=5 值，但不同的值可能会产生不同的结果。

前面的叙述（从本节的开头开始）描述了 GPT-4 将遵循的过程，以使用 kNN 算法和 death.csv 数据集训练机器学习模型。

GPT-4 生成的实际 Python 代码显示在列表 6.1 中，其中包含 knn_gpt4.py 的代码。请注意，此文件名是手动选择的（不是由 GPT-4 本身选择），以反映此任务 Python 代码的内容。

列表 6.1：knn_gpt4.py

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p169.jpg)

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p170.jpg)

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p171.jpg)

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p172.jpg)

列表 6.1（代码列表之前）中对代码的描述说明了 GPT-4 如何使用 kNN 算法执行机器学习任务。您可以将 GPT-4 在列表 6.1 中生成的 Python 代码与解决机器学习任务的手写 Python 代码进行比较。运行列表 6.1 中的代码，您将看到以下输出：

=> 准确度：0.9809220985691574

基于决策树算法的机器学习模型

本节包含了一个 GPT-4 使用 kNN 算法和 death.csv 数据集生成机器学习模型的示例。本节的前半部分包含了 GPT-4 执行的步骤的解释，以及引用代码适当部分的“标记”，随后是列表 6.2，其中包含 GPT-4 生成的基于 Python 的代码。

以下提示被提供给 GPT-4 以生成使用决策树算法的模型的 Python 代码，随后是对代码的描述：

“请生成一个使用决策树算法和 death.csv 数据集的机器学习模型。”

ChatGPT 的响应如下：

我将概述我们将遵循的步骤，以使用决策树算法生成机器学习模型：

+   加载数据：我们之前已经加载了 death.csv 数据集。

+   数据预处理：我们之前已经对数据集进行了大部分预处理。我们将继续使用相同的预处理数据。

+   模型训练：使用决策树算法在训练集上训练模型。

+   模型测试：评估模型在测试集上的性能。

+   性能指标：计算如准确度等指标，以了解模型的性能如何。

[注意：GPT-4 由于内部处理错误生成了以下语句。]

让我们从训练一个决策树分类器开始。

我为造成的不便表示歉意，但似乎出现了技术问题。

让我们重新训练决策树分类器，并计算其在测试集上的准确率。

我为之前的疏忽道歉。由于代码执行状态被重置，我需要重新导入必要的库并再次预处理数据。

我将快速浏览预处理数据的步骤，然后训练决策树分类器。

我为造成的不便表示歉意。由于状态重置，需要重新上传数据集。

请您重新上传 death.csv 数据集，这样我们就可以继续进行决策树算法建模。

作者：“请继续。”

ChatGPT 的响应如下：

感谢您重新上传数据集。让我们继续预处理数据，然后训练决策树分类器。

[注意：GPT-4 遇到了以下错误序列。]

我为之前的疏忽表示歉意。错误表明，数据集中仍然存在我们在早期预处理步骤中遗漏的非数字字符。

让我们通过处理非数字字符来纠正数据预处理，然后再次训练决策树分类器。

我再次为之前的疏忽道歉。我忘记定义 cols_to_convert 列的列表以进行处理。让我纠正这一点，并继续进行预处理和决策树分类器的训练。

我为重复的疏忽表示歉意。似乎我在预处理数据集时犯了一个错误。我将纠正它，并确保在训练决策树分类器之前数据集被正确清理。

让我们处理非数字字符，然后进行模型训练。

我为重复的错误表示歉意。数据预处理步骤似乎仍然遇到未适当处理的字符串值。

为了确保问题得到解决，我将采取不同的方法：

我将调查每一列的唯一值以识别任何非数字字符。我将确保这些非数字字符得到适当的处理。然后，我将继续进行决策树分类器的训练。

看起来没有剩余包含非数字字符的列。这很令人费解，因为错误提示了相反的情况。

我将采取不同的方法：我将识别并删除特征集中包含非数字字符的任何行，然后继续进行决策树分类器的训练。

决策树分类器在测试数据集上达到了 100%的准确率。这表明模型能够完美地预测给定测试数据集的目标变量 met_objective_of_45_5_1。

然而，我们必须谨慎对待这样的结果。100%的准确率可能表明模型已经过度拟合了训练数据，特别是对于像决策树这样的模型，它们容易过度拟合。

验证这一点的其中一种方法是对模型进行交叉验证或检查模型在不同、未见过的数据集上的性能。

[注意：这是由 GPT-4 生成的文本的结尾。](https://wiki.example.org/gpt-4_generated_text_conclusion)

列表 6.2 展示了 decision_tree_gpt4.py 的内容，该内容说明了如何使用决策树算法和 death.csv 数据集创建机器学习模型。

列表 6.2：decision_tree_gpt4.py

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p174.jpg)

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p175.jpg)

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p176.jpg)

列表 6.2（紧接代码列表之前）中对代码的描述说明了 GPT-4 如何使用决策树分类器执行机器学习任务。列表 6.2 中的代码使您能够比较 GPT-4 生成的用于创建机器学习模型的 Python 代码与手写的用于创建使用决策树算法的机器学习模型的 Python 代码。运行 列表 6.2 中的代码，您将看到以下输出：

accuracy_dt：1.0

使用随机森林算法的机器学习模型

本节包含 GPT-4 使用随机森林算法和 death.csv 数据集生成机器学习模型的示例。本节的前半部分包含对 GPT-4 执行的步骤的解释，以及引用代码中适当部分的“标记”，随后是 列表 6.3，其中包含 GPT-4 生成的基于 Python 的代码。

为了生成使用随机森林算法的模型代码，向 GPT-4 提供了以下提示：

“请使用随机森林算法和 death.csv 数据集生成一个机器学习模型。”

ChatGPT 的响应如下：

该数据集包含与美国不同县死亡率相关的各种列。以下是关键列：

county：县名。

fips：该县的 FIPS 代码。

met_objective_of_45_5_1：表示该县是否达到某个特定目标（标题中未指定）。

age_adjusted_death_rate：该县年龄调整后的死亡率。

lower_95_confidence_interval_for_death_rate：死亡率 95%置信区间的下限。

upper_95_confidence_interval_for_death_rate：死亡率 95%置信区间的上限。

average_deaths_per_year：该县每年平均死亡人数。

recent_trend_2：死亡率近期的趋势。

recent_5_year_trend_2_in_death_rates：死亡率近 5 年的趋势。

lower_95_confidence_interval_for_trend：趋势 95%置信区间的下限。

upper_95_confidence_interval_for_trend：趋势 95%置信区间的上限。

要使用随机森林算法构建机器学习模型，我们需要确定目标变量和特征。目标变量可能是“age_adjusted_death_rate”或“average_deaths_per_year”等，而特征将是数据集中的其他列。

让我们继续预处理数据，然后构建随机森林模型。你能指定你想要预测的变量吗？以及是否有任何特定的列你想要用作或排除为特征？

作者：“请预测列变量 met_objective_of_45_5_1。”

ChatGPT 的响应如下：

随机森林模型被训练来预测你数据集中的“met_objective_of_45_5_1”变量。以下是模型评估的结果：

+   准确率：模型达到了大约 62.8%的准确率。这意味着在测试集中，它在大约 62.8%的情况下正确预测了该县是否达到了目标。

+   分类报告：报告提供了模型性能的详细分析：

+   精度：它衡量了模型对正预测的准确性。例如，当模型预测一个县达到了目标时，对于其中一个类别，它大约有 78%的时间是正确的。

+   召回率：它衡量模型通过将其标记为正例来捕获的实际正例的数量。例如，对于其中一个类别，模型正确识别了所有实际达到目标的县中的 74%。

+   F1 分数：这是精度和召回率的加权平均值。对于表现最好的类别，F1 分数为 0.76，表明精度和召回率之间有相对平衡的性能。

+   支持度：这显示了指定数据集中每个类别的实际发生次数。例如，在测试数据集中有一个类别的实例有 407 个。

这些结果表明，虽然模型在预测“met_objective_of_45_5_1”变量方面表现相当不错，但仍有改进的空间，特别是在精度和召回率得分较低的类别中。微调模型、选择不同的特征，甚至采用不同的建模方法可能会潜在地提高性能。

作者向 ChatGPT：“请生成一个使用随机森林算法和 death.csv 数据集的机器学习模型的 Python 代码。”

ChatGPT 的响应如下：

随机森林模型被训练来预测你数据集中的“met_objective_of_45_5_1”变量。以下是模型评估的结果：

+   准确率：模型达到了大约 62.8%的准确率。这意味着在测试集中，它在大约 62.8%的情况下正确预测了该县是否达到了目标。

+   分类报告：报告提供了模型性能的详细分析：

+   精度：它衡量了正预测的准确性。例如，当模型预测一个县达到了目标时，对于其中一个类别，它大约有 78%的时间是正确的。

+   召回率：它衡量模型通过将其标记为正例来捕获的实际正例的数量。例如，对于其中一个类别，模型正确识别了所有实际达到目标的县中的 74%。

+   F1 分数：这是精确率和召回率的加权平均值。对于表现最好的类别，F1 分数为 0.76，表明精确率和召回率之间有相对平衡的性能。

+   支持度：这显示了指定数据集中每个类别的实际发生次数。例如，测试数据集中有一个类别的实例有 407 个。

这些结果表明，虽然模型在预测“met_objective_of_45_5_1”变量方面表现合理，但仍有改进空间，特别是在精度和召回率得分较低的类别中。微调模型、选择不同的特征或甚至采用不同的建模方法可能会潜在地提高性能。

作者：“请生成一个使用随机森林算法和 death.csv 数据集的机器学习模型的 Python 代码。”

ChatGPT 的响应如下：

当然！以下是用随机森林算法和 death.csv 数据集创建机器学习模型的 Python 代码。此代码包括数据预处理、将数据集划分为训练集和测试集、构建随机森林模型以及评估其性能的步骤。

列表 6.3 显示了 random_forest_gpt4.py 的内容，说明了如何使用随机森林算法和 death.csv 数据集创建机器学习模型。

列表 6.3：random_forest_gpt4.py

导入 pandas 库

从 sklearn.model_selection 导入 train_test_split

从 sklearn.ensemble 导入 RandomForestClassifier

从 sklearn.metrics 导入 classification_report, accuracy_score

从 sklearn.preprocessing 导入 LabelEncoder

导入 numpy 库

# 加载数据集

data = pd.read_csv('/path/to/death.csv') # 用正确的文件路径替换

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

# 将数据集划分为训练集和测试集

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

记住将 '/path/to/death.csv' 替换为您 death.csv 文件的实际路径。此代码假定您想要预测的目标变量是 'met_objective_of_45_5_1'，并且它使用数据集中的所有数值列作为特征，排除任何包含非数值数据的列。根据您分析的具体要求可能需要进行调整。

ChatGPT 可能会出错。请考虑检查重要信息。

作者：“请解释你刚才生成的 Python 代码。”

ChatGPT 的响应如下：

当然，我会一步步带你走 Python 代码：

1. 导入库

+   pandas 用于数据处理和分析。

+   使用 sklearn.model_selection 的 train_test_split 函数将数据集分割为训练集和测试集。

+   sklearn.ensemble 的 RandomForestClassifier 是用于分类任务的随机森林模型。

+   sklearn.metrics 包含用于评估模型性能的函数，如 classification_report 和 accuracy_score。

+   sklearn.preprocessing.LabelEncoder 用于将分类文本数据转换为模型可理解的数值格式。

+   numpy 用于数值运算。

2. 加载数据集

+   使用 pandas 的 read_csv 函数读取 death.csv 文件。您需要将“/path/to/death.csv”替换为您数据集的实际路径。

3. 预处理

+   使用 LabelEncoder 将目标变量“met_objective_of_45_5_1”编码为数值格式，因为 sklearn 中的随机森林需要数值输入。

+   然后过滤数据集，只包含数值列，因为模型不能直接处理非数值数据。

4. 处理缺失值

+   删除数据集中剩余的任何缺失值，以确保模型接收到的数据是干净的。

5. 定义目标和特征变量

+   X（特征）被分配除了目标变量（“met_objective_of_45_5_1_encoded”）之外的所有列。

+   y（目标）被编码为“met_objective_of_45_5_1”列。

6. 分割数据集

+   使用 train_test_split 将数据集分割为训练集（80%）和测试集（20%），并设置 random_state 以确保结果的复现性。

7. 构建随机森林模型

+   创建一个 RandomForestClassifier 对象，并在训练数据（X_train 和 y_train）上训练。

8. 预测和评估模型

+   使用模型对测试集（X_test）进行预测。

+   使用 accuracy_score（用于衡量整体准确率）和 classification_report（用于查看每个类的精确率、召回率、f1 分数和支持）来评估预测结果。

9. 输出结果

+   最后，打印出准确率和分类报告，以查看模型的性能表现如何。

此代码提供了一个使用随机森林分类器进行机器学习任务的基本框架。根据您的数据集和问题的具体细节，可能需要额外的步骤，如更复杂的数据清理、特征工程或模型超参数调整，以获得最佳结果。

在 列表 6.3 中启动代码，您将看到以下输出：

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p182.jpg)

使用 SVM 算法的机器学习模型

本节包含 GPT-4 使用 SVM 算法和 death.csv 数据集生成机器学习模型的示例。本节的前半部分包含 GPT-4 执行的步骤解释，以及引用代码中适当部分的“标记”，随后是 列表 6.4 包含 GPT-4 生成的基于 Python 的代码。

为了生成使用 SVM 算法和 death.csv 数据集的模型 Python 代码，向 GPT-4 提供了以下提示：“请生成使用 SVM 算法和 death.csv 数据集的机器学习模型 Python 代码，并提供 Python 代码的解释。”

ChatGPT 的响应如下：

当然！以下是使用 SVM 算法与 death.csv 数据集创建机器学习模型的 Python 代码。代码之后，我将提供解释。

列表 6.4 展示了 svm_gpt4.py 的内容，该内容说明了如何使用 SVM 算法和 death.csv 数据集创建机器学习模型。

列表 6.4：svm_gpt4.py

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

print("Accuracy:", accuracy)

print("Classification Report:\n", report)

代码解释

1. 导入库：

2. 与随机森林模型使用相同的库，增加了 sklearn.svm.SVC（SVM 分类器）和 sklearn.preprocessing.StandardScaler（特征缩放）。

3. 加载数据集：

4. 从 CSV 文件加载数据集。您需要将“/path/to/death.csv”替换为实际文件路径。

5. 预处理：

6. 目标变量（“met_objective_of_45_5_1”）使用 LabelEncoder 编码成数值格式。

7. 非数值列被排除，任何缺失值都被删除。

8. 特征缩放：

9. 应用 StandardScaler 对特征进行标准化。这是 SVM 的重要步骤，因为它对输入特征的规模很敏感。

10. 定义目标和特征：

11. X 是特征集，y 是目标变量。

12. 数据集拆分：

13. 数据集被划分为训练集和测试集。

14. 构建 SVM 模型：

15. 在训练数据上实例化并训练了一个 SVM 分类器（SVC）。

16. 模型预测和评估：

17. 模型在测试集上进行预测，并使用准确率和分类报告评估其性能。

18. 输出结果：

19. 打印准确率和分类报告以评估模型的性能。

此代码提供了一个 SVM 模型分类的基本实现。与任何机器学习模型一样，可能需要进行进一步的调整和验证，以优化其在特定数据集上的性能。

在列表 6.3 中运行代码，您将看到以下输出：

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p184.jpg)

[注意：这是由 GPT-4 生成的文本和输出的结尾。]

**逻辑回归算法**

逻辑回归是一种统计方法和机器学习算法，用于对结果为分类的数据集进行建模和分析。虽然其名称包含“回归”，但它主要用于二元分类任务（即输出可以有两个可能的值）。它也可以扩展以处理多类分类。

基本概念

逻辑回归模型预测给定实例属于特定类别的概率。它预测事件发生的对数几率，而对数几率的转换给出概率。

数学表示

对于二元分类（带有标签 0 和 1），概率 P(Y=1) 被建模如下：

P(Y=1)=11+e−z

P(Y=1)=1+e−z1

其中：

e 是自然对数的底数。

z 是预测变量的线性组合：z=β0+β1X1+β2X2+...

步骤

1. 线性变换：计算输入特征的加权总和（加上一个偏差项）。

2. 逻辑变换：将步骤 1 的结果通过逻辑（Sigmoid）函数传递，以得到概率 P(Y=1)。

3. 决策阈值：使用阈值将概率转换为二元结果（0 或 1），通常为 0.5。

参数估计

逻辑回归模型的系数（参数）通常使用最大似然估计（MLE）来估计。目标是找到一组参数，以最大化观察数据的似然度。

优点

+   可解释性：系数可以解释为赔率比，这使得解释预测变量的影响变得容易。

+   效率：它不需要太多的计算资源

+   输出概率：它提供了一个概率框架，这对于理解预测的置信度可能很有用

缺点

+   假设线性：它假设决策边界是线性的，这可能无法捕捉到没有特征工程的情况下更复杂的关系。

+   不适合复杂关系：对于高度非线性的关系，其他算法如决策树或神经网络可能更合适。

+   易于过拟合：当特征数量较多时，它可能会过拟合，尤其是在特征相关的情况下。

用例

逻辑回归在医学（疾病诊断）、金融（信用批准）、营销（客户流失预测）等多个领域得到广泛应用，这些领域的结果是二元的。

扩展

1. 多项式逻辑回归：当目标变量有多个类别时使用

2. 正则化逻辑回归：通过引入 L1（Lasso）或 L2（Ridge）正则化来防止过拟合

逻辑回归是二元分类任务的基础算法，它既提供了良好的可解释性，又为预测提供了一个概率框架。

朴素贝叶斯算法

高斯朴素贝叶斯是一种基于贝叶斯定理的概率机器学习算法，它假设预测变量之间相互独立（因此得名“朴素”）。尽管其简单和朴素假设，但该算法在许多任务中都非常有效，尤其是在文本分类场景中，如垃圾邮件过滤或情感分析。

贝叶斯定理提供了一种基于先验知识计算假设概率的方法。其公式如下：

P(A∣B) = P(B∣A)×P(A)/P(B)

其中

P(A∣B) 是在数据 B 的条件下假设 A 的后验概率。

P(A) 是 A 的先验概率。

P(B∣A) 是似然，给定假设 A 的数据 B 的概率。

P(B) 是证据，数据 B 的概率。

朴素贝叶斯分类

对于一个具有响应变量 Y 和预测变量 X1,X2,...,Xn 的分类问题，朴素贝叶斯分类器估计条件概率：

P(Y=k∣X1,X2,...,Xn)

P(Y=k∣X1,X2,...,Xn)

基于独立性假设，这可以简化为以下形式：

P(Y=k∣X1,X2,...,Xn)∝P(Y=k)×∏i=1nP(Xi∣Y=k)

P(Y=k∣X1,X2,...,Xn)∝P(Y=k)×i=1∏nP(Xi∣Y=k)

具有最高后验概率的类别 k 是给定输入的预测。

朴素贝叶斯的类型

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

+   数据分布：如果模型的分布假设（例如，高斯分布）与实际数据分布不一致，模型的性能可能会受到影响。

用例

朴素贝叶斯在以下方面特别受欢迎：

1. 文本分类：如垃圾邮件检测、情感分析和新闻文章分类

2. 推荐系统：如建议新闻文章或音乐

3. 人脸识别：作为更大系统的一部分

朴素贝叶斯是一种多才多艺且计算效率高的分类算法。其优势在于其简单性、概率性质以及在许多场景中出人意料的稳健性能，尤其是在数据维度较高时。

SVM 算法

SVM 是一种监督机器学习算法，主要用于分类任务，尽管它也可以用于回归。它以其鲁棒性和处理高维数据的能力而闻名。SVM 的主要目标是找到最佳超平面，以最好地将数据集划分为类别。

基本概念

对于一个双分类问题，想象你在多维空间中绘制你的数据点。SVM 试图找到一个最佳的超平面（在 2D 中是一条线，在 3D 中是一个平面，等等），以最好地分隔两个类别。最佳超平面是具有最大边缘的超平面，即两个类别数据点之间的最大距离。

重要组件

1. 支持向量：这些是位于超平面最近的数据点，有效地定义了它。如果它们被移除，这些数据点会改变超平面的位置。

2. 边缘：这是最近的数据点（任何类别）与超平面之间的距离。SVM 的目标是最大化这个边缘。

3. 超平面：这是分隔类别的决策边界。在二维空间中，它是一条线。

类型

1. 线性 SVM：用于线性可分的数据。它找到一个最佳的超平面来分隔两个类别。

2. 非线性 SVM（核 SVM）：当数据不可线性分隔时，SVM 使用一种称为“核技巧”的技巧，将数据投影到一个更高维的空间，在那里它是线性可分的。常见的核包括多项式、径向基函数（RBF）和 sigmoid。

优点

+   在高维空间中有效：即使特征数量大于样本数量，它也能很好地工作。

+   鲁棒：它最大化了间隔，使其对异常值具有鲁棒性。

+   多功能性：核技巧可以使算法适应非线性数据。

缺点

+   不适用于大数据集：由于其计算复杂性，它可能不是非常大的数据集的最佳选择。

+   对噪声敏感：少量错误标记的示例可以显著降低性能。

+   核函数的选择：性能可能对核函数及其参数的选择敏感。

用例

支持向量机（SVMs）在各种应用中使用。

1. 文本分类：由于其处理高维数据的能力，支持向量机（SVMs）常用于文本分类。

2. 图像识别：作为图像分类管道的一部分

3. 生物信息学：用于蛋白质分类和癌症分类

4. 手写识别：用于识别手写字符

支持向量机（SVMs）为分类任务提供了一种强大的方法，尤其是在数据具有许多特征或类别不是线性可分时。适当的调整，尤其是在使用核 SVM 时，对于实现最佳性能至关重要。

决策树算法

决策树是一种类似于流程图、树状结构的算法，用于机器学习中的分类和回归任务。它在将数据集分解成越来越小的子集的同时，逐步开发相关的决策树。

基本概念

决策树算法试图通过使用树表示来解决问题。树中的每个内部节点对应一个特征，每个叶节点对应一个响应或类别标签。

重要组件

1. 决策节点：由正方形表示，这些节点包含对单个属性的决策或测试。

2. 分支：表示测试的结果并连接节点

3. 叶节点：终端节点，用于预测结果

算法

1. 属性选择：根据指标（如信息增益或基尼不纯度）选择放置在决策节点上的属性。目标是选择提供最佳分割的属性。

2. 分支创建：为所选属性的每个可能值创建一个分支。

3. 递归分割：步骤 1 和 2 随后对每个分支重复，使用与该分支关联的数据子集。

4. 终止：当满足某个停止条件时，递归停止，例如达到最大树深度、达到最小节点大小或节点包含来自单个类别的数据。

类型

1. 分类树：当响应变量是分类变量时使用。结果是类别标签。

2. 回归树：当响应是数值或连续时使用。结果是实数值。

分割指标

1. 信息增益：衡量一个特征为我们提供的关于类别的信息量。它基于熵。

2. Gini 不纯度：衡量一组元素的混乱程度。它被 CART（分类和回归树）算法用于分类任务。

3. 方差减少：由 CART 用于回归树

优点

+   可解释性：树可以可视化，并且即使是非专家也容易理解。

+   最小数据准备：它不需要归一化或虚拟变量

+   处理连续和分类变量：它可以用于分类和回归任务。

+   非参数：它不对分布和分类器结构做出假设。

缺点

+   过度拟合：如果没有适当的调整，树可能会记住训练数据，从而导致过度拟合。

+   不稳定性：数据中的微小变化可能导致完全不同的树。

+   优化：找到一组数据的最佳树是 NP-hard 问题。因此，使用贪婪算法等启发式方法，这有时会导致次优树。

用例

决策树是多功能的，可以用于各种应用，包括以下：

1. 医疗诊断：根据症状，预测疾病的可能性

2. 信用风险分析：决定是否批准或拒绝贷款

3. 营销：识别营销活动的潜在客户

扩展

1. 随机森林：决策树的集成，通过减少过度拟合提供更好的预测性能

2. 梯度提升树：顺序构建决策树，其中每棵树都纠正其前一棵树的错误

决策树提供了一种直观且易于视觉化的决策过程方法。它们的简单性和易于解释使它们在各种领域成为流行的选择，但必须小心处理它们的局限性。

随机森林算法

随机森林是一种主要用于分类和回归任务的集成学习方法。它在训练过程中构建多个决策树，并输出由单个树产生的类别的众数（用于分类）或均值（用于回归）。

基本概念

1. 自举：随机森林首先从数据集中提取多个自举样本（带有替换的随机样本）。这引入了可变性，并确保森林中的每棵树都在略微不同的数据子集上训练。

2. 特征随机性：在决策树的每个分割中，只考虑特征的一个随机子集。这进一步确保森林中树的多样性，使集成更少相关且更稳健。

3. 聚合：

+   对于分类，森林中的每棵树都对一个类别“投票”，得票最多的类别是随机森林的预测。

+   对于回归，所有树的平均预测值是最终预测。

优点

+   高精度：它结合多个树来产生一个高精度的分类器。

+   过度拟合控制：在树构建中引入的集成特性和随机性有助于控制过度拟合。

+   处理大数据：它能够高效地处理具有更多特征和观测值的集合。

+   特征重要性：它提供了关于不同特征在预测中的重要性见解。

+   多功能性：它可以用于分类和回归任务。

+   处理缺失值：它可以处理包含缺失值的集合。

缺点

+   复杂性：它比单个决策树更计算密集。

+   可解释性：虽然单个树是可解释的，但森林可能不那么直观易懂。

+   预测较慢：在森林中的所有树上进行聚合以进行预测可能比其他算法慢。

超参数

在调整随机森林时需要考虑的一些关键超参数包括以下内容：

1. 树的数量：森林中的树的数量

2. 最大深度：每棵树的最大深度

3. 内部节点最小分割样本数：分割内部节点所需的最小样本数

4. 叶节点最小样本数：达到叶节点所需的最小样本数

用例

随机森林是多功能的，并在各个领域都有应用，包括以下内容：

+   银行：信用风险分析

+   医学：疾病识别

+   电子商务：推荐系统

+   遥感：卫星图像分类

随机森林是一种强大且灵活的算法，它建立在决策树的优势之上，同时解决了一些弱点。通过聚合多个、多样化的树的结果，它实现了高精度和对抗过拟合的鲁棒性。在需要快速基线模型或解释性不是主要关注点的情况下，它特别有价值。

摘要

本章内容丰富，这是您的第二个完整章节，其中包含由 GPT-4 生成的分类器材料。您简要介绍了 scikit-learn，随后讨论了 kNN 算法。

接下来，您学习了交叉验证、偏差-方差权衡和距离度量。此外，您还学习了在 kNN 算法中选择 k 的最佳值的肘部方法。

此外，您还看到了由 GPT-4 生成的涉及 kNN 算法、决策树算法、SVM 算法和逻辑回归算法的代码示例。

本章的最后部分包含了一个由 GPT-4 生成的高级算法描述，包括逻辑回归、朴素贝叶斯、SVG、决策树和随机森林。

第七章

使用 GPT-4 进行机器学习聚类

本章包含由 GPT-4 生成的 Python 代码示例，这是第三章节，其中包括三个流行的机器学习聚类任务的 Python 代码。

本章的第一部分向您介绍了机器学习中的聚类，随后列出了十个聚类算法。本节还描述了 k-means、层次聚类和 DBSCAN 算法的优点和缺点。

本章的第二部分包含三个基于 Python 的代码示例，用于 k-means、层次聚类和 DBSCAN 算法，使用合成数据集。所有代码示例都是通过向 GPT-4 提供合适的提示生成的。

什么是聚类？

聚类是机器学习中的一个基本概念，尤其是在无监督学习中。聚类是将数据集划分为称为簇的组的过程，使得同一组中的项目彼此之间比其他组中的项目更相似。

重要点

+   学习类型：聚类是一种无监督学习形式。这意味着您不需要标记数据来与聚类算法一起工作。相反，目标是发现数据中的隐藏模式。

+   目标：主要目标是分离具有相似特征的组并将它们分配到簇中。

应用

+   市场细分：根据购买历史分组客户

+   社交网络分析：在网络中识别社区

+   搜索结果分组：将相似的文档或网页分组在搜索结果中

+   图像分割：根据像素相似性将图像划分为区域

+   异常检测：检测不符合预期行为的异常模式（异常值）

度量标准

+   簇内平方和 (WCSS)：这衡量了簇内所有点到簇中心的平均距离的平方。

+   轮廓分数：这衡量了簇中每个点到邻近簇中点的接近程度。

+   戴维斯-博尔丁指数：这是衡量每个簇与其最相似簇之间平均相似度的指标，其中相似度是簇内距离与簇间距离的比率。值越低越好。

流行的聚类算法

+   K-means：这将数据划分为 k 个不同的、非重叠的子集（或簇）。它通过最小化数据与相应簇质心的平方距离之和来实现这一点。

+   层次聚类：这产生一组嵌套簇，组织成层次树。这种聚类可以可视化为一棵树状图（树形图），展示了形成簇的顺序。

+   DBSCAN（基于密度的空间聚类应用噪声）：它根据数据点的密度创建簇。它可以找到任意形状的簇，并且对于有噪声和异常值的数据很有用。

+   高斯混合模型 (GMMs)：这些模型假设数据是由几个高斯分布的混合生成的。GMM 试图识别这些高斯分布。

+   聚类：与层次聚类类似，但通常更具可扩展性。它从每个项目作为一个单独的簇开始，并将它们合并成更大的簇。

挑战

+   簇的数量：聚类中的一个挑战是确定算法应将数据分割成多少个簇。对于 k-means，一种流行的技术是“肘部方法”。

+   簇的形状和大小：一些算法假设簇是球形且大小相等的，这并不总是情况。

+   特征缩放：聚类算法，尤其是像 k-means 这样的基于距离的方法，对特征缩放很敏感。你应该缩放特征，使它们具有相似的量级。

+   高维性：在高维空间中进行聚类可能会出现问题，这被称为“维度诅咒”。可以使用 PCA（主成分分析）等技术来降低维度。

聚类可以深入了解数据的分布、分类和结构。它是数据分析、异常检测和预处理步骤（如数据降维）的强大工具。

十种聚类算法

本节包含机器学习中的十种聚类算法列表，以及它们的优缺点：

+   k-means 聚类

+   层次聚类

+   基于密度的空间聚类应用（DBSCAN）

+   聚类

+   均值漂移聚类

+   高斯混合模型 (GMM)

+   相似传播

+   谱聚类

+   聚类

+   OPTICS（按顺序排列点以识别聚类结构）

K-means 聚类

优点

+   简单且易于实现

+   对于球形且大小相等的簇效果良好

+   对于大量变量来说很快

缺点

+   它假设簇是球形且大小相等的，这并不总是情况。

+   必须事先指定簇的数量 k。

+   对初始化敏感，因为不同的初始质心可能导致不同的簇。

层次聚类

优点

+   不需要指定簇的数量。

+   它提供了一个树状图，这对于理解数据层次结构可能很有用。

缺点

+   比 k-means 计算成本更高。

+   对于非常大的数据集来说不可扩展。

基于密度的空间聚类应用（DBSCAN）

优点

+   可以找到任意形状的簇

+   不需要指定簇的数量

+   可以识别噪声/异常值

缺点

+   可能难以处理密度变化的簇

+   不总是确定性的：可以从多个簇到达的边界点可以是任一簇的一部分。

聚类

优点

+   适用于较小的数据集

+   不需要指定簇的数量（尽管在实践中通常指定）

缺点

+   对于非常大的数据集不可扩展

均值漂移聚类

优点

+   不假设关于簇数量的任何先验知识

+   可以找到任意形状的簇

缺点

+   计算成本更高

+   需要仔细选择带宽参数。

高斯混合模型 (GMM)

优点

+   假设每个簇遵循高斯分布

+   可以建模椭圆簇

缺点

+   比 k-means 计算量更大

+   需要估计更多参数

相似传播

优点

+   自动确定簇的数量

+   使用所有数据点作为潜在的示例

缺点

+   对于大数据集来说，可能很慢且需要更多内存

+   可能会产生大量簇

谱聚类

优点

+   可以捕捉复杂的簇结构

+   可以用来识别非凸簇

缺点

+   对于大数据集来说，计算成本可能很高

+   必须事先指定簇的数量

聚类

优点

+   提供了一种分层方法，导致簇树

+   适用于较小的数据集

缺点

+   不适用于大数据集

+   需要指定簇的数量。

OPTICS（按顺序排列点以识别聚类结构）

优点

+   不需要指定簇的数量

+   可以识别不同密度的簇

缺点

+   比简单的算法如 k-means 计算成本更高

每个这些聚类算法都有其自己的假设，适用于不同类型的数据和要求。算法的选择通常取决于数据的大小、维度和性质，以及具体问题的背景。

机器学习中三种最受欢迎的聚类算法是前述章节列表中的前三种算法。这些算法将在随后的章节中描述，包括基于 Python 的代码示例。

聚类算法的度量标准

本节包含了一组你可以用于评估聚类算法的度量标准。聚类算法的评估对于确定算法的性能至关重要。以下是一组常用的聚类算法评估度量标准，以及它们的优缺点：

+   Silhouette 分数

+   Calinski-Harabasz 指数

+   Davies-Bouldin 指数

+   Dunn 指数

+   调整后的兰德指数 (ARI)

+   归一化互信息 (NMI)

+   Fowlkes-Mallows 指数

+   纯度

+   凝聚力

+   分离度

Silhouette 分数

优点

+   衡量一个对象与其簇相比与其他簇的相似度

+   值范围从 -1 到 1，高值表示好的聚类

缺点

+   不适用于非凸簇或密度变化的簇

+   对于大数据集，计算成本可能很高

Davies-Bouldin 指数

优点

+   衡量每个簇与其最相似簇之间的平均相似度

+   较低的值表示聚类更好。

缺点

+   它假设簇是凸的和各向同性的，这并不总是情况。

Calinski-Harabasz 指数

优点

+   计算簇间散布均值与簇内散布均值的比率

+   较高的值表示聚类更好。

缺点

+   它假设簇是凸的和各向同性的。

Dunn 指数

优点

+   考虑最小簇间距离与最大簇内距离之间的比率

+   较高的 Dunn 指数表示聚类更好。

缺点

+   计算成本高

调整后的兰德指数 (ARI)

优点

+   测量两个聚类之间的相似度

+   考虑到偶然性进行调整，提供更可靠的分数

缺点

+   需要了解真实情况

标准化互信息 (NMI)

优点

+   测量两个聚类之间的互信息

+   标准化到范围 [0, 1]

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

+   简单易懂和计算

缺点

+   需要了解真实情况

+   不考虑聚类大小

聚合

优点

+   测量同一聚类内实例的相关性

缺点

+   对聚类数量敏感

分离

优点

+   测量一个聚类与其他聚类区分或分离的程度

缺点

+   对聚类数量敏感

当评估聚类算法时，考虑数据的性质和具体用例至关重要。根据上下文，某些指标可能比其他指标更合适。使用多个指标以全面了解聚类性能也是有益的。

K-MEANS 聚类

优点

+   简单性：该算法简单且易于实现。

+   效率：它计算速度快，尤其是在使用 Elkan 算法等优化变体时。

+   可扩展性：K-means 在大数据集上扩展良好，尤其是在使用 MiniBatch k-means 时。

+   流行：由于其简单性和适用性，它在实践中被广泛使用。

缺点

+   聚类数量：您需要事先指定聚类数量 k，这并不总是可行的。

+   球形假设：它假设聚类是球形且大小相等。对于细长或不规则形状的聚类，可能表现不佳。

+   初始化敏感性：算法的结果可能因初始质心位置而异。尽管 k-means++ 等技术有所帮助，但收敛到局部最小值仍然可能是一个问题。

+   对异常值敏感：异常值会严重影响质心的位置。

+   特征缩放：它对特征缩放敏感。特征需要缩放才能使算法正常工作。

层次聚类

优点

+   系谱图：层次聚类产生系谱图，这可以是一个理解数据层次结构的有用工具，也可以用于可视化。

+   无需指定 k：与 k-Means 不同，您不需要事先指定聚类数量。

+   灵活性：它可以产生各种不同的聚类结构，使其适用于各种应用。

+   确定性：给定相同的输入和参数，总是产生相同的聚类结果。

缺点

+   计算复杂度：标准算法具有高计算复杂度，使其不太适合大型数据集。

+   敏感性：它可能对噪声和异常值敏感。

+   选择正确级别的困难：决定在层次结构中切割和形成聚类的级别可能很棘手。

DBSCAN（基于密度的空间聚类应用，无噪声）

优点

+   无需指定聚类数量：DBSCAN 根据数据自动确定聚类数量。

+   形状灵活性：它可以找到任意形状的聚类，这是相对于 k-means 的一个显著优势。

+   噪声处理：它可以识别和处理噪声和异常值。

+   无需指定聚类结构：它不假设聚类是球形的或任何特定形状。

缺点

+   处理不同密度聚类的困难：当聚类具有显著不同的密度时，它会有所挣扎。

+   边界点：可以从多个聚类到达的点可能被分配到错误的聚类。

+   参数敏感性：它需要设置参数（如邻域半径和最小点数），这些参数可以极大地影响结果。

虽然这些是三种最受欢迎的聚类算法，但最佳算法通常取决于特定的数据集和问题要求。尝试多种算法并评估哪种算法最适合给定场景是一种常见做法。

现在你已经对机器学习中的聚类有了基本了解，让我们来看一个基于 k-means 算法的机器学习模型，这是下一节的主题。

什么是 k-means 算法？

由于其简单性和效率，k-means 算法是最广泛使用的聚类方法之一。

K-means 聚类概述

K-means 是一种分区方法，它将数据集划分为 k 个不同的、非重叠的子集（或聚类）。k-means 算法的目标是在数据中找到组，组数由变量 k 表示。

算法

+   初始化：随机选择 k 个数据点（种子）作为初始质心。

+   作业：将每个数据点分配到最近的质心。分配给质心的所有点构成一个聚类。

+   更新：计算每个聚类的新的均值（质心）。

+   迭代：重复步骤 2 和 3，直到质心没有显著变化，或者达到预定的迭代次数。

重要概念

+   质心：聚类的中心。在 k-Means 中，质心是聚类中所有点的平均值。

+   WCSS（簇内平方和）：它衡量簇内所有点到簇中心的平方平均距离。k-Means 的目标是使这个指标最小化。

确定 k 的值

k-means 的一个挑战是选择合适的聚类数量 k。一种常见的技术是“肘部方法”。

1. 对不同的 k 值（例如，k 从 1 到 10）计算聚类算法。

2. 对于每个 k，计算总 WCSS。

3. 绘制 WCSS 与聚类数量 k 的曲线图。

4. 图中弯曲点（“肘部”）的位置通常被认为是适当聚类数量的指标。

优势

+   简单且易于实现

+   在计算成本方面高效

+   适用于大型数据集

局限性

+   它假设聚类是球形且大小相等的，这并不总是情况。

+   必须事先设置聚类数量 k。

+   它对质心的初始化敏感。这个问题通常通过多次运行算法并使用不同的初始化来解决这个问题，并选择最佳结果。

+   它可能收敛到局部最优。这就是为什么通常需要多次运行整个过程，每次使用不同的起始条件。

+   它对特征缩放敏感。

变体

+   k-means++：这种变体旨在通过指定在执行标准 k-means 优化迭代之前初始化质心的程序来解决 k-means 的随机初始化弱点。

K-means 是一种基础聚类算法，已在各种应用中被广泛使用。虽然它功能强大且可扩展，但为了得到有意义的聚类分配，对数据进行仔细的预处理以及考虑其假设是至关重要的。

层次聚类算法是什么？

层次聚类算法是一种聚类算法，通过自下而上或自上而下的方法构建聚类层次结构。层次聚类构建一个聚类树。这个树，称为树状图，有助于可视化聚类合并或分割的顺序。

层次聚类的两种主要策略是：

1. 聚合（自下而上）：这是最常用的策略。它从将每个对象视为单元素聚类开始。成对的聚类依次合并，直到所有聚类都合并成一个包含所有对象的单个大聚类。

2. 分裂（自上而下）：它从单个聚类中的所有对象开始。在后续步骤中，聚类被分割成更小的聚类，直到每个对象都有自己的单元素聚类。

聚类层次聚类算法

在这里，我们将关注更常用的聚合层次聚类。

1. 初始化：将每个数据点视为一个单独的聚类，导致 nn 个数据点有 nn 个聚类。

2. 聚合

+   找到彼此最近的两个聚类对。

+   将这两个聚类合并成一个聚类。

+   更新距离矩阵（用于存储聚类之间的距离）。

+   重复此过程，直到只剩下一个聚类。

3. 补充：上述过程的结果是一个树状图，称为树状图。树状图表示聚类合并的顺序。

距离度量

距离度量的选择在层次聚类中至关重要。

+   欧几里得距离：欧几里得空间中两点之间的普通直线距离

+   曼哈顿距离：它们坐标的绝对差之和

+   余弦相似度：衡量两个非零向量之间角度的余弦值

连接标准

当两个簇 S 和 T 合并成更大的簇时，如何定义簇之间的距离的选择由连接标准决定：

+   单连接：两个簇之间的距离定义为每个簇中两点之间的最短距离。

+   完全连接：两个簇之间的距离定义为簇内任意两点之间的最大距离。

+   平均连接：两个簇之间的距离定义为簇内每个点到另一个簇中每个点的平均距离。

+   瓦德方法：此方法最小化了合并簇之间距离的方差。

优点

+   离散树图：提供了对数据层次结构的深入洞察

+   无需指定簇数：与 k-means 不同，您不需要事先指定簇数。

+   灵活性：可以产生各种不同的簇结构，使其适用于各种应用

缺点

+   计算复杂度：对于非常大的数据集不可扩展

+   不可逆：一旦做出合并两个簇的决定，就不能撤销。

+   对噪声和异常值的敏感性：噪声数据可能导致簇被错误地合并。

+   连接标准的选择：不同的连接方法可以产生不同的层次结构。选择正确的连接标准至关重要。

层次聚类在数据中存在层次结构时特别有用。它适用于较小的数据集，当树状图对分析或展示有益时。然而，对于大型数据集或当计算效率是一个关注点时，其他聚类方法，如 k-means 或 DBSCAN，可能更合适。

什么是 DBSCAN 算法？

基于密度的空间聚类应用噪声（DBSCAN）是一种著名的聚类算法，以其检测任意形状簇的能力和对输入数据顺序的不敏感性而闻名。

原则

DBSCAN 根据距离测量（通常是欧几里得距离）和最小数据点数将彼此靠近的数据点分组在一起。它还将位于低密度区域内的点标记为异常值。

步骤

1. 随机点选择：从一个尚未访问的任意数据点开始。

2. 邻域检查：检索此点的邻域（所有在预定义距离 εε 内的点）。

3. 扩展簇：

+   如果有足够多的邻居（大于阈值 minPts），将当前点标记为核心点并形成一个簇。

+   将此簇内所有可到达的数据点（直接和间接的）添加到距离 εε 内。

+   对聚类中的每个未访问点重复此过程。

4. 标记噪声：如果一个点不属于任何聚类且没有足够的邻居，则将其标记为噪声或异常值。

5. 迭代：重复此过程，直到所有点都被分配到聚类或标记为噪声。

重要概念

+   核心点：如果一个数据点在 ε 距离内有超过 minPts 个点，则它是核心点。

+   边界点：如果一个数据点在 ε 距离内有少于 minPts 个点，但位于核心点的 ε 距离内，则它是边界点。

+   噪声/异常值：如果一个数据点既不是核心点也不是边界点，则它是噪声。

+   直接密度可达：如果 PP 在 QQ 的 ε 距离内，并且 QQ 是核心点，则点 PP 直接从点 QQ 密度可达。

+   密度可达：如果存在一个点序列 P1,...,Pn，其中 P1=Q 且 Pn=P，并且 Pi+1 从 Pi 直接密度可达，则点 PP 从 QQ 密度可达。

优点

+   任意形状的聚类：与 k-means 不同，DBSCAN 可以找到任意形状的聚类，而不仅仅是球形。

+   噪声处理：它可以有效地处理噪声和异常值。

+   无需指定聚类数量：该算法不需要事先指定聚类数量。

缺点

+   参数敏感性：结果可能根据距离阈值 ε 和 minPts 的选择而变化。选择合适的值可能具有挑战性。

+   变化的密度：当聚类具有显著不同的密度时，DBSCAN 可能会遇到困难。

+   高维数据：随着数据维度的增加，算法的有效性会降低。

DBSCAN 是一种强大的算法，尤其是在聚类形状各异且需要区分异常值时。它特别适用于空间数据和有噪声的数据。然而，参数调整和对数据本质的理解对于获得 DBSCAN 的最佳结果至关重要。

基于 k-means 算法的机器学习模型

本节包含 GPT-4 使用 k-means 算法和合成数据集生成机器学习模型的示例。本节的前半部分包含对 GPT-4 执行的步骤的解释，随后是 列表 7.1，其中包含 GPT-4 生成的基于 Python 的代码。

这里是我们将要进行的概述：

1. 生成数据集：我们将使用 Scikit-learn 的 make_blobs 函数创建具有聚类的合成数据集。

2. 可视化数据集：我们将绘制数据集以查看聚类。

3. k-means 聚类：我们将使用 k-means 算法来识别聚类。

4. 可视化聚类：我们将再次绘制数据集，但这次将根据 k-means 识别的聚类进行着色。

让我们生成合成数据集并可视化它。以下是具有三个聚类的生成数据集。颜色代表实际的聚类（由于这是一个合成数据集，我们知道真实的聚类分配）。

接下来，我们将使用 k-means 算法来识别数据集中的聚类。我们将 kk（聚类数）设置为 3，因为我们使用了 3 个中心来生成数据集。聚类后，我们将可视化结果。

可视化显示了 k-means 聚类的结果。数据点根据 k-means 算法确定的聚类着色。红色的“X”标记代表 k-means 确定的聚类中心。

如观察所示，k-means 算法已成功识别合成数据集中的聚类。

列表 7.1 显示了 kMeans_GPT4.py 的内容，说明了如何使用 k-means 算法和 death.csv 数据集创建机器学习模型。

列表 7.1: kMeans_GPT4.py

从 sklearn.datasets 导入 make_blobs

导入 matplotlib.pyplot 库作为 plt

# 生成具有 3 个聚类的合成数据集

X, y = make_blobs(n_samples=300, centers=3, random_state=42, cluster_std=2.0)

# 可视化数据集

设置 plt.figure 的大小为(8, 6)

使用 plt.scatter 在 X 的第 0 列和第 1 列上绘制散点图，颜色为 y，大小为 50，颜色映射为'viridis'

设置标题为"具有 3 个聚类的生成数据集"

设置 x 轴标签为"特征 1"

设置 y 轴标签为"特征 2"

显示 plt

# 由于重置而重新导入必要的库

从 sklearn.datasets 导入 make_blobs

导入 matplotlib.pyplot 库作为 plt

# 再次生成合成数据集

X, y = make_blobs(n_samples=300, centers=3, random_state=42, cluster_std=2.0)

# 可视化数据集

设置 plt.figure 的大小为(8, 6)

使用 plt.scatter 在 X 的第 0 列和第 1 列上绘制散点图，颜色为 y，大小为 50，颜色映射为'viridis'

设置标题为"具有 3 个聚类的生成数据集"

设置 x 轴标签为"特征 1"

设置 y 轴标签为"特征 2"

显示 plt

从 sklearn.cluster 导入 KMeans

# 应用 kMeans 聚类

kmeans = KMeans(n_clusters=3, random_state=42)

kmeans_labels = kmeans.fit_predict(X)

# 可视化识别的聚类

设置 plt.figure 的大小为(8, 6)

使用 plt.scatter 在 X 的第 0 列和第 1 列上绘制散点图，颜色为 kmeans_labels，大小为 50，颜色映射为'viridis'

使用 plt.scatter 在 kmeans.cluster_centers_ 的第 0 列和第 1 列上绘制散点图，大小为 200，颜色为红色，标记为'X'，标签为'Cluster Centers'

设置标题为"kMeans 聚类结果"

设置 x 轴标签为"特征 1"

设置 y 轴标签为"特征 2"

添加图例

显示 plt

列表 7.1 从几个导入语句开始，随后调用 make_blobs()创建一个合成数据集。接下来的代码块通过此代码片段生成并显示从生成的数据集中的数据生成的散点图：

使用 plt.scatter 在 X 的第 0 列和第 1 列上绘制散点图，颜色为 y，大小为 50，颜色映射为'viridis'

列表 7.1 的下一部分实际上是多余的：代码中先前发生的导入语句对再次导入。此外，生成了相同的散点图，这也是多余的。

代码列表 7.1 的下一段初始化变量 kmeans 为从 sklearn.cluster 导入的类 KMeans 的实例。接下来，变量 kmeans_labels 使用 kmeans 变量的 fit_predict()方法的结果进行初始化。在下一个代码块中，生成了一个散点图，通过这两段代码显示每个簇的中心信息：

plt.scatter(X[:, 0], X[:, 1], c=kmeans_labels, s=50, cmap='viridis')

plt.scatter(kmeans.cluster_centers_[:, 0], kmeans.cluster_centers_[:, 1], s=200, c='red', marker='X', label='Cluster Centers')

运行代码列表 7.1 中的代码，你会看到生成两个图像。图 7.1 显示了三个簇，图 7.2 显示了三个簇及其用红色表示的质心。

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p212-1.jpg)

图 7.1 三簇

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p212-2.jpg)

图 7.2 三簇及其质心

带有层次聚类算法的机器学习模型

本节包含了一个 GPT-4 使用层次聚类算法和合成数据集生成机器学习模型的示例。本节的前半部分包含了 GPT-4 执行的步骤解释，随后是代码列表 7.2，其中包含了 GPT-4 生成的基于 Python 的代码。

让我们通过以下步骤在数据集上应用层次聚类算法：

1. 生成合成数据集：我们将使用 Scikit-learn 的 make_blobs 函数创建一个带有簇的合成数据集。

2. 可视化数据集：绘制数据集以查看簇。

3. 计算连接矩阵：使用 SciPy 的 linkage 函数，它将捕捉点之间的层次关系。

4. 树状图可视化：显示树状图以可视化簇的逐步合并过程。

5. 切割树状图：为了确定簇的数量，我们将切割树状图并检索簇标签。

6. 可视化簇：我们将绘制由层次聚类识别的簇着色的数据集。

让我们再次通过生成合成数据集并对其应用层次聚类算法来继续进行。

这是生成的包含三个簇的数据集。

接下来，我们将使用 SciPy 库中的 linkage 函数计算连接矩阵。这个矩阵将捕捉数据点之间的层次关系。然后，我们将使用树状图可视化这种关系。

这是层次聚类产生的树状图。每条垂直线代表两个聚类的合并。垂直线的高度表示合并发生的距离。当你从树状图的底部移动到顶部时，聚类会依次合并，直到只剩下一个大聚类。

为了决定我们数据集的聚类数量，我们将切割树状图。一种常见的做法是选择一个距离阈值，并在该距离处画一条水平线。水平线与垂直线相交的垂直线数量就是聚类的数量。

对于这个演示，我们将切割树状图以检索三个聚类（因为我们最初生成数据时包含三个聚类）。然后我们将可视化这些聚类。

这里是层次聚类算法在合成数据集上的结果。数据点根据切割树状图识别的聚类进行着色。

算法已成功识别并将数据点分组为三个不同的聚类，这与合成数据的生成方式相吻合。

列表 7.2 展示了 hierarchical_clustering_GPT4.py 的内容，该内容说明了如何使用层次聚类算法和 death.csv 数据集创建机器学习模型。

列表 7.2：hierarchical_clustering_GPT4.py

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

plt.title("包含 3 个聚类的生成数据集")

plt.xlabel("特征 1")

plt.ylabel("特征 2")

plt.show()

# 计算连接矩阵

Z = linkage(X_hc, 'ward') # 使用 'ward' 方法作为连接标准

# 显示树状图

plt.figure(figsize=(10, 7))

dendrogram(Z)

plt.title("层次聚类树状图")

plt.xlabel("数据点")

plt.ylabel("欧几里得距离")

plt.show()

列表 7.2 从几个导入语句开始，然后调用 make_blobs() 创建合成数据集。下一个代码块通过此代码片段生成并显示从生成数据集中的数据创建的散点图：

plt.scatter(X[:, 0], X[:, 1], c=y, s=50, cmap='viridis')

列表 7.2 列表 7.2 的下一部分通过调用 linkage() 方法初始化变量 Z 以执行层次/聚合聚类，随后是一段调用 dendrogram(Z) 来显示树状图的代码块。有关更详细的信息，请参阅 sklearn 文档中关于 linkage() 方法的说明：

[`docs.scipy.org/doc/scipy/reference/generated/scipy.cluster.hierarchy.linkage.html#scipy.cluster.hierarchy.linkage`](https://docs.scipy.org/doc/scipy/reference/generated/scipy.cluster.hierarchy.linkage.html#scipy.cluster.hierarchy.linkage)

运行列表 7.2 中的代码，你将看到生成三个图像。图 7.3(#fig_7-3)显示了三个聚类，图 7.4(#fig_7-4)显示了一棵树状图（这是一种树状结构），它可视化了图 7.3(#fig_7-3)中显示的三个聚类。

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p215.jpg)

图 7.3 三聚类

使用 DBSCAN 算法的机器学习模型

本节包含了一个 GPT-4 使用 DBSCAN 算法和合成数据集生成机器学习模型的示例。本节的前半部分包含了 GPT-4 执行步骤的解释，随后是列表 7.3，其中包含了 GPT-4 生成的基于 Python 的代码。

使用 DBSCAN 算法创建 ML 模型的流程包括以下步骤：

1. 生成合成数据集：我们将重复使用之前创建的带有 blob 的数据集。

2. 可视化数据集：为了理解聚类分布

3. 应用 DBSCAN：使用 DBSCAN 算法识别数据集中的聚类。

4. 可视化结果：根据 DBSCAN 识别出的聚类对数据集进行着色。

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p216.jpg)

图 7.4 一棵树状图

让我们从可视化之前生成的合成数据集开始。

这里是我们将使用 DBSCAN 算法进行聚类的生成数据集。

现在，让我们应用 DBSCAN 算法来识别聚类。

这里是 DBSCAN 算法在合成数据集上的结果。数据点根据 DBSCAN 识别出的聚类进行着色。

DBSCAN 已成功识别数据集中的聚类。请注意，DBSCAN 可能会将一些点标记为噪声（通常标记为“-1”）。在这个可视化中，似乎所有点都被分配到了聚类中，这表明在这个特定实例中没有噪声。

列表 7.3 展示了 DBSCAN_GPT4.py 的内容，说明了如何使用 DBSCAN 算法和 death.csv 数据集创建机器学习模型。

列表 7.3：DBSCAN_GPT4.py

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

plt.title("生成数据集")

plt.xlabel("特征 1")

plt.ylabel("特征 2")

plt.show()

from sklearn.cluster import DBSCAN

# 应用 DBSCAN 聚类

dbscan = DBSCAN(eps=2.5, min_samples=5)

dbscan_labels = dbscan.fit_predict(X_hc)

# 可视化 DBSCAN 识别出的聚类

plt.figure(figsize=(8, 6))

plt.scatter(X_hc[:, 0], X_hc[:, 1], c=dbscan_labels, s=50, cmap='viridis')

plt.title("DBSCAN 聚类结果")

plt.xlabel("特征 1")

plt.ylabel("特征 2")

plt.show()

列表 7.3 从几个导入语句开始，接着调用 make_blobs()来创建一个合成数据集。下一个代码块从生成的数据集中的数据生成并显示散点图。

列表 7.3 的下一部分初始化变量 dbscan 为从 sklearn.cluster 导入的类 DBSCAN 的一个实例。请注意，变量 dbscan_labels 使用调用变量 dbscan 的 fit_predict()方法的结果进行初始化。dbscan_labels 的内容是一系列簇标签，其中“噪声”样本被分配标签“-1”。此外，参数 eps 指定两个样本之间的最大距离，一个样本被视为另一个样本的邻域。

列表 7.3 的最后一部分创建了一个散点图，显示了 DBSCAN 在数据集中识别出的簇。运行列表 7.3 中的代码，你会看到生成两个图像。图 7.5 显示了三个簇，图 7.6 显示了带有簇标签的三个簇。

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p218-1.jpg)

图 7.5 生成的数据集

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p218-2.jpg)

图 7.6 带有聚类标签的三个簇

摘要

本章是关于聚类材料的第三个完整章节，这些材料是由 GPT-4 生成的。在对聚类进行简要概述后，你看到了十个聚类算法的列表，包括它们的优缺点。此外，你还学习了聚类算法的度量标准。

最后，你看到了 GPT-4 生成的 kMeans、层次聚类和 DBSCAN 聚类算法的 Python 代码示例。

接下来，你看到了一个基于 Python 的 k-means 算法代码示例，这是机器学习中流行的聚类算法之一。然后，你学习了层次聚类算法，随后是一个使用该算法的基于 Python 的代码示例。此外，你还看到了一个基于 Python 的 DBSCAN 算法代码示例，这是机器学习中的另一个流行聚类算法。

第八章

CHATGPT 与数据可视化

本章包含使用 ChatGPT 和 GPT-4 进行数据可视化的示例，例如基于数据集（例如，泰坦尼克号数据集）的图表和图形。ChatGPT 通过高级数据分析插件生成了所有代码示例。ChatGPT 还生成了一些与基于 Python 的代码示例相关的文本。

本章的第一部分描述了在 ChatGPT 中上传数据集的过程，然后提供了诸如解释给定数据集的特征、生成可视化以及下载精选数据集等任务的提示。你还将学习如何提示 ChatGPT 创建和训练机器学习模型。

本章的第二部分包含使用 Matplotlib 进行数据可视化的示例，其中代码示例由 ChatGPT 生成。本章的第三部分包含使用 Seaborn 进行数据可视化的示例，其中代码示例由 ChatGPT 生成。

在你阅读本章内容之前，请记住，本章以及第五章、第六章和第七章中 GPT-4 生成的 AI 内容已经应用了一些格式。然而，额外的格式已被保持在最低限度，以便你熟悉 GPT-4 的风格。

工作与图表和图形

如果你已经与图表和图形工作过，那么你已经知道每种图表类型都有其独特的优势，并且最适合特定类型的数据和分析。图表的选择通常取决于数据的性质和希望得出的具体见解。本节包含多个子节，提供了有关各种图表和图形的信息，如下所示：

+   条形图

+   饼图

+   折线图

+   热图

+   直方图

+   箱线图

+   帕累托图

+   雷达图

+   树状图

+   水流图

+   散点图

上一条目列表中的大多数图表和图形将在以下子节中进行讨论。

条形图

条形图用矩形条表示数据。条形的长度与它们所代表的值成比例。它们可以是垂直的（柱状图）或水平的。一个使用示例是比较商店中不同产品的销售情况。

列出以下条形图的优点：

+   容易理解且广泛认可

+   可以比较单个或多个数据系列

+   适用于显示跨越多个类别的数据

列出以下条形图的缺点：

+   不适合显示随时间变化的模式或趋势

+   比较太多类别时可能会变得杂乱

饼图

饼图以圆形格式表示数据，其中各个部分（切片）显示类别与整体的比例。一个使用示例是表示一个行业中不同公司的市场份额。

列出以下饼图的优点：

+   简单的视觉表示，显示部分与整体的关系

+   可以清楚地表明比例

+   当类别有限时，效果较好

列出以下饼图的缺点：

+   不适合比较单个类别

+   当切片过多时，可能会变得无效且难以解释

+   不显示绝对值，只显示比例

折线图

折线图通过直线连接数据点。它们主要用于可视化连续区间或时间段内的值。一个使用示例是跟踪一家公司在几年内的收入增长。

列出以下折线图的优点：

+   适用于显示随时间变化的趋势

+   可以在一个图表上比较多个数据系列

+   清晰地可视化数据点和区间

下面列出了线图的缺点：

+   不适合显示部分与整体的关系

+   显示太多数据系列时可能会变得杂乱

+   需要数据点的有意义顺序

热图

热图以矩阵格式表示数据，其中单个值以颜色表示。颜色强度通常表示值的幅度。一个使用示例涉及可视化网页不同部分的访问者活动。

下面列出了热图的优点：

+   快速识别模式、相关性和集中区域

+   有效地使用颜色来传达关于大小信息

下面列出了热图的缺点：

+   不适合详细数值分析

+   颜色选择至关重要；选择不当可能导致误解。

直方图

直方图是数据集分布的图形表示。它是连续变量概率分布的估计。一个使用示例涉及展示人口中年龄的分布。

下面列出了直方图的优点：

+   通过指示位于值范围内的数据点数量来提供数值数据的视觉解释

+   可以帮助识别数据分布模式

下面列出了直方图的缺点：

+   不显示确切值

+   箱的数目和宽度可以影响感知

箱线图

箱线图，或箱线图，使用四分位数来总结数据集。其中，“箱”显示四分位距，而“胡须”表示超出上下四分位数的变异性。一个使用示例涉及比较不同团队的销售额表现。

下面列出了箱线图的优点：

+   快速可视化数据的分布和偏斜

+   识别异常值

下面列出了箱线图的缺点：

+   不适合详细分布分析

+   不显示数据的频率分布

帕累托图

帕累托图结合柱状图和折线图来表示发生累积频率。它识别数据集中的最重要因素。一个使用示例涉及确定哪些产品缺陷最频繁发生。

下面列出了帕累托图的优点：

+   高效地突出大型数据集中最重要的因素

+   帮助优先考虑努力

下面列出了帕累托图的缺点：

+   限于与排名和优先排序相关的数据集

+   不适合显示数据点之间的关系

雷达图

雷达图是一种在二维图表中显示三个或更多定量数据的图形方法。数据点绘制在从中心开始的轴上。一个使用示例涉及比较产品的性能指标。

下面列出了雷达图的优点：

+   可以比较多个定量变量

+   提供数据的视觉概述

雷达图的以下缺点如下：

+   比较过多数据集时可能会变得杂乱

+   当值相似时难以解释

树图

树图以嵌套矩形的形式显示层次数据。每个层次分支由彩色矩形表示。一个使用示例涉及可视化计算机上的存储使用情况。

树图的以下优点如下：

+   空间使用效率高

+   可以使用大小和颜色表示多个维度

树图的以下缺点如下：

+   不适用于具有大量层次的数据集

+   可能变得难以解释

水流图

水流图表示依次发生的正或负值的累积效应。一个使用示例涉及可视化利润或收入如何受各种因素的影响。

水流图的以下优点如下：

+   清晰地可视化正负顺序变化

+   帮助理解从一个数据点到另一个数据点的逐渐过渡

水流图的以下缺点如下：

+   限于需要理解顺序变化的情况

+   数据点过多时可能会变得难以理解

使用 Matplotlib 的线形图

以下提示被提供给 GPT-4 以生成简单的线形图的 Python 代码：“请生成用于可视化趋势的简单线形图的 Python 代码。”

列表 8.1 显示了 ChatGPT 生成的 line_plots.py 的内容，该内容用于使用 Matplotlib 渲染线形图。

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

plot_line(x, y, '样本线形图', 'X 轴', 'Y 轴')

列表 8.1 从一个导入语句开始，然后定义了一个名为 plot_line() 的函数，该函数用于渲染线形图。Matplotlib 的 plot() 函数提供了一个创建线图的直接方法。在这个函数中，我们可视化 x 轴和 y 轴上的趋势。

以下代码段初始化了 Python 列表 x 和 y，然后使用三个字符串调用 plot_line()，这三个字符串分别是标题、水平轴和垂直轴的值。图 8.1 显示了在 列表 8.1 中启动代码的输出。

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p226.jpg)

图 8.1 使用 Matplotlib 创建的线形图

使用 Matplotlib 的饼图

饼图非常适合显示类别之间的比例数据。Matplotlib 的饼图函数提供了一个简单的方法来实现这一点。以下提示被提供给 GPT-4 以生成用于饼图的 Python 代码：“请生成显示简单饼图的 Python 代码。”

列表 8.2 显示了 ChatGPT 生成的 pie_chart1.py 的内容，该内容用于使用 Matplotlib 渲染饼图。

列表 8.2: pie_chart1.py

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p227-2.jpg)

列表 8.2 以与列表 8.1 类似的方式开始，除了生成了用于生成饼图的 plot_pie()函数。列表 8.2 的下一部分初始化 Python 列表的标签和大小。使用这些列表以及一个作为饼图标题显示的字符串调用 plot_pie()函数。图 8.2 显示了通过在列表 8.2 中启动代码生成的饼图。

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p227-1.jpg)

图 8.2 使用 Matplotlib 创建的饼图

使用 Matplotlib 绘制箱型和须图

箱型图，或箱型和须图，提供了数据分布的总结，突出了中心趋势、变异性和异常值的存在。它们在比较不同组之间的分布时特别有用。它们可以根据最小值、第一四分位数、中位数、第三四分位数和最大值显示数据的分布。

以下提示被提供给 GPT-4 以生成用于绘制箱型图的 Python 代码：“请生成用于绘制箱型图的 Python 代码。”

列表 8.3 显示了 ChatGPT 生成的用于使用 Seaborn 绘制箱型图的 boxplot1.py 的内容。

列表 8.3：boxplot1.py

导入 matplotlib.pyplot 库作为 plt

导入 seaborn 库作为 sns

导入 matplotlib.pyplot 库作为 plt

定义 plot_box(data, column)函数

plt.boxplot(data[column])

plt.show()

# 用法

data = sns.load_dataset("iris")

plot_box(data, "sepal_length")

列表 8.3 包含三个导入语句，随后是生成箱型图的 plot_box()函数。列表 8.3 的下一部分初始化变量 data 为 Seaborn 内置的 iris 数据集的内容，然后使用 data 和一个字符串调用 plot_box()，该字符串指定了在绘制箱型图时使用的特征（列）。图 8.3 显示了通过在列表 8.3 中启动代码生成的箱型图。

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p228.jpg)

图 8.3 使用 Matplotlib 创建的箱型图

使用 Matplotlib 进行时间序列可视化

时间序列数据，其中观察值在固定时间间隔内进行，可以使用折线图进行可视化。这使分析师能够识别趋势、模式和异常。以下提示被提供给 GPT-4 以生成用于时间序列数据的 Python 代码：“请生成用于绘制时间序列数据的 Python 代码。”

列表 8.4 显示了 ChatGPT 生成的用于使用 Matplotlib 绘制时间序列的 time_series.py 的内容。

列表 8.4：time_series.py

导入 matplotlib.pyplot 库作为 plt

导入 pandas 库作为 pd

定义 plot_time_series(dates, values, title)函数

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

图 8.4 展示了通过运行列表 8.4 中的代码生成的时间序列。

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p229.jpg)

图 8.4 使用 Matplotlib 创建的时间序列

使用 Matplotlib 的堆叠柱状图

堆叠柱状图允许在每个类别中表示子组，从而在类别之间提供总大小的感觉，并在其中显示子组分布。以下提示被提供给 GPT-4 以生成堆叠柱状图的 Python 代码：“请生成显示堆叠柱状图的 Python 代码。”

列表 8.5 展示了 ChatGPT 生成的用于使用 Matplotlib 绘制堆叠柱状图的`stacked_bar_charts.py`的内容。

列表 8.5: stacked_bar_charts.py

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p230-1.jpg)

图 8.5 展示了通过运行列表 8.5 中的代码生成的堆叠柱状图。

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p230-2.jpg)

图 8.5 ChatGPT 生成的堆叠柱状图

使用 Matplotlib 的饼图

饼图是饼图的变体。空心中心可以用于额外的注释或只是提供不同的美学。它们在类别之间按比例表示数据，类似于饼图，但具有空心中心。以下提示被提供给 GPT-4 以生成饼图的 Python 代码：“请生成绘制饼图的 Python 代码。”

列表 8.6 展示了 ChatGPT 生成的用于使用 Matplotlib 绘制饼图的`donut_charts.py`的内容。

列表 8.6: donut_charts.py

import matplotlib.pyplot as plt

def plot_donut_chart(sizes, labels, title, hole_size=0.3):

fig, ax = plt.subplots()

ax.pie(sizes, labels=labels, autopct='%1.1f%%',

startangle=90, wedgeprops=dict(width=hole_size))

ax.axis('equal')

plt.title(title)

plt.show()

# 用法

labels = ['A', 'B', 'C']

sizes = [215, 130, 245]

plot_donut_chart(sizes, labels, 'Sample Donut Char')

图 8.6 展示了通过运行列表 8.6 中的代码生成的饼图。

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p231.jpg)

图 8.6 使用 Matplotlib 创建的饼图

使用 Matplotlib 的 3D 表面图

三维（3D）表面图用于可视化具有两个变量的函数。它们可以揭示数据中的复杂模式和关系。以下提示被提供给 GPT-4 以生成 3D 表面的 Python 代码：“请生成绘制 3D 表面的 Python 代码。”

列表 8.7 展示了 ChatGPT 生成的用于使用 mpl_toolkits 渲染 3D 表面的`3d_surface.py`的内容。

偶然间，如果你遇到 mpl_toolkits 的问题，请阅读以下帖子，其中包含有用的信息：

[`stackoverflow.com/questions/37661119/python-mpl-toolkits-installation-issue`](https://stackoverflow.com/questions/37661119/python-mpl-toolkits-installation-issue)

列表 8.7: 3d_surface.py

import matplotlib.pyplot as plt

导入 numpy 库作为 np

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

列表 8.7 以两个导入语句开始，后面是渲染 3D 图的 plot_3d_surface() 函数。列表 8.7 的后半部分通过 NumPy 函数 linspace() 初始化变量 x 和 y，该函数将区间划分为一组等大小的子区间。

例如，代码片段 np.linspace(-5, 5, 50) 将区间 [-5,5] 划分为 50 个等间距的点，这意味着有 49 个宽度相等的区间。你可以通过将 50 替换为 3 来说服自己这是正确的：结果是左端点 -5、中点和右端点 5，这创建了 2 (=3-1) 个区间。

下一个代码片段在调用 NumPy 中的 meshgrid() 函数的结果更新 x 和 y 之后，将 z 定义为应用于点 (x,y) 到原点距离的三角正弦函数。尽管后者随着点 (x,y) 从原点移开而单调增加，而 z 是该距离的正弦值，它是一个周期函数：因此，你会看到滚动波浪状的效果。

列表 8.7 中的最后一个代码片段使用变量 x、y 和 z 中的值调用 plot_3d_surface() 函数。运行 列表 8.7 中的代码，你将看到 图 8.7 中显示的 3D 曲面。

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p233.jpg)

图 8.7 使用 Matplotlib 创建的 3D 曲面

使用 MATPLOTLIB 的径向（或蜘蛛）图

径向（或蜘蛛）图用于以二维图表的形式可视化多维数据，其中包含三个或更多定量变量。每个变量都表示在从图表中心开始的单独轴上。以下提示被提供给 GPT-4 以生成用于径向图的 Python 代码：“请生成用于显示径向图的 Python 代码。”

列表 8.8 显示了 ChatGPT 生成的 radial_charts.py 的内容，用于使用 Matplotlib 渲染径向图。

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

# 下面的代码片段会导致错误：

# ax.set_xticks(angles)

# 下面的代码片段是正确的：

ax.set_xticks(angles[:-1]) # 排除最后一个角度，因为它具有周期性

ax.set_xticklabels(categories)

plt.title(title, size=20, color="blue", y=1.1)

plt.show()

# 用法

categories = ["A", "B", "C", "D"]

values = [50, 30, 60, 40]

plot_spider_chart(values, categories, 'Sample Spider Chart')

列表 8.8 以两个导入语句开始，随后是 Python 函数 plot_spider_chart()，该函数用于渲染径向图。列表 8.8 的第二个部分初始化变量 categories 和 values 为两个 Python 列表，然后使用变量 categories、values 和一个用于图表标题的文本字符串调用函数 plot_spider_chart()。图 8.8 显示了通过运行列表 8.8 中的代码生成的径向图。

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p234.jpg)

图 8.8 使用 Seaborn 创建的径向图

有一个细节可以帮助您调试 ChatGPT 为您生成的代码。让我们看看列表 8.8 中加粗的代码块：

# 以下代码片段导致错误：

# ax.set_xticks(angles)

# 以下代码片段是正确的：

ax.set_xticks(angles[:-1]) # 排除最后一个角度，因为它具有循环性

如果您交换这两个代码片段的顺序，代码将无法正确工作。以下是与 ChatGPT 的“对话”，以请求解决方案。

作者：“我上传了 radial_charts.py，其中包含您为我编写的代码。然而，这段代码导致以下错误：ValueError：FixedLocator 位置的数目（5），通常由 set_ticks 调用设置，与 ticklabels 的数目（4）不匹配。您能提供解决方案吗？”

ChatGPT 的响应如下：

感谢您提供 radial_charts.py 文件。让我们首先读取其内容，以了解代码的结构和上下文。之后，我将分析提到的错误潜在原因，并提出解决方案。

提供的 radial_charts.py 文件包含一个名为 plot_spider_chart 的函数，该函数旨在使用给定的值和类别绘制蜘蛛图（或雷达图）。

根据您报告的错误和代码结构，问题可能源于 tick 位置的数目（由 ax.set_xticks(angles)设置）与 tick 标签的数目（由 ax.set_xticklabels(categories)设置）不匹配。

为了解决这个问题，我将确保 tick 位置的数目与 tick 标签的数目相匹配。让我们进行这个调整，并提供函数的修正版本。

作者：“现在工作正常了！感谢您的帮助！”

ChatGPT 的响应如下：

欢迎您！很高兴听到它现在按预期工作。如果您将来有任何更多问题或需要进一步的帮助，请随时联系。祝您编码愉快！

MATPLOTLIB 的等高线图

等高线图有助于使用等高线在二维中可视化三维数据。每条等高线代表相等值的点。以下提示被提供给 GPT-4 以生成绘制等高线的 Python 代码：“请生成绘制等高线的 Python 代码。”

列表 8.9 显示了 ChatGPT 生成的用于使用 Matplotlib 绘制等高线的 contour_lines.py 的内容。

列表 8.9: contour_lines.py

导入 matplotlib.pyplot 库作为 plt

导入 numpy 库作为 np

def plot_contour(x, y, z):

plt.contourf(x, y, z, 20, cmap='viridis')

plt.colorbar()

plt.show()

# 使用方法

x = np.linspace(-5, 5, 50)

y = np.linspace(-5, 5, 50)

x, y = np.meshgrid(x, y)

z = np.sin(np.sqrt(x**2 + y**2))

绘制等高线图：plot_contour(x, y, z)

列表 8.9 包含两个导入语句，然后定义了一个函数 plot_contour()，用于渲染代码示例的等高线。注意，列表 8.9 的第二部分几乎与列表 8.7 的后半部分代码相同。图 8.9 显示了通过运行列表 8.9 中的代码生成的等高线图。

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p236.jpg)

图 8.9 使用 Seaborn 创建的等高线图

矢量场流线图

流线图用于显示矢量场，如风向。它们提供了流动轨迹的快照，并且可以用于标量数据，并且可以可视化矢量场作为流线。以下提示被提供给 GPT-4 以生成用于矢量场的 Python 代码：“请生成用于显示矢量场的 Python 代码。”

列表 8.10 显示了 ChatGPT 生成的 stream_plot.py 的内容，用于使用 Seaborn 渲染流线图。

列表 8.10: stream_plot.py

导入 matplotlib.pyplot 库作为 plt

导入 seaborn 库作为 sns

导入 numpy 库作为 np

定义一个函数 plot_streamplot(x, y, u, v)，用于渲染代码示例的等高线

plt.streamplot(x, y, u, v, density=1)

plt.show()

# 使用方法

x = np.linspace(-5, 5, 10)

y = np.linspace(-5, 5, 10)

# 这导致了一个错误：

#y, x = np.meshgrid(y, x)

# 这行是正确的：

x, y = np.meshgrid(x, y)

u = -1 - x**2 + y

v = 1 + x - y**2

plot_streamplot(x, y, u, v)

图 8.10 显示了通过运行列表 8.10 中的代码生成的流线图。

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p237.jpg)

图 8.10 使用 Seaborn 创建的流线图

ChatGPT 在列表 8.10 中的初始代码没有正确运行，所以我要求 ChatGPT 在接下来的“对话”中提供解决方案。

作者：“我上传了包含你为我编写的代码的 stream_plot.py。这段代码导致以下错误：ValueError：'x'的行必须相等。你能提供解决方案吗？”

ChatGPT 的响应如下：

数组 x、y、u 和 v 的形状都是(10,10)，这意味着它们在尺寸上是一致的。错误信息“ValueError：'x'的行必须相等”表明，可能存在 x 数组行中的值的问题，而不是其形状。

语句 y, x = np.meshgrid(y, x)交换了原始的 x 和 y 数组。这可能会导致 x 数组的行中存在不一致性。

为了解决错误，我将修改网格创建方式，并确保 x 和 y 数组被正确初始化。让我们进行必要的调整。

作者：“这行得通！感谢你的帮助！”

ChatGPT 的响应如下：

您好！很高兴听到它现在按预期工作。如果您将来有任何更多问题或需要进一步的帮助，请随时联系。祝您编码愉快！

矢量场箭头图

箭头图在表示矢量场时非常有用，可以显示矢量的方向和大小。例如，在物理学中，它们可以用来显示电场或流体流动方向。以下提示被提供给 GPT-4 以生成绘制箭头图的 Python 代码：“请生成绘制箭头图的 Python 代码。”

列表 8.11 展示了 ChatGPT 生成的 quiver_plot.py 文件内容，用于使用 Matplotlib 绘制箭头图。

列表 8.11: quiver_plot.py

import matplotlib.pyplot as plt

import numpy as np

def plot_quiver(x, y, u, v):

plt.quiver(x, y, u, v, scale=20)

plt.show()

# 用法

x, y = np.meshgrid(np.arange(0, 2 * np.pi, .2), np.arange(0, 2 * np.pi, .2))

u = np.sin(x)

v = np.cos(y)

plot_quiver(x, y, u, v)

图 8.11 展示了通过运行 列表 8.11 中的代码生成的箭头图。

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p239.jpg)

图 8.11 使用 Seaborn 创建的箭头图

极坐标图

极坐标图（或径向图）适合在二维图表中显示多元数据，其中变量从同一点开始表示在轴上。它们对于根据角度和大小查看模式非常有用。以下提示被提供给 GPT-4 以生成极坐标图的 Python 代码：“请生成显示极坐标图的 Python 代码。”

列表 8.12 展示了 ChatGPT 生成的 polar_plots.py 文件内容，用于使用 Seaborn 绘制堆叠的极坐标图。

列表 8.12: polar_plots.py

import matplotlib.pyplot as plt

import numpy as np

def plot_polar(theta, radii, title=""):

plt.figure(figsize=(8, 4))

ax = plt.subplot(111, projection='polar')

ax.plot(theta, radii)

ax.set_title(title)

plt.show()

# 用法

theta = np.linspace(0, 2 * np.pi, 100)

radii = np.abs(np.sin(theta) * 2)

plot_polar(theta, radii, "示例极坐标图")

图 8.12 展示了通过运行 列表 8.12 中的代码生成的极坐标图。

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p240.jpg)

图 8.12 使用 Matplotlib 创建的极坐标图

使用 Seaborn 的条形图

Seaborn 为 Matplotlib 提供了一个高级接口，使得创建时尚的图表更加容易。此条形图有助于可视化不同类别中的数据。以下提示被提供给 GPT-4 以生成条形图的 Python 代码：“请生成绘制条形图的 Python 代码。”

注意：Seaborn 与 Pandas 集成时效果最佳。

列表 8.13 展示了 ChatGPT 生成的 bar_chart1.py 文件内容，用于使用 Seaborn 绘制条形图。

列表 8.13: bar_chart1.py

import matplotlib.pyplot as plt

import seaborn as sns

import pandas as pd

def plot_bar(data, x_col, y_col):

sns.barplot(x=x_col, y=y_col, data=data)

plt.show()

# 用法

data = pd.DataFrame({

'Category': ['A', 'B', 'C'],

'Values': [10, 20, 15]

})

plot_bar(data, 'Category', 'Values')

列表 8.13 以三个导入语句开始，随后是绘制条形图的 plot_bar() 函数。列表 8.13 的后半部分初始化 Pandas 数据帧 data，然后使用 data 和用于标记水平轴的字符串以及用于标记垂直轴的另一个字符串调用 plot_bar()。图 8.13 显示了通过启动列表 8.13 中的代码生成的条形图。

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p241.jpg)

图 8.13 ChatGPT 生成的条形图

使用 SEABORN 绘制带有回归线的散点图

散点图显示数据点，并使用回归线帮助揭示关系。以下提示被提供给 GPT-4 以生成用于绘制回归线的 Python 代码：“请生成用于绘制回归线的 Python 代码。”

列表 8.14 显示了 ChatGPT 生成的用于使用 Seaborn 绘制散点图的 scatter_plot.py 的内容。

列表 8.14: scatter_plot.py

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

列表 8.14 以三个导入语句和绘制散点图的 plot_scattter_with_regression() 函数开始。列表 8.13 的后半部分初始化 Pandas 数据帧 data，然后使用变量 data 调用 plot_scattter_with_regression()。图 8.14 显示了通过启动列表 8.14 中的代码生成的散点图。

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p242.jpg)

图 8.14 ChatGPT 生成的散点图

使用 SEABORN 绘制相关矩阵的热图

热图用于表示数据矩阵，颜色表示大小。一个常见的用例是可视化相关矩阵，这有助于揭示不同变量之间的关系。以下提示被提供给 GPT-4 以生成用于简单线图的 Python 代码：“请生成用于绘制热图的 Python 代码。”

列表 8.15 显示了 ChatGPT 生成的用于使用 Matplotlib 绘制线的 heatmap1.py 的内容。

列表 8.15: heatmap1.py

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

列表 8.15 从三个导入语句和用于渲染热图的 plot_heatmap() 函数开始。列表 8.15 的后半部分初始化 Pandas 数据帧 data，然后使用变量 data 调用 plot_heatmap()。图 8.15 显示了通过运行列表 8.15 中的代码渲染的热图。

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p243.jpg)

图 8.15 使用 Matplotlib 创建的热图

使用 Seaborn 绘制直方图

直方图是可视化数据分布的强大工具。Seaborn 的 histplot() 函数提供了一种轻松生成直方图的方法，并具有额外的功能，如核密度估计。以下提示被提供给 GPT-4 以生成用于直方图的 Python 代码：“请生成用于绘制直方图的 Python 代码。”

列表 8.16 显示了 ChatGPT 生成的用于使用 Seaborn 绘制直方图的 histogram1.py 的内容。

列表 8.16：histogram1.py

import matplotlib.pyplot as plt

import seaborn as sns

def plot_histogram(data, column, bins=10):

sns.histplot(data[column], bins=bins)

plt.show()

# 用法

data = sns.load_dataset("iris")

plot_histogram(data, "sepal_length")

列表 8.16 从两个导入语句和用于渲染直方图的 plot_histogram() 函数开始。列表 8.16 的后半部分使用 Seaborn 内置数据集 iris 的内容初始化 Pandas 数据帧 data，然后使用变量 data 调用 plot_histogram()。图 8.16 显示了通过运行列表 8.16 中的代码渲染的 iris 数据集的热图。

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p244.jpg)

图 8.16 ChatGPT 生成的直方图

使用 Seaborn 绘制小提琴图

小提琴图提供了对数据分布的更深入理解。它们结合了箱线图和直方图的特点，显示了数据在不同值处的概率密度。您可以将箱线图和直方图的方面结合起来，以提供对数据分布的更丰富描述。以下提示被提供给 GPT-4 以生成用于小提琴图的 Python 代码：“请生成用于绘制小提琴图的 Python 代码。”

列表 8.17 显示了 ChatGPT 生成的用于使用 Seaborn 绘制小提琴图的 violin_plots.py 的内容。

列表 8.17：violin_plots.py

import seaborn as sns

def plot_violin(data, x_col, y_col):

sns.violinplot(x=x_col, y=y_col, data=data)

plt.show()

# 用法

data = sns.load_dataset("iris")

plot_violin(data, "species", "sepal_length")

列表 8.17 从一个导入语句和用于渲染小提琴图的 plot_violin() 函数开始。列表 8.17 的后半部分使用 Seaborn 内置数据集 iris 的内容初始化 Pandas 数据帧 data。它使用变量 data 调用 plot_violin()。图 8.17 显示了通过运行列表 8.17 中的代码渲染的小提琴图。

![image](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p245.jpg)

图 8.17 使用 Seaborn 创建的小提琴图

使用 SEABORN 创建的配对图

当处理具有多个特征的集合时，可视化特征之间的成对关系通常很有帮助。Seaborn 有一个 pairplot() 函数，可以生成散点图的矩阵，允许探索此类关系。以下提示被提供给 GPT-4 以生成用于配对图的 Python 代码：“请生成显示配对图的 Python 代码。”

列表 8.18 显示了 ChatGPT 生成的 pair_plots.py 的内容，用于使用 Matplotlib 绘制线条。

列表 8.18：pair_plots.py

import matplotlib.pyplot as plt

import seaborn as sns

def plot_pairplot(data):

sns.pairplot(data)

plt.show()

# 使用方法

data = sns.load_dataset("iris")

plot_pairplot(data)

列表 8.18 从两个导入语句和用于渲染配对图的 plot_pairplot() 函数开始。列表 8.18 的第二部分使用 Seaborn 内置数据集 iris 的内容初始化 Pandas 数据帧 data，然后使用变量 data 调用 plot_pair()。图 8.18 显示了通过运行列表 8.18 中的代码渲染的配对图。

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p247.jpg)

图 8.18 使用 Matplotlib 创建的配对图

使用 SEABORN 创建的分面网格

分面网格是基于分类变量在多个子图中可视化数据分布的一种方式。每个分面（子图）代表一个类别。以下提示被提供给 GPT-4 以生成用于分面网格的 Python 代码：“请生成绘制分面网格的 Python 代码。”

列表 8.19 显示了 ChatGPT 生成的 facet_grids.py 的内容，用于创建和渲染按类别分割的多个图表。

列表 8.19：facet_grids.py

import matplotlib.pyplot as plt

import seaborn as sns

def plot_facetgrid(data, x_col, y_col, facet_col):

g = sns.FacetGrid(data, col=facet_col)

g.map(sns.scatterplot, x_col, y_col)

g.add_legend()

plt.show()

# 使用方法

data = sns.load_dataset("iris")

plot_facetgrid(data, "sepal_length", "sepal_width", "species")

列表 8.19 从两个导入语句和用于渲染分面的 plot_facetgrid() 函数开始。列表 8.19 的第二部分使用 Seaborn 内置数据集 iris 的内容初始化 Pandas 数据帧 data，然后使用变量 data 调用 plot_pair()。图 8.19 显示了通过运行列表 8.19 中的代码渲染的分面网格。

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p248.jpg)

图 8.19 使用 Seaborn 创建的分面网格

层次聚类

Seaborn 的 clustermap 是一个二维矩阵数据集表示，其中行和列都是层次聚类的。这允许从复杂数据集中出现模式。以热图格式可视化层次聚类关系。以下提示被提供给 GPT-4 以生成层次聚类的 Python 代码：“请生成用于显示层次聚类的 Python 代码。”

列表 8.20: cluster_map.py

导入 matplotlib.pyplot 库为 plt

导入 seaborn 库为 sns

def plot_clustermap(data):

sns.clustermap(data, method='average', cmap='coolwarm')

plt.show()

# 用法

data = sns.load_dataset("iris").drop("species", axis=1)

plot_clustermap(data)

列表 8.20 从两个导入语句和用于渲染聚类图的 plot_clustermap() 函数开始。列表 8.20 的第二部分使用 Seaborn 内置数据集 iris 的内容初始化 Pandas 数据帧 data，然后使用变量 data 调用 plot_pair() 函数。图 8.20 显示了通过运行列表 8.20 中的代码渲染的聚类图。

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p249.jpg)

使用 Seaborn 创建的聚类图 8.20

SWARM 图

Swarm plot 将每个数据点在分类轴上以最小重叠的方式定位，从而更好地表示值的分布。它创建了一个非重叠点的分类散点图。以下提示被提供给 GPT-4 以生成用于绘制 swarm plot 的 Python 代码：“请生成用于绘制 swarm plot 的 Python 代码。”

列表 8.21 显示了 ChatGPT 生成的用于使用 Seaborn 渲染等高线的 swarm_plot.py 的内容。

列表 8.21: swarm_plot.py

导入 matplotlib.pyplot 库为 plt

导入 seaborn 库为 sns

def plot_swarm(data, x_col, y_col):

sns.swarmplot(x=x_col, y=y_col, data=data)

plt.show()

# 用法

data = sns.load_dataset("iris")

plot_swarm(data, "species", "sepal_length")

列表 8.21 从两个导入语句和用于渲染 swarm 图的 plot_swarm() 函数开始。列表 8.21 的第二部分使用 Seaborn 内置数据集 iris 的内容初始化 Pandas 数据帧 data，然后使用变量 data 调用 plot_swarm() 函数。图 8.21 显示了通过运行列表 8.21 中的代码渲染的 swarm 图。

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p250.jpg)

图 8.21 使用 Seaborn 创建的 swarm 图

双变量数据的联合图

Seaborn 的 jointplot 显示了两个变量之间的关系。它结合了散点图、回归图，甚至与直方图结合的六边形图。它显示了两个变量之间的关系，以及它们的各自分布。以下提示被提供给 GPT-4 以生成用于双变量数据的 swarm plot 的 Python 代码：“请生成用于绘制双变量 swarm plot 的 Python 代码。”

列表 8.22 显示了 ChatGPT 生成的用于使用 Seaborn 渲染联合图的 joint_plot.py 的内容。

列表 8.22：joint_plot.py

import matplotlib.pyplot as plt

import seaborn as sns

def plot_jointplot(data, x_col, y_col, kind='scatter'):

sns.jointplot(x=x_col, y=y_col, data=data, kind=kind)

plt.show()

# 用法

data = sns.load_dataset("iris")

plot_jointplot(data, "sepal_length", "sepal_width", "hex")

列表 8.22 从两个导入语句和一个用于绘制联合图的 plot_joint() 函数开始。列表 8.22 的第二部分使用 Seaborn 内置数据集 iris 的内容初始化 Pandas 数据帧 data，然后使用变量 data 调用 plot_pair()。图 8.22 显示了通过运行列表 8.22 中的代码生成的联合图。

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p251.jpg)

图 8.22 使用 Seaborn 创建的联合图

因子视图的点图

点图可以用来突出显示点之间的差异，尤其是在按因素（如使用示例中的性别）分类时。连接点的线条可以帮助强调任何趋势。用线条强调点之间的比较。以下提示被提供给 GPT-4 以生成用于点图的 Python 代码：“请生成用于显示点图的 Python 代码。”

列表 8.23 展示了 ChatGPT 生成的用于使用 Seaborn 绘制点图的 point_plot.py 的内容。

列表 8.23：point_plot.py

import matplotlib.pyplot as plt

import seaborn as sns

def plot_pointplot(data, x_col, y_col, hue=None):

sns.pointplot(x=x_col, y=y_col, hue=hue, data=data)

plt.show()

# 用法

data = sns.load_dataset("tips")

plot_pointplot(data, "day", "total_bill", "sex")

列表 8.23 从两个导入语句和一个用于绘制点图的 plot_pointplot() 函数开始。列表 8.23 的第二部分使用 Seaborn 内置数据集 tips 的内容初始化 Pandas 数据帧 data，然后使用变量 data 调用 plot_pointplot()。图 8.23 显示了通过运行列表 8.23 中的代码生成的点图。

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p252.jpg)

图 8.23 使用 Seaborn 创建的点图

SEABORN 的 KDE 密度估计图

核密度估计（KDE）图可视化连续变量的概率密度。它们可以被视为平滑的直方图，当想要辨别数据集的潜在分布时特别有用。以下提示被提供给 GPT-4 以生成用于 KDE 图的 Python 代码：“请生成用于绘制 KDE 图的 Python 代码。”

列表 8.24 展示了 ChatGPT 生成的用于使用 Seaborn 绘制 KDE 图的 kde_plot.py 的内容。

列表 8.24：kde_plot.py

import matplotlib.pyplot as plt

import seaborn as sns

def plot_kde(data, column):

sns.kdeplot(data[column], shade=True)

plt.show()

# 用法

data = sns.load_dataset("iris")

plot_kde(data, "sepal_length")

列表 8.24 从两个导入语句和渲染 KDE 图的 plot_kde()函数开始。列表 8.23 的第二部分使用 Seaborn 内置数据集 iris 的内容初始化 Pandas 数据帧 data，然后使用变量 data 调用 plot_kde()。图 8.24 显示了通过在列表 8.24 中启动代码生成的点图。

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p253.jpg)

图 8.24 使用 Seaborn 创建的 KDE 图

SEABORN 的脊状图

脊状图本质上是一系列 KDE 图叠加在一起，允许比较不同类别之间的分布。它们显示叠加的分布图，这对于可视化类别间的分布变化非常有用。以下提示被提供给 GPT-4 以生成绘制脊状图的 Python 代码：“请生成绘制脊状图的 Python 代码。”

列表 8.25 显示了 ChatGPT 生成的用于使用 Seaborn 渲染脊状图的 ridge_plot.py 的内容。

列表 8.25：ridge_plot.py

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

plt.show()

# 使用方法

data = sns.load_dataset("diamonds")

subset_data = data[data['cut'].isin(['Ideal', 'Fair', 'Good'])]

plot_ridge(subset_data, "price", "cut")

列表 8.25 从两个导入语句和渲染脊状图的 plot_ridge()函数开始。列表 8.25 的第二部分使用 Seaborn 内置数据集 diamonds 的内容初始化 Pandas 数据帧 data，然后使用变量 data 调用 plot_ridge()。图 8.25 显示了通过在列表 8.25 中启动代码生成的脊状图。

![图片](img/human-vs-chatgpt-language-of-advertising-in-beauty-products-advertisements-p255.jpg)

图 8.25 使用 Seaborn 创建的脊状图

摘要

本章包含 ChatGPT 为各种任务生成的基于 Python 的解决方案。您学习了各种图表和图形的类型、何时使用它们以及每种图表和图形的优点和缺点。

您学习了如何使用一个流行的开源 Python 库 Matplotlib 进行数据可视化，它可以渲染多种类型的图表和图形。

您还学习了如何渲染直方图、小提琴图和时间序列可视化。通过掌握这些技术，可以从数据中构建引人入胜的故事，帮助决策和洞察力的生成。精心制作的可视化胜过千行原始数据。

索引

A

准确率，46–47

激活函数，78–81

添加变量（部分回归）图，154

额外的模型诊断，155–156

调整后的 R²，132–133

调整后的兰德指数 (ARI)，201–202

高级数据分析，108

Claude 2 对比，108–109

代码倾听者，109

机器学习和 ChatGPT，115–116

相似传播，199

聚类分析，196，198–199

聚类层次聚类算法，206–207

AI21，95

来自 OpenAI 的基于 AI 的聊天机器人，102

Ajax，123

Akaika 信息准则 (AIC)，132–133

Alexa，89

算法选择，39

AlphaGo，92

AlphaGo 100-0，92

AlphaGo Zero，92

AlphaStar，92

AlphaZero，92

ChatGPT 的替代方案，114–115

异常检测，37，196

人类学，96

Apple GPT，123

艺术和音乐创作，88

人工智能 (AI)，159–160

属性选择，41

自相关，153

自动编码器，42

B

条形图，222

使用 Seaborn，240–241

贝叶斯分类器，66，76–77

贝叶斯推理，74–76

贝叶斯定理，74–76

最大后验 (MAP) 假设，75–76

术语，75

贝叶斯信息准则 (BIC)，133

偏差-方差权衡，45，165

二元对多类分类，67

Bing Chat，123

双变量分析，141，143

以及多元分析，146–148

布尔数据框，8–9

箱线图，224，228

使用 Matplotlib 绘制胡须图，228

C

Calinski-Harabasz 指数，201

标准相关分析 (CCA)，42

ChatBotX，98

ChatGPT，94，100，102–106，110–111，129

替代方案，114–115

自定义指令，104

和数据可视化，221–256

教育者，110

生成和危险话题，110–111

Google “代码红色”，103

Google 搜索与，103–104

和 GPT-4，91–92，121–126

GPTBot, 105–106

机器学习和，115–116

在移动设备和浏览器上，104–105

游戏场，106

插件，107

和提示，105

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

二元对多类分类，67

决策树，69–73

定义，66

评估，77–78

指数线性单元 (ELU)，82

hardmax 函数，83

kNN (k-最近邻) 算法，68

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

在 kNN 中的绑定，68–69

训练分类器，77

Claude 2，96，108–109，124

与高级数据分析，108–109

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

指标，196，200–203

Code Whisperer，109

Codex，94，123

决定系数，131–132

Cohere，94

凝聚性，202

计算效率，165

条件数，155

混淆矩阵，46

等高线图，Matplotlib，235–236

对话式 AI，89

评估，90

与生成式 AI，89–90

在 Pandas 中将字符串转换为日期，18–20

卷积神经网络（CNNs），66–67，82

库克距离，155

CoPilot (OpenAI/Microsoft)，122–123

正确的模型指定，154

相关性分析，142

余弦相似度，207

反事实后悔最小化（CFR），93

反事实价值-策略网络（CVPN），93

协方差矩阵，42–43

创建与分类的比较，88

交叉验证，164

维度诅咒，197

曲线拟合与线性回归的比较，49

客户支持聊天机器人，89

D

DALL-E，90–91

DALL-E 2，96

Dask（用于分布式处理），3

数据

增强现实，89

清洗，39

生成，88

归一化与标准化，45

类型系列，2

数据帧，1–3，6–8

和数据清洗任务，3

特征，3

作为 HTML 网页，31–33

输入类型，1

带有 Numpy 示例，4–6

和随机数，9–11

数据点，36

数据集，36

线性回归的准备过程，139–141

数据表（Python 中的 R 数据表），3

数据可视化和 ChatGPT

层次聚类，248–249

联合图用于双变量数据，250–251

核密度估计（KDE）图用于密度估计，252–253

Matplotlib

带有 3D 表面图的，232–233

使用箱线图，228

等高线图，235–236

使用饼图，231

带有线条图的，225–226

使用饼图，227

带有径向（或蜘蛛）图的，23–235

带有堆叠柱状图的，230

使用时间序列可视化，229

因子视图的点图，251–252

极坐标图，239–240

向量场的箭头图，238–239

带有脊图的，254–255

Seaborn

带有柱状图的，240–241

带有分面网格的，247–248

使用热图进行相关矩阵，242–243

使用直方图，244

使用 pairplot()函数，246–247

使用回归线绘制散点图，241–242

带有提琴图的，245

向量场流线图，236–238

蜂群图，249–250

与图表和图形一起工作，222–225

戴维斯-博尔丁指数，196，201

DBSCAN（基于密度的噪声空间聚类应用），196，198，204

算法，208–209

death.csv 数据集，线性回归

带有代码，150–153

详细的数据探索分析，143–145

特征，138–139

决策树，38，66，69–73

算法，189–191

优点和缺点，191

算法，190

案例，191

概念和组件，189–190

扩展，191

带有机器学习模型，172–176

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

邓恩指数，201

重复值，40

杜宾-沃森统计量，132–133

E

肘部方法，196

对于 k 近邻（kNN）算法，165–166

嵌入策略，41

实体提取，90

错误矩阵，46

欧几里得距离，207

评估，77–78

偶数 k 与奇数 k 的对比，165

期望最大化，37–38

探索性数据分析（EDA），141–143

death.csv 数据集，线性回归，143–145

指数线性单元（ELU），80，82

F

F1 分数，48

使用 Seaborn 的面元网格，247–248

特征，36

工程，40–41

提取，40–41

投影，40–41

缩放，197

选择，39–41

联邦信息处理标准（FIPS）代码，138，140

少样本学习，97

少样本提示，97

过滤策略，41

微调模型，39

修复错误值，39

Fowlkes-Mallows 指数，202

F 统计量，132–133

G

GANs，参见生成对抗网络（GANs）

门控循环单元（GRU），82–83

高斯混合模型（GMM），196，199

Gemini，122

广义判别分析（GDA），42

生成文本检测，109–110

生成对抗网络（GANs），88，90

生成式 AI

高级数据分析，108

AI21，95

ChatGPT 的替代方案，114–115

人类中心主义，96

ChatGPT，102–106，110–111

ChatGPT 和 GPT-4，91–92

Claude 2，108–109

代码解析器，109

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

机器学习和 ChatGPT，115–116

OpenAI，93–94

提示工程，96–102

ChatGPT 的示例查询和响应，112–113

技术应用，88

第三方 ChatGPT 插件，107

VizGPT 和可视化，117–120

生成模型，88–89

地理空间分析，142

巨型语言模型测试室 (GLTR)，110

GitHub CoPilot，122–123

Gmail，124

高斯猜想，112–113

Google “代码红色警报”，103

Google Gemini，114，123

Google 搜索与 ChatGPT，103–104

GPT2 检测器，109

GPT-3，92，94，96，100

应用，123

- 基于的 LLM，123

GPT-4，92，94，100，120–121，125，129

竞争对手，121–126

微调，121

线性回归

与数据集相关，137–138

与随机数据相关，133–136

推荐，156–157

参数，121

以及考试成绩，120–121

基于转换器的 AR (自回归) 模型，121

GPT-5，126–127

基于 GPT 的模型，94

GPTBot，105–106

GPT-Index，121

GPT-x 系列的 LLM，93

基于图的核 PCA，42

增长树 CFR（GT-CFR），93

H

hardmax 函数，83

hdate1，29

hdate2，29

热图，223

用于 Seaborn 的关联矩阵，242–243

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

分段，196

综合，89

不朽，82

不完全信息，92

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

核密度估计（KDE）图用于密度估计，252–253

核密度图，154

核 PCA，37，42

k-fold 交叉验证技术，44，77

k-means，37–38，196，206

算法，65，205–206

聚类，197，203

k 近邻（kNN），38，42，66

算法，68，163–164

优缺点，163–164

案例，164

概念，163

肘部方法，165–166

带有机器学习模型，166–172

k 的值，164–165

L

L1 & L2 正则化，44

LangChain，121

语言模型，99

学习分布，88，91–92

线性分类器，66，68

线性判别分析（LDA），42，65

线性，154

假设，153

线性回归，37，48–49

额外的模型诊断，155–156

双变量和多变量分析，146–148

与曲线拟合，49

数据集，准备过程，139–141

death.csv 数据集

与代码，150–153

详细 EDA，143–145

特征，138–139

定义，130

探索性数据分析（EDA），141–143

GPT-4

与数据集，137–138

与随机数据，133–136

建议，156–157

与交互项，130

指标，131–133

模型诊断，153–155

模型选择过程，148–150

多变量分析，50

精确值解，49–50

类型，130–131

线形图，223

使用 Matplotlib 绘制的线图，225–226

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

低方差滤波器，39

低方差滤波器技术，40

M

机器学习

算法，类型，37–39

偏差-方差权衡，45

与 ChatGPT，115–116

使用 GPT-4 进行聚类，参见聚类

协方差矩阵，43

定义，35–36

维度约简，41–42

特征工程，选择和提取，40–41

使用 np.linspace()生成线性数据，60–61

线性回归，48–49

与曲线拟合比较，49

多变量分析，50

精确解，49–50

均方误差（MSE）

公式，58–59

手动，59–60

使用 np.linspace()API，61–63

模型度量指标

准确率与精确率与召回率比较，46–47

混淆矩阵，46

受试者工作特征（ROC）曲线，47

R-squared 值，46

Numpy 和 Matplotlib（1）

扰动技术，55

二次散点图，56–57

使用散点图，54–55

主成分分析（PCA），42

回归类型，50–51

正则化

数据归一化与标准化比较，45

与特征缩放，44

统计术语

F1 分数，48

p 值，48

任务，39–40

类型，36–37

处理数据集

交叉验证，44

训练数据与测试数据对比，43

在平面中处理线（可选），51–54

使用 GPT-4 的机器学习分类器

应用，160–161

挑战，161

概念，160

决策树算法，189–191

与机器学习模型结合，172–176

k 近邻（kNN）算法，163–164

肘部法则，165–166

与机器学习模型结合，166–172

k 的值，164–165

逻辑回归算法，185–186

朴素贝叶斯算法，186–188

随机森林算法，177–182，191–193

Scikit-learn，161–162

与 SVM 算法结合，182–184，188–189

类型，160

机器学习模型

聚类

与 DBSCAN 算法结合，215–218

与层次聚类算法结合，213–215

与 k-means 算法结合，209–212

与决策树算法结合，172–176

与随机森林算法结合，177–182

与 SVM 算法结合，182–184

曼哈顿距离，207

市场细分，196

在 Pandas 中匹配和拆分字符串，16–18

Matplotlib，133

使用 3D 表面图，232–233

使用箱线图，228

等高线图，235–236

使用环形图，231

使用线图，225–226

使用饼图，227

使用径向（或蜘蛛）图，23–235

使用堆叠条形图，230

使用它进行时间序列可视化，229

矩阵合并，78

均方绝对误差 (MAE)，58，131–132

均值漂移，38

聚类，198

均方误差 (MSE)，131–132

定义，35

公式，58–59

手动，59–60

使用 np.linspace()API，61–63

均方误差 (MSE)，130

Med-PaLM 2，124

在 Pandas 中合并和拆分列，28–30

度量，196，200–203

对于线性回归，131–133

微软，93，120，122–123

微软 365 CoPilot，122–123

微软 Bing AI，123

MiniBatch k-means，203

Pandas 中的缺失日期

检测，21–22

插值，22–24

“缺失”模式，142

缺失值比率技术，39–40

缺失值分析，143

专家混合 (MoE) 架构，120，127

MNIST 数据集，36，38，66

模型诊断，线性回归，153–155

模型选择过程，线性回归，148–150

Modin（性能更快），3

MT-NLG，92

多重共线性，154–155

多标签分类，67–68

多项式分类器，67

多个独立的树，38

多元线性回归，130

多变量分析，37，50，141

N

天真贝叶斯，38

算法，186–188

分类器，67，76–77

自然语言处理 (NLP) 技术，90，92

神经网络，162

非线性最小二乘法，58–59

非负矩阵分解（NMF），42

残差的正态性，153

标准化互信息（NMI），202

Numpy 和 Matplotlib（1）

扰动技术，55

二次散点图，56–57

使用散点图，54–55

NumPy API，129

NumPy 数组，4–5

O

单次学习，97

单次提示，97

一对全（OvA）技术，67

一对一（OvO）技术，67

一对多（OvO）技术，67

OpenAI，92–94

ChatGPT，123

Codex，123

开放式对话，117

在 Pandas 中处理日期，24–28

OPTICS（按顺序排列点以识别聚类结构），200

异常值检测，143

异常值和杠杆点，154

P

使用 Seaborn 的 pairplot()函数，246–247

PaLM 2，122

PaLM-2，124

Pandas

替代方案，3–4

布尔数据框，8–9

将分类数据转换为数值数据，13–16

将字符串转换为日期，18–20

数据框，2–3，6–8

和数据清洗任务，3

作为 HTML 网页，31–33

使用 Numpy 示例，4–6

和随机数，9–11

定义，1–2

HTML 网页中的，30

中的 loc()和 iloc()方法，12–13

匹配和拆分字符串，16–18

在中合并和拆分列，28–30

缺失日期，24–28

检测，21–22

插值，22–24

在日期中进行操作，24–28

选项和设置，2

读取 CSV 文件，11–12

在日期范围内工作，20–21

帕累托图，224

Pathways 语言模型，124

完美信息，92

Pi，115

饼图，222–223

使用 Matplotlib，227

游戏玩家（PoG），93

来自 LinkedIn 的 POE，115

因子视图的点图，251–252

极坐标图，239–240

多项式回归，130

精度，46–47

精度-召回（PR）曲线，78

预测误差，41

主成分分析（PCA），37，42，161，197

提示工程，96–102

和完成，97

DALL-E 2，96

定义，96

对于不同的 LLM，100–101

GPT-3，96

指令提示，98

提示和完成，97

提示模板，99–100

反向提示，98

系统提示与代理提示，98–99

模板，99–100

文本到图像生成，96

类型，97

词汇提示，101–102

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

向量场箭头图，238–239

R

雷达图，224–225

使用 Matplotlib 的径向（或蜘蛛）图，233–235

随机森林，38，66，73

算法，177–182，191–193

分类器，67

在 Pandas 中读取 CSV 文件，11–12

召回，46–47

接收者操作特征 (ROC) 曲线，47，77–78

循环神经网络 (RNNs)，65，88

回归，37

系数，45–46，131

任务，36

类型，50–51

回归规格误差测试 (RESET)，154

正则化，44

和特征缩放，44

从人类反馈中进行强化学习 (RLHF)，115，117

相对误差，58–59

ReLU，81–82

剩余标准误差 (RSE)，132

解决重复值，39

解决缺失值，39

反向提示，98

鞍形图，254–255

RMSPROP，58

RNNs，参见循环神经网络 (RNNs)

鲁棒回归方法，156

根均方误差 (RMSE)，58，131–132

根均方层归一化 (RMSNorm)，126

R²，45–46

S

可扩展性，162

按比例扩展指数线性单元 (SELU)，80

使用 Seaborn 绘制带有回归线的散点图，241–242

Scikit-learn，161–162

实现，38

Seaborn，数据可视化和 ChatGPT

使用条形图，240–241

使用 facet grids，247–248

使用相关矩阵的热图，242–243

使用散点图，244

使用 pairplot() 函数，246–247

使用带有回归线的散点图，241–242

使用小提琴图，245

搜索结果分组，196

二次多项式，131

半监督学习，36–37

分隔，202–203

sep 参数，12

Shapiro-Wilk 检验，154

sigmoid 函数，83

Silhouette 分数，196，200–201

简单线性回归，130

Siri，89

社交网络分析，196

softmax 激活函数，82

softmax 函数，83

softplus 激活函数，82

精确值解，线性回归，49–50

SOTA（当前最佳水平）

AI21，95

性能，92

谱聚类，199

平方根规则，165

使用 Matplotlib 绘制堆叠条形图，230

标准化残差与杠杆作用图，154

StarCraft II，93

向量场流线图，236–238

风格迁移，89

摘要报告，142

监督学习技术，36–38

支持向量机（SVM）算法，38，66，73–74

优缺点，189

案例，189

组件，188

概念，188

和机器学习模型，182–184

类型，188

蜂群图，249–250

SwiGLU，126

合成，88

系统提示与代理提示，98–99

T

tanh 激活函数，83

T 属性，9

t-distributed Stochastic Neighbor Embedding (t-SNE)，37，42

TensorFlow，130，162

API，65

测试模型，39

文本

生成，89，91

-相关任务，91

-到图像生成，96

第三方 ChatGPT 插件，107

使用 Matplotlib 绘制 3D 表面图，232–233

阈值值，84

在 kNN 中绑定，68–69

使用 Matplotlib 进行时间序列可视化，229

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

使用 Seaborn 的提琴图，245

Visual Studio Code 扩展，122–123

VizGPT 和数据可视化，117–120

“汽车数据集”行，118

“汽车数据集”可视化，119

语音操作虚拟助手，89

W

水平图，225

簇内平方和（WCSS），166，196，205

文字提示，101–102

工作

带图表和图形，222–225

带数据集

交叉验证，44

训练数据与测试数据，43

在 Pandas 中的日期范围，20–21

在平面中的线条（可选），51–54

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
