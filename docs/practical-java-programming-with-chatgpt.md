# ChatGPT Java 编程实用指南

> 原文：[Practical Java Programming with ChatGPT:](https://annas-archive.org/md5/d2af62694cb06957b1167a35690c370a)
> 
> 译者：[飞龙](https://github.com/wizardforcel)
> 
> 协议：[CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)


![cover](img/practical-java-programming-with-chatgpt-cover.jpg)

![image](img/practical-java-programming-with-chatgpt-cover.jpg)

# 献给

*我深爱的妻子，Jenny*

*我的孩子们，Julie和Rosalie

和他们的家人* 

# 关于作者

Alan S. Bluck是 ASB 软件开发有限公司的总监，同时也是系统架构师顾问，提供从高级技术设计到代码开发指导、FileNet 核心产品的安装和配置等一系列服务。

2022 年被提名为 IBM 冠军，并在 2023 年再次当选，作者已经出版了 5 本技术书籍和超过 30 篇 ResearchGate 论文，这些论文均可免费下载。

他负责现有和新 FileNet 系统的高级分析和配置。他还负责指导和解决高级系统和问题。

他在商业和科学系统中拥有超过 45 年的软件开发经验；作为项目经理/分析师开发人员有 5 年经验，作为 12 名软件工程师团队的软件开发经理有 11 年经验，作为技术顾问有 11 年经验，作为解决方案架构师有 20 年经验。

# 关于审稿人

吉尔·梅特卡夫拥有漫长而多样化的职业生涯，最初作为一名工业微生物学家在一家石油公司工作，参与有关重金属微生物采矿和废弃油井提高采收率的项目。此后，他在一家大型制药公司工作了多年，担任过多个角色，包括项目经理、开发团队领导和网络管理员。在这段时间里，他为临床试验管理开发了软件，以及医院用于管理癌症患者的关键工具。在他作为解决方案架构师在软件行业工作的许多年里，他在许多领域和行业中积累了丰富的经验，尤其是在金融技术领域，但也包括制造业、物流和能源市场。他对许多软件领域有深入的了解，包括与现代商业实践相关的领域。这些包括文档和内容管理、案例管理、业务流程管理和流程自动化、文档生命周期管理、身份管理和在线银行技术。他被认为是行业内的专家。与许多知名银行和机构合作，他带来了广泛的知识和对细节的敏锐洞察力，同时能够看到并理解更广泛的图景。这使得他能够成功地解决大型金融机构面临的难题。他的洞察力和创新方法已在许多案例和应用中得到应用，为整个行业带来了成功。

他现在是一名拥有超过 25 年软件行业经验的软件架构师。他在为许多知名企业设计和实施解决方案方面发挥了关键作用，并在过去十年里主要与金融科技解决方案合作。他在文档捕获、文档管理、业务自动化和身份管理领域拥有众多资质。他最近一直在研究移动银行应用程序的配置文件管理和无密码认证方法。吉尔认为，成功的软件架构的关键在于一系列基本技能；对软件的理解只是其中之一。同样重要的是一些更软性的能力，例如能够向非技术性受众（如用户和主管）解释复杂的软件概念，能够看到解决方案的全面图景（包括风险和陷阱），以及能够从往往是模糊的愿望清单中提炼出需求。他说，为解决方案设计做准备通常是“同时进行外推和内插的练习！”。他是多个专业协会的成员，包括英国特许信息系统协会、身份管理协会和国际软件架构师协会。

# 致谢

在我撰写这本书的过程中，有几个人我想要感谢他们持续和持续的支持。首先，我想要感谢我的妻子 Jenny，她不断地鼓励我写这本书——没有她的支持，我无法完成这本书。

我对 ResearchGate 网站的支持表示感谢，自 2019 年以来，该网站已保存了我超过 30 篇免费出版物，其中大部分我在本书中进行了引用。

我还要感谢 AVA Orange 团队的支持和奉献，这使我能够在如此短的时间内出版这本书，并在生产过程中更新材料，因为人工智能软件是一个快速发展的领域，涵盖了广泛的应用。

我还要感谢 Giles Metcalf，本书的技术审稿人，感谢他的勤奋和有益的建议。

# 前言

本书中的问题与 Java 程序软件开发相关，这些问题是针对 ChatGPT 安卓手机应用提出的。这些问题基于以前的发展（许多算法最初需要花费数天时间编写）。这些回应令人惊讶，并在几秒钟内出现！在这本书中，我们以 ChatGPT 提供的示例 Java 代码为例，使用最新的 Eclipse IDE 进行实现。我们还确定，ChatGPT 生成的所有基础代码均可免费使用！

ChatGPT 为 Java 程序员提供了加速代码编写的能力。软件开发人员、程序员和软件工程师可能需要花费数天时间编写应用程序的代码。在这本书中，我们通过示例描述了可用于 ChatGPT 来自动化 ChatGPT Java 代码生成过程的提示。

本书包含与软件开发相关的问题，这些问题（以粗体显示）是针对 ChatGPT 安卓手机应用提出的。然后我们描述了实现工作 Java 代码的详细步骤并验证结果。

本书分为13 章，旨在为 Java 程序员、IT 顾问、系统和解决方案架构师提供示例，他们拥有基本的通用 IT 知识。本书提供了使用 OpenAI ChatGPT 服务器系统和前端 AI 系统开发 Java 编程解决方案的工作模板，这些示例用于支持开发者开发用于数据处理、数学分析和文档管理程序，以及用于制造业、银行和保险公司的实施。

第一章涵盖了与软件开发相关的问题，这些问题（以粗体显示）是针对 ChatGPT 3.5 AskAI“手机应用”提出的。我们还涵盖了 ChatGPT 作为网络应用和安卓移动“手机应用”的安装。描述了响应的版权问题和 ChatGPT 的基本使用。

第二章 讲述了用于测试 ChatGPT 对良好编程实践知识了解的 ChatGPT 提示。我们要求它定义它对“SOLID”原则的了解，它几乎立即就做到了。以下输出只是介绍：

“SOLID 是一组由罗伯特·C·马丁（也称为 Uncle Bob）提出的面向对象编程原则。这些原则旨在使软件设计更加健壮、灵活和易于维护。以下是 SOLID 原则的简要概述以及它们如何应用于 Java：”

第三章 讲述了使用 OpenAI Java API 与 ChatGPT AI 系统接口所需的 Java 代码。ChatGPT 提供了一个使用 OkHttp 库向 API 发送请求的示例。为了使用 API，我们描述了获取 OpenAI API 密钥所需的方法。

第四章 讲述了提出的问题，以提供一个用于使用二分查找的 Java 程序代码。二分查找方法接受一个整数排序数组和要搜索的目标整数。如果找到目标整数，则返回它在数组中的索引，如果没有找到，则返回-1。

第五章 我们介绍了最新开源 Eclipse Java IDE（Eclipse IDE 2023-06 R – Eclipse IDE for Java Developers）的下载和安装，以及如何在 MS Windows 10 和 RedHat Enterprise Linux（RHEL 8.x）上逐步安装。然后，我们通过创建 Java BinarySearch 项目并检查 Java 程序输出，详细描述了二分查找程序的实现和验证。

第六章 讲述了对 MP4 音乐文件的傅里叶分析，以分离乐器和人声。这是一个复杂任务，涉及多个步骤，如解码 MP4 文件、执行信号处理以及应用源分离技术。ChatGPT 提供了所需步骤的概述指南，并为每个步骤建议了一些库。ChatGPT 还提供了一个更简单的任务，即使用 Java 代码对正弦波的傅里叶分析，并为该任务提供了完整的可工作代码。

第七章 介绍了 ChatGPT 生成的用于快速傅里叶变换（FFT）的 Java 代码。ChatGPT 被要求提供示例 Java 代码来演示快速傅里叶变换。显示了一个示例 Java 代码，它使用 Apache Commons Math 库演示了快速傅里叶变换（FFT）。

第八章 讲述了 ChatGPT 生成的用于索引文档并输出关键词及其相关文档页码的 Java 代码示例。ChatGPT 提供的代码创建了一个文档及其相关关键词的索引，使用 Lucene 库。它还允许根据关键词搜索文档，并返回文档路径。

第九章 描述了 ChatGPT 如何被提示提供一个 Java 代码，用于从测量不透明材料截面尺寸分布来计算粒子尺寸分布的 Saltikov 方法。ChatGPT 生成的代码提示用户输入测量的截面数量、每个截面的尺寸和曲线下的面积。然后它使用 Saltikov 方法计算粒子尺寸分布并打印结果。

第十章 解释了 ChatGPT 如何生成 Java 代码来逆一个三角矩阵以获得多项式的系数。ChatGPT 被提示编写一个示例 Java 程序，其中包含逆三角矩阵以获得多项式系数的代码，作为一组多项式方程的结果。创建的 Java 代码提示用户输入多项式的次数和一组多项式方程的系数。然后它使用高斯消元法逆矩阵并获取多项式的系数。最后，它打印出多项式的系数。

第十一章 讲述了如何使用 ChatGPT 生成示例 Java 代码，将文档存储在最新的 IBM FileNet 文档管理系统，使用 FileNet Java API。ChatGPT 生成的代码，在下载一些额外的库之后，建立了与 FileNet 服务器的连接，创建了一个新文档，设置了文档属性，添加了内容，保存了文档，并将其存入指定的对象存储文件夹。

第十二章 讨论了 ChatGPT 在程序开发方面的结论和未来。我们描述了 ChatGPT 3.5 在 2021 年 9 月的知识截止点，以及 OpenAI 基金会随后为增强这个知识库和快速开发目前发布的 beta ChatGPT 4.0 所进行的持续发展。我们还为 ChatGPT 5.0 未来版本的路线图提供了一些指示。

第十三章 提供了附录，包括参考文献和额外的 ChatGPT 问题，包括关于其他支持 AI 开发的 IBM 系统以及量子计算发展对 AI 处理的影响的信息。

# 下载代码

打包和彩色图像

请点击链接下载

书籍的代码打包：

# [`github.com/OrangeAVA/Practical-Java-Programming-with-ChatGPT`](https://github.com/OrangeAVA/Practical-Java-Programming-with-ChatGPT)

书籍的代码打包和图像也托管在

[*https://rebrand.ly/6821ed*](https://rebrand.ly/6821ed)

如果代码有更新，它将在现有的 GitHub 仓库中更新。

# 错误清单

我们在 Orange Education Pvt Ltd 的工作中感到无比自豪，并遵循最佳实践以确保我们内容的准确性，为我们的订阅者提供令人愉悦的阅读体验。我们的读者是我们的镜子，我们利用他们的反馈来反思和改进在出版过程中可能发生的任何人为错误。为了让我们保持质量并帮助我们接触到可能因任何意外错误而遇到困难的读者，请通过以下方式与我们联系：

errata@orangeava.com

您的支持、建议和反馈非常受赞赏。

# 你知道吗？

你知道吗，Orange Education Pvt Ltd 提供每本书的电子书版本，包括 PDF 和 ePub 文件？您可以在[www.orangeava.com](http://www.orangeava.com)升级到电子书版本，并且作为印刷书客户，您有权获得电子书副本的折扣。想了解更多详情，请联系我们：info@orangeava.com。

在[www.orangeava.com](http://www.orangeava.com)，您还可以阅读一系列免费的技术文章，订阅各种免费通讯，并享受 AVA™书籍和电子书的独家折扣和优惠。

# 侵权

如果您在互联网上以任何形式发现我们作品的非法副本，如果您能提供位置地址或网站名称，我们将不胜感激。请通过info@orangeava.com与我们联系，并提供材料的链接。

# 您有兴趣与我们合作撰写书籍吗？

如果您在某个领域有专业知识，并且您有兴趣撰写或为书籍做出贡献，请通过business@orangeava.com与我们联系。我们正在努力帮助开发者和技术专业人士了解全球正在发生的科技发展和创新，并建立一个相信知识通过分享和学习他人而获得最佳效果的社区。请与我们联系，了解我们的受众需求以及您如何成为这一教育改革的一部分。我们也欢迎技术专家的想法，并帮助他们为其领域构建学习和发展的内容。

# 评论

请留下评论。一旦您阅读并使用了这本书，为什么不在您购买它的网站上留下评论呢？潜在的读者可以查看并使用您的客观意见来做出购买决定。Orange Education 的我们非常希望了解您对我们产品的看法，我们的作者也可以从您的反馈中学习。谢谢！

想了解更多关于 Orange Education 的信息，请访问[www.orangeava.com](http://www.orangeava.com)。

# 目录

1. ChatGPT 入门

简介

结构

AI 建议的书籍标题

AI 生成 Java 代码的版权法律

为免费 ChatGPT V. 3.5 创建账户

安装和使用 Android 手机应用，Ask AI

为订阅 ChatGPT-4 创建账户

结论

需要记住的要点

多项选择题

答案

问题

关键术语

2. Java 编程 - ChatGPT 所述的最佳实践

简介

结构

SOLID 原则

Java 代码缩进的最佳实践

SOLID 代码示例

单一职责原则 (SRP)

开放/封闭原则 (OCP)

Liskov 替换原则 (LSP)

接口隔离原则 (ISP)

依赖倒置原则 (DIP)

结论

需要记住的要点

多项选择题

答案

问题

关键术语

3. 开发用于利用 ChatGPT API 的 Java 代码

简介

结构

ChatGPT API 概述

验证建议的 API 代码

访问 ChatGPT 引用的 OkHttp Java 库 Jar 文件

访问 ChatGPT 秘密 API 密钥

使用 ChatGPT 模型 ID

结论

需要记住的要点

多项选择题

答案

问题

关键术语

4. 使用二分查找的 Java 程序

简介

结构

AI 提示和响应

使用 Eclipse Java 代码进行 Java 代码验证

结论

需要记住的要点

多项选择题

答案

问题

关键术语

5. 最新开源 Eclipse Java IDE 的安装

简介

结构

下载 Eclipse Java IDE

使用 Eclipse IDE 验证二分查找代码

困惑度

创建 Java BinarySearch 类

运行 Eclipse Java 程序

二分查找验证 Java 程序输出

结论

需要记住的要点

多项选择题

答案

问题

关键术语

6. ChatGPT 生成的傅里叶分析 Java 代码

简介

结构

MP4 傅里叶分析 Java 代码

根据 OpenAI ChatGPT 的 MP4 傅里叶分析 Java 代码

使用 Eclipse Java 程序项目验证 MP4 傅里叶分析的 Java 代码

ChatGPT 生成的用于正弦波傅里叶分析的 Java 代码

使用 Eclipse Java 验证正弦波傅里叶分析的 Java 代码

结论

需要记住的要点

多项选择题

答案

问题

关键词

7. ChatGPT 生成的用于快速傅里叶变换的 Java 代码

引言

结构

AI 快速傅里叶变换 Java 代码 ChatGPT 提示的 Java 程序

使用 Eclipse Java 程序项目验证快速傅里叶变换 Java 代码

结论

需要记住的要点

多项选择题

答案

问题

关键词

8. ChatGPT 生成的用于索引文档的 Java 代码

引言

结构

ChatGPT 生成的用于索引文档的关键词和页码的 Java 代码

使用 Eclipse Java 程序项目验证文档索引 Java 代码

结论

需要记住的要点

多项选择题

答案

问题

关键词

9. ChatGPT 生成的用于 Saltikov 粒子分布的 Java 代码

引言

结构

ChatGPT 生成的用于 Saltikov 确定粒子尺寸分布的 Java 代码

Saltikov 确定粒子的尺寸分布 - 使用新的 Eclipse IDE 项目验证 Java 代码

结论

需要记住的要点

多项选择题

答案

问题

关键词

10. ChatGPT 生成的用于求逆三角矩阵的 Java 代码

引言

结构

ChatGPT 生成的用于求逆三角矩阵以获得多项式系数的 Java 代码

通过逆三角矩阵求多项式系数 - 使用 Eclipse Java 程序项目验证 Java 代码

验证测试 1

验证测试 2

魔方阵示例

结论

需要记住的要点

多项选择题

答案

问题

关键词

11. ChatGPT 生成的用于在 IBM FileNet 系统中存储文档的 Java 代码

引言

结构

ChatGPT 生成的 Java 代码用于存储最新的 IBM FileNet 文档管理系统中的文档

在最新的 IBM FileNet 文档管理系统中存储文档 - 使用 Eclipse Java 程序项目进行 Java 代码验证

结论

要点

多项选择题

答案

问题

关键术语

12. 结论和 ChatGPT 在程序开发中的未来

引言

结构

结论和 ChatGPT 在程序开发中的未来

AI 和 ChatGPT 的未来

AI 偏见对响应的影响

ChatGPT 取代人们的职业

使用您自己的附加数据构建自定义 ChatGPT

使用 AI 迁移学习

IBM 和 Watsonx 生成式 AI

安全威胁和隐私问题

替代代码助手 AI 软件 - 自动编码程序的 ChatGPT 替代方案

Llama 2 代码 AI 免费使用

设置 Jupyter Notebook 环境

GPT4All 及其工作原理

GitHub Copilot

Google Duet AI

Codeium

CodeWhisperer

Falcon-180B

结论

要点

多项选择题

答案

问题

关键术语

13. 附录 - 额外问题的附录

引言

结构

附录 A – ChatGPT 的更多 AI 问题

附录 B - ChatGPT 常见问题及答案

常见问题解答（来自网站）

附录 C – ASB 软件开发有限公司出版物

分子生物学安装 - ASB 软件开发有限公司出版物

IBM 安装 - ASB 软件开发有限公司出版物

联系方式

结论

要点

多项选择题

相关

答案

问题

关键术语

参考文献

索引

# 第一章

# 开始使用 ChatGPT

# 引言

本书包含与 Java 软件开发相关的问题，这些问题（粗体）是向 OpenAI 组织、AI 软件、ChatGPT 3.5、使用安卓手机应用 Ask AI 提出的。

这些问题基于我之前的发展（许多算法最初需要花费数天时间编写，而且大多数是用 Fortran IV 语言编写的）。

响应令人惊讶，并且几乎在瞬间出现！

在本章中，我们将介绍如何将 ChatGPT 作为网络应用程序安装，并使用安装在 Android 手机上的Ask AI ChatGPT前端界面应用程序。

我们还涵盖了当前响应的版权所有法律和 ChatGPT 的基本使用方法。

# 结构

在本章中，我们将讨论以下主题：

+   AI 建议的书籍标题

+   AI 生成 Java 代码的当前版权法律

+   为免费 ChatGPT 3.5 版本创建账户

+   为订阅版 ChatGPT-4 版本创建账户

# AI 建议的书籍标题

为了说明使用ChatGPT 3.5（截止到 2021 年 9 月有一个互联网知识库）的Ask AI移动应用程序的提示和响应，以下问题被提出。（所有问题都用粗体表示，ChatGPT AI的响应用斜体表示）

我想写一本关于使用 ChatGPT 帮助 Java 程序员的书籍。你能为我建议一个对他们有吸引力的书名吗？

*当然可以！以下是一些关于使用 ChatGPT 帮助 Java 程序员的书籍标题建议：*

1.  *"用 ChatGPT 掌握 Java：释放 AI 增强编程技能"*

1.  *"Java 程序员用 ChatGPT：革新您的编码体验"*

1.  *"AI 驱动 Java 开发者：释放 ChatGPT 的力量"*

1.  *"Java 编程变得更聪明：利用 ChatGPT 提高效率和生产力"*

1.  *"ChatGPT 伴侣：用 AI 辅助工具赋能 Java 程序员"*

1.  *"对话式编码：借助 ChatGPT 的智能指导掌握 Java"*

1.  "利用 ChatGPT 增强 Java 开发：您的 AI 编程助手"

1.  *"智能 Java 开发者：利用 ChatGPT 提高效率"*

1.  *"AI 辅助 Java 编程：与 ChatGPT 一起开拓新领域"*

1.  *"在 AI 时代进行 Java 编程：利用 ChatGPT 取得成功"*

*请随意定制这些建议，或者告诉我你是否需要更多选项！*

粗体标题（由Ask AI应用提出的第七个标题）被选中。这个标题被选中是因为它强调了程序员的作用。应仔细验证由 AI 软件生成的代码。（已知其产生过有误的结果！）

# AI 生成 Java 代码的版权法律

媒体上对 ChatGPT 提供的响应的法律地位存在一些争议。目前有几个具体领域正在挑战 AI 响应的合法性，例如，一些作者认为他们的版权可能因 2021 年用于训练 ChatGPT 的网页“抓取”过程中获取的响应数据的复制而被侵犯。

当前英国版权法中 AI 软件输出的法律地位使得这一职位变得复杂：

“*根据英国法律，目前禁止人工智能拥有版权（甚至承认是人工智能创建的），因为它不是人类，因此不能根据版权、设计和专利法案被视为作者或所有者。鉴于英国政府对人工智能咨询的回应，这种立场在不久的将来不太可能改变。*”

参见：[`www.port.ac.uk/news-events-and-blogs/blogs/security-and-risk/chatgpt-what-the-law-says-about-who-owns-the-copyright-of-ai-generated-content`](https://www.port.ac.uk/news-events-and-blogs/blogs/security-and-risk/chatgpt-what-the-law-says-about-who-owns-the-copyright-of-ai-generated-content)

注意

*在许多其他网站上发现了讨论与版权相关的法律要求的文章，如下：*

世界知识产权组织（WIPO），目前（在许多其他声明和更多相关问题的背景下！）表示：

“*人工智能应用越来越能够生成文学和艺术作品。这种能力为版权制度提出了重大的政策问题，版权制度始终与人类的创造性精神以及尊重和奖励人类创造性的表达密切相关。关于将版权归因于人工智能生成作品的立场将触及版权制度存在的社会目的的核心。如果人工智能生成作品被排除在版权保护资格之外，版权制度将被视为鼓励和优先考虑人类创造力尊严而非机器创造力的工具。如果赋予人工智能生成作品版权保护，版权制度将倾向于被视为优先考虑消费者能够获得最大数量的创意作品，并将人类和机器创造力视为具有同等价值。*”

完整论文可以从世界知识产权组织（WIPO）免费下载，涵盖了人工智能知识产权的许多方面，并提出了更多附加的、非常有趣的问题。该文件可以作为 PDF 文件（wipo_ip_ai_2_ge_20_1_rev.pdf）下载，下载地址如下：

[`www.wipo.int/edocs/mdocs/mdocs/en/wipo_ip_ai_2_ge_20/wipo_ip_ai_2_ge_20_1_rev.pdf`](https://www.wipo.int/edocs/mdocs/mdocs/en/wipo_ip_ai_2_ge_20/wipo_ip_ai_2_ge_20_1_rev.pdf)

以下参考资料 [`sprintlaw.com.au/articles/chatgpt-copyright-issues/`](https://sprintlaw.com.au/articles/chatgpt-copyright-issues/) 中有关于澳大利亚版权法在人工智能生成内容方面的以下声明：

*"澳大利亚案例法已裁定，人工智能系统不能拥有知识产权（因为它不是自然人）。这一点在 Thaler 诉专利专员[2021]案中得到了广泛讨论——我们在这里对此案有更多介绍。*”

*因此，当涉及到版权时，一般规则是 AI 生成的内容不受版权法保护。*

智力财产权法律实践杂志在以下链接中有一篇文章：

见：(第 17 卷，第 3 期，2022 年 3 月，第 321-326 页，https://doi.org/10.1093/jiplp/jpac013)

同样，请参阅以下链接：https://academic.oup.com/jiplp/article/17/3/321/6550465

以下段落：

例如，欧洲专利局（EPO）最近在上诉中确认了 DABUS 申请 EP 18 275 163 和 EP 18 275 174 的拒绝。虽然该决定尚未公开，但欧洲专利局明确表示“只有人类发明者才能成为发明者”以及“机器不能将任何权利转让给申请人。”²³除非通过国际法寻求——并希望实现——协调，否则在国家层面的干预只会带来不一致的风险。相反，根据上诉法院在*Thaler v Comptroller General of Patents*²⁴案件中的判决，当前的英国立场是一种相对的法律确定性——我们知道 AI *不能* 被列为发明者，并且从经验上看，没有任何迹象表明有迫切需要改变这一点。”

要了解 AI 对版权问题的看法，向使用ChatGPT 3.5的Ask AI提出了关于将AI生成内容用于商业目的的意见。

我可以使用 ChatGPT 的输出进行商业用途吗？

使用ChatGPT 3.5的Ask AI移动应用程序给出了以下回应：

*“将 OpenAI 的 GPT 模型（如 ChatGPT）的输出用于商业目的可能受到某些限制，并需要从 OpenAI 获得适当的许可或许可。*

*OpenAI 的 GPT 模型受多个许可的约束，包括 Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)许可。*

*本许可允许在适当归属的情况下，非商业用途和分发由模型生成的输出，只要结果作品是在相同或类似许可下分发。*

*如果您打算将 ChatGPT 的输出用于商业目的，您应咨询 OpenAI 或法律专业人士，以确保您拥有适当的许可和权限。此外，您应了解与 AI 生成内容在商业应用中使用相关的任何潜在伦理或法律问题。*

CC BY-NC-SA 4.0 Creative Commons，Attribution-ShareAlike 4.0许可允许他人修改和基于许可材料进行构建，甚至用于商业目的，只要作者得到认可，并且材料在相同条款下发布。这个许可实际上是“无版权”的，并且是一个开源软件许可。

# 为 Free ChatGPT V. 3.5 创建账户

既然 ChatGPT 输出的 Java 代码在英国法律和OpenAI组织看来是免费使用的，我们需要注册免费账户以访问ChatGPT V3.5，因此采取了以下步骤：

1.  使用网络浏览器访问ChatGPT网站[`chat.openai.com/auth/login`](https://chat.openai.com/auth/login)，以显示如图*图 1.1*所示的欢迎登录提示：![](img/practical-java-programming-with-chatgpt-Figure-1.01.jpg)

    图 1.1：ChatGPT 登录网页

1.  首先，我们需要点击如图*图 1.1*所示的突出显示的注册按钮。

1.  接下来，我们必须提供一个电子邮件地址，选择一个强密码，并接受服务条款，如图*图 1.2*和*1.3*所示。![](img/practical-java-programming-with-chatgpt-Figure-1.02.jpg)

    图 1.2：ChatGPT 账户创建网页

    需要一个有效的电子邮件地址，您能够访问，因为 OpenAI 使用双因素认证机制，这要求您点击发送到您邮箱的验证链接。必须输入如图*图 1.3*所示要求的强密码。

    ![](img/practical-java-programming-with-chatgpt-Figure-1.03.jpg)

    图 1.3：输入 ChatGPT 账户密码

    如前所述，您将被提示验证发送给您的电子邮件以完成账户创建，如图*图 1.4*所示：

    ![](img/practical-java-programming-with-chatgpt-Figure-1.04.jpg)

    图 1.4：ChatGPT 账户必须进行验证

1.  接下来，您需要检查您的电子邮件收件箱以获取验证消息，并点击链接来验证您的电子邮件地址，如图*图 1.5*所示。![](img/practical-java-programming-with-chatgpt-Figure-1.05.jpg)

    图 1.5：使用“验证电子邮件地址”按钮验证 ChatGPT 账户

    点击验证电子邮件地址按钮后，您将收到如图*图 1.6*所示的如下消息：

    ![](img/practical-java-programming-with-chatgpt-Figure-1.06.jpg)

    图 1.6：ChatGPT 账户验证已确认

    显示的网页如图*图 1.7*所示：

    ![](img/practical-java-programming-with-chatgpt-Figure-1.07.jpg)

    图 1.7：验证页面现在显示

1.  在注册页面上填写您的名字和姓氏，然后点击如图所示的`继续`按钮，*图 1.8*所示。![](img/practical-java-programming-with-chatgpt-Figure-1.08.jpg)

    图 1.8：现在显示登录页面以登录新账户

    新账户需要提供额外的GDPR保护（通用数据保护条例）的个人信息，如图*图 1.9*所示。

    ![](img/practical-java-programming-with-chatgpt-Figure-1.09.jpg)

    图 1.9：ChatGPT 账户提示输入更具体的信息

1.  为了验证您的电话号码，您必须输入一个 6 位数的 OTP（一次性密码）代码，该代码将被发送到您的手机。

    开发用于利用 ChatGPT API 的 Java 代码

    ![](img/practical-java-programming-with-chatgpt-Figure-1.10.jpg)

    图 1.10：ChatGPT 账户提示输入用户的手机号码

    您的移动电话应开启并连接到您的服务提供商，因为会向您输入的电话号码发送短信。请记住从下拉列表中选择您居住的国家。您收到的短信将包含您被提示输入的代码，如图*图 1.11*所示。

    ![图片](img/practical-java-programming-with-chatgpt-Figure-1.11.jpg)

    图 1.11：从短信文本输入ChatGPT账户，两步验证码。

1.  完成这些步骤后，您将成功注册ChatGPT，并可以开始使用它，如图*图 1.12*所示。![图片](img/practical-java-programming-with-chatgpt-Figure-1.12.jpg)

    图 1.12：成功登录后显示的ChatGPT仪表板。

建议首先运行快速入门教程：

[`platform.openai.com/docs/quickstart`](https://platform.openai.com/docs/quickstart)

按照说明操作，您将能够成功创建账户并开始使用ChatGPT。

使用游乐场：

[`platform.openai.com/playground/p/default-qa?model=gpt-3.5-turbo-0301`](https://platform.openai.com/playground/p/default-qa?model=gpt-3.5-turbo-0301)

注意

*我发现随着时间的推移，可用的模型（目前选择为gpt-3.5-turbo-0301）可能会改变，因此您可能需要从可用的下拉列表中选择另一个。*

![图片](img/practical-java-programming-with-chatgpt-Figure-1.13.jpg)

图 1.13：ChatGPT OpenAI 游乐场的问题。

因此，以下问题是用以下文本提出的：

“你有一个二分查找程序的 Java 代码方法吗？”

![图片](img/practical-java-programming-with-chatgpt-Figure-1.14.jpg)

图 1.14：二分查找 Java 代码的 ChatGPT 响应示例

或者，选择以下链接，带您进入ChatGPT：

[`chat.openai.com/`](https://chat.openai.com/)

![图片](img/practical-java-programming-with-chatgpt-Figure-1.15.jpg)

图 1.15：显示输入消息窗口（默认包含发送消息）

`发送消息`灰色字体文本表示您需要输入问题的位置，如图*图 1.16*所示：

![图片](img/practical-java-programming-with-chatgpt-Figure-1.16.jpg)

图 1.16：可以像上面所示那样使用消息窗口，点击白色箭头图标。

点击白色箭头（如图*图 1.16*所示，背景为绿色），显示如图*图 1.17*所示：

![图片](img/practical-java-programming-with-chatgpt-Figure-1.17.jpg)

图 1.17：使用复制代码按钮复制的ChatGPT代码。

这将给出输出代码和文本描述（对于代码，请点击内嵌窗口右上角的复制代码，如图*图 1.17*所示。）生成的代码如下：

注意

实际生成的代码可能会随着时间的推移而改变。例如，我们已将早期响应中的一些新增内容加粗。

`public class BinarySearch {`

`/`

` * 二分查找方法用于在有序数组中查找目标元素。`

` *`

` * @param arr The sorted array to search in.`

` * @param target The element to search for.`

` * @return The index of the target element if found; otherwise, -1.`

` */`

`public static int binarySearch(int[] arr, int target) {`

`int left = 0;`

`int right = arr.length - 1;`

`while (left <= right) {`

`// 如果中间元素是目标，则返回其索引`

`if (arr[mid] == target) {`

`return mid;`

`}`

`// 如果目标在左侧，则丢弃右侧`

`if (arr[mid] > target) {`

`right = mid - 1;`

`} else { // 如果目标在右侧，则丢弃左侧`

`left = mid + 1;`

`}`

`}`

```py`` `// If the target is not found, return -1`    `return -1;`    `}`   ```` `public static void main(String[] args) {`    `int[] arr = {2, 5, 8, 12, 16, 23, 38, 45, 56, 72, 91};`    `int target = 23;`   ```py `int index = binarySearch(arr, target);`   `` `if (index != -1) {`    `System.out.println("Element found at index: " + index);`    `} else {`    `System.out.println("Element not found in the array.");`    `}`    `}`    `}`    We can scroll down past the code window to show the ChatGPT AI description, as follows:    *In this example, we have a sorted array arr, and we're searching for the target element using the binarySearch method. If the target element is found, the method will return its index; otherwise, it will return -1 to indicate that the element is not present in the array. The provided main method demonstrates how to use the binarySearch method with a sample array.*    # Installing and using the Android phone App, Ask AI    This other option, which gives similar responses, is to use the Android phone app, Ask AI, created by Codeway Dijital.    (This can be used for up to three questions per day for free)    It costs £4.89/week or £٣٩.٩٩ for Lifetime unlimited access.  ![](img/practical-java-programming-with-chatgpt-Figure-1.18.jpg)  Figure 1.18: The ChatGPT Android app on Google Play    The Install now option is clicked as shown in *Figure 1.19 (a)* and opened as shown in *Figure 1.19 (b)*.  ![](img/practical-java-programming-with-chatgpt-Figure-1.19.jpg)  Figure 1.19: (a) The *Ask AI ChatGPT* app is installed from the Google Play web site. (b) The installed *Ask AI ChatGPT* app is started with the *Open* button    On the Android mobile phone we can now tap on the newly installed Ask AI icon as shown in *Figure 1.20*.  ![](img/practical-java-programming-with-chatgpt-Figure-1.20.jpg)  Figure 1.20: The *Ask AI ChatGPT* app icon is shown in the Android ‘phone screen    The icon highlighted in *Figure 1.20* is tapped to display the window shown in *Figure 1.21*:  ![](img/practical-java-programming-with-chatgpt-Figure-1.21.jpg)  Figure 1.21: (a) The X close on the top left, gives the “free” default screen (b) Three free questions are allowed    # Creating an account for the Subscribed ChatGPT-4    To log in to GPT-4, the following steps are recommended:    1.  Sign up for OpenAI in the previous section.          After loading the OpenAI website, as shown in Figure 1.15, mouse-over on the “GPT-4” button located in the upper-center of the screen, as shown in Figure 1.22.and then select the Upgrade to ChatGPT Plus button. Follow the prompts to create your OpenAI account.          ![](img/practical-java-programming-with-chatgpt-Figure-1.22.jpg)          Figure 1.22: The option to upgrade to ChatGPT Plus           2.  You can now Subscribe to Chat GPT Plus: You will be prompted to subscribe to the Chat GPT Plus plan, which costs $20 per month. Follow the instructions to complete the subscription process. By subscribing to Chat GPT Plus, you will gain access to the GPT-4 version.          But, why pay for this when you can get the power of ChatGPT Plus from the Microsoft Windows Bing search engine?                    You will notice that the latest MS Windows 10 version (kindly updated for free by Microsoft) has a new search box:          ![](img/practical-java-programming-with-chatgpt-Figure-1.23.jpg)          Figure 1.23: The latest Windows Search box with its Ouroboros snake logo              So, just knowing Microsoft’s search engine is called Bing, we entered the following text into the Box in *Figure 1.24*    “What does Bing use for its AI”  ![](img/practical-java-programming-with-chatgpt-Figure-1.24.jpg)  Figure 1.24: The Bing search engine reply to “What does Bing use for its AI”    Then we asked:    “Which version of ChatGPT does Bing use?”    Which gave the response:    *"ChatGPT 3.5, which is what powers the chatbot that's gained notoriety since launching last November, relied on information from 2021 and before. The new OpenAI large language model that powers Bing has been optimized for search. It's built on learning from ChatGPT and GPT-3.5.*"    Disappointing, but just as the snake is shown eating its tail, if you paste this response as a search, back into the text box, you get    *"There has been speculation that Bing Chat uses GPT-4, and Microsoft confirmed that’s the case after OpenAI announced the launch of ChatGPT-4."*    Just to confirm this amazing response, we feed this reply text back again into the search box too, with the response from the Bing search engine, as shown in *Figure 1.25*:  ![](img/practical-java-programming-with-chatgpt-Figure-1.25.jpg)  Figure 1.25: The confirmation that we are using *ChatGPT Version 4* through *MS Bing* search    Out of curiosity, we repeated the question asked earlier in ChaptGPT 3.5:    Have you got a java code method for a binary search program?  ![](img/practical-java-programming-with-chatgpt-Figure-1.26.jpg)  Figure 1.26: We ask Bing the question we asked previously for a Binary search code method    This gives the link:    [`www.softwaretestinghelp.com/binary-search-in-java/`](https://www.softwaretestinghelp.com/binary-search-in-java/)    (Updated on June 25, 2023)    This link has a full tutorial, so provides a very good introduction for a student Java programmer. It also uses a smarter version of the Binary Search code, using the standard Java Arrays.binarySearch method.    Note    *You may have noticed in the code example given, that the Array position of the number 50 is the fifth number in the list, so you might think the program has given the wrong answer for the index of 4.*    Here you have to remember that Java array elements are numbered with the first element indexed from zero.    Be sure to check the use of any of the code given in this link as the material is copyright protected!    We found the following on their website ( [`www.softwaretestinghelp.com/copyright-policy/`](https://www.softwaretestinghelp.com/copyright-policy/) ):    “Fair use allowed:    If you want to refer to any article from this website you can post article excerpts or summaries generally not more than one paragraph and a link back to Softwaretestinghelp.com original article.”    # Conclusion    There are a number of options available to use OpenAI’s ChatGPT AI application as a free tool for assisting a Java software developer as described, step-by-step in this first chapter.    The Java code for the Binary Search example we used was requested in the Free Bing search engine as shown in *Figure 1.26*, the link provided gives a full description of the algorithm and examples of the Java code we require.    In the next chapter, we will look at Java programming best practices as stated by ChatGPT.    # Points to remember    *   For copyright, it is important to use due diligence and research yourself to confirm the code you wish to use is really in the public domain. *   The web pages supplied by ChatGPT are regularly updated by OpenAI. This AI system is always evolving, so be aware that the examples supplied in this book may change over time. The book attempts to focus on making the best use of AI systems, to suit the expertise of the Java programmer, so we have covered access to bare code and the use of the Bing search engine for in-depth assistance. *   The actual code generated may very well change over time. As an example, we have emboldened some of the additions made from an earlier response given in the code listed for the Binary Search code shown in this Chapter.    # Multiple choice questions    1.  Which version of ChatGPT is charged at $20 per month?     1.  ChatGPT model GPT-4     2.  ChatGPT model GPT-3-5     3.  gpt-3.5-turbo-0301     4.  Microsoft Bing 2.  GDPR is the pneumonic for?     1.  General Digital Processing Regulations     2.  General Digital Protection Requirements     3.  General Data Protection Regulations     4.  General Data Processing Regulations 3.  Which of the following is the name for the Android mobile ‘phone app?     1.  ChatGPT     2.  Ask AI     3.  Bing     4.  OpenAI    # Answers    1.  a 2.  c 3.  b    # Questions    1.  Which is the most expensive option for using the ChatGPT AI, also describe the limitations of each of the ‘free’ versions. 2.  What are the main reasons that Copyright is not assignable to the content produced by an AI program? 3.  Why should you still be careful to validate the responses created by ChatGPT? 4.  Why is it important to provide a valid email address when applying for an OpenAI account?    # Key terms    *   AI: Artificial Intelligence Software that mimics the responses you might expect to questions supplied by a human operator. *   OpenAI: is the American artificial intelligence research laboratory that developed ChatGPT comprising the non-profit OpenAI organization and its for-profit subsidiary corporation OpenAI Limited. *   API: Application Programmer’s Interface – a set of callable methods to allow a server system to be accessed for functionality using code used for a client-based program. *   Ask AI: The Android mobile phone app is available for access to ChatGPT 3.5. *   CC BY-NC-SA: Creative Commons, by NonCommercial-ShareAlike Attribution, effectively a copyright-free software license providing the content is correctly attributed with a reference link to the original software source. *   ChatGPT: ChatGPT is a language model developed by OpenAI. It is based on the GPT (Generative Pre-trained Transformer) architecture, specifically GPT-3.5 for the free use option. The model is designed to generate human-like text responses to user inputs, making it capable of engaging in interactive and natural-sounding conversations. ChatGPT has been trained on a massive amount of diverse textual data from the internet, allowing it to acquire a broad understanding of language and context. It uses deep learning techniques, particularly transformers, which enable it to process and generate text effectively. This language model has a wide range of applications, including answering questions, providing explanations, giving recommendations, offering creative writing assistance, language translation, and code generation. It can be integrated into various software operating systems and hardware platforms and can be used to create software applications to offer interactive and conversational experiences for users using the ChatGPT API interface. *   EPO: The European Patent Office. *   EU: The European Union *   Fortran: Early scientific computer language, derived from Formula Translation. *   GDPR: General Data Protection Regulations, *   SMS: Short Message Service, used to send the text through to a cell mobile phone, from another cell ‘phone, or a computer server. *   WIPO: The World Intellectual Property Organisation. `` ``` ```py` `````  ```py```````py```````py```````py```````py```````py```````py```````py```````py````` ```py```````py```````py```````py```````py```````py```````py```````py```````py```` # 第二章    # Java 编程 – ChatGPT 阐述的最佳实践    # 引言    在本章中，我们提示 ChatGPT 测试其对良好编程实践的知识。我们要求它定义其所知的“SOLID”原则，它几乎立即就做到了，以下输出仅为引言：    “*SOLID 是一组由罗伯特·C·马丁（也称为鲍勃大叔）提出的面向对象编程的五项原则。这些原则旨在使软件设计更加健壮、灵活和可维护。以下是 SOLID 原则的简要概述及其在 Java 中的应用方式*：”    # 结构    在本章中，我们将讨论以下主题：    *   SOLID 原则 *   Java 代码缩进的最佳实践 *   SOLID 代码示例     *   单一职责原则 (SRP)     *   开闭原则 (OCP)     *   里氏替换原则 (LSP)     *   接口隔离原则 (ISP)     *   依赖倒置原则 (DIP)    # SOLID 原则    当我们提出以下问题时，ChatGPT 关于使用面向对象编程的五项原则的回应编号如下：    “什么是用于 Java 程序开发的 SOLID 原则？”    1.  单一职责原则 (SRP)： 一个类应该只有一个引起变化的原因。这意味着一个类应该只负责一项职责或工作。如果一个类承担多项职责，它将变得难以更改、测试和维护。在 Java 中，您可以通过创建更小、更专注、只做好一件事的类来应用 SRP。 2.  开闭原则 (OCP)： 软件实体（类、模块、函数）应该对扩展开放，对修改关闭。这意味着您应该能够在不修改现有代码的情况下为程序添加新功能。在 Java 中，您可以通过使用接口和抽象类来应用 OCP，为客户端提供稳定的接口，同时允许实现细节变化。 3.  里氏替换原则 (LSP)： 子类型应该可以替换其基类型。这意味着任何子类都应该能够替代其父类使用而不会引发问题。在 Java 中，您可以通过遵循类之间的“is-a”关系并确保子类方法不违反其父类的契约来应用 LSP。 4.  接口隔离原则 (ISP)： 客户端不应该被迫依赖它们不使用的接口。这意味着您应该设计符合其客户端特定需求的接口。在 Java 中，您可以通过创建目的明确、仅包含与客户端相关方法的更小接口来应用 ISP。 5.  依赖倒置原则 (DIP)： 高层模块不应该依赖低层模块。两者都应该依赖抽象。抽象不应该依赖细节。细节应该依赖抽象。这意味着您应该设计代码，使高层模块与低层模块解耦，并且两者都依赖抽象。在 Java 中，您可以通过使用依赖注入来为对象提供其依赖项，并通过面向接口编程而非具体类来应用 DIP。    # Java 代码缩进的最佳实践    在以下问题中，我们使用了可通过基于网页的链接访问的 ChatGPT 3.5：    [`chat.openai.com/`](https://chat.openai.com/) :    您能描述一下 Java 代码缩进的最佳实践吗？    正确的代码缩进对于编写干净、可读和可维护的 Java 代码至关重要。一致且格式良好的代码可以提高开发人员之间的协作效率，并减少引入错误的机会。以下是 Java 代码缩进的一些最佳实践：    *   使用一致的缩进风格： 选择特定的缩进风格（例如，2 个空格、4 个空格或制表符），并在整个代码库中坚持使用。一致性是可读性的关键。 *   块的缩进： 缩进每个代码块（如类、方法、循环和条件语句），以直观地显示它们的层次结构。块的内容应进一步缩进一级。w![](img/practical-java-programming-with-chatgpt-Figure-2.1.jpg)          图 2.1： ChatGPT Java 代码缩进示例           *   垂直对齐： 垂直对齐相似元素以提高可读性。这对于赋值、方法调用或多个变量声明特别有用。![](img/practical-java-programming-with-chatgpt-Figure-2.2.jpg)          图 2.2： ChatGPT Java 代码垂直对齐示例           *   链式调用和方法调用： 当进行链式方法调用时，对齐点号以提高清晰度。如果参数在一行内容纳不下，也可以对齐参数。![](img/practical-java-programming-with-chatgpt-Figure-2.3.jpg)          图 2.3： ChatGPT Java 代码垂直对齐示例           *   换行缩进： 当一行过长并换行到多行时，后续行应缩进以表示其延续。![](img/practical-java-programming-with-chatgpt-Figure-2.4.jpg)          图 2.4： ChatGPT Java 代码换行缩进示例           *   嵌套结构的缩进： 处理嵌套结构时，相应增加缩进级别以显示其嵌套层次。![](img/practical-java-programming-with-chatgpt-Figure-2.5.jpg)          图 2.5： ChatGPT Java 代码嵌套结构缩进示例           *   注释和注解： 注释和注解通常应与其关联的代码保持相同的缩进级别。![](img/practical-java-programming-with-chatgpt-Figure-2.6.jpg)          图 2.6： ChatGPT Java 代码注释和注解缩进示例           *   对齐参数： 对于具有多个参数的方法调用，考虑对齐参数以提高可读性。![](img/practical-java-programming-with-chatgpt-Figure-2.7.jpg)          图 2.7： ChatGPT Java 代码对齐参数示例           *   Switch 语句中的缩进： 缩进 switch 语句中的 case 标签，并缩进每个 case 块内的代码。![](img/practical-java-programming-with-chatgpt-Figure-2.8.jpg)          图 2.8： ChatGPT Java 代码 Switch 语句缩进示例           *   使用 IDE 的格式化工具： 大多数现代集成开发环境 (IDE) 都提供自动代码格式化工具。配置 IDE 设置以遵循您首选的缩进风格，并定期使用自动格式化功能。 *   通过遵循这些最佳实践，您可以创建易于阅读、理解和维护的 Java 代码，从而实现更高效和协作的开发过程。    # SOLID 代码示例    我们通过向 ChatGPT Ask AI 手机应用程序提出以下针对其列出的每项原则的问题，详细检查了面向对象编程的五项“SOLID”最佳实践 Java 编码原则，如下节所示：    # 单一职责原则 (SRP)    您有说明 SOLID 单一职责原则的 Java 代码示例吗？    当然！单一职责原则 (SRP) 规定一个类应该只有一个引起变化的原因，意味着它应该只有一个职责。以下是一个演示 SRP 的 Java 代码示例：    ```py` ```java ```py`    `*// UserService class responsible for user-related operations*`    `*public class UserService {*`    `*public void registerUser(String username, String password) {*`    `// logic for registering a user`    `}`    `*public void authenticateUser(String username, String password) {*`    `*// logic for authenticating a user*`    `*}*`   ``````py```````py```````py```````py```````py````` `*public void resetPassword(String username) {*`    `*// 重置用户密码的逻辑*`    `*}*`   ```py```````py```````py```````py```````py```````py `// other user-related methods…`    `*}*`    `*// EmailService class responsible for sending emails*`    `public class EmailService {`    `*public void sendEmail(String recipient, String message) {*`    `// logic for sending an email`    `}`   ``````py```````py```````py```````py```````py``` `// other email-related methods…`    `}`    ```` ```py ````    在上面的示例中，我们有两个类：UserService 和 EmailService。UserService 类负责与用户相关的操作，如用户注册、身份验证和密码重置。它遵循 SRP，因为它只有一个管理用户相关操作的职责。    另一方面，EmailService 类负责发送电子邮件。它遵循 SRP，因为它只有一个管理电子邮件相关操作的职责。    通过将关注点分离到两个独立的类中，我们遵循了 SRP，并在代码中实现了更好的可维护性和灵活性。如果需要对用户相关操作进行更改，我们只需修改 UserService 类，而不会影响 EmailService 类，反之亦然。    # 开闭原则 (OCP)    您有说明 SOLID 开闭原则的 Java 代码示例吗？    当然！开闭原则 (OCP) 规定类应该对扩展开放，对修改关闭。换句话说，您应该能够在不修改现有代码的情况下为类添加新功能。以下是一个演示 OCP 的 Java 代码示例：    ```py` ```java ```py`    `*// Shape interface representing a geometric shape*`    `*public interface Shape {*`    `*double calculateArea();*`    `}`   ``````py```````py```````py```````py```````py`` `*// Rectangle class implementing the Shape interface*`    `*public class Rectangle implements Shape {*`    `private double width;`    `private double height;`   ``````py```````py```````py```````py```````py` `*public Rectangle(double width, double height) {*`    `this.width = width;`    `this.height = height;`    `}`   ``````py```````py```````py```````py```````py `*public double getWidth() {*`    `return width;`    `}`   ``````py```````py```````py```````py`````` `*public double getHeight() {*`    `not`    `*return height;*`    `}`   ```py```````py```````py```````py```````py` `*public double calculateArea() {*`    `return width * height;`    `}`    `*}*`   ``````py```````py```````py```````py```` `*// Circle 类实现 Shape 接口*`    `*public class Circle implements Shape {*`    `private double radius;`   ```py```````py```````py```````py`````` `*public Circle(double radius) {*`    `this.radius = radius;`    `}`    `*public double getRadius() {*`    `return radius;`    `}`   ```py```````py```````py```````py````` `*public double calculateArea() {*`    `return Math.PI * radius * radius;`    `}`    `}`   ```py```````py```````py```````py```` `*// AreaCalculator 类负责计算形状的总面积*`    `*public class AreaCalculator {*`    `*public double calculateTotalArea(Shape[] shapes) {*`    `double totalArea = 0;`    `for (Shape shape : shapes) {`    `totalArea += shape.calculateArea();`    `}`    `return totalArea;`    `}`    `}`    ```py` ``` ```py`    In the above example, we have an AreaCalculator class that is responsible for calculating the total area of shapes. It follows the OCP because it is open for extension. If we want to add a new shape, such as a Triangle, we can create a new class that implements the `Shape` interface without modifying the existing code.    The Rectangle and Circle classes are examples of shapes that implement the Shape interface. They are closed for modification because their code does not need to be changed when adding a new shape.    By adhering to the OCP, we can easily introduce new shapes by creating new classes that implement the Shape interface, without modifying the AreaCalculator class or existing shape classes. This promotes code reusability and maintainability.    # Liskov Substitution Principle (LSP)    The response to this question by ChatGPT Ask AI, uses the same example Java code, as a base that was used in the previous section, entitled Open/Closed Principle (OCP) so, we have highlighted the additional Java code that was added in the response below, in bold italic.    Do you have a Java Code example that illustrates the SOLID Liskov Substitution Principle?    Certainly! The Liskov Substitution Principle (LSP) states that objects of a superclass should be replaceable with objects of its subclasses without affecting the correctness of the program. Here's a Java code example that illustrates the LSP:    ```` ```pyjava ````    `// Shape 接口表示几何形状`    `public interface Shape {`    `double calculateArea();`    `}`   ```py```````py```````py```````py``` `// Rectangle class implementing the Shape interface`    `public class Rectangle implements Shape {`    `private double width;`    `private double height;`   ``````py```````py```````py`````` `public Rectangle(double width, double height) {`    `this.width = width;`    `this.height = height;`    `}`   ```py```````py```````py```````py` `public double getWidth() {`    `return width;`    `}`   ``````py```````py```````py```` `public void setWidth(double width) {`    `this.width = width;`    `}`   ```py```````py```````py`````` `public double getHeight() {`    `return height;`    `}`   ```py```````py```````py````` `public void setHeight(double height) {`    `this.height = height;`    `}`    `public double calculateArea() {`    `return width * height;`    `}`    `*}*`   ```py```````py```````py```` `*// Square class extending the Rectangle class*`    `*public class Square extends Rectangle {*`    `public Square(double sideLength) {`    `super(sideLength, sideLength);`    `}`    `@Override`    `public void setWidth(double width) {`    `super.setWidth(width);`    `super.setHeight(width);`    `}`    `@Override`    `public void setHeight(double height) {`    `super.setWidth(height);`    `super.setHeight(height);`    `}`    `*}*`    `*// AreaCalculator class responsible for calculating the total area of shapes*`    `*public class AreaCalculator {*`    `public double calculateTotalArea(Shape[] shapes) {`    `double totalArea = 0;`    `for (Shape shape : shapes) {`    `totalArea += shape.calculateArea();`    `}`    `return totalArea;`    `}`    `}`    ```py` ``` ```py`    In the above example, we have an AreaCalculator class that calculates the total area of shapes. The Shape interface represents a geometric shape and includes a calculateArea() method.    The Rectangle class implements the Shape interface and represents a rectangle with a width and height. The Square class extends the Rectangle class and represents a square with equal side lengths.    The Square class overrides the setWidth() and setHeight() methods from the Rectangle class to ensure that the width and height are always the same for a square. While this contradicts the usual behavior of a rectangle, it adheres to the LSP because objects of the `Square` class can be substituted for objects of the `Rectangle` class without affecting the correctness of the program.    By following the LSP, we can safely substitute objects of a superclass (Rectangle) with objects of its subclasses (Square) without introducing unexpected behavior or breaking the functionality of the program.    # Interface Segregation Principle (ISP)    In the following question, we used the ChatGPT 3.5 available using the web-based link:    [`chat.openai.com/`](https://chat.openai.com/) :    You will notice that, in this example, ChatGPT illustrates code that violates the principle as a way of describing the basis of the concept.    Do you have a Java Code example that illustrates the SOLID Interface Segregation Principle?    Certainly! The Interface Segregation Principle (ISP) is one of the SOLID principles that states that a class should not be forced to implement interfaces it doesn't use. Instead of having a large, monolithic interface, you should create smaller, more specific interfaces that cater to the needs of individual classes. This promotes better separation of concerns and avoids unnecessary dependencies.    Here's a Java code example that illustrates the Interface Segregation Principle    `// Interface Segregation Principle Violation`    `// Suppose we have a monolithic interface that contains multiple methods.`    `interface Worker {`    `void work();`    `void eat();`    `void sleep();`    `}`   ``````py```````py```````py `class Employee implements Worker {`    `@Override`    `public void work() {`    `System.out.println("Employee is working.");`    `}`   ``````py```````py`````` `@Override`    `public void eat() {`    `System.out.println("Employee is eating.");`    `}`   ```py```````py```````py` `@Override`    `public void sleep() {`    `System.out.println("Employee is sleeping.");`    `}`    `}`   ``````py```````py```` `class Robot implements Worker {`    `@Override`    `public void work() {`    `System.out.println("Robot is working.");`    `}`   ```py```````py`````` `@Override`    `public void eat() {`    `// Robots don't eat, so this method is irrelevant and violates ISP.`    `throw new UnsupportedOperationException("Robots don't eat.");`    `}`   ```py```````py````` `@Override`    `public void sleep() {`    `// Robots don't sleep, so this method is irrelevant and violates ISP.`    `throw new UnsupportedOperationException("Robots don't sleep.");`    `}`    `}`   ```py```````py```` `public class Main {`    `public static void main(String[] args) {`    `Worker employee = new Employee();`    `employee.work();`    `employee.eat();`    `employee.sleep();`   ```py```````py``` `Worker robot = new Robot();`    `robot.work();`    `robot.eat(); // 这个调用对 Robot 没有意义，可能导致错误。`    `robot.sleep(); // 这个调用对 Robot 没有意义，可能导致错误。`    `}`    `}`    在这个例子中，Worker 接口违反了接口隔离原则，因为它强制所有实现类为像 eat() 和 sleep() 这样的方法提供实现，即使这些方法并非对所有类型的 worker（如机器人）都相关。    为了遵循接口隔离原则，您需要将庞大的 Worker 接口分解为更小、更专注的接口，基于每种 worker 类型的特定职责，例如 Workable、Eatable 和 Sleepable。这样，每个类只需要实现与其行为相关的接口。    # 依赖倒置原则 (DIP)    在以下问题中，我们也使用了可通过基于网页的链接访问的 ChatGPT 3.5：    [`chat.openai.com/`](https://chat.openai.com/) :    您有说明 SOLID 依赖倒置原则的 Java 代码示例吗？    当然！依赖倒置原则 (DIP) 是 SOLID 原则之一，它规定高层模块不应该依赖低层模块。两者都应该依赖抽象。此外，抽象不应该依赖细节；细节应该依赖抽象。简单来说，这个原则鼓励使用接口或抽象类来定义高层结构和组件之间的关系，促进松耦合和灵活性。    以下是一个说明依赖倒置原则的 Java 代码示例：    在这个例子中，通过引入 Switchable 接口来演示依赖倒置原则。LightBulb 和 Fan 类都实现了 Switchable 接口。Switch 类依赖于 Switchable 抽象，而不是具体实现。这允许您轻松地在不同类型的设备（灯泡、风扇等）之间切换，而无需修改 Switch 类。    `// 依赖倒置原则示例`    `// 依赖抽象的高层模块。`    `class LightBulb {`    `void turnOn() {`    `System.out.println("LightBulb: 灯泡已打开。");`    `}`   ``````py`````` `void turnOff() {`    `System.out.println("LightBulb: 灯泡已关闭。");`    `}`    `}`   ```py```````py` `// Another high-level module that also depends on the same abstraction.`    `class Switch {`    `private final Switchable device;`   ``````py```` `Switch(Switchable device) {`    `this.device = device;`    `}`   ```py`````` `void turnOn() {`    `System.out.println("Switch: 正在打开…");`    `device.turnOn();`    `}`   ```py````` `void turnOff() {`    `System.out.println("Switch: 正在关闭…");`    `device.turnOff();`    `}`    `}`   ```py```` `// 抽象（接口），高层模块都依赖它。`    `interface Switchable {`    `void turnOn();`    `void turnOff();`    `}`   ```py``` `// 实现抽象的低层模块。`    `class Fan implements Switchable {`    `@Override`    `public void turnOn() {`    `System.out.println("Fan: 风扇已打开。");`    `}`   ````` `@Override`    `public void turnOff() {`    `System.out.println("Fan: Fan turned off.");`    `}`    `}`   ```py` `public class Main {`    `public static void main(String[] args) {`    `Switchable fan = new Fan();`   ``` `Switch fanSwitch = new Switch(fan);`    `fanSwitch.turnOn();`    `fanSwitch.turnOff();`   `` `LightBulb bulb = new LightBulb();`    `Switch bulbSwitch = new Switch(bulb);`    `bulbSwitch.turnOn();`    `bulbSwitch.turnOff();`    `}`    `}`    By adhering to the Dependency Inversion Principle, the code becomes more flexible, maintainable, and easier to extend. High-level modules are not tightly coupled to low-level modules, and changes in low-level modules do not affect the high-level modules.    # Conclusion    In this chapter, we prompted ChatGPT to test its knowledge of good programming practice. We asked it to define what it knew about the “SOLID” principles which it did almost instantaneously. The AI program also provided code examples to illustrate the best practice for Java code indentation. (The following link covers the reasons why the ChatGPT AI can be very slow: [`ecoagi.ai/topics/ChatGPT/why-is-chatgpt-slow`](https://ecoagi.ai/topics/ChatGPT/why-is-chatgpt-slow) )    In the next chapter, we try using the OpenAI Java API to interface with the ChatGPT AI system. ChatGPT provided an example of how to make a request to the API using the OkHttp library.    We also try the REST API service provided for ChatGPT and the new Whisper speech to text feature.    # Points to remember    *   SOLID is a set of five principles for object-oriented programming, aim to make software designs more robust, flexible, and maintainable. *   Proper code indentation is essential for writing clean, readable, and maintainable Java code *   Take advantage of your Java Integrated Development Environments (IDE) auto-formatting feature to provide automatic code formatting, configured to follow your organizations indentation style. *   A Java class should have one single responsibility. *   You should be able to add new functionality to a Java class without modifying its existing code. *   Objects of a Java superclass should be replaceable with Objects of its subclasses without affecting the correctness of the program. *   Create smaller, more specific interfaces that cater to the needs of individual classes to promote better separation of concerns and avoid unnecessary dependencies. *   High-level Java modules should not depend on low-level modules. Both should depend on abstractions.    # Multiple choice questions    1.  Which of the following is the best description of the Liskov Substitution Principle (LSP)?     1.  A Java class should have one single responsibility.     2.  You should be able to add new functionality to a Java class without modifying its existing code.     3.  Objects of a Java superclass should be replaceable with Objects of its subclasses without affecting the correctness of the program.     4.  Create smaller, more specific interfaces that cater to the needs of individual classes to promote better separation of concerns and avoid unnecessary dependencies.     5.  High-level Java modules should not depend on low-level modules. Both should depend on abstractions. 2.  Which of the following is the best description of the Interface Segregation Principle (ISP)?     1.  A Java class should have one single responsibility.     2.  You should be able to add new functionality to a Java class without modifying its existing code.     3.  Objects of a Java superclass should be replaceable with Objects of its subclasses without affecting the correctness of the program.     4.  Create smaller, more specific interfaces that cater to the needs of individual classes to promote better separation of concerns and avoid unnecessary dependencies.     5.  High-level Java modules should not depend on low-level modules. Both should depend on abstractions. 3.  Which recommendation best describes the indentation for Chaining and Method Calls?     1.  Indent the case labels.     2.  Subsequent lines should be indented to indicate their continuation.     3.  Align the parameters for improved readability.     4.  Align the dots for better clarity.    # Answers    1.  c 2.  d 3.  d    # Questions    1.  Describe three different examples of Java code which displays the use of the SOLID principles.? 2.  Can you think of one advantage of using the ChatGPT 3.5 AI available using the web-based OpenAI link, [`chat.openai.com/`](https://chat.openai.com/) compared with the ChatGPT 3.5 AI available through the Ask AI Mobile 'phone App?? 3.  There are a couple of methods missing from the Java code example which illustrates the SOLID Open/Closed Principle compared with the code given for the SOLID Liskov Substitution Principle. Can you describe the purpose of these two methods?    # Key terms    *   AI: Artificial Intelligence Software that mimics the responses you might expect to questions supplied by a human operator. *   OpenAI: is the American artificial intelligence research laboratory that developed ChatGPT comprising the non-profit OpenAI organization and its for-profit subsidiary corporation OpenAI Limited. *   Ask AI: The Android mobile phone app is available for access to ChatGPT 3.5. *   SOLID: A set of five principles for object-oriented programming that were introduced by Robert C. Martin (also known as Uncle Bob). *   SRP: Single Responsibility Principle – the first listed principle. *   OCP: Open/Closed Principle– the second listed principle *   LSP: Liskov Substitution Principle– the third listed principle *   ISP: Interface Segregation Principle– the fourth listed principle *   DIP: Dependency Inversion Principle – the fifth listed principle *   ChatGPT: ChatGPT is a language model developed by OpenAI. It is based on the GPT (Generative Pre-trained Transformer) architecture, specifically GPT-3.5 for the free use option. The model is designed to generate human-like text responses to user inputs, making it capable of engaging in interactive and natural-sounding conversations. ChatGPT has been trained on a massive amount of diverse textual data from the internet, allowing it to acquire a broad understanding of language and context. It uses deep learning techniques, particularly transformers, which enable it to process and generate text effectively. This language model has a wide range of applications, including answering questions, providing explanations, giving recommendations, offering creative writing assistance, language translation, and code generation. It can be integrated into various software operating systems and hardware platforms and can be used to create software applications to offer interactive and conversational experiences for users using the ChatGPT API interface. `` ```py ```` ```py`` ``````py ``````py` ``````py`` ``````py``` ``````py```` ```py```````py` ``````py`````` ```py```````py``` ``````py```````py` ``````py```````py`` ``````py```````py``` ``````py```````py```` ```py```````py```````py` ``````py```````py`````` ```py```````py```````py``` ``````py```````py```````py` ``````py```````py```````py`` ``````py```````py```````py``` ``````py```````py```````py```` ```py```````py```````py```````py` ``````py```````py```````py`````` ```py```````py```````py```````py``` ``````py```````py```````py```````py` ``````py```````py```````py```````py`` ``````py```````py```````py```````py``` ``````py```````py```````py```````py```` ```py```````py```````py```````py```````py` ``````py```````py```````py```````py`````` ```py```````py```````py```````py```````py``` ``````py```````py```````py```````py```````py` ``````py```````py```````py```````py```````py`` ``````py```````py```````py```````py```````py``` ``````py```````py```````py```````py```````py```` ```py```````py```````py```````py```````py```````py`  ``````py```````py```````py```````py```````py```````py```````py```````py```````py ``````py```````py```````py```````py```````py```````py```````py```````py`````` # CHAPTER 3    # Developing Java Code for Utilizing the ChatGPT API    # Introduction    This chapter describes the use of the OpenAI Java API to interface with the ChatGPT AI system. ChatGPT provided an example of how to make a request to the API using the OkHttp library.    # Structure    In this chapter, we will discuss the following topics:    *   The ChatGPT API overview *   ChatGPT’s AI-Generated Java code API examples *   Validation of the suggested API Code     *   Accessing the ChatGPT-referenced OkHttp Java Library Jar files     *   Accessing the ChatGPT Secret API Key     *   Using ChatGPT Model Ids    # The ChatGPT API overview    An overview of the ChatGPT and OpenAI organization systems available can be found, after obtaining an OpenAI account, using the link:    [`platform.openai.com/overview`](https://platform.openai.com/overview)    There is a “quick start” link for developers, accessible from this web page:    [`platform.openai.com/docs/quickstart/build-your-application`](https://platform.openai.com/docs/quickstart/build-your-application)    Originally, most GPT models processed unstructured text, presented to the model as a sequence of "tokens". ChatGPT models operate differently, using a sequence of messages together with metadata. Although the input is rendered to the model as a sequence of "tokens" for the model to process, the raw format used is in a format, which OpenAI refers to as Chat Markup Language ("ChatML").    OpenAI uses a pay-as-you-go system per 1,000 tokens. For the initial three months of use, they provide $5 in free credit to developers. They use the text-davinci-003 model in their javascript code example, but they suggest that the new gpt-3.5-turbo model may be best for initial testing. Later, you can progress to check other models to compare the efficiency of the responses, as different models might perform better depending on the required functionality.    The total number of tokens processed in a single request (both prompt and completion) can’t exceed the model's maximum context length. For most models, this is 4,096 tokens or about 3,000 words (1 token is approximately 4 characters or 0.75 words for English text).    OpenAI has recently announced that ChatGPT can now be integrated with its Whisper models, through the ChatGPT API.    The Whisper models give access to language and speech-to-text functionality. OpenAI has provided programmers with complete access to their open-source Whisper large-v2 model in the API, giving much faster (and more efficient processor) results.    OpenAI has developed a REST API endpoint to interact with their ChatGPT models.    The example code pattern they provide for this interaction is as follows:    `curl https://api.openai.com/v1/chat/completions \`    `-H "Authorization: Bearer $OPENAI_API_KEY" \`    `-H "Content-Type: application/json" \`    `-d '{`    `"model": "gpt-3.5-turbo",`    `"messages": [{"role": "user", "content": "What is the OpenAI mission?"}]`    `}'`    Note: There is a free-to-download publication from ResearchGate (copyright ASB Software Development Limited), which you can use to install a free RedHat RHEL 8.x Linux operating system, including the supporting VMware virtual server running on an MS Windows operating system: https://doi.org/10.13140/RG.2.2.14590.95049    This REST URL gives the following result, after posting, when we use our OpenAI key in a Linux command window:  ![](img/practical-java-programming-with-chatgpt-Figure-3.1.jpg)  Figure 3.1: The OpenAI REST API endpoint example    The $OPENAI_API_KEY environment variable just needs to be set with a unique key, as shown in the redacted example. This involves using the OpenAI key, which we will show how to download from your OpenAI account later in this chapter, in the section Accessing the ChatGPT Secret API Key.    I have highlighted in bold the JSON formatted response returned by the ChatGPT AI.    `(base) [root@ECMUKDEMO6 ~]# export OPENAI_API_KEY=skxxxxxxxxxxxxxxxxxxxxxxxBlbkFJVAxxxxxxxxxxxxxxxxxx`    `(base) [root@ECMUKDEMO6 ~]# echo $OPENAI_API_KEY`    `skxxxxxxxxxxxxxxxxxxxxxxxBlbkFJVAxxxxxxxxxxxxxxxxxx`    `(base) [root@ECMUKDEMO6 ~]# curl https://api.openai.com/v1/chat/completions \`    `>  -H "Authorization: Bearer $OPENAI_API_KEY" \`    `>  -H "Content-Type: application/json" \`    `>  -d '{`    `>  "model": "gpt-3.5-turbo",`    `>  "messages": [{"role": "user", "content": "What is the OpenAI mission?"}]`    `>  }'`    `{`    `"id": "chatcmpl-7kBI4h7I2KeQzzGMVnjjTqn7avwUU",`    `"object": "chat.completion",`    `"created": 1691240844,`    `"model": "gpt-3.5-turbo-0613",`    `"choices": [`    `{`    `"index": 0,`    `"message": {`    `"role": "assistant",`    `"content": "The OpenAI mission is to ensure that artificial general intelligence (AGI) benefits all of humanity. AGI refers to highly autonomous systems that outperform humans at most economically valuable work. OpenAI aims to build safe and beneficial AGI directly or to aid others in achieving this outcome. OpenAI commits to using any influence it obtains over AGI’s deployment to ensure that it benefits everyone and avoids uses that harm humanity or unduly concentrate power. The organization also emphasizes the importance of long-term safety, conducting research to make AGI safe and driving its adoption in the AI community. OpenAI further pledges to cooperate with other research and policy institutions to create a global community working together towards AGI’s societal challenges."`    `},`    `"finish_reason": "stop"`    `}`    `],`    `"usage": {`    `"prompt_tokens": 14,`    `"completion_tokens": 142,`    `"total_tokens": 156`    `}`    `}`    `(base) [root@ECMUKDEMO6 ~]#`    Whisper, the speech-to-text model, was released in September 2022 by OpenAI and was recently updated to the large-v2 model available through the Whisper API (this is charged as $0.006/minute).    Whisper API currently accepts the following sound file formats:    m4a, mp3, mp4, mpeg, mpga, wav, webm    OpenAI has also supplied an example code pattern for Whisper AI:    `curl https://api.openai.com/v1/audio/transcriptions \`    `-H "Authorization: Bearer $OPENAI_API_KEY" \`    `-H "Content-Type: multipart/form-data" \`    `-F model="whisper-1" \`    `-F file="@/path/to/file/openai.mp3"`    We used a mobile phone to record a .wav file and copied it to use on the Linux system.    (This sound file, `Recording9.wav`, was converted to text (highlighted in bold) with 100% accuracy!)    First, we copied the original emailed file (`Recording 9.wav`) to the Linux VMWare server `/root` directory and removed the space from the file name using the `mv` command to rename it:    `(base) [root@ECMUKDEMO6 ~]# cp /mnt/hgfs/Installs/Recording\ 9.wav .`    `(base) [root@ECMUKDEMO6 ~]# mv Recording\ 9.wav Recording9.wav`    `(base) [root@ECMUKDEMO6 ~]# pwd`    `/root`    The command was then run (with the key already set in the `OPEN_API_KEY` environment variable) using the following:    `(base) [root@ECMUKDEMO6 ~]# curl https://api.openai.com/v1/audio/transcriptions \`    `>   -H "Authorization: Bearer $OPENAI_API_KEY" \`    `>   -H "Content-Type: multipart/form-data" \`    `>   -F model="whisper-1" \`    `>   -F file="@/root/Recording9.wav"`    `{"text":"This is a very short example file to show the availability of ChatGPT to translate a voice file into a text stream."(((((base) [root@ECMUKDEMO6 ~]#`  ![](img/practical-java-programming-with-chatgpt-Figure-3.2.jpg)  Figure 3.2: The *OpenAI* REST *API* endpoint example using the *whisper-1* model    For additional links, please visit [`openai.com/blog/introducing-chatgpt-and-whisper-apis`](https://openai.com/blog/introducing-chatgpt-and-whisper-apis).    In this link, OpenAI restates for developers that they are:    "Simplifying our Terms of Service and Usage Policies, including terms around data ownership: users own the input and output of the models.”    ChatGPT’s AI-Generated Java code API examples    Using Ask AI on the mobile phone, we asked ChatGPT for a Java program example for using the API interfacing to the server-based AI.    Is there an example of a Java program code to interface with the ChatGPT AI system?    *Yes, you can use the OpenAI API to interface with the ChatGPT AI system in Java. Here is an example of how to make a request to the API using the OkHttp library:*    ```py`*```java*```py`    `*import okhttp3.*;*`    `*public class ChatGPTApi {*`    `*private static final String API_KEY = "YOUR_API_KEY";*`    `*private static final String MODEL_ID = "YOUR_MODEL_ID";*`    `*private static final String API_URL = "https://api.openai.com/v1/engines/" + MODEL_ID + "/completions";*`   ``````py `*public static String getResponseFromGPT(String prompt) throws Exception {*`    `OkHttpClient client = new OkHttpClient().newBuilder().build();`    `MediaType mediaType = MediaType.parse("application/json");`    `RequestBody body = RequestBody.create(mediaType, "{\"prompt\": \"" + prompt + "\",\"temperature\":0.7,\"max_tokens\":60}");`    `Request request = new Request.Builder()`    `.url(API_URL)`    `.method("POST", body)`    `.addHeader("Content-Type", "application/json")`    `.addHeader("Authorization", "Bearer " + API_KEY)`    `.build();`    `Response response = client.newCall(request).execute();`    `String responseJson = response.body().string();`    `response.close();`    `return responseJson;`    `}`   ````` `public static void main(String[] args) throws Exception {`    `String responseJson = getResponseFromGPT("Hello, how are you?");`    `System.out.println(responseJson);`    `}`    `}`    ```py` ``` ```py`    *In this example, you need to replace `YOUR_API_KEY` with your actual OpenAI API key and `YOUR_MODEL_ID` with the ID of the ChatGPT model you want to use. You can find the model ID in your OpenAI dashboard.*    *The `getResponseFromGPT` method takes a prompt string as an argument and returns a JSON string containing the response from the ChatGPT model. The `main` method, in this example, demonstrates how to use the `getResponseFromGPT` method to get a response from the ChatGPT model.*    *Note that using the OpenAI API requires that you have an OpenAI API key, which you can obtain by signing up for an OpenAI account and creating an API key.*    # Validation of the suggested API Code    We must now test the Java code created by ChatGPT to validate that we have working code. So, we need to load this code into a suitable Java program development IDE. For this book, we used the latest available Eclipse IDE. The download and installation of Eclipse IDE 2023-06 is covered step-by-step in Chapter 5, Installation of the latest Open-Source Eclipse Java IDE.    ChatGPT, like many other LLM-based AI systems, can give incorrect results (There can also be issues with the generation of AI Hallucinations). See the free pdf file article available at: [`assets.cureus.com/uploads/editorial/pdf/138667/20230219-28928-6kcyip.pdf`](https://assets.cureus.com/uploads/editorial/pdf/138667/20230219-28928-6kcyip.pdf)    In this article on medical diagnosis, from a ChatGPT response, they quoted:    *ChatGPT defines artificial hallucination in the following section. “Artificial hallucination refers to the phenomenon of a machine, such as a chatbot, generating seemingly realistic sensory experiences that do not correspond to any real-world input. This can include visual, auditory, or other types of hallucinations. …. there have been instances where advanced AI systems, such as generative models, have been found to produce hallucinations, particularly when trained on large amounts of unsupervised data.”*    # Accessing the ChatGPT-referenced OkHttp Java Library Jar files    This raises the question about how to access the Java Library jar files, such as OkHttp, which are referenced in the ChatGPT responses. So, I asked ChatGPT:    What are the best Java Jar file Download Sites?  ![](img/practical-java-programming-with-chatgpt-Figure3.3.jpg)  Figure 3.3: (a) ASK AI Phone App question 2 (b) Press down on the window areas to copy    The Android phone Ask AI mobile phone application responses (and questions) can be copied, as shown in *Figure 3.3 (b)*, by pressing a finger on the question or response window area and then selecting Copy Message to obtain the following response:    *“As an AI language model, I can provide you with a list of popular websites where you can download Java JAR files. Here are some of the most widely used ones:*    1.  *Maven Central Repository: Maven Central is the primary repository for Java libraries and dependencies. You can search for JAR files by specifying the group ID and artifact ID of the library you need. Visit the website at [`mvnrepository.com/`](https://mvnrepository.com/).* 2.  *GitHub: Many open-source Java projects host their JAR files on GitHub. You can search for repositories related to the library you are interested in and find the JAR files in their releases or downloads section. The main GitHub website is [`github.com/`](https://github.com/).* 3.  *SourceForge: SourceForge is a popular platform for hosting open-source software, including Java projects. You can search for Java libraries and download JAR files from the project's files section. Visit SourceForge at [`sourceforge.net/`](https://sourceforge.net/).* 4.  *JCenter: JCenter was a popular repository for Java libraries, but it has been sunsetted and is no longer recommended for new projects. However, existing projects may still have JAR files available on JCenter. Visit the website at [`bintray.com/bintray/jcenter`](https://bintray.com/bintray/jcenter).* 5.  *Apache Maven Repository: Apache Maven also hosts a repository for Java libraries and dependencies. You can search for JAR files using the Maven coordinates of the library you want. The website for Apache Maven Repository is [`repository.apache.org/`](https://repository.apache.org/).*    *Please note that when downloading JAR files from external websites, it's important to verify the integrity and authenticity of the files to ensure they are from trusted sources. Additionally, consider using a build automation tool like Maven or Gradle, which can manage dependencies and automatically download JAR files from reputable sources.”*    We used the first option, using the following link:    [`mvnrepository.com/`](https://mvnrepository.com/)  ![](img/practical-java-programming-with-chatgpt-Figure3.4.jpg)  Figure 3.4: The Maven repository search field is used to search for the *okhttp.jar* file    Searching for the okhttp3 jar gives:    [`mvnrepository.com/artifact/com.squareup.okhttp3/okhttp`](https://mvnrepository.com/artifact/com.squareup.okhttp3/okhttp)    Note    *We had to use Version 3.2 eventually, as some features we needed were removed in the later versions of the okhttp.jar file.*  ![](img/practical-java-programming-with-chatgpt-Figure3.5.jpg)  Figure 3.5: The maven repository web page showing the *OkHttp3 jar* download page    This gave the highlighted link, as shown in *Figure 3.5*. Clicking on this link gives the Jar, which is selected using the highlighted link in *Figure 3.6*.  ![](img/practical-java-programming-with-chatgpt-Figure3.6.jpg)  Figure 3.6: The highlighted link is clicked to download the *ChatGPT-*referenced *OkHttp3* jar    When this version failed, we used the earlier version 3.2, available at the following links:    [`mvnrepository.com/artifact/com.squareup.okhttp3/okhttp/3.2.0`](https://mvnrepository.com/artifact/com.squareup.okhttp3/okhttp/3.2.0)    and    [`repo1.maven.org/maven2/com/squareup/okhttp3/okhttp/3.2.0/okhttp-3.2.0.jar`](https://repo1.maven.org/maven2/com/squareup/okhttp3/okhttp/3.2.0/okhttp-3.2.0.jar)    Note    *We also found we had to change the Eclipse project JVM from Java 17 to Java 11*    The Chrome browser prompted us to ensure that we were happy to download a .jar file (which could contain malware). We selected the Keep option, as shown in *Figure 3.7*.  ![](img/practical-java-programming-with-chatgpt-Figure3.7.jpg)  Figure 3.7: The Chrome browser warns about the download of jar files, we selected *Keep*    # Accessing the ChatGPT Secret API Key    The next thing we need is the Secret API Key in the OpenAI Account. The steps are as follows:    Log in using [`platform.openai.com/`](https://platform.openai.com/)    1.  Once logged in, click on your profile name or Icon to open the menu.![](img/practical-java-programming-with-chatgpt-Figure3.8.jpg)          Figure 3.8: The *View API keys* dropdown menu item is selected           2.  On the API Keys page, you will see a list of existing Secret Keys.          The first time into the profile, you need to select the Create new secret key, as highlighted in *Figure 3.9*.          ![](img/practical-java-programming-with-chatgpt-Figure3.9.jpg)          Figure 3.9: The Create new secret key link is clicked as highlighted           3.  Then, click the green icon on the popup page to copy your OpenAI secret key to a safe place, as shown in *Figure 3.10*.![](img/practical-java-programming-with-chatgpt-Figure3.10.jpg)          Figure 3.10: The *Create secret key* button is clicked                    First, select the ![](img/practical-java-programming-with-chatgpt-78.jpg) icon to copy the generated key, as shown in *Figure 3.11*.          ![](img/practical-java-programming-with-chatgpt-Figure3.11.jpg)          Figure 3.11: The new key can now be copied using the highlighted icon                    Next, we need to paste the copied key to a suitable safe text file and save it for use in the Java code.                    After you have a secure copy of the key, you can click Done.          ![](img/practical-java-programming-with-chatgpt-Figure3.12.jpg)          Figure 3.12: The generated key is now listed                    A link to the API introduction tutorial can be accessed by clicking on the green “Authentication” link, as shown in *Figure 3.12*.                    (This links to [`platform.openai.com/docs/api-reference/introduction`](https://platform.openai.com/docs/api-reference/introduction))                    There is a link on the OpenAI website as follows:                    [`openai.com/blog/gpt-4-api-general-availability`](https://openai.com/blog/gpt-4-api-general-availability)                    This shows the status of the ChatGPT version available for access.              # Using ChatGPT Model Ids    ChatGPT models are described in detail in the link [`platform.openai.com/docs/models/overview`](https://platform.openai.com/docs/models/overview)    The model used for our example queries was gpt-3.5-turbo. The installation of the Eclipse IDE is shown step-by-step in *Chapter 5, Installation of the latest Open-Source Eclipse Java IDE.*    Running the ChatGPT API code example, we create a project in the Eclipse IDE by following these steps and clicking on the Create a Java project link, as shown in *Figure 3.13*.  ![](img/practical-java-programming-with-chatgpt-Figure3.13.jpg)  Figure 3.13: The Create a Java project was selected in the new Eclipse installation    We enter the Eclipse IDE Project name as ChatGPTAPI_ExampleChapter3, highlighted in *Figure 3.14*.  ![](img/practical-java-programming-with-chatgpt-Figure3.14.jpg)  Figure 3.14: The Project name is entered as *ChatGPTAPI_ExampleChapter3*    The new project is created once we click the Finish button, as shown in *Figure 3.15*.  ![](img/practical-java-programming-with-chatgpt-Figure3.15.jpg)  Figure 3.15: The Finish button is clicked to create the Eclipse project in the IDE    We now create a new class called ChatGPTApi, with a package name of com.asb, as highlighted in *Figure 3.16*.  ![](img/practical-java-programming-with-chatgpt-Figure3.16.jpg)  Figure 3.16: A new Java class called *ChatGPTApi* is created    After the Finish button is clicked, the new ChatGPTApi Java class is given an empty “skeleton” structure, ready for pasting code into, as shown in *Figure 3.17*.  ![](img/practical-java-programming-with-chatgpt-Figure3.17.jpg)  Figure 3.17: The empty code structure is displayed    As shown in *Figure 3.18*, the loaded code has a number of issues. First, we need to provide a valid version of the okhttp3.jar file, as this is missing from the Class Path of the project.  ![](img/practical-java-programming-with-chatgpt-Figure3.18.jpg)  Figure 3.18: The initial load of the original ChatGPT response Java code    We can now copy the downloaded okhttp-4.11.0.jar file, obtained from the Maven website, to a new Eclipse directory area, /root/eclipse/eclipse/AILibs, on the Linux server. This is used to hold the external .jar file libraries to support the ChatGPT API dependencies.  ![](img/practical-java-programming-with-chatgpt-Figure3.19.jpg)  Figure 3.19: The recommended *ChatGPT* jar file, *okhttp-4.11.0.jar,* is copied to an *Eclipse* area    The Project properties are selected to update the project Class path, as shown in *Figure 3.20*.  ![](img/practical-java-programming-with-chatgpt-Figure3.20.jpg)  Figure 3.20: The Project properties are selected to update the project Class path    The Add External jars option is used to update the Class path, as shown in *Figure 3.21*.  ![](img/practical-java-programming-with-chatgpt-Figure3.21.jpg)  Figure 3.21: The *Add External JARs* button is clicked    We can now add the jar file we downloaded and copied by browsing the Eclipse jar area we created, as shown in *Figure 3.22*.  ![](img/practical-java-programming-with-chatgpt-Figure3.22.jpg)  Figure 3.22: The *okhttp-4.11.0.jar* file is selected from the directory */root/eclipse/eclipse/AILibs*    We discovered the need for another supporting Java library. While running the program, an error occurred:    “The type `okio.ByteString` cannot be resolved. It is indirectly referenced from required type okhttp3.RequestBody ChatGPTApi.java /ChatGPTAPI_ExampleChapter3/src/com/asb line 1 Java Problem”    which we searched finding the link:    [`stackoverflow.com/questions/35329028/okhttp-error-cannot-access-bytestring`](https://stackoverflow.com/questions/35329028/okhttp-error-cannot-access-bytestring)    So, we needed to download the okio jar file. We used the link: [`mvnrepository.com/artifact/com.squareup.okio/okio`](https://mvnrepository.com/artifact/com.squareup.okio/okio)    This jar has the highlighted link:    [`mvnrepository.com/artifact/com.squareup.okio/okio/2.8.0`](https://mvnrepository.com/artifact/com.squareup.okio/okio/2.8.0)    We selected the latest working stable version, which is 2.8 (as shown in the blog error response).    Note    *The later* *okio* *jar file versions 3.4 and 3.5 do not work (we tried them) and also are much smaller.*  ![](img/practical-java-programming-with-chatgpt-Figure3.23.jpg)  Figure 3.23: The *okio-2.8.0.jar* file was added from */root/eclipse/eclipse/AILibs*    On the first run, we get:    `Exception in thread "main" java.lang.NoClassDefFoundError: kotlin/jvm/internal/markers/KMappedMarker`    Internet searches suggested that we needed kotlin-stdlib-1.3.41.jar. (This can be found on the page: [`mvnrepository.com/artifact/org.jetbrains.kotlin/kotlin-stdlib-jdk7/1.3.41`](https://mvnrepository.com/artifact/org.jetbrains.kotlin/kotlin-stdlib-jdk7/1.3.41) )    Then, we also added kotlin-runtime-1.2.71.jar using the following URL links:    [`mvnrepository.com/artifact/org.jetbrains.kotlin/kotlin-runtime`](https://mvnrepository.com/artifact/org.jetbrains.kotlin/kotlin-runtime)    [`repo1.maven.org/maven2/org/jetbrains/kotlin/kotlin-runtime/1.2.71/kotlin-runtime-1.2.71.jar`](https://repo1.maven.org/maven2/org/jetbrains/kotlin/kotlin-runtime/1.2.71/kotlin-runtime-1.2.71.jar)    Now, we get the error message:    `Error caused by: java.lang.ClassNotFoundException: kotlin.collections.AbstractList`    We selected the following link for some ideas on how to fix this:    [`beginnersbook.com/2017/12/kotlin-in-eclipse-ide/`](https://beginnersbook.com/2017/12/kotlin-in-eclipse-ide/)    So, we realized that we need to install the Kotlin plugin framework for Eclipse to satisfy the project dependencies. We selected the Help drop-down menu, Eclipse Marketplace… menu option, as shown in *Figure 3.24*.  ![](img/practical-java-programming-with-chatgpt-Figure3.24.jpg)  Figure 3.24: The *Help* drop-down menu, *Eclipse Marketplace…* menu option is clicked    We select the Enhanced Kotlin for Eclipse in the search results, as shown in *Figure 3.25*, and select all the boxes.  ![](img/practical-java-programming-with-chatgpt-Figure3.25.jpg)  Figure 3.25: The Kotlin install options are displayed    All the supporting packages for Kotlin are selected, as shown in *Figure 3.26*.  ![](img/practical-java-programming-with-chatgpt-Figure3.26.jpg)  Figure 3.26: The full set of Kotlin installation option tick boxes are selected    The License text is displayed, and we click the highlighted I accept radio button option, as shown in *Figure 3.27*.  ![](img/practical-java-programming-with-chatgpt-Figure3.27.jpg)  Figure 3.27: The *I accept* option is selected and the *Finish* button is clicked    The next screen displays the Trust authorities, which we can select to allow updates, as shown in *Figure 3.28*.  ![](img/practical-java-programming-with-chatgpt-Figure3.28.jpg)  Figure 3.28: The Trust Authorities are required to be selected to allow updates as required    On the first (partly successful) run of the code suggested by ChatGPT, we got:    `{`    `"error": {`    `"message": "This is a chat model and not supported in the v1/completions endpoint. Did you mean to use v1/chat/completions?",`    `"type": "invalid_request_error",`    `"param": "model",`    `"code": null`    `}`    `}`    The aforementioned message illustrates the “churn” described in several articles on the code supported by the ChatGPT API. Unfortunately, the API parameters are not at all stable. The model reference names and web links are regularly changed by OpenAI, causing the ChatGPT responses for example API code given in responses to quickly become outdated.    However, even given this limitation, there are very useful ChatGPT responses to more stable requirements such as the algorithms for Java code we are using as examples in the rest of this book.    The preceding issues were still present, even after updating several imports for libraries, as shown in *Figure 3.29*, and using the Kotlin plugin for Eclipse.  ![](img/practical-java-programming-with-chatgpt-Figure3.29.jpg)  Figure 3.29: The final Project jar file list allowing the code to be run    To even get this far, we had to follow these steps:    1.  Add the following imports:          `package com.asb;`                    `import okhttp3.MediaType;`                    `import okhttp3.OkHttpClient;`                    `import okhttp3.Request;`                    `import okhttp3.RequestBody;`                    `import okhttp3.Response;`           2.  Then run the Enhanced Kotlin plugin installation for Eclipse using the Eclipse Market Place. 3.  Finally, we have the libraries required to run the program code, without error, but still not with a valid JSON structure,          We finally get:                    `Request=Request{method=POST, url=https://api.openai.com/v1/chat/completions, headers=[Authorization:Bearer sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxBlbkFJVAxxxxxxxxxxxxxxxxxxx, Content-Type:application/json, messages:[{"role": "user", "content": "What is the OpenAI mission?" }]}{`                    `"error": {`                    `"message": "We could not parse the JSON body of your request. (HINT: This likely means you aren't using your HTTP library correctly. The OpenAI API expects a JSON payload, but what was sent was not valid JSON. If you have trouble figuring out how to fix this, please contact us through our help center at help.openai.com.)",`                    `"type": "invalid_request_error",`                    `"param": null,`                    `"code": null`                    `}`                    `}`                    The final version of the code we had, using the preceding libraries, was as follows:                    `package com.asb;`                    `import okhttp3.MediaType;`                    `import okhttp3.OkHttpClient;`                    `import okhttp3.Request;`                    `import okhttp3.RequestBody;`                    `import okhttp3.Response;`                    `public class ChatGPTApi {`                    `private static final String *API_KEY* = "sk-xxxxxxxxxxxxxxxxxxxxxxBlbkFJVAxxxxxxxxxxxxxxxxxx";`                    `private static final String *MODEL_ID* = "\"gpt-3.5-turbo\"";`                    `/*`                    ` * ASB Software Development Addition and URL change we know the following URL works:`                    ` *`                    ` * https://api.openai.com/v1/chat/completions -H "Authorization: Bearer sk-xxxxxxxxxxxxxxxxxxxxxxBlbkFJVAxxxxxxxxxxxxxxxxxx" -H "Content-Type: application/json" -d '{"model": "gpt-3.5-turbo", "messages": [{"role": "user", "content": "What is the OpenAI mission?"}] }'`                    ` *`                    ` */`                    `// Original private static final String API_URL = "https://api.openai.com/v1/engines/" + MODEL_ID + "/completions";`                    `// NEW private static final String API_URL =`                    `"https://api.openai.com/v1/chat/completions/";`                    `private static final String *API_URL* = "https://api.openai.com/v1/chat/completions";`                    `public static String getResponseFromGPT(String prompt) throws Exception {`                    `OkHttpClient client = new OkHttpClient().newBuilder().build();`                    `MediaType mediaType = MediaType.*parse*("application/json");`                    `// ASB Original line gave the error "message": "you must provide a model parameter",`                    `//RequestBody body = RequestBody.create(mediaType, "{  \"prompt\": \"" + prompt + "\",\"temperature\":0.7,\"max_tokens\":60}");`                    `RequestBody body = RequestBody.create(mediaType, "{  \"\"model\"\":  \"" + *MODEL_ID* + "\",\"messages\": [{\"role\": \"user\", \"content\":" + prompt + "\",\"temperature\":0.7,\"max_tokens\":60}");`                    `Request request = new Request.Builder()`                    `.url(*API_URL*)`                    `.method("POST", body)`                    `.addHeader("Authorization", " Bearer " + *API_KEY*)`                    `.addHeader("Content-Type", "application/json")`                    `.addHeader("messages", " [{\"role\": \"user\", \"content\": \"What is the OpenAI mission?\" }") //}]`                    `.build();`                    `System.*out*.print("Request=" + request.toString());`                    `Response response = client.newCall(request).execute();`                    `String responseJson = response.body().string();`                    `response.close();`                    `return responseJson;`                    `}`                    `public static void main(String[] args) throws Exception {`                    `String responseJson = *getResponseFromGPT*("Hello, how are you?");`                    `System.*out*.println(responseJson); // ASB for debug output`                    `}`                    `}`              Note    *The following link gives a more useful example:*    *[`www.infoworld.com/article/3697151/build-a-java-application-to-talk-to-chatgpt.html`](https://www.infoworld.com/article/3697151/build-a-java-application-to-talk-to-chatgpt.html)*    # Conclusion    The example Java code we received from ChatGPT in this Chapter illustrates the “churn” described in several articles on the code supported by the ChatGPT API.    We need to be aware that the model reference names are regularly changed by OpenAI and so the ChatGPT responses for the example API code given in responses are outdated very quickly.    However, even given this limitation, there are very useful responses to more stable requirements, such as the algorithms for Java code that we are using as examples in the rest of this book.    The aforementioned issues were still present, even after updating several imports for libraries. In the next chapter, we will look at the response obtained for our question on a Binary Search algorithm. We will see that the response from ChatGPT for this is much more useful.    # Points to Remember    *   To use the OpenAI API, you need an OpenAI API key, which can be obtained by signing up for an OpenAI account. This allows the creation of an API key to use the ChatGPT API. *   There is a free-to-download publication from ResearchGate (copyright ASB Software Development Limited), which can be used to install a free RedHat RHEL 8.x Linux operating system, including the supporting VMware virtual server running on an MS Windows operating system: https://doi.org/10.13140/RG.2.2.14590.95049 *   We had to use Version 3.2 of the okhttp.jar file eventually, as some features we needed were removed in the later versions. *   In Eclipse, we also found that we had to change the Eclipse project JVM from Java 17 to Java 11 to get the OkHttp system to run. *   The later okio jar file versions 3.4 and 3.5 do not work (we tried them) and also are much smaller than the 2.8 version. The kotlin-stdlib-1.3.41.jar is also required. (This can be found on the page: [`mvnrepository.com/artifact/org.jetbrains.kotlin/kotlin-stdlib-jdk7/1.3.41`](https://mvnrepository.com/artifact/org.jetbrains.kotlin/kotlin-stdlib-jdk7/1.3.41)).    # Multiple Choice Questions    1.  Which ChatGPT model can be used for sound file to text translation?     1.  text-davinci-003     2.  gpt-3.5-turbo     3.  whisper-1     4.  ChatML3 2.  Which supporting Java library is required for the I/O used by OkHttp?     1.  annotations-13.jar     2.  kotlin-reflect.jar     3.  okio-2.8.0.jar     4.  kotlin-stdlib.jar 3.  Which of the following are the current list of file extensions of sound files supported by Whisper?     1.  m4a, mp3, mp4, mpeg, mpga, wav, webm     2.  mtm, ec3, sf2, midi, mpga, wav, webm     3.  m4a, mp3, mp4, mpeg, mtm, ec3, sf2     4.  vpw, sds, dct, vag, mp4, mpeg, mtm 4.  What Linux command can be used to remove the space from a file name by renaming it?     1.  pwd     2.  cp     3.  ls     4.  mv 5.  Which of the following Java download sites did we use for the download of the ChatGPT java library files used in this Chapter?     1.  GitHub     2.  Maven Central Repository     3.  SourceForge     4.  JCenter    # Answers    1.  c 2.  c 3.  a 4.  d 5.  b    # Questions    1.  What are the main drawbacks to the use of ChatGPT to develop Java code for its own API interface? 2.  Why is it important to validate the responses from ChatGPT? What does the term Hallucination mean? 3.  Describe the steps you would use to validate the Java code generated from a ChatGPT response. 4.  What is the Kotlin plugin framework for Eclipse used for? What advantages are there in using this language in a Java project?    # Key Terms    *   HTTP: Hypertext Transfer Protocol (HTTP) is an internet communications protocol for use between a web browser or client program and a server to post and get data in standard formats (XML, HTML, and JSON), which can be interpreted by any system. *   Eclipse IDE: Eclipse is an integrated development environment (IDE) used in computer programming, which has been demonstrated for use with Java and Kotlin languages in this chapter. It contains a base workspace and an extensible plug-in system, which provides the Kotlin plugin, which we also showed how to install. *   HTML: Hypertext Markup Language. *   JSON: JavaScript Object Notation (JSON) is a standard nested text-based format, with tags similar to XML, but with curly bracket delimiters, rather than the angle brackets used for XML; both standards are used for representing structured data. *   JVM: Java Virtual Machine runs Java class files, which are then compiled into machine-specific Java JVM binary code, called bytecode, which the machine interprets, but can also be compiled for faster execution. *   Kotlin: Kotlin is a language, very similar to Java, which can be run with Java code, as it uses the same jar file structure. It is a high-level programming language, designed to interoperate fully with Java, and the JVM version of Kotlin's standard library depends on the Java Class Library. It is said to be around 40% more condensed in coding lines than Java and so more efficient. *   LLM: This stands for Large Language Model (LLM) used by ChatGPT and other AI systems to train their knowledge databases. They are nearly always huge data sets, often measured in petabytes used to generate and predict new content. *   REST API: A REST API, which is sometimes called a "RESTful" API, is a type of API (Application Programmers Interface) that posts commands from a program or web browser to an HTTP-based target web server, which is designed to process the data and return a result. REST stands for Representational State Transfer. The sent and returned data is usually structured into an XML or JSON message. We have covered the use of this, in the examples in this Chapter, for the ChatGPT AI API interface, which is REST based. *   URL: Uniform Resource Locator identifies a specific web server and usually a web page or a downloadable file or document and links to content online, which can be accessed from a browser or client program. *   XML: Extensible Markup Extensible (XML) is a markup language, with a very similar use as JSON, which is used for holding structured data. The angle brackets used for XML allow the structured data to be easily parsed to enable the extraction of subsets for further processing. XML is used for some older REST API services, but JSON is the most frequently used. ````` ```py```  ``````py```````py```````py```````py```````py```````py```````py```````py````` ```py```````py```````py```````py```````py```````py```````py```````py```````py # CHAPTER 4    # Java Program for Using Binary Search    # Introduction    In this chapter, we prompt ChatGPT for a Java program for using Binary Search. The Binary Search method takes a sorted array of integers and a target integer to search for. It returns the index of the target integer in the array if it is found, or -1 if it is not found. The method starts by initializing two variables, `left` and `right`, which represent the left and right boundaries of the search space. Initially, the search space is the entire array. The method then enters a loop that continues as long as the search space has not been exhausted.    # Structure    In this chapter, we will discuss the following topics:    *   AI prompt and response *   Java code validation using Eclipse Java code    # AI prompt and response    We first asked the Ask AI mobile ‘phone App, the following question and received the response (which is based on ChatGPT 3.5) as follows:    1.  Have you got a java code method for a program to use a binary search?          *“Sure! Here's an example Java code method for a binary search:”*                    ```` ```pyjava ````                    `public static int binarySearch(int[] array, int target) {`                    `int left = 0;`                    `int right = array.length - 1;`                    `while (left <= right) {`                    `int mid = left + (right - left) / 2;`                    `if (array[mid] == target) {`                    `return mid;`                    `} else if (array[mid] < target) {`                    `left = mid + 1;`                    `} else {`                    `right = mid - 1;`                    `}`                    `}`                    `return -1;`                    `}`              *“This method takes in an array of integers and a target integer to search for. It returns the index of the target integer in the array if it is found, or -1 if it is not found.*    *By*    *The method starts by initializing two variables, `left` and `right`, which represent the left and right boundaries of the search space. Initially, the search space is the entire array.*    *The method then enters a loop that continues as long as the search space has not been exhausted (i.e., `left <= right`). Inside the loop, it calculates the midpoint of the current search space using the formula `mid = left + (right - left) / 2`. It then compares the value at the midpoint of the array to the target value.*    *If the value at the midpoint is equal to the target, the method returns the index of the midpoint. If the value at the midpoint is less than the target, the method updates `left` to be `mid + 1`, effectively narrowing the search space to the right half of the current search space. If the value at the midpoint is greater than the target, the method updates `right` to be `mid - 1`, effectively narrowing the search space to the left half of the current search space.*    *If the method completes its loop without finding the target value, it returns -1 to indicate that the target value was not found in the array.”*    In the preceding example, ChatGPT 3.5, accessed through the Ask AI mobile ‘phone app, did not supply a main Java program method for testing the algorithm. When we asked the same question for the ChatGPT web application ([`chat.openai.com/`](https://chat.openai.com/) got the following code, which did include a main method, but the description was very much less detailed.  ![](img/practical-java-programming-with-chatgpt-Figure-4.1.jpg)  Figure 4.1: The Main java code is supplied here but with a shorter description    Note    *The actual code generated may very well change over time. As an example, I have emboldened some of the additions made from an earlier response given.*    `public class BinarySearch {`    `/`    ` * Binary search method to find the target element in a sorted array.`    ` *`    ` * @param arr The sorted array to search in.`    ` * @param target The element to search for.`    ` * @return The index of the target element if found; otherwise, -1.`    ` */`    `public static int binarySearch(int[] arr, int target) {`    `int left = 0;`    `int right = arr.length - 1;`    `while (left <= right) {`    `// If the middle element is the target, return its index`    `if (arr[mid] == target) {`    `return mid;`    `}`    `// If the target is in the left half, discard the right half`    `if (arr[mid] > target) {`    `right = mid - 1;`    `} else { // If the target is in the right half, discard the left half`    `left = mid + 1;`    `}`    `}`   ```py```````py```````py```````py`````` `// If the target is not found, return -1`    `return -1;`    `}`   ```py```````py```````py```````py````` `public static void main(String[] args) {`    `int[] arr = {2, 5, 8, 12, 16, 23, 38, 45, 56, 72, 91};`    `int target = 23;`   ```py```````py```````py```````py```` `int index = binarySearch(arr, target);`   ```py```````py```````py```````py``` `if (index != -1) {`    `System.out.println("Element found at index: " + index);`    `} else {`    `System.out.println("Element not found in the array.");`    `}`    `}`    `}`    我们可以向下滚动代码窗口以显示 ChatGPT AI 的描述，如下所示：    *在这个例子中，我们有一个已排序的数组 arr，我们使用 binarySearch 方法搜索目标元素。如果找到目标元素，该方法将返回其索引；否则，将返回 -1 表示数组中不存在该元素。提供的 main 方法演示了如何使用带有示例数组的 binarySearch 方法。*    # 使用 Eclipse Java 代码进行 Java 代码验证    为了完全验证二分查找算法，我们需要提供的一个要求是已排序的数组。因此，我们向 ChatGPT 网页应用程序（[`chat.openai.com`](https://chat.openai.com)) 提出了这个问题。这个问题及其回应如下：    您有使用 Java 程序将整数值数组按升序数字顺序排序的高效排序算法示例吗？    我们得到的回应如下：    “当然！一种高效的排序算法是快速排序算法。它是一种分治算法，通过选择一个‘枢轴’元素并将数组划分为两个子数组，一个包含小于枢轴的元素，另一个包含大于枢轴的元素。然后递归地对子数组进行排序。    以下是一个实现快速排序算法将整数值数组按升序数字顺序排序的 Java 程序：    `public class QuickSort {`    `public static void main(String[] args) {`    `int[] arr = { 9, 7, 5, 11, 12, 2, 14, 3, 10, 6 };`   ``````py```````py```````py`````` `System.out.println("Original array:");`    `printArray(arr);`   ```py```````py```````py```````py` `quickSort(arr, 0, arr.length - 1);`   ``````py```````py```````py```` `System.out.println("Sorted array:");`    `printArray(arr);`    `}`   ```py```````py```````py`````` `public static void quickSort(int[] arr, int low, int high) {`    `if (low < high) {`    `int pi = partition(arr, low, high);`   ```py```````py```````py````` `quickSort(arr, low, pi - 1);`    `quickSort(arr, pi + 1, high);`    `}`    `}`   ```py```````py```````py```` `public static int partition(int[] arr, int low, int high) {`    `int pivot = arr[high];`    `int i = (low - 1);`    `for (int j = low; j < high; j++) {`    `if (arr[j] < pivot) {`    `i++;`    `int temp = arr[i];`    `arr[i] = arr[j];`    `arr[j] = temp;`    `}`    `}`    `int temp = arr[i + 1];quickSort`   ```py```````py```````py``` `arr[i + 1] = arr[high];`    `arr[high] = temp;`   ``````py```````py`````` `return i + 1;`    `}`   ```py```````py```````py` `public static void printArray(int[] arr) {`    `for (int num : arr) {`    `System.out.print(num + " ");`    `}`    `System.out.println();`    `}`    `}`    `“`    In this program, the quickSort method is the main driver for the QuickSort algorithm, and the partition method is responsible for rearranging the elements around the pivot. The printArray method is just for displaying the array before and after sorting.    *Remember, while QuickSort is efficient on average, its performance can degrade in the worst-case scenario. Other sorting algorithms like MergeSort or TimSort might be better suited for scenarios where worst-case performance is a concern.”*  ![](img/practical-java-programming-with-chatgpt-Figure-4.2.jpg)  Figure 4.2: The ChatGPT response to our sort algorithm question    If we want to get the most efficient sort, we need to be able to check the other sort algorithms referenced by ChatGPT and also ask it for additional code to provide timings.    So, we asked the questions as follows:quickSort    Do you have an example of the MergeSort algorithm using a Java program to sort an array of integer values into ascending numeric order including code to measure the performance of the sort?    *Certainly! Here's an example of the MergeSort algorithm implemented in Java, along with code to measure the performance of the sort using the System.currentTimeMillis() method. MergeSort is a divide-and-conquer sorting algorithm that divides the unsorted list into smaller sublists until each sublist contains a single element. It then repeatedly merges these sublists to produce a sorted output.*    `import java.util.Arrays;`    `public class MergeSortExample {`   ``````py```````py```` `public static void merge(int[] arr, int left, int mid, int right) {`    `int n1 = mid - left + 1;`    `int n2 = right - mid;`   ```py```````py`````` `int[] leftArray = new int[n1];`    `int[] rightArray = new int[n2];`   ```py```````py````` `System.arraycopy(arr, left, leftArray, 0, n1);`    `System.arraycopy(arr, mid + 1, rightArray, 0, n2);`   ```py```````py```` `int i = 0, j = 0, k = left;`   ```py```````py``` `while (i < n1 && j < n2) {`    `if (leftArray[i] <= rightArray[j]) {`    `arr[k++] = leftArray[i++];`    `} else {`    `arr[k++] = rightArray[j++];`    `}`    `}`   ``````py`````` `while (i < n1) {`    `arr[k++] = leftArray[i++];`    `}`   ```py```````py` `while (j < n2) {`    `arr[k++] = rightArray[j++];`    `}`    `}`    `public static void mergeSort(int[] arr, int left, int right) {`    `if (left < right) {`    `int mid = left + (right - left) / 2;`   ``````py```` `mergeSort(arr, left, mid);`    `mergeSort(arr, mid + 1, right);`   ```py`````` `merge(arr, left, mid, right);`    `}`    `}`   ```py````` `public static void main(String[] args) {`    `int[] arr = {12, 11, 13, 5, 6, 7};`   ```py```` `System.out.println("Original array: " + Arrays.toString(arr));`   ```py``` `long startTime = System.currentTimeMillis();`    `mergeSort(arr, 0, arr.length - 1);`    `long endTime = System.currentTimeMillis();`   ````` `System.out.println("Sorted array: " + Arrays.toString(arr));`    `System.out.println("Time taken: " + (endTime - startTime) + " milliseconds");`    `}`    `}`    In this example, the merge method merges two sorted subarrays, and the mergeSort method divides the array into smaller parts recursively. The main method demonstrates how to use these methods to sort an array of integers and measure the time taken for the sorting process. Keep in mind that for more precise performance measurement, you might consider using System.nanoTime() instead of System.currentTimeMillis().  ![](img/practical-java-programming-with-chatgpt-Figure-4.3.jpg)  Figure 4.3: The ChatGPT response to the MergeSort question    We also posed a similar question for the TimSort algorithm, referenced in the first ChatGPT response:    Do you have an example of the TimSort algorithm using a Java program to sort an array of integer values into ascending numeric order including code to measure the performance of the sort?    Certainly! TimSort is a hybrid sorting algorithm derived from merge sort and insertion sort. It has been Python's standard sorting algorithm since version 2.3 and is also used in Java's Arrays.sort() and Collections.sort() methods. Here's an example of using TimSort to sort an array of integer values in Java, including code to measure the performance of the sort:    `*import java.util.Arrays;*`    `public class TimSortExample {`   ```py` `public static void main(String[] args) {`    `int[] arr = {12, 11, 13, 5, 6, 7};`   ``` `System.out.println("Original array: " + Arrays.toString(arr));`    `long startTime = System.currentTimeMillis();`    `Arrays.sort(arr);`    `long endTime = System.currentTimeMillis();`   `` `System.out.println("Sorted array: " + Arrays.toString(arr));`    `System.out.println("Time taken: " + (endTime - startTime) + " milliseconds");`    `}`    `}`    In this example, the Arrays.sort() method is used to perform the TimSort algorithm on the input array. The main method demonstrates how to use this method to sort an array of integers and measure the time taken for the sorting process. Keep in mind that for more precise performance measurement, you might consider using System.nanoTime() instead of System.currentTimeMillis().  ![](img/practical-java-programming-with-chatgpt-Figure-4.4.jpg)  Figure 4.4: The ChatGPT response to the TimSort question    You will notice that the last Java code array sorting example we obtained from ChatGPT was much more concise and also made use of the industry standard built-in method for sorting an array in Java.    This illustrates the importance of following up with further questions and also, that the ChatGPT AI does not necessarily give the best response first!    Now we can test each of the sort algorithms supplied by ChatGPT and validate the code supplied to sort the array we will use, using the Eclipse IDE (the installation for this is covered in the next chapter, Installation of the latest Open-Source Eclipse Java IDE).    So, first, we will test the first program given by ChatGPT, QuickSort, by creating a new Java project in the Eclipse IDE, QuickSortValidation_Chapter4 as illustrated in *Figure 4.5*:  ![](img/practical-java-programming-with-chatgpt-Figure-4.5.jpg)  Figure 4.5: The *ChatGPT* *QuickSortValidation_Chapter4* project is created in the *Eclipse IDE*    Clicking on the Next> button shows the basic src folder structure as shown in *Figure 4.6*:  ![](img/practical-java-programming-with-chatgpt-Figure-4.6.jpg)  Figure 4.6: The ChatGPT *QuickSortValidation_Chapter4* project folder structure is shown    On Clicking the Finish button in *Figure 4.6*, we can add a Java Class of QuickSort, with a package name of com.asb, as shown in *Figure 4.7*:  ![](img/practical-java-programming-with-chatgpt-Figure-4.7.jpg)  Figure 4.7: The *ChatGPT* *QuickSort* class is added under our *com.asb* package    On Clicking the Finish button in *Figure 4.7*, we get the “skeleton” java shown in *Figure 4.8*, which we can update by pasting in the QuickSort code given by ChatGPT:  ![](img/practical-java-programming-with-chatgpt-Figure-4.8.jpg)  Figure 4.8: The *QuickSort* skeleton code, created by the *IDE*, before pasting the *ChatGPT* code    The QuickSort code from ChatGPT is pasted into the Eclipse IDE as shown in *Figure 4.9*:  ![](img/practical-java-programming-with-chatgpt-Figure-4.9.jpg)  Figure 4.9: The ChatGPT    The QuickSort Java code pasted into the class as shown in *Figure 4.9* can be seen to compile with no syntax errors and is run as a Java application as shown in *Figure 4.10:*  ![](img/practical-java-programming-with-chatgpt-Figure-4.10.jpg)  Figure 4.10: The ChatGPT *QuickSort* example Java code is run in the *Eclipse IDE*    The code in *Figure 4.10* runs successfully, giving the output in *Figure 4.11*:  ![](img/practical-java-programming-with-chatgpt-Figure-4.11.jpg)  Figure 4.11: The ChatGPT *QuickSort* run output, showing the sorted array of integers    We can now repeat the above procedure from the creation of the QuickSort Class in *Figure 4.7*, for the MergeSort and TimSort classes.    We made just one small change to the code just to alter the class name from MergeSortExample to MergeSort as highlighted in *Figure 4.12*:  ![](img/practical-java-programming-with-chatgpt-Figure-4.12.jpg)  Figure 4.12: The ChatGPT *MergeSort* run output, showing the sorted array of integers    We also made a similar small change to the code just to alter the class name from TimSortExample to TimSort as shown in the highlighted run of the code in *Figure 4.13*:  ![](img/practical-java-programming-with-chatgpt-Figure-4.13.jpg)  Figure 4.13: The ChatGPT *TimSort* run output, showing the sorted array of integers    Just one more test was made to use the ChatGPT suggested change for the timings to `System.nanoTime()`    This gave the following result, as shown in *Figure 4.14*:  ![](img/practical-java-programming-with-chatgpt-Figure-4.14.jpg)  Figure 4.14: The results when the code was updated to use *System.nanoTime();*    This change to using System.nanoTime(); was repeated for the other two sort algorithms:  ![](img/practical-java-programming-with-chatgpt-Figure-4.15.jpg)  Figure 4.15: The results of the timing for the MergeSort is now in nanoseconds    So, the MergeSort on a short 6-element array is around 50 times faster than the TimSort.    There is one other small change that we made since the reported time differences should be named as nanoseconds. Also, it is worth repeating the runs several times to get an average. We also need to test with much larger arrays to compare the impact of larger data arrays on the timings.    For the QuickSort, we added the code for timing and got the output as follows:    `Original array:`    `9 7 5 11 12 2 14 3 10 6`    `Sorted array:`    `2 3 5 6 7 9 10 11 12 14`    `Time taken: 1829824 nanoseconds`    So, the MergeSort is over 100 times faster than the QuickSort.    But you may notice that there are 10 elements in the QuickSort test data, so we changed this to match the other two code examples, we got.    `Original array:`    `12 11 13 5 6 7`    `Sorted array:`    `5 6 7 11 12 13`    `Time taken: 1739028 nanoseconds`    So, it is faster but still over 100 times slower than the MergeSort.    So, on the tests we tried, the fastest algorithm is the MergeSort, it is also the longest algorithm at 60 lines, next fastest is the TimSort, although around 50 times slower than the MergeSort, it is the shortest in code length at 21 lines of code. The originally suggested QuickSort code is the slowest and uses around 50 lines of code.    # Conclusion    In this chapter, we have covered the algorithm created by ChatGPT for the Binary Search java method. We compared the different codes created by the web-based ChatGPT with the Ask AI version. We asked additional questions for sorting an array as the input for the Binary Search algorithm and discovered that the first response from ChatGPT isn’t always the best response.    In *Chapter 5, Installation of the latest Open-Source Eclipse Java IDE*, we introduce the latest available version of the Eclipse Java IDE (Eclipse IDE 2023-06 R - Eclipse IDE for Java Developers), which is downloaded and we describe the step-by-step installation on MS Windows 10 and RedHat Enterprise Linux, RHEL 8.x.    # Points to remember    *   The actual code generated by ChatGPT may very well change over time. *   It is important to follow up with further questions since ChatGPT AI does not necessarily give the best response first! *   It is recommended to test each of the algorithms supplied by ChatGPT and validate the code supplied and its efficiency.    # Multiple choice questions    1.  Which sort algorithm takes the fewest lines of code?     1.  QuickSort     2.  MergeSort     3.  TimSort     4.  partition 2.  Which sort algorithm is the most efficient?     1.  QuickSort     2.  MergeSort     3.  TimSort     4.  partition 3.  In the example QuickSort program given by ChatGPT which method is responsible for rearranging the elements around the pivot?     1.  The quickSort method     2.  The partition method     3.  The printArray method     4.  The main method    # Answers    1.  c 2.  b 3.  b    # Questions    1.  Which algorithm would you use to presort an integer array for the Binary Search program we are testing? 2.  How would you validate that the algorithm you have chosen is the best one to use? 3.  What question would you ask ChatGPT to establish that you were using the fastest sort algorithm? (You could try this and see what response you get from the AI).    # Key terms    *   AI: Artificial Intelligence Software that mimics the responses you might expect to questions supplied by a human operator. *   OpenAI: is the American artificial intelligence research laboratory that developed ChatGPT comprising the non-profit OpenAI organization and its for-profit subsidiary corporation OpenAI Limited. *   Ask AI: The Android mobile phone app is available for access to ChatGPT 3.5. *   ChatGPT: ChatGPT is a language model developed by OpenAI. It is based on the GPT (Generative Pre-trained Transformer) architecture, specifically GPT-3.5 for the free use option. The model is designed to generate human-like text responses to user inputs, making it capable of engaging in interactive and natural-sounding conversations. `` ```py ```` ```py`` ``````py ``````py` ``````py`` ``````py``` ``````py```` ```py```````py` ``````py`````` ```py```````py``` ``````py```````py` ``````py```````py`` ``````py```````py``` ``````py```````py```` ```py```````py```````py` ``````py```````py`````` ```py```````py```````py``` ``````py```````py```````py` ``````py```````py```````py`` ``````py```````py```````py``` ``````py```````py```````py```` ```py```````py```````py```````py` ``````py```````py```````py`````` ```py```````py```````py```````py``` ``````py```````py```````py```````py` ``````py```````py```````py```````py`` ``````py```````py```````py```````py```  ``````py```````py```````py```````py```````py```````py```````py```````py``` ``````py```````py```````py```````py```````py```````py```````py```````py`` # CHAPTER 5    # Installation of the Latest Open-source Eclipse Java IDE    # Introduction    In this chapter, we introduce the latest available version of the Eclipse Java IDE (Eclipse IDE 2023-06 R - Eclipse IDE for Java Developers), which is then downloaded. We subsequently describe the step-by-step installation process on MS Windows 10 and RedHat Enterprise Linux (RHEL 8.x).    # Structure    In this chapter, we will discuss the following topics:    *   Downloading the Eclipse Java IDE *   Eclipse IDE validation of the Binary Search code     *   Perplexity *   Creating the Java BinarySearch project *   Running the Eclipse Java program *   Binary Search validation Java Program output    # Downloading the Eclipse Java IDE    The latest available version of the Eclipse Java IDE was downloaded (at the time of writing in June 2023) from the Eclipse organization webpage as follows:    [`www.eclipse.org/downloads/`](https://www.eclipse.org/downloads/)    Click on the Download x86_64 button on the home webpage, as shown in *Figure 5.1*, to open the webpage link for the eclipse-inst-jre-win64.exe Windows installation program, as shown in *Figure 5.2*.  ![](img/practical-java-programming-with-chatgpt-Figure5.1.jpg)  Figure 5.1: The *Download x86_64* button on the home page is selected    As shown in *Figure 5.2*, the eclipse-inst-jre-win64.exe Windows installation program is now available by clicking the Download button. The mirror site is randomly selected, for example, Germany – dogado GmbH based on our location in the European zone. However, if needed, you can choose another server by clicking the Select Another Mirror link and selecting from the list as follows:    Europe    Germany: dogado GmbH    Czech Republic: UPC Ceska republika, a.s.    Russian Federation: Tomsk State Pedagogical University    Germany: University of Applied Sciences Esslingen    Sweden: Academic Computer Club, Umea University    France: CNRS IBCP    Germany: University of Erlangen-Nuremberg    Germany: RWTH Aachen University    Italy: Consortium GARR    Netherlands: SNT, University of Twente    Turkey: Linux Kullanicilari Dernegi    North America    Canada: Rafal Rzeczkowski    United States: Jevin Canders    United States: Clarkson University Open Source Institute    Canada: University of Waterloo Computer Science Club    United States: University of Maryland    United States: XMission Internet    United States: OSU Open Source Lab    Asia    Republic of Korea: Kakao Corp.    China: Dalian Neusoft University of Information (大连东软信息学院)    Cyprus: University of Cyprus, Library    Japan: Japan Advanced Institute of Science and Technology    Japan: Yamagata University    Japan: Yamagata University    China: eScience Center, Nanjing University    Australia/Oceania    Australia: Australian Academic Research Network    South America    Brazil: C3SL - Federal University of Parana  ![](img/practical-java-programming-with-chatgpt-Figure5.2.jpg)  Figure 5.2: Click the Download button to get an eclipse-inst-jre-win64.exe Windows version    The progress of the 123 Mbyte download can be viewed in the browser’s status bar window, as shown in *Figure 5.3*.  ![](img/practical-java-programming-with-chatgpt-Figure5.3.jpg)  Figure 5.3: The progress of the 123 Mbyte download can be viewed    For Linux installs, we can use the following link as a starting point:    [`www.eclipse.org/downloads/packages/`](https://www.eclipse.org/downloads/packages/)    This displays the following webpage, as illustrated in *Figure 5.4*.  ![](img/practical-java-programming-with-chatgpt-Figure5.4.jpg)  Figure 5.4: The highlighted *Linux x86_64* is selected to download for our *RHEL 8.x* server    The Linux tar and gzipped Eclipse file, eclipse-java-2023-06-R-linux-gtk-x86_64.tar.gz file, is obtained by clicking on the highlighted Download button, as shown in *Figure 5.5*.  ![](img/practical-java-programming-with-chatgpt-Figure5.5.jpg)  Figure 5.5: The Linux file, *eclipse-java-2023-06-R-linux-gtk-x86_64.tar.gz*, is downloaded    We can check the progress of the 326 Mbyte download in the browser’s status window, as shown in *Figure 5.6*.  ![](img/practical-java-programming-with-chatgpt-Figure5.6.jpg)  Figure 5.6: The progress of the 326 Mbyte download can be viewed    The downloaded eclipse-java-2023-06-R-linux-gtk-x86_64.tar.gz file is copied from the mapped Windows Installs directory area to our VMware RedHat Linux RHEL 8 server and then unpacked, as shown in *Figure 5.7*.  ![](img/practical-java-programming-with-chatgpt-Figure5.7.jpg)  Figure 5.7: The downloaded *eclipse-java-2023-06-R-linux-gtk-x86_64.tar.gz* file is extracted    We have created an eclipse directory under the /root folder of the root users and then copied and unpacked the Eclipse IDE program using the following commands:    `mkdir eclipse`    `cp /mnt/hgfs/Installs/eclipse-java-2023-06-R-linux-gtk-x86_64.tar.gz .`    `tar -zxvf eclipse-java-2023-06-R-linux-gtk-x86_64.tar.gz`    The eclipse program can now be launched from the unpacked /root/eclipse/eclipse folder by using the command ./eclipse, as shown in *Figure 5.8*.  ![](img/practical-java-programming-with-chatgpt-Figure5.8.jpg)  Figure 5.8: The eclipse program is launched from */root/eclipse/eclipse* using *./eclipse*    The splash screen of the Eclipse program is displayed on the launch of the program, showing the version and the load progress status bar, as shown in *Figure 5.9*.  ![](img/practical-java-programming-with-chatgpt-Figure5.9.jpg)  Figure 5.9: The Eclipse 2023-06 version splash screen    The Launch button is clicked (we use the default Eclipse workspace directory area), as shown in *Figure 5.10*.  ![](img/practical-java-programming-with-chatgpt-Figure5.10.jpg)  Figure 5.10: The *Eclipse* program *Launch* button is clicked (using the default workspace area)    Finally, the Welcome page is displayed for the launched Eclipse IDE program, as illustrated in *Figure 5.11*.  ![](img/practical-java-programming-with-chatgpt-Figure5.11.jpg)  Figure 5.11: The Welcome page is displayed for the launched Eclipse IDE program    # Eclipse IDE validation of the Binary Search code    In the previous *Chapter 4, Java Program for using Binary Search*, we were shown several versions of the Java code for implementing a Binary Search algorithm. In addition, we looked, in-depth, into numerous supporting program code snippets to provide the sorted array of integer values required as input for the Binary Search Java code examples we found.    In this section, we will explore another front-end client application for the ChatGPT AI, which provides some additional features that were missing in the previous Ask AI Android mobile phone app demonstrated earlier in the book.    # Perplexity    There is another mobile phone app available for free to use in its default mode, which has even more useful features than the Ask AI we have been using.    There is a comparison site that lists several AI application options, as follows:    [`sourceforge.net/software/product/Perplexity-AI/alternatives`](https://sourceforge.net/software/product/Perplexity-AI/alternatives)    Although this link is informative, its comparison tables, as shown in *Figure 5.12*, were out of date for Perplexity, as it has no tick box for an Android mobile phone app or Apple iPad support (which, as of 12th August 2023, we will demonstrate is fully supported).    There was a review of Perplexity on 31st March 2023 at the following link, entitled    “*How to use Perplexity, the only iPhone ChatGPT app that matters (bgr.com)”*:    [`bgr.com/entertainment/how-to-use-perplexity-the-only-iphone-chatgpt-app-that-matters/`](https://bgr.com/entertainment/how-to-use-perplexity-the-only-iphone-chatgpt-app-that-matters/)    However, things have obviously changed since the March release of Perplexity. The article states:    “*The best part of Perplexity AI is that, unlike the ChatGPT clients for iPhone or the ChatGPT web experience, you don’t need to set up an account. Perplexity AI will work as soon as you load it in a browser or install the iPhone app.* *But Perplexity will not offer other ChatGPT features. It won’t write code or essays for you.”*    The first statement is true: the Perplexity App from the Apple store is free and doesn’t require an Open AI account. The last point in the statement is demonstrably not true, at least when using the current release of Perplexity, as we will show in this section of the chapter.  ![](img/practical-java-programming-with-chatgpt-Figure5.12.jpg)  Figure 5.12: The SourceForge website (12/08/2023) comparison table for *Perplexity*    Perplexity AI was established in August 2022 by a group of AI software engineers: Denis Yarats, Aravind Srinivas, Johnny Ho, and Andy Konwinski.    The Perplexity app now runs on iPhone, Android, and iPad and has a search interface powered by OpenAI's GPT 3.5 and Microsoft Bing, which answers user questions (and currently uses GPT 4).    Perplexity is very fast and has very useful features, which are not currently available from the Ask AI App. It displays the internet search sources for all of its responses. In addition, it has a Copilot mode option, which provides additional clarification and summarizes search results.    Another really useful feature is that each resource is flagged as a subscript number in the descriptive text that is displayed under the code that is produced.    The iPad version of Perplexity can be installed by searching in the Apple store to show the following screen, as illustrated in *Figure 5.13*.  ![](img/practical-java-programming-with-chatgpt-Figure5.13.jpg)  Figure 5.13: The *Perplexity App* for download in the *Apple* store for the *iPad*    Upon selecting the Get button on the iPad, as shown in *Figure 5.13*, we get the pop-up window, as shown in *Figure 5.14*.  ![](img/practical-java-programming-with-chatgpt-Figure5.14.jpg)  Figure 5.14: The *Touch ID* or a password for the *Apple* store can be entered with the keyboard    The sign-in is prompted for the Apple ID email password to allow the Perplexity App to be installed, as shown in *Figure 5.15*.  ![](img/practical-java-programming-with-chatgpt-Figure5.15.jpg)  Figure 5.15: The sign-in is prompted for the *Apple ID* email password    We then proceed to download Perplexity and receive a prompt to launch the App, with a choice of authentication mechanisms, through a Google account, an existing Apple account, or another email address, as illustrated by *Figure 5.16*.  ![](img/practical-java-programming-with-chatgpt-Figure5.16.jpg)  Figure 5.16: The *Continue with email* option is selected    The email address (redacted) is entered, as shown in *Figure 5.17.*  ![](img/practical-java-programming-with-chatgpt-Figure5.17.jpg)  Figure 5.17: The email address is entered to launch the *Perplexity AI App* prompt screen    We entered the question, which was originally posed to Ask AI and also to the Open AI ChatGPT web application, on the newly installed Perplexity App on the iPad, as shown in *Figure 5.18.*  ![](img/practical-java-programming-with-chatgpt-Figure5.18.jpg)  Figure 5.18: The question, on the example for a *Binary Search*, posed to the *Perplexity App* on the *iPad*    The Perplexity AI App provides not only the standard features of the OpenAI ChatGPT in its response page but also provides, as is illustrated in *Figure 5.19*, the list of further resource links available  ![](img/practical-java-programming-with-chatgpt-Figure5.19.jpg)  Figure 5.19: The list of resources available is shown in the AI response on scrolling down    Clicking on the +2 more button, as shown on the right-hand side in *Figure 5.19*, we get a list of sources and their details in the pop-up window, as shown in *Figure 5.20.*  ![](img/practical-java-programming-with-chatgpt-Figure5.20.jpg)  Figure 5.20: The list of links to further details on the *Binary Search* algorithm on the internet    The links, displayed in *Figure 5.20*, can be followed as expanded below:    1.  Binary Search in Java – Javatpoint:          [`www.javatpoint.com/binary-search-in-java`](https://www.javatpoint.com/binary-search-in-java)           2.  Binary Search Algorithm in Java – Implementation & Examples – Software Testing Help:          [`www.softwaretestinghelp.com/binary-search-in-java/`](https://www.softwaretestinghelp.com/binary-search-in-java/)           3.  Binary Search in Java – GeeksforGeeks:          [`www.geeksforgeeks.org/binary-search-in-java/`](https://www.geeksforgeeks.org/binary-search-in-java/)           4.  Java Program to Implement Binary Search Algorithm – Programiz:          [`www.programiz.com/java-programming/examples/binary-search`](https://www.programiz.com/java-programming/examples/binary-search)           5.  What is Binary Search in Java? How to Implement it? – Edureka:          [`www.edureka.co/blog/binary-search-in-java/`](https://www.edureka.co/blog/binary-search-in-java/)           6.  Binary Search in Java – Algorithm Example – freeCodeCamp:          [`www.freecodecamp.org/news/binary-search-in-java-algorithm-example/`](https://www.freecodecamp.org/news/binary-search-in-java-algorithm-example/)              On importing the code created by Perplexity, we can run it as shown in *Figure 5.21*.  ![](img/practical-java-programming-with-chatgpt-Figure5.21.jpg)  Figure 5.21: The Binary Search algorithm is initially validated    In the next section, we will show how the installed Eclipse IDE was used to create this initial Binary Search program validation, as shown in *Figure 5.21*, using a step-by-step procedure.    # Creating the Java BinarySearch class  ![](img/practical-java-programming-with-chatgpt-Figure5.22.jpg)  Figure 5.22: The existing *com.asb* package is right-clicked for the *New-> Class* menu    The BinarySearch class is created under the com.asb package after entering the class name, as shown in *Figure 5.23*.  ![](img/practical-java-programming-with-chatgpt-Figure5.23.jpg)  Figure 5.23: The *BinarySearch* Java Class is created by selecting the *Finish* button    # Running the Eclipse Java Program    After pasting the code copied from the Perplexity App into the Eclipse Java IDE, we need to test run the application, as shown in *Figure 5.24*. The result of this test is shown in *Figure 5.21*: (*The Binary Search algorithm is initially validated*)  ![](img/practical-java-programming-with-chatgpt-Figure5.24.jpg)  Figure 5.24: The initial run of the *BinarySearch* validation program    # Binary Search Validation Java Program Output    We can provide improvements to the initial output of the BinarySearch program. First, you will notice that the original array had just 5 elements:    `int[] arr = {1, 2, 3, 4, 5};`    The element value to be searched is set in the next line of the main program:    `int key = 3;`    You might be surprised that the program’s output is given as:    Element found at index 2:    In the Java language, you have to remember that array elements are indexed with the first array element with an index starting from zero.    We asked the additional question using the Perplexity AI App to see if it can provide additional Java code to supply a more challenging example for testing to augment our MergeSort code, which can then be used to feed the BinarySearch for a more robust validation:    Have you an example of a Java program which will populate an integer array with numbers obtained from a random function generator?    This provided the following Java code example  ![](img/practical-java-programming-with-chatgpt-Figure5.25.jpg)  Figure 5.25: The *RandomArray* class Java code that we asked from Perplexity    The text of the Java code generated by Perplexity, as shown in *Figure 5.25*, is displayed as follows:    `package com.asb;`    `import java.util.Random;`    `public class RandomArray {`    `public static void main(String[] args) {`    `int[] arr = new int[10];`    `Random rand = new Random();`    `for (int i = 0; i < arr.length; i++) {`    `arr[i] = rand.nextInt(100); // generate random integer between 0 and 99`    `}`    `// print the array`    `for (int i = 0; i < arr.length; i++) {`    `System.*out*.print(arr[i] + " ");`    `}`    `}`    `}`    The additional code was then manually updated from the original BinarySearch code as follows:    *   The RandomArray code was incorporated into the BinarySearch main program to generate the test array to be sorted using a new BinarySearchValidation class. *   The MergeSort code was called to sort the array created by the RandomArray code. *   The original BinarySearch function was called from the BinarySearch main program.          `package com.asb;`                    `import java.util.Arrays;`                    `import java.util.Random; //ASB New Import from the RandomArray code example`                    `import com.asb.MergeSort; //ASB New Import from the MergeSort class created in Chapter 4`                    `public class BinarySearchValidatiion {`                    `// public class BinarySearch { //ASB Original Class name changed: 13-08-2023`                    `public static int binarySearchValidation(int[] arr, int key) { //ASB method changed 13-08-2023`                    `int low = 0;`                    `int high = arr.length - 1;`                    `while (low <= high) {`                    `int mid = low + (high - low) / 2;`                    `if (arr[mid] == key) {`                    `return mid; // ASB We return here if the key is found`                    `} else if (arr[mid] < key) {`                    `low = mid + 1;`                    `} else {`                    `high = mid - 1;`                    `}`                    `}`                    `return -1;`                    `}`                    `public static void main(String[] args) {`                    `// int[] arr = {1, 2, 3, 4, 5};`                    `// int key = 3; //ASB see below, We want to ensure we find one of the actual elements`                    `// ASB -New Code added from Perplexity to populate a test array, start time and sort it`                    `long startTime = System.*nanoTime*(); //ASB We log the start time`                    `int[] arr = new int[10];`                    `Random rand = new Random();`                    `for (int i = 0; i < arr.length; i++) {`                    `arr[i] = rand.nextInt(100); // generate random integer between 0 and 99`                    `}`                    `// print the array`                    `int key = 0; //ASB We set the key starting at zero,`                    `//then we use the last Randomly generated element for the key`                    `for (int i = 0; i < arr.length; i++) {`                    `System.*out*.print(arr[i] + " ");`                    `key = arr[i]; //ASB this should give us the randomly selected last element`                    `//as the key to be searched`                    `}`                    `//ASB Now we use the MergeSort we created earlier in Chapter 4`                    `System.*out*.println("Original array: " + Arrays.*toString*(arr));`                    `System.*out*.println("Search key: " + Integer.*toString*(key)); //ASB we also print the key to be found`                    `MergeSort.*mergeSort*(arr, 0, arr.length - 1);`                    `System.*out*.println("Sorted array: " + Arrays.*toString*(arr));`                    `// ASB -New Code End`                    `int result = *binarySearchValidation*(arr, key); //ASB Original method name changed 13-08-2023`                    `long endTime = System.*nanoTime*(); //ASB We log the end time`                    `System.*out*.println("Time taken: " + (endTime - startTime) + " nanoseconds"); //ASB Changed to nanoseconds from milliseconds`                    `if (result == -1) {`                    `System.*out*.println("Element not found");`                    `} else {`                    `System.*out*.println("Element found at index " + result);`                    `}`                    `}`                    `}`              Now each run will give a different test data set, the first run results were as follows:    First run:    `28 97 40 16 44 97 76 55 89 16 Original array: [28, 97, 40, 16, 44, 97, 76, 55, 89, 16]`    `Search key: 16`    `Sorted array: [16, 16, 28, 40, 44, 55, 76, 89, 97, 97]`    `Time taken: 4188251 nanoseconds`    `Element found at index 1`    Note that in the first run, we have located the second value of the sorted array element (which is still correct as 16).    Second run:    `87 68 89 90 12 86 92 99 88 75 Original array: [87, 68, 89, 90, 12, 86, 92, 99, 88, 75]`    `Search key: 75`    `Sorted array: [12, 68, 75, 86, 87, 88, 89, 90, 92, 99]`    `Time taken: 3934707 nanoseconds`    `Element found at index 2`    This time there are no duplicate values in the randomly generated array, the index value correctly locates the Search key of 75.    # Conclusion    In this chapter, we have demonstrated the download of the currently available Eclipse IDE and then used this to validate the BinarySearch algorithm. We have also introduced the Perplexity AI App, which can be run on an Android mobile phone or an Apple iPad.    In the next chapter, we will cover the use of ChatGPT to assist us to create Java code for the Fourier analysis of a sine wave.    # Points to Remember    *   There are several ChatGPT-based client Applications, and the platforms they run on are being extended so quickly that reference comparison sites such as SourceForge cannot keep pace. *   The Perplexity AI App has the additional feature of listing the website sources it uses for its responses and the links to their web pages. *   In the Java programming language, array elements are numbered starting from zero. *   We can combine the code snippets supplied by ChatGPT to provide additional functionality.    # Multiple Choice Questions    1.  Which of the following Mirror sites would be the most appropriate for downloading Eclipse for a user based in North America?     1.  Consortium GARR     2.  Jevin Canders     3.  Yamagata University     4.  C3SL - Federal University of Parana 2.  Which of the following commands is used to unpack the Eclipse installation file on a Linux system?     1.  cp /mnt/hgfs/Installs/eclipse-java-2023-06-R-linux-gtk-x86_64.tar.gz .     2.  tar -zxvf eclipse-java-2023-06-R-linux-gtk-x86_64.tar.gz     3.  ./eclipse     4.  mkdir eclipse 3.  The SourceForge website (12/08/2023) comparison table for Perplexity shows support for which one of the following platform lists?     1.  Mac, Linux, iPhone, iPad     2.  SaaS/Web, iPhone, iPad, Android     3.  iPhone, SaaS/Web     4.  SaaS/Web, iPhone, iPad 4.  In the final version of the BinarySearchValidation program, which of the following Java methods is used for presorting the array to be searched?     1.  QuickSort     2.  RandomArray     3.  TimSort     4.  MergeSort    # Answers    1.  b 2.  b 3.  a 4.  d    # Questions    1.  List the current advantages of Perplexity AI over Ask AI. 2.  How could you modify the final version of the example BinarySearch Validation Java program to try processing 10 different arrays in a single run of the program?          *(Hint: this can be achieved by adding just two additional lines of Java code).*           3.  Explain why the program output is given as "Element found at index 2:" When the Key number found is the third element of the array.    # Key Terms    *   *Apple:* Short for Apple Computer company, established on April 1, 1976, by Steve Jobs and Steve Wozniak. They developed the Apple Mac desktop computer and then other company products were produced including the iPhone and iPad. *   *iPad:* The brand name for a small tablet computer made by Apple with a touch-sensitive screen and built-in Wi-Fi connectivity, usually with just one USB port. *   *Mirror:* Mirror sites or mirrors are replicas of a master website. The idea of a Mirror site is to provide a fast, geographically local server for a country network. It supplies HTTP and/or FTP services with different URL links while providing the same content for download. *   *MergeSort:* Merge sort is a "divide-and-conquer" algorithm that was invented by John von Neumann in 1945\. In the worst-case scenario, merge sort uses approximately 39% fewer comparisons than quicksort. *   *Perplexity:* It is a mobile phone app, free to use in its default mode, which has even more useful features than the Ask AI mobile phone app. The Perplexity AI was established in August 2022 by a group of AI software engineers: Denis Yarats, Aravind Srinivas, Johnny Ho, and Andy Konwinski. The Perplexity App now runs on iPhone, Android, and iPad and has a search interface powered by OpenAI's GPT 3.5 and Microsoft Bing, which answers user questions (currently using GPT 4). Perplexity also has a Copilot mode. *   *QuickSort:* Quicksort is a general-purpose sorting algorithm developed by Tony Hoare in the UK in 1959 and published in 1961. *   *RandomArray:* This method is used in this chapter to randomly assign a range of integer numbers to an array of integer elements, after which the array is sorted as input for the Binary Search example code we developed in this chapter. *   *TimSort:* TimSort is a stable sorting algorithm, derived from merge sort and insertion sort. It was first implemented by Tim Peters in 2002 for use in the Python programming language. (Hence, the name!)    # CHAPTER 6    # ChatGPT Generated Java Code for Fourier Analysis    # Introduction    Performing Fourier analysis on an MP4 music file to separate instruments and vocals is a complex task. It involves multiple steps like decoding the MP4 file, performing signal processing, and applying source separation techniques. ChatGPT provided an outline guide for the steps required and suggested some libraries for each step.    We did eventually manage to successfully split an MP3 music file using a Java program to call a python library routine called Spleeter. Unfortunately, the Java code provided by ChatGPT was incorrect, although it was helpful in its suggestion to use Spleeter.    Also, the MP4 format is mainly used for video files (although there is an MP4 to MP3 convertor at [`cloudconvert.com/mp4-to-mp3`](https://cloudconvert.com/mp4-to-mp3) ) ChatGPT did not flag this as an issue.    A simpler task, which ChatGPT did provide the full working code for, was for the Fourier analysis of a sine wave using Java code and through Microsoft Bing webchat, a graphical display program (this is using the OpenAI GPT-4.5).    # Structure    In this chapter, we will discuss the following topics:    *   MP4 Fourier Analysis Java Code     *   MP4 Fourier Analysis Java Code – according to OpenAI ChatGPT *   Fourier Analysis for MP4 java code validation using an Eclipse Java Program Project *   ChatGPT generated Java code for Fourier Analysis of a Sine wave *   Sine wave Fourier Analysis Java code validation using an Eclipse Java    # MP4 Fourier Analysis Java Code    Is there java code for the Fourier analysis of an MP4 music file to separate the instruments and vocals?    (This was according to Ask AI)    Performing Fourier analysis on an MP4 music file to separate instruments and vocals is a complex task. It involves multiple steps like decoding the MP4 file, performing signal processing, and applying source separation techniques. While I can't give you a full Java code solution, I can guide you through the steps and suggest some libraries for each step.    1.  Decode the MP4 file: To read and decode MP4 music files, you can use a Java library like Xuggler *(*[`www.xuggle.com/xuggler/`](http://www.xuggle.com/xuggler/) *).* 2.  Perform Fourier analysis: Once you have the audio data, you can perform Fourier analysis on it. For this, you can use the Fast Fourier Transform (FFT) algorithm provided by the JTransforms library *(*[`github.com/wendykierp/JTransforms`](https://github.com/wendykierp/JTransforms) *).* 3.  Separate instruments and vocals: This is the most challenging part. Separating instruments and vocals typically involves source separation techniques, such as Non-negative Matrix Factorization (NMF) or deep learning methods like U-Net. There may not be readily available Java libraries for this step, and you may need to implement the algorithms yourself based on research papers or use other programming languages with available libraries, like Python.          Here's a high-level outline of how the code might look like:                    ```` ```pyjava ````                    `import com.xuggle.mediatool.IMediaReader;`                    `import com.xuggle.mediatool.IMediaWriter;`                    `import com.xuggle.mediatool.ToolFactory;`                    `import com.xuggle.mediatool.event.IAudioSamplesEvent;`                    `import com.xuggle.mediatool.event.IVideoPictureEvent;`                    `import com.xuggle.xuggler.IContainer;`                    `// … other imports …`                    `public class MusicFileAnalyzer {`                    `public static void main(String[] args) {`                    `// Step 1: Decode MP4 file`                    `IMediaReader mediaReader = ToolFactory.makeReader("input.mp4");`                    `mediaReader.addListener(new AudioSampleListener());`                    `while (mediaReader.readPacket() == null) {`                    `// continue reading the file`                    `}`                    `// Step 2: Perform Fourier analysis using JTransforms`                    `// Step 3: Separate instruments and vocals using source separation techniques`                    `}`                    `}`                    `class AudioSampleListener extends MediaListenerAdapter {`                    `@Override`                    `public void onAudioSamples(IAudioSamplesEvent event) {`                    `// Process audio samples here`                    `}`                    `}`                    ```py` ``` ```py`              *Keep in mind that separating instruments and vocals can be challenging and may not produce perfect results. If you're open to using Python, there are more advanced libraries like Spleeter ([`github.com/deezer/spleeter`](https://github.com/deezer/spleeter)) that can help you achieve better source separation results.*    The suggestion in bold from the AI proved to be the best (and simplest) advice given by ChatGPT.    # MP4 Fourier Analysis Java Code – according to OpenAI ChatGPT    Next, we tried Perplexity, since the skeleton Java code given by Ask AI was often just a list of comments, and it responded as follows:  ![](img/practical-java-programming-with-chatgpt-Figure6.1.jpg)  Figure 6.1: The Perplexity App on the iPad gives us it’s advice on the question    We then opened up the second, related thread supplied by Perplexity, which gave the response as shown in *Figure 6.2*:  ![](img/practical-java-programming-with-chatgpt-Figure6.2.jpg)  Figure 6.2: The *Perplexity App* on the *iPad* still does not provide any code    So, we tried the third thread as shown in *Figure 6.3*:  ![](img/practical-java-programming-with-chatgpt-Figure6.3.jpg)  Figure 6.3: The *Perplexity App* on the *iPad* provides interesting links, but still no code    We were a little disappointed that the Ask AI and Perplexity Apps didn’t provide us with the full Java code, so we tried the OpenAI web application at [`chat.openai.com/`](https://chat.openai.com/) as shown in *Figure 6.4*:  ![](img/practical-java-programming-with-chatgpt-Figure6.4.jpg)  Figure 6.4: The OpenAI web application at [`chat.openai.com/response`](https://chat.openai.com/response)    The full response from OpenAI is shown here:    Performing Fourier analysis on an MP4 music file to separate instruments and vocals is a complex task that typically involves more than just basic Java code. It involves digital signal processing techniques, machine learning, and potentially deep learning approaches. Here's a high-level overview of the steps you might take, but keep in mind that this is a very advanced topic that requires a deep understanding of signal processing, audio processing, and programming skills beyond basic Java.    1.  Load and Decode the Audio: You'll need to extract the audio data from the MP4 file. This can be done using libraries like JavaZoom's JLayer or the Java Sound API. 2.  Preprocessing: Perform any necessary preprocessing steps, such as resampling the audio to a common sample rate or converting it to mono if necessary. 3.  Short-Time Fourier Transform (STFT): The STFT is a technique to analyze the frequency content of a signal over time. You'll apply the STFT to your audio signal to convert it into a time-frequency representation. 4.  Spectral Source Separation: This is the heart of the process. There are different methods you can use, including:     1.  Non-negative Matrix Factorization (NMF): NMF can be used to factorize the spectrogram into basis components (instruments/vocals) and their corresponding activations.     2.  Deep Learning Models: Using deep learning models like convolutional neural networks (CNNs) or recurrent neural networks (RNNs) trained on source separation tasks. 5.  Reconstruction: Once you've separated the different sources (instruments and vocals), you need to reconstruct the audio signals from the processed spectrogram data. This involves an inverse STFT process. 6.  Post-processing: Clean up any artifacts or imperfections introduced during separation and reconstruction.    Here's a very simplified example of how you might use the Java Sound API and JTransforms library to perform STFT:    ```` ```pyjava ````    `import javax.sound.sampled.*;`    `import org.jtransforms.fft.FloatFFT_2D;`   ```py```````py```````py```````py```````py```````py```````py```````py``` `public class AudioAnalysis {`    `public static void main(String[] args) {`    `try {`    `AudioInputStream audioInputStream = AudioSystem.getAudioInputStream(new File("input.mp4"));`    `AudioFormat format = audioInputStream.getFormat();`   ``````py```````py```````py```````py```````py```````py```````py`````` `// Read and process audio data in chunks`    `int chunkSize = 2048; // Adjust as needed`    `byte[] audioData = new byte[chunkSize];`   ```py```````py```````py```````py```````py```````py```````py```````py` `FloatFFT_2D fft = new FloatFFT_2D(chunkSize, 1);`   ``````py```````py```````py```````py```````py```````py```````py```` `// Process each chunk of audio data`    `while (audioInputStream.read(audioData) != -1) {`    `float[] audioSamples = convertBytesToFloats(audioData);`   ```py```````py```````py```````py```````py```````py```````py`````` `// Apply FFT`    `float[] spectrum = new float[2 * chunkSize];`    `System.arraycopy(audioSamples, 0, spectrum, 0, chunkSize);`    `fft.realForwardFull(spectrum);`   ```py```````py```````py```````py```````py```````py```````py````` `// Process the spectrum data (e.g., separate sources)`   ```py```````py```````py```````py```````py```````py```````py```` `// Inverse FFT to reconstruct audio`    `fft.realInverseFull(spectrum, true);`   ```py```````py```````py```````py```````py```````py```````py``` `// Process the reconstructed audio (e.g., post-processing)`    `}`   ``````py```````py```````py```````py```````py```````py`````` `audioInputStream.close();`    `} catch (Exception e) {`    `e.printStackTrace();`    `}`    `}`   ```py```````py```````py```````py```````py```````py```````py` `private static float[] convertBytesToFloats(byte[] bytes) {`    `float[] floats = new float[bytes.length / 2];`    `for (int i = 0; i < floats.length; i++) {`    `floats[i] = (float) ((bytes[2 * i] & 0xFF) | (bytes[2 * i + 1] << 8));`    `}`    `return floats;`    `}`    `}`    Please note that this example is extremely simplified and doesn't perform any actual source separation or reconstruction. Real-world source separation requires sophisticated algorithms and often deep learning models.    For a more practical and robust solution, you might want to explore existing libraries and tools specialized in audio source separation, such as Spleeter by Deezer, which is a pre-trained model for separating vocals and accompaniments in music recordings. This can be used through Python, and you can potentially integrate it with your Java application using appropriate interfacing methods like calling Python scripts from Java.    So, again the Java code only achieves the “skeleton” of a working program. Optimistically, we then asked:    Can ChatGPT input an MP4 music file and separate the instruments and vocals?    Which was responded with:    “No, ChatGPT cannot directly process or analyze audio or video files, including MP4 music files. It's a text-based language model and doesn't have the capability to handle audio or video data directly. Separating instruments and vocals from an audio file requires complex signal processing and machine learning techniques that are beyond the capabilities of a text-based model like ChatGPT.    To perform audio source separation tasks like separating instruments and vocals from an MP4 music file, you would need to use specialized tools, libraries, and software designed for audio processing and source separation. These tools often involve a combination of digital signal processing methods and machine learning algorithms. Libraries like Spleeter, as mentioned earlier, are examples of tools that can perform this kind of audio source separation.    Keep in mind that these tasks are quite advanced and might require some expertise in audio processing and programming to achieve meaningful results.”    We have highlighted the text above since it does indicate that ChatGPT has some memory of the previous responses it gave.    So, we tried a different approach, which did appear to be more promising. We asked:    Do you have example java code to call the Spleeter python libraries for source separation of an MP4 audio file?    On posing this question, we do get some Java code, as shown in *Figure 6.5*:  ![](img/practical-java-programming-with-chatgpt-Figure6.5.jpg)  Figure 6.5: The *OpenAI* web application gives us some Java code we can use at last    This gave a full example of a method to achieve our original goal of separating the vocals from the instruments, though not directly using Fourier Analysis:    Certainly, you can use Java to call Python code using the `ProcessBuilder` class to execute a Python script. Here's an example of how you might call the Spleeter Python library from a Java program to perform audio source separation on an MP4 audio file:    1.  Install Spleeter:          Before proceeding, make sure you have installed Spleeter. You can install it using the following command in your terminal:                    ```` ```py ````                    `pip install spleeter`                    ```py` ``` ```py`           2.  Create a Java class:          Create a Java class that calls a Python script. For simplicity, let's assume you have a Python script named `spleeter_separate.py` that performs the source separation using Spleeter. This script takes the input audio file path and output directory as command-line arguments.                    Here's an example of how you might structure your Java class:                    ```````pyjava````                    `import java.io.BufferedReader;`                    `import java.io.IOException;`                    `import java.io.InputStreamReader;`                    `public class SpleeterCaller {`                    `public static void main(String[] args) {`                    `try {`                    `String pythonScriptPath = "path/to/spleeter_separate.py"; // Replace with actual path`                    `String inputFile = "path/to/input.mp4"; // Replace with actual input file path`                    `String outputDirectory = "path/to/output/"; // Replace with desired output directory`           ```py```````py `// 构造执行 Python 脚本的命令`    `String[] command = {"python", pythonScriptPath, inputFile, outputDirectory};`   ``````py``` `ProcessBuilder processBuilder = new ProcessBuilder(command);`    `processBuilder.redirectErrorStream(true);`   ``````py`` `Process process = processBuilder.start();`   ``````py` `// Read the output of the Python script`    `BufferedReader reader = new BufferedReader(new InputStreamReader(process.getInputStream()));`    `String line;`    `while ((line = reader.readLine()) != null) {`    `System.out.println(line);`    `}`   ``````py `// 等待进程完成`    `int exitCode = process.waitFor();`    `System.out.println("Python script exited with code: " + exitCode);`   ````` `} catch (IOException | InterruptedException e) {`    `e.printStackTrace();`    `}`    `}`    `}`    ```py` ``` ```py` ````` ```py``` ``````py` ``````py`` ``````py``` ``````py````  ```py``` ````` *   *Python 脚本 (`spleeter_separate.py`):*          ``创建一个名为 `spleeter_separate.py` 的 Python 脚本，使用 Spleeter 库执行音频源分离。以下是该脚本的简化示例：``                    ```py` ```*python* ```py`                    `*import sys*`                    `*from spleeter.separator import Separator*`                    `*def main():*`                    `*if len(sys.argv) != 4:*`                    `*print("Usage: python spleeter_separate.py input_audio output_directory")*`                    `*return*`                    `*input_audio = sys.argv[1]*`                    `*output_directory = sys.argv[2]*`                    `*separator = Separator('spleeter:2stems') # Use desired separation model*`                    `*separator.separate_to_file(input_audio, output_directory)*`                    `*if __name__ == "__main__":*`                    `*main()*`                    ```` ```py ```` ```py`` ``````py    ``````py```````py```````py```````py```````py```````py```` ```py```````py```````py```````py```````py```````py`````` 请记住，根据您想要分离的源数量，将 `'spleeter:2stems'` 替换为适当的分离模型。您可以在 [官方 Spleeter 文档] ([`github.com/deezer/spleeter`](https://github.com/deezer/spleeter) ) 中找到有关 Spleeter 及其可用模型的更多信息。    请注意，此示例演示了从 Java 调用 Python 脚本以使用 Spleeter 执行源分离的基本过程。您可能需要根据您的具体用例调整代码，并更稳健地处理错误情况。此外，请确保您的 Java 和 Python 环境都已正确配置。    # 使用 Eclipse Java 程序项目验证 MP4 的傅里叶分析 Java 代码    因此，我们有几个独立的 Java 程序需要验证，包括对 python 库的 Java 调用。    首先，按照 ChatGPT 的建议，我们安装了 Spleeter python 库，它引用为：    1.  安装 Spleeter:          我们使用了如下命令：                    `pip install Spleeter`              我们后来注意到，大写的“S”似乎没有引起问题（我们应该使用小写“s”的 spleeter）。    第一次尝试给出了：    `bash: pip: command not found…`    因此，我们意识到必须首先在我们的 RHEL 8.8 Linux 服务器上使用 Python pip 安装程序，这实际上被引用为 pip2 或 pip3，因为主要版本可以在 RHEL Linux 上共存。因此，可以使用其中任何一个，如下所示：    `[root@ECMUKDEMO22 eclipse]# pip3 --version`    `pip 9.0.3 from /usr/lib/python3.6/site-packages (python 3.6)`    `[root@ECMUKDEMO22 eclipse]# pip2 --version`    `pip 9.0.3 from /usr/lib/python2.7/site-packages (python 2.7)`    `[root@ECMUKDEMO22 eclipse]#`    然后我们使用了：    `pip3 install Spleeter`    这给出了一个错误，指示缺少一个名为 tensorflow 2.5.0 的依赖项，如 *图 6.6* 所示：  ![](img/practical-java-programming-with-chatgpt-Figure6.6.jpg)  图 6.6： 第一次尝试使用 pip3 安装时出现关于 *tensorflow 2.5.0* 的错误    因此，我们首先安装它，使用：    `pip3 install tensorflow`    但是，这最终也给出了错误：    ``您在 RHEL/Fedora 上，尚未运行 `yum install python3-devel` 或``    `` `dnf install python3-devel`（确保您也安装了 redhat-rpm-config） ``    因此，我们再次重复，使用：    `yum install redhat-rpm-config`  ![](img/practical-java-programming-with-chatgpt-Figure6.7.jpg)  图 6.7： 安装了 *redhat-rpm-config*    然后我们需要按照建议安装 python3-devel 包：    `yum install python3-devel`    `python3-devel` 库的安装成功，如 *图 6.8* 所示：  ![](img/practical-java-programming-with-chatgpt-Figure6.8.jpg)  图 6.8： 安装了 `python3-devel` 库    现在我们尝试安装缺失的 tensorflow 包库，如 *图 6.9* 所示。    `pip3 install tensorflow`  ![](img/practical-java-programming-with-chatgpt-Figure6.9.jpg)  图 6.9： 使用 `pip3 install tensorflow` 命令并安装了库    这也安装了 `tensorflow-2.5.0`，如 *图 6.10* 所示：  ![](img/practical-java-programming-with-chatgpt-Figure6.10.jpg)  图 6.10： 安装了 `tensorflow-2.5.0` 库    我们还需要运行 pip3 升级：    （这里有一个链接有帮助；[`qiita.com/palao/items/699f4148249481c64ad7`](https://qiita.com/palao/items/699f4148249481c64ad7) 尽管描述语言是日语！命令仍然可以遵循，因为它们是标准的 Linux 命令。）    `cd /usr/local/lib64/python3.6/site-packages`    `pip3 install --upgrade pip`    然后我们尝试运行 Spleeter 的安装，注意这里我们使用小写的 spleeter 名称。    `pip3 install spleeter`    然后，我们使用命令行过程获取一个测试 MP3 文件，如日语链接中所述，以尝试该包。    `wget https://github.com/deezer/spleeter/raw/master/audio_example.mp3`    接下来，我们还安装了以下库，如日语博客中所建议的：    `pip3 install -U urllib3`    这些安装如 *图 6.11* 所示，命令已高亮：  ![](img/practical-java-programming-with-chatgpt-Figure6.11.jpg)  图 6.11： 下载了 audio_example.mp3 文件作为测试输入并安装了 `urllib3`    然后，我们尝试从 Linux 命令窗口运行 spleeter 命令：    `spleeter separate -p spleeter:2stems -o output audio_example.mp3`    首先，我们得到了错误：    `[root@ECMUKDEMO22 site-packages]# spleeter separate -p spleeter:2stems -o output audio_example.mp3`    `ERROR:spleeter:ffmpeg binary not found`    在 Google 中搜索该错误，我们从链接中获得了一个推荐：[`computingforgeeks.com/how-to-install-ffmpeg-on-centos-rhel-8/`](https://computingforgeeks.com/how-to-install-ffmpeg-on-centos-rhel-8/)    我们需要运行以下命令：    `dnf -y install https://download.fedoraproject.org/pub/epel/epel-release-latest-8.noarch.rpm`    因此，向上滚动日语博客，我也找到了这个的安装方法：    `dnf install http://rpmfind.net/linux/epel/7/x86_64/Packages/s/SDL2-2.0.14-2.el7.x86_64.rpm`  ![](img/practical-java-programming-with-chatgpt-Figure6.12.jpg)  图 6.12： 我们需要安装 *EPEL* 包以支持 *Spleeter python* 程序    我们运行以下命令来安装推荐的 CRB 存储库，如 *图 6.12* 所推荐。    `subscription-manager repos --enable codeready-builder-for-rhel-8-x86_64-rpms`    该存储库按预期启用，如 *图 6.13* 所示：  ![](img/practical-java-programming-with-chatgpt-Figure6.13.jpg)  图 6.13： 我们安装了推荐的 CRB 存储库    现在我们需要更新订阅 rpm 包文件，使用以下命令：    `dnf install -y https://download1.rpmfusion.org/nonfree/el/rpmfusion-nonfree-release-8.noarch.rpm`    在安装过程中，我们被提示导入两个 GPG 安全密钥，如 *图 6.14* 所示    （GPG 安全密钥用于公钥/私钥加密，以确保数据以加密格式安全传输）。  ![](img/practical-java-programming-with-chatgpt-Figure6.14.jpg)  图 6.14： 我们确认使用两个 *GPG* 安全密钥，使用高亮行    运行此 rpm 包安装的输出如 *图 6.15* 所示：  ![](img/practical-java-programming-with-chatgpt-Figure6.15.jpg)  图 6.15： 我们更新了订阅 rpm 包文件，如上高亮    然后我们运行推荐的 ffmpeg 和 ffmpeg-devel 包安装，如 *图 6.16* 所示：    `yum install ffmpeg ffmpeg-devel`  ![](img/practical-java-programming-with-chatgpt-Figure6.16.jpg)  图 6.16： 我们使用 `yum install ffmpeg ffmpeg-devel` 安装了 29 个包库    我们需要的已安装 ffmpeg 包显示成功安装，如 *图 6.17* 所示：  ![](img/practical-java-programming-with-chatgpt-Figure6.17.jpg)  图 6.17： 我们需要的已安装 *ffmpeg* 包显示成功安装    现在安装正常，因此我们重试命令，如 *图 6.18* 所示：    `spleeter separate -p spleeter:2stems -o output audio_example.mp3`  ![](img/practical-java-programming-with-chatgpt-Figure6.18.jpg)  图 6.18： `spleeter separate -p spleeter:2stems -o output audio_example.mp3` 命令    现在运行没有任何错误，如 *图 6.18* 所示。    请注意，该程序使用了一个训练模型，它会下载该模型，如 ChatGPT 所示。    因此，最终我们取得了有效的结果，但我们必须付出大量额外的努力才能实现这一结果，而且我们不需要 Java 程序来完成它。    两个分割文件输出为 accompaniment.wav 和 vocals.wav，通过聆听原始的 audio_example.mp3 文件和输出的分割文件，可以听到原始声音的惊人分离（播放的 .wav 文件列在 *图 6.19* 中）。  ![](img/practical-java-programming-with-chatgpt-Figure6.19.jpg)  图 6.19： 两个分割文件输出为 `accompaniment.wav` 和 `vocals.wav.`    然而，我们确实想要验证我们要求 ChatGPT 提供的 Java 程序，因此我们使用 Eclipse IDE 在 com.asb Java 包下创建了一个新类 SpleeterCaller，如 *图 6.20* 所示：  ![](img/practical-java-programming-with-chatgpt-Figure6.20.jpg)  图 6.20： 在 com.asb 包下创建了 SpleeterCaller Java 类    首先，按照建议，我们创建了 spleeter_separate.py python 脚本文件，如 *图 6.21* 所示：  ![](img/practical-java-programming-with-chatgpt-Figure6.21.jpg)  图 6.21： `spleeter_separate.py` python 脚本文件    在粘贴了 ChatGPT 建议的代码后，我们保存了类文件 `SpleeterCaller.java`，并运行了应用程序主 Java 类，如 *图 6.22* 所示：  ![](img/practical-java-programming-with-chatgpt-Figure6.22.jpg)  图 6.22： 运行了 SpleeterCaller.java 主 Java 类应用程序    起初，我们遇到了与 python 相关的错误，我们尝试通过使用 yum install python39 命令升级到最新的 python 版本 3.9 来修复，如 *图 6.23* 所示：  ![](img/practical-java-programming-with-chatgpt-Figure6.23.jpg)  图 6.23： 我们尝试使用 `yum install python39` 命令升级到最新的 Python 版本 3.9    我们最终发现 ChatGPT 给出的代码存在许多问题。最重要的问题是 ChatGPT 给出的命令行代码定义为 Java String 数组，这不起作用（至少对于用于启动 spleeter 程序 python 脚本的 ProcessBuilder 类而言）。第二个问题是对 python 脚本的调用，我们意识到这根本不需要，因为 spleeter 调用可以直接在命令行上进行。    因此，我们更新了代码，我们的第一次尝试按预期运行，如下所示，如 *图 6.24* 所示：  ![](img/practical-java-programming-with-chatgpt-Figure6.24.jpg)  图 6.24： 第一次成功从 *Java* 代码程序运行 spleeter 程序    文件按预期分割，但是，在一个带有空格的奇怪目录路径中，如 *图 6.25* 所示。  ![](img/practical-java-programming-with-chatgpt-Figure6.25.jpg)  图 6.25： 创建了两个 wav 输出文件，但位于意外的子文件夹路径中    代码已更新，如 *图 6.26* 中高亮所示，并重新运行程序：  ![](img/practical-java-programming-with-chatgpt-Figure6.26.jpg)  图 6.26： 程序重新运行，现在在预期路径中创建分割文件    现在可以在预期路径中看到输出文件，如 *图 6.27* 所示：  ![](img/practical-java-programming-with-chatgpt-Figure6.27.jpg)  图 6.27： 输出文件现在按预期出现在预期路径中    我们更新的最终工作代码现在如 *图 6.26* 所示，列出如下：
