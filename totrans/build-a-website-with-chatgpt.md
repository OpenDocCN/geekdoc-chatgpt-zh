![Manning_copyright](img/build-a-website-with-chatgpt-Manning_copyright.png)

# 使用 ChatGPT 构建网站

Paul McFedries

要评论请访问 [liveBook](https://livebook.manning.com/#!/book/build-a-website-with-chatgpt/discussion)

![Manning_M_small](img/build-a-website-with-chatgpt-Manning_M_small.png)

Manning

Shelter Island

更多关于此书和其他 Manning 书籍的信息，请访问

[www.manning.com](https://www.manning.com/)

# 版权

对于这些书籍以及其他 Manning 书籍的在线信息和订购，请访问 [www.manning.com](https://www.manning.com/)。当批量订购时，出版商提供折扣。

更多信息，请联系

特别销售部

Manning 出版公司

20 Baldwin Road

PO Box 761

Shelter Island, NY 11964

电子邮件：orders@manning.com

©2024 by Manning 出版公司。保留所有权利。

本出版物任何部分不得以任何形式或通过电子、机械、影印或其他方式复制、存储在检索系统中或传输，除非事先获得出版商的书面许可。

许多制造商和销售商使用的标识以区分其产品，均被声明为商标。在这些标识出现在书中，且 Manning 出版公司知道有商标声明的情况下，这些标识已用大写字母或全部大写字母印刷。

♾ 认识到保护已撰写内容的重要性，Manning 的政策是将其出版的书籍印刷在无酸纸上，并为此付出最大努力。同时，认识到我们也有责任保护地球资源，Manning 的书籍至少使用 15% 的回收纸，并且在不使用元素氯的情况下进行处理。

| ![Manning_M_small](img/build-a-website-with-chatgpt-Manning_M_small.png)     | Manning 出版公司 20 Baldwin Road 技术部 PO Box 761 Shelter Island, NY 11964 |
| --- | --- |
| 开发编辑：   | Karen Miller |
| 技术编辑：   | Anirudh Prabhu |
| 审稿编辑：   | Kishor Rit |
| 制作编辑：   | Kathy Rossland |
| 文案编辑：   | Tiffany Taylor |
| 校对：   | Keri Hales |
| 技术校对：   | Adam London |
| 排版编辑：   | Tamara Švelić Sabljić |
| 封面设计师：   | Monica Kamsvaag |

ISBN: 9781633436961

# 献词

致 Karen 和 Chase，我最喜欢的聊天伙伴

# 目录

前言部分

前言

致谢

关于本书

关于作者

1    介绍使用 ChatGPT 创建网站

1.1    什么是 ChatGPT？

1.2    ChatGPT 使任何人都能创建网页

1.3    了解您可以（和不能）创建的页面类型

1.4    使用 ChatGPT 帮助您构建网页

提示 ChatGPT

查看 ChatGPT 的结果

将代码放入文件中

部署 HTML 文件

根据需要重复

精炼和修改你的提示

2     创建和部署你的第一个网页

2.1   理解过程

2.2   提示 ChatGPT 生成你的网页代码

检查结果

检查一些单页网站的其它提示

2.3   复制 ChatGPT 的网页代码

将网页代码保存到 HTML 文件中

2.4   在浏览器中测试你的网页

2.5   部署你的网页

3     处理字体、颜色和标题

3.1   预览本章的项目

3.2   构建个人主页

获取网站标题和副标题建议

设计字体样式

设置字体大小

处理字体样式

从 ChatGPT 获取字体建议

生成配色方案

理解网页标题

制作提示

3.3   检查个人主页代码

检查 HTML

检查 CSS

3.4   自定义个人主页

4     向页面添加结构

4.1   理解本章的项目

4.2   构建读书俱乐部页面

介绍页面标题

介绍页面页脚

介绍填充、边框和边距

处理图片

添加社交媒体链接

制作提示

4.3   检查代码

检查 HTML

检查 CSS

4.4   自定义页面

5     发布页面帖子

5.1   理解本章的项目

5.2   构建在线日志页面

处理可折叠面板

使用 GPT-4 和 DALL-E 生成图像

制作提示

5.3   检查代码

检查 HTML

检查 CSS

5.4   自定义页面

6    添加链接和导航

6.1   理解本章的项目

6.2   构建信息网站主页

创建链接

创建导航栏

制作主页提示

6.3   检查主页代码

检查 HTML

检查 CSS

6.4   自定义主页

6.5   构建其他网站页面的提示

7    创建网站内容

7.1   理解本章的项目

7.2   使用 ChatGPT 生成和编辑文本

让 ChatGPT 建议写作想法

为如何撰写一个主题的想法生成

为研究一个主题获取 ChatGPT 的帮助

让 ChatGPT 用你自己的声音写作

重写帖子文本

不要忘记 HTML 标签

7.3   构建主页

处理英雄图像

制作主页提示

7.4   检查主页代码

检查 HTML

检查 CSS

自定义主页

7.5   构建其他网站页面的提示

8    生成网站表单

8.1   查看本章的项目

8.2   获取发送给你的表单数据

设置 Getform 账户

创建 Getform 端点

8.3   构建表单

指定表单的端点

使用文本框收集文本

为每个控件添加标签

使用文本区域处理更多文本

使用复选框获取是或否信息

使用单选按钮选择几个选项之一

使用列表提供更多选择

使用按钮提交表单

8.4   制作活动注册页面的提示

8.5   检查活动注册页面代码

检查 HTML

检查 CSS

8.6   自定义活动注册页面

9   向您的页面添加列表

9.1   查看本章的项目

9.2   构建项目符号列表

处理较长的列表项

嵌套项目符号列表

更改项目符号类型

9.3   构建编号列表

反转列表顺序

更改列表的起始编号

嵌套编号列表

更改编号样式

9.4   制作食谱页面提示

9.5   检查食谱页面代码

检查 HTML

检查 CSS

9.6   自定义食谱页面

10   设置照片画廊

10.1   查看本章的项目

10.2   更详细地查看图像

查看<img>标签

添加占位符图像

与图像缩略图一起工作

添加图像标题

10.3   实现相册覆盖层

10.4   相册：由 JavaScript 驱动

10.5   使用 Flexbox 布局画廊

10.6   制作照片画廊的提示

10.7   检查照片画廊代码

检查 HTML

检查 CSS

检查 JavaScript

10.8   自定义照片画廊

11   创建作品集页面

11.1   了解本章的项目

11.2   构建作品集页面

构建卡片

使图像延伸到卡片边缘

添加阴影

圆角

使您的页面响应式

11.3    制作投资组合页面的提示

11.4    检查投资组合页面代码

检查 HTML

检查 CSS

11.5    自定义投资组合页面

12    构建文章页面

12.1    了解本章的项目

12.2    构建文章页面

审查 HTML 页面布局元素

使用文章元素

在页面上包含侧边栏

向文章添加新部分

向文章、部分或 aside 添加新段落

标记特殊单词和短语

在文章开头使用首字母下沉

使用 CSS Grid 布局文章

调整文章页面布局以适应小屏幕

12.3    向页面添加内容

12.4    检查文章页面代码

检查 HTML

检查 CSS

12.5    自定义文章页面

13    编写交互式课程目录

13.1    检查本章的项目

13.2    从 Excel 获取数据

准备您的 Excel 数据

了解 JSON 数据格式

将您的 Excel 文件上传到 ChatGPT

提示 ChatGPT 将您的 Excel 数据转换为 JSON

13.3    获取并显示 JSON 数据

13.4    搜索、排序和过滤课程目录

搜索数据

过滤数据

对数据进行排序

13.5    制作课程目录的提示

13.6    检查课程目录代码

检查 HTML

检查 CSS

检查 JavaScript

13.7    自定义课程目录

13.8    从这里开始

附录 A.    准备使用 ChatGPT 构建网页

附录 B.    部署您的网站

附录 C. 学习几个 ChatGPT 最佳实践

索引

# 前言

## 前言

“哦，勇敢的新世界，它有这样的人！”这句话出自威廉·莎士比亚的戏剧《暴风雨》，是孩子米兰达第一次遇到一群人时说的。你可能作为一个孩子并没有被流放到遥远的岛屿，但当你第一次遇到任何当前的人工智能（AI）应用程序时，你可能会发现自己正在重复米兰达的话。这确实是一个勇敢的新世界，它有这样的人工智能聊天机器人。

像 ChatGPT 这样的工具一开始看起来很神奇，因为它们似乎很擅长将词语组合起来。要求 ChatGPT“写一首莎士比亚风格的十四行诗，总结科马克·麦卡锡的小说《路》的情节”，它会照做。不，产生的诗歌不会是莎士比亚级别的，但它*确实*会很有趣。但过了一段时间，这种廉价的娱乐就会变得乏味，大多数 ChatGPT 用户发现自己会问一个类似的问题：“ChatGPT*真正*有什么用？”

这通常是一个难以回答的问题，只有一个例外：代码。ChatGPT 真正有用，可以将文本指令转换为编程代码。特别是，ChatGPT 擅长将文本转换为构建网页所需的代码。这是非凡的，这意味着现在*任何人*都可以在网络上建立自己的存在，即使他们不想或不能学习网络开发的复杂性。

然而，这种新颖的上网方式有几个陷阱。首先，是的，ChatGPT 非常擅长将文本转换为网页代码，但前提是你知道如何用详细的指令来制定这个文本，以便 ChatGPT 遵循。其次，即使 ChatGPT 已经成功生成了构建网页所需的全部代码，你仍然需要将这段代码保存到某个地方，然后以某种方式将其放到网络上。

这些可能看起来像是难以跨越的障碍，但这就是这本书的作用所在。在接下来的章节中，你不仅会学到如何像专业人士一样指导 ChatGPT，以获得你想要的网页，还会学到如何保存这些代码，然后将它们部署到网络上，让全世界都能看到。那么，欢迎来到一个勇敢的新世界，在那里你可以借助 ChatGPT 建立自己的网站。

## 致谢

美国散文家和诗人 E. B. White 曾将编辑描述为“一个比作家更懂写作的人，但他已经摆脱了那种可怕的写作欲望。”我相信这是真的，不仅因为 E. B. White 是一个智者，而且因为我已经习惯于依赖我的编辑，让我看起来比实际写得更好！

我相信小说和回忆录等书籍的编辑们手头的工作已经非常繁重，需要将稿件整理得井井有条，但请为那些可怜的计算机书籍编辑们留下一刻。他们必须确保计算机书籍读起来流畅，不会出现拼写错误和语法错误，同时还要确保书籍的技术准确性。为什么？因为即使是作者（或编辑）的微小失误也可能导致一本引起困惑和不安而不是确定和喜悦的书籍。

曼宁出版公司的同事们确保每本书都读起来流畅且内容准确，他们通过让每一份稿件接受一系列的审阅来做到这一点，审阅者不仅包括编辑专业人士，还包括一支专门的第三方团队。在只有一个或几个读者审阅稿件的过程中，曼宁的书籍则由数十人仔细审查。结果如何？你正在阅读的这本书包含了准确且相关的信息，这些信息已经通过了业界一些最敏锐的眼耳的检验。是的，封面上的名字可能只有我一个，但许多人都在创造书页内容方面发挥了重要作用（无论是实体书还是虚拟书）。这些审阅者包括 Adam Wan、Andres Sacco、Andriani Stylianou、Ashwin Mhatre、Beardsley Ruml、Bruno Sonnino、Charles Lam、Drew Leon、Erim Ertürk、Ganesh Falak、Halil Karakose、James Coates、Jeff Smith、José Alberto Reyes Quevedo、Julien Pohie、Lars Pesch、Marvin Schwarze、Matteo Battista、Mikhail Karaashev、Ozren Harlovic、Radhakrishna MV、Ranjit Sahai、Rui Liu、Saravanan Muniraj、Steve Prior、Swapneelkumar Deshpande 和 Tony Holdroyd。

感谢技术编辑 Anirudh Prabhu，他是一位经验丰富的用户界面开发者，拥有超过十年的行业经验。他的职业生涯中充满了值得注意的成就，包括出版了四本备受赞誉的书籍。此外，他还担任了多家知名出版社各种书籍的技术审稿人，并通过为 HTML、CSS 和 jQuery 创建全面的培训材料，在塑造 Web 开发未来方面发挥了积极作用。

我还要向出版人 Marjan Bace、采购编辑 Brian Sawyer、开发编辑 Karen Miller、项目协调员 Malena Selić、校对编辑 Tiffany Taylor 以及所有帮助本书成形的曼宁出版社的其他制作人员表示衷心的感谢。

最后，我还要感谢所有抽出时间审阅本书早期稿件并提出评论和建议的人们。你们的宝贵意见非常受重视。

## 关于本书

在这本书中，你将学习如何指导 ChatGPT 生成必要的网页代码，以便按照你的要求部署页面。不需要具备 ChatGPT 或网页开发的经验。你需要知道的一切都会在你需要时提供，你不会在这些页面上找到任何冗长的技术讨论或哲学争论。我的目标是帮助你借助 ChatGPT 的力量上网，本书中的所有内容都是为了实现这个目标。如果你曾经想要建立一个网页，但无法或不想学习如何编码，这本书将帮助你通过 ChatGPT 的强大助力实现这一目标。

我假设你除了电脑屏幕之外还有自己的生活，因此这本书的编排方式是让你不必从头到尾阅读。如果你是刚开始，请阅读第一章以获得坚实的基础，然后尝试第二章中的简单项目，以获得一个真正的 ChatGPT 生成的网页页面。从那里开始，你可以按任何顺序尝试第三章至第十二章中的任何项目。为了便于查找，章节“本书的组织结构：路线图”为你提供了本书 13 章（以及 3 个附录）的概述。

### 适合阅读这本书的人

这本书首先针对的是任何想要在网络上建立存在感的人，无论这种存在感是一个谦逊的个人主页，一个展示爱好或兴趣的页面，还是书友会、活动、组织或团队的网站。更具体地说，我将这本书的目标读者定位为以下三种类型：

+   *不知道如何编码网页且不想学习的人*——网页开发的细节长期以来一直是许多人建立网络存在感的障碍。这本书旨在展示 ChatGPT 如何为那些对学习如何编码不感兴趣的人改变这一切。

+   *不知道如何编码网页但想学习的人*——这本书主要关注你必须提供给 ChatGPT 的指令，以便它生成你想要的网页代码。然而，我也提供了本书中使用的每种网页代码技术的背景信息。将这种背景知识与本书的项目实践方法相结合，你将学到很多关于网页开发的知识。

+   *知道如何编码网页的人*——即使你已经掌握了至少网页开发的基础知识，你也可以使用 ChatGPT 来加速你的开发工作，并将一些更繁琐的任务委托给 ChatGPT。本书将向你展示你可以使用的提示，以诱导 ChatGPT 成为你的编程助手。

### 本书组织结构：路线图

*第一章*介绍了 ChatGPT 的一般知识，以及如何使用 ChatGPT 生成网页代码。你将了解在 ChatGPT 的帮助下可以构建哪些类型的页面，并得到一个关于整个过程的概览。

*第二章* 带你通过 ChatGPT 创建和部署你的第一个网页。你将学习如何提示 ChatGPT 生成代码、复制该代码并将其保存到文件中。然后，你在网页浏览器中测试代码，并将其免费部署到网络上。

*第三章* 介绍了如何提示 ChatGPT 在网页上使用字体、颜色和标题。你将学习如何请求 ChatGPT 为你的网站标题和标语、使用的字体以及要应用的配色方案提供建议。然后，你将这些内容整合到一个提示中，请求 ChatGPT 生成个人主页的代码。

*第四章* 专注于网页结构，因此你将了解标题、页脚、填充、边框和边距。你还学习如何将图像和社交媒体链接添加到页面中。章节的最终目标是提示 ChatGPT 生成构建读书俱乐部页面的代码。

*第五章* 讲解了如何在页面上发布帖子以及使用 AI 将文本提示转换为图像。你将这些内容整合到一个提示中，指导 ChatGPT 生成在线日志页面的代码。

*第六章* 全部关于链接和导航。你将学习链接代码的工作原理，这样你就可以手动创建链接，而无需总是请求 ChatGPT 来完成。你还学习如何指导 ChatGPT 创建带有链接到其他网站页面的页面导航栏。本章的项目是一个信息网站。

*第七章* 探讨了 ChatGPT 的写作能力，你将学习如何提示聊天机器人获取主题想法、写作指南和研究建议。你甚至将学习如何以最佳方式提示 ChatGPT 以你自己的风格进行写作。在章节的后面部分，你将构建一个提示，让 ChatGPT 生成兴趣或爱好页面的代码。

*第八章* 提供了你指导 ChatGPT 构建包含文本框、复选框、单选按钮、列表等网页表单所需的工具。你还学习如何注册一个服务，该服务可以将表单数据发送到你的电子邮件地址。你将这些内容整合到一个提示中，请求 ChatGPT 生成活动报名页面的代码。

*第九章* 介绍了两个常见的网页功能：项目符号列表和编号列表。你将学习如何指导 ChatGPT 构建这些列表，并学习各种定制它们以满足你需求的方法。章节结束时，你将提示 ChatGPT 生成构建食谱页面的代码。

*第十章* 更详细地介绍了在网页上处理图像。你将学习如何手动编码图像、如何使用占位符图像以及如何处理图像缩略图。章节的项目是一个复杂的相册页面。

*第十一章* 介绍了最受欢迎的网页模式之一：卡片，你可以用它来展示艺术品、爱好、人物或活动等。当使用 ChatGPT 帮助你构建本章的项目：一个作品集页面时，你将充分利用这些卡片知识。

*第十二章* 提供了使用网页布局标签的完整教程，同时向您展示如何标记重要词汇以及如何在页面上强调词汇。您还将学习一种强大的技术，使您的页面在小屏幕上看起来很好。本章的项目是一个显示长文章并带有侧边的页面。

*第十三章* 介绍了数据驱动的网页，其中大部分页面内容是从单独的数据文件中渲染的。您首先学习如何让 ChatGPT 从您的 Excel 数据创建数据文件。然后您学习如何通过过滤、排序和搜索来让您的用户与数据交互。本章的项目是一个显示虚构大学在线课程目录的页面。

*附录 A* 为您提供了使用 ChatGPT 构建网页的有用背景信息。您将学习如何设置 ChatGPT 账户、测试您的代码以及处理网页文件。

*附录 B* 专注于将您的网页代码上线。您将学习如何将代码部署到两个免费网站——Netlify 和 Cloudflare——以及其他网站。

*附录 C* 通过向您展示一系列关于提示 ChatGPT 的最佳实践和如何处理出现的任何错误，来提升您的 ChatGPT 技能。

### 关于代码

毫不奇怪，一本关于让 AI 聊天机器人生成网页代码的书包含大量的代码！为了帮助区分网页代码和文本的其他部分，本书中，代码以`固定宽度字体`格式呈现。本书还包含许多单独的代码列表。在这些列表中，我尽可能让每一行都适应可用的页面宽度。然而，有些情况下，一行代码太长而无法适应页面宽度，因此该行代码会延续到下一行，并且下一行前面会有一个行延续标记（➥）。

如果您认为您需要手动输入所有这些代码，那么您可能会觉得本书中 ChatGPT 生成的代码量令人畏惧。但并非如此！本书的所有网页代码以及所有 ChatGPT 提示都可在本书的 GitHub 仓库[`github.com/paulmcfe/websites-with-chatgpt`](https://github.com/paulmcfe/websites-with-chatgpt)中查看、下载和复制。要下载所有内容，请点击绿色的“代码”按钮，然后点击“下载 ZIP”。否则，点击一个章节，然后点击您想要查看的文件。

您可以从本书的在线（liveBook）版本中获取可执行的代码片段，链接为[`livebook.manning.com/book/build-a-website-with-chatgpt`](https://livebook.manning.com/book/build-a-website-with-chatgpt)。书中示例的完整代码也可以从 Manning 网站[www.manning.com/books/build-a-website-with-chatgpt](https://www.manning.com/books/build-a-website-with-chatgpt)下载。

### liveBook 讨论论坛

购买《使用 ChatGPT 构建网站》包括免费访问 liveBook，曼宁的在线阅读平台。使用 liveBook 的独特讨论功能，您可以在全球范围内或针对特定章节或段落附加评论。为自己做笔记、提出和回答技术问题，以及从作者和其他用户那里获得帮助都非常简单。要访问论坛，请访问[`livebook.manning.com/book/build-a-website-with-chatgpt/discussion`](https://livebook.manning.com/book/build-a-website-with-chatgpt/discussion)。您还可以在[`livebook.manning.com/discussion`](https://livebook.manning.com/discussion)了解更多关于曼宁论坛和行为准则的信息。

曼宁对读者的承诺是提供一个平台，让读者之间以及读者与作者之间可以进行有意义的对话。这并不是对作者参与特定数量活动的承诺，作者对论坛的贡献仍然是自愿的（且未支付报酬）。我们建议您尝试向作者提出一些挑战性的问题，以免他的兴趣转移！只要书籍仍在印刷中，论坛和先前讨论的存档将可通过出版社的网站访问。

## 关于作者

![保罗·麦克费德斯](img/build-a-website-with-chatgpt-Paul_McFedries.png)

保罗·麦克费德斯（Paul McFedries）是一位拥有超过 30 年专业技术写作经验的作家。他拥有超过 100 本书，总销量超过 400 万册。他的另一本曼宁出版社的书籍是《Web Design Playground，第二版》。当他不写书时，保罗会构建网页，他自 1996 年开始这样做，对 HTML 和 CSS 都有深入的了解。保罗亲手编码了许多网站，包括他的个人网站（[`paulmcfedries.com`](https://paulmcfedries.com)）、Word Spy（[`wordspy.com`](https://wordspy.com)）、WebDev Workshop（[`webdevworkshop.io`](https://webdevworkshop.io)）和 Web Design Playground（[`webdesignplayground.io/2`](https://webdesignplayground.io/2)）。保罗热爱教学，他的写作清晰且逻辑性强，他拥有从记住最初学习某个学科的感受中获得的同理心。

# 1 使用 ChatGPT 介绍网站创建

本章涵盖

+   介绍 ChatGPT

+   理解在 ChatGPT 的帮助下可以创建哪些类型的网页

+   了解使用 ChatGPT 制作网页的限制

+   学习如何使用 ChatGPT 创建自己的网页

英国科幻作家亚瑟·C·克拉克曾经提出了三个众所周知的原则，被称为 *Clarke’s three laws*，其中第三个原则是最常被引用的：“任何足够先进的技术都和魔法无法区分。”如果你一直想创建网页但又对技术感到畏惧，那么这本书的假设——你 *可以* 在 ChatGPT 的帮助下创建自己的网站——对你来说可能就像魔法一样。这并不奇怪，因为如果任何最近的技术值得被称为“足够先进”，那么 ChatGPT 和类似的所谓 *generative AI*——能够创作诗歌、散文，甚至网页的人工智能应用——就当之无愧。

在本章中，我的目标是揭开 ChatGPT 的神秘面纱，让它看起来不那么神奇，而更加实用。在接下来的几页中，你将获得对 ChatGPT 基础知识的简要解释，以及使用 ChatGPT 创建的页面类型的概述（以及为了平衡，一些关于你 *不能* 创建的页面类型的说明），以及一个幕后且非技术性的导游，展示你如何使用 ChatGPT 来完成看似神奇的——但实际上仅仅是数学——壮举：将一个简单的、打字请求转换成一个完整的、可以浏览的网页。

## 1.1 什么是 ChatGPT？

除非你在过去一年或两年里一直隐居在隐居地，否则你很可能已经听说过 GPT 和/或 ChatGPT，这些人工智能代理已经席卷了世界（至少是那些关注社交媒体的那部分世界）。然而，了解 *关于* ChatGPT 是一回事，但了解 ChatGPT 实际上 *是什么*，则是另一回事。

为了帮助你了解 ChatGPT 是什么以及它能做什么，将名称的每个部分分解来看其含义是很有帮助的。我将从 GPT 开始：

+   *G*—在 *GPT* 中的 *G* 代表 *generative*，这意味着 GPT 可以创建或 *generate* 新内容。GPT 是一个 *large language model* (LLM)，通常意味着它被设计用来生成文本，例如文章、故事，甚至是诗歌。更具体地说，对于本书的目的而言，GPT 的生成能力也扩展到了编程代码，尤其是网页背后的代码。

+   *P*—在 *GPT* 中的 *P* 代表 *pretrained*，这意味着 GPT 接触到了大量的文本（这就是 *large language model* 中的“large”所指的）。在这次 *pretraining* 过程中，GPT 学习了语言中的模式和结构，例如句子通常是如何形成的。特别是，给定一些现有的文本，预训练使 GPT 能够预测接下来通常会出现什么单词或短语。从某种意义上说，这就是 GPT 真正在做的事情：预测下一个单词！GPT 还在难以想象的庞大的编程数据集上进行了训练；因此，由于编程代码通常比常规写作更可预测，GPT 在生成代码方面表现出色。

+   *T*—在 *GPT* 中的 *T* 代表 *transformer*，这意味着 GPT 能够接收一些文本输入（例如创建网页的请求）并将这些文本转换为其最重要的组成部分，同时忽略或给予文本中不那么重要的部分较低的优先级。这使得 GPT 能够产生更具相关性和准确性的结果。

*ChatGPT* 中的 *Chat* 部分意味着你可以与 GPT 进行对话式访问，这意味着你可以像在聊天对话中一样与 GPT 交换消息。在创建网页的背景下，这些“对话”将涉及你请求一些页面组件，而 ChatGPT 则提供所需的代码。然而，ChatGPT 也有有限的“记住”当前对话中先前消息的能力，这在你的网站创建任务中有时可能很有用。

当我写下这些时，有两种主要的 GPT 版本可用：2022 年 11 月发布的 GPT-3.5 和 2023 年 3 月发布的 GPT-4。如果你使用 OpenAI 应用（稍后讨论）并且拥有免费的 ChatGPT 账户（更多信息请见附录 A）或者没有账户，你只能访问 GPT-3.5；如果你拥有付费的 ChatGPT Plus 账户并且使用 OpenAI 应用，你可以访问 GPT-3.5 和 GPT-4。

要访问 ChatGPT 以帮助你创建网页，你有三种首选选择：

+   *OpenAI 应用*—这是由 GPT 和 ChatGPT 的创造者 OpenAI 运营的在线应用。该应用可在 [`chat.openai.com`](https://chat.openai.com) 访问。访问它不需要 OpenAI 账户，但拥有账户可以移除某些限制（请参阅附录 A 了解如何创建账户以访问 ChatGPT）。如果你拥有付费的 ChatGPT Plus 账户，你可以选择 GPT-3.5 和 GPT-4，如图 1.1 所示。

![图片](img/build-a-website-with-chatgpt-CH01_F01_Mcfedries3.png)

图 1.1：拥有 ChatGPT Plus 账户时，OpenAI 应用为你提供访问 GPT-3.5 和 GPT-4 的权限。

+   *Microsoft Copilot in Bing*—这是微软搜索引擎的 AI 增强版本，它提供了一个使用 GPT-4 在幕后进行聊天并可以访问网络的聊天功能。按照图 1.2 所示，导航至 [`bing.com`](https://bing.com) 并选择 Copilot 标签开始使用。请注意，使用 Bing Copilot 不需要 ChatGPT 账户。（如果你想知道三种“对话风格”选择，我在附录 A 中详细解释了它们。）

![图片](img/build-a-website-with-chatgpt-CH01_F02_Mcfedries3.png)

图 1.2：使用 Bing Copilot 与 GPT-4 一起工作。

+   *Microsoft Copilot*—这是微软版本的 ChatGPT 的独立实现，它使用 GPT-4 模型。按照图 1.3 所示，导航至 [`copilot.microsoft.com`](https://copilot.microsoft.com)。请注意，使用 Microsoft Copilot 不需要 ChatGPT 账户，但你确实需要一个微软账户。（再次提醒，我在附录 A 中解释了三种“对话风格”选择。）

![图片](img/build-a-website-with-chatgpt-CH01_F03_Mcfedries3.png)

图 1.3 如果您拥有微软账户，请使用 Copilot 与 GPT-4 协作。

注意：访问 ChatGPT 的方法有很多，无论是直接还是间接。例如，有适用于 iOS 和 Android 的 ChatGPT 应用。这些其他方法可以用来与 ChatGPT 打趣，但对于创建网页来说，最好坚持使用 OpenAI 应用、Bing Copilot 或 Microsoft Copilot，因为它们可以轻松访问 ChatGPT 生成的代码。

您应该使用哪种方法来访问 ChatGPT？当涉及到这本书中涵盖的相对简单的网页代码时，这并不是很重要。GPT-4 通常会产生更“现代”的代码，这通常是一件好事。（然而，这可能意味着您的页面在旧浏览器（如 Internet Explorer）中可能无法很好地工作。我的建议？忽略那些古老的浏览器，拥抱现代网络！）如果您没有 ChatGPT 账户，也不想受到 Open AI 应用对非账户持有者的限制，那么 Bing Copilot 是一个不错的选择。

## 1.2 ChatGPT 使任何人都能创建网页

我从未有过如此幸运，拥有一个助手，但我可以想象这会是一笔划算的交易。毕竟，谁会不高兴有人专门负责执行那些必要但枯燥的任务，比如安排虚拟会议；预订航班、酒店和其他旅行细节；以及准备演示文稿？如果您不知道（也不想知道）如何设置 Zoom 会议、浏览 Expedia 网站，或者构建 PowerPoint 演示文稿，那么拥有一个助手就更有价值了。

这些任务当然不是微不足道的，但与设计、编码和部署一个网页或整个网站相比，它们似乎就像是幼儿园的练习。当然，市面上有一些模板和类似的页面构建工具可以提供现成的网页，但结果几乎总是令人失望，因为您对输出的控制非常有限。您有一个网站的好主题，您也有一个关于它应该看起来怎样的心理图像，但您和您的愿景之间有一个障碍：网页代码。

三个主要的网页代码类型——HTML、CSS 和 JavaScript——位于一个陡峭的学习曲线之上：对于许多人来说，这是一个过于艰巨的攀登，因为他们只想为自己或团队、爱好、项目、慈善机构或活动搭建一个或几个页面。如果你想在网上建立自己的存在，但要么对现有的预制解决方案感到失望，要么对学习 HTML、CSS 和 JavaScript 的想法感到恐惧，那么一切并非毫无希望，因为现在你可以“雇佣”（如果你愿意免费的话）一个助手来根据你的精确规格生成网页代码。这个助手就是 ChatGPT，它位于网页开发学习曲线的另一端，准备好、愿意并且非常能够帮助你将你的网页愿景变为现实。通过向模型提供一些简单、通俗易懂的指令，你可以说服 ChatGPT 将这些指令转化为可工作的网页代码。然后，你将代码上传到网上（ChatGPT 甚至可以帮助你完成这一步），任务就完成了！

好吧，这可能并不像听起来那么简单（否则，就没有必要写这本书的其余部分了！）。但基本步骤和我在这里概述的完全一样。

## 1.3 理解你可以（和不可以）创建的页面类型

到现在为止，你可能已经在想，将 ChatGPT 转变为网站建设机器人助手肯定有一些代价。毕竟，对于初学者来说，构建网页似乎是一项几乎本质上复杂的任务，所以声称你可以将几乎所有这些劳动外包给一个 AI 模型，而不必自己学习编码，这肯定伴随着一个相当大的“陷阱”。令人惊讶的是，ChatGPT 中并没有这样的缺陷，但也有一些前提条件需要记住。

首先，你需要知道，最容易在 ChatGPT 的帮助下创建的网页类型是在网页开发行业中被称为*静态*的页面。静态网页是指页面加载后包含的文本和数据不会发生变化。这听起来可能有些限制，但事实上，你要求 ChatGPT 帮助你构建的静态页面类型几乎没有限制。以下有 10 个想法：

+   个人主页

+   团队、组织或活动的信息页面

+   产品着陆页面

+   爱好页面

+   照片画廊

+   简历页面

+   帖子页面（文章、评论、同人小说，或任何内容）

+   前 10 名列表

+   指令说明

+   旅行指南

我敢打赌你很容易就能自己想出 10 个。这些就是你在本书中通过 ChatGPT 的帮助学习如何创建的页面类型。而且，好消息是，除非你选择付费的 ChatGPT Plus 订阅，否则你可以完全免费地做任何事情——从访问 ChatGPT 到保存生成的代码，再到部署你的页面。

第二，我刚才列出的一类网页的特点之一是，它们只需要网络开发爱好者所说的*前端*代码，这意味着在网页浏览器中运行的代码（HTML、CSS 和 JavaScript）。与之截然不同的是*后端*代码，这意味着在网页服务器上运行的代码，通常用于为*动态*网页提供文本和数据，其中文本和数据会实时更改。

从技术上讲，你可以要求 ChatGPT 提供这样的后端代码，但从实际角度来说，你谈论的是比这复杂一个数量级的设置任务，在组织和部署生成的代码方面更为复杂，*巨大的*安全风险，因为网络服务器容易受到多种攻击，并且必须使用高级编码技术来加固后端代码以抵御恶意用户，而且几乎总是会增加成本，因为允许访问服务器的网络托管账户通常需要付费订阅计划。出于所有这些原因，本书中不会介绍如何使用 ChatGPT 生成后端代码。

## 1.4 使用 ChatGPT 帮助你构建网页

*Fritterware* 是一个古老的计算机术语，指的是任何诱使用户花费大量时间在程序的功能和选项上玩耍的软件。一旦你拥有一个 ChatGPT 账户（我在附录 A 中进行了介绍；然而，请记住，拥有账户是可选的），你就可以立即访问有史以来最伟大的碎片软件之一！很容易花费大量时间让 ChatGPT 做各种有趣和愚蠢的事情，但最终，你将想要停止浪费并开始创作。

ChatGPT 创作过程因你制作的内容而异，但就我们的目的而言，你需要了解获取 ChatGPT 帮助你创建网页的整体过程。该过程的简化版本总结在图 1.4 中。接下来的几节将解释每个步骤，而第二章将带你通过该过程的完整示例。

![](img/build-a-website-with-chatgpt-CH01_F04_Mcfedries3.png)

图 1.4 使用 ChatGPT 帮助你创建网页的过程简化图

### 1.4.1 提示 ChatGPT

这个过程总是从一个指定你希望 ChatGPT 为你创建什么的请求开始。这个请求被称为*提示*。当你登录到 ChatGPT 应用程序（参见图 1.1）或导航到 Bing Copilot（参见图 1.2）时，你会看到一个文本框，你可以在这里输入你的提示。

提示可以是简单的单句（如图 1.3 所示），也可以是复杂的多个段落。然而，这里的天空绝对不是极限，因为大多数版本的 ChatGPT 每个提示只能接受最多 4,000 个字符。这大约是 500 个单词，对于大多数网页创作提示来说应该足够了。

不得不说，提示 ChatGPT 是最重要的一步，因为你的提示质量直接决定了 ChatGPT 返回的结果质量。从某种意义上说，这本书的整个内容都是关于提供高质量提示，以使 ChatGPT 执行特定的网页创建任务。我还专门在附录 C 中用相当多的篇幅解释了一些与提示 ChatGPT 相关的最佳实践（专家们称之为*提示工程*的过程）。

警告：尽管一般来说 ChatGPT 是一个质量输入，质量输出的模型，但它像所有大型语言模型一样，有时即使提示很好，也可能会偶尔产生不可用或非常奇怪的结果。我在附录 A 中讨论了一些解决此类问题的方法。

### 1.4.2 查看 ChatGPT 的结果

当你提交你的提示时，ChatGPT 开始工作，通常在几秒钟内就开始“输入”它的响应。图 1.5 显示了以下提示的示例响应：

```py
Write web page code to display “Hello World!” in a large font.
```

![](img/build-a-website-with-chatgpt-CH01_F05_McFedries3.png)

图 1.5 在这个例子中，ChatGPT 对提示的响应包括请求的代码。

如图 1.5 所示，这个结果包括对你的提示的友好响应，后面跟着一个标题为`html`的框，其中包含请求的网页代码。这个代码在你看来可能像是几乎无法辨认的乱码，但请相信我，它确实做了提示所要求的事情：以大号字体（在这种情况下，48 号字体）显示消息`Hello World!`。请注意，由于各种技术原因，ChatGPT 每次运行提示时可能不会返回相同的代码。然而，由于 HTML 和 CSS 通常有多种方式可以达到相同的结果，生成的代码仍然会生成看起来相同（或者至少非常相似）的网页。

### 1.4.3 将代码放入文件

在上一节中我使用的示例提示确实很简单，但仍然令人惊叹的是，在提交这个提示后的几秒钟内，ChatGPT 就生成了一些可行的网页代码，满足了请求。当你与 ChatGPT 一起工作在网页项目上时，仿佛这种惊奇感会一次又一次地出现，因为模型快速且看似毫不费力地生成了你要求的代码。

然而，ChatGPT 生成的网页代码，无论其准确性如何或是否符合你的需求，都不会做任何事情。这是因为，就其本身而言，网页代码是静止的；它只是一系列单词和看起来奇怪的符号。为了让网页代码变得活跃，它必须在网页浏览器中显示；在你能够做到这一点之前，你必须将代码放入浏览器可以访问的文件中。

附录 A 以适当的详细程度深入探讨了网页文件的细节。图 1.6 展示了 ChatGPT 生成的代码（参见图 1.5）粘贴到 HTML 文件中，该文件已保存为 index.xhtml。此时，你可以将保存的 HTML 文件加载到你的浏览器中（详见第二章），但一个真正的网页项目还需要额外一步：将代码部署到网络本身。

![图片](img/build-a-website-with-chatgpt-CH01_F06_McFedries3.png)

图 1.6 从 ChatGPT 复制并保存到 HTML 文件的代码

### 1.4.4 部署 HTML 文件

要让其他人能够查看你的页面，你必须将它们放在网络上。对于本书中创建的相对简单的项目，这个部署过程涉及将 ChatGPT 帮助你创建的文件或文件复制到托管网页的服务器上。我在附录 B 中更详细地介绍了这个过程，但基本上，这意味着将存储网页文件的文件夹上传到主机。图 1.7 展示了示例过程，我将右边的 Finder 窗口中的 hello-world 文件夹拖动，准备将其放在左边的窗口上。当你上传了网页文件后，你可以在你的浏览器中立即查看它们，如图 1.8 所示。

![图片](img/build-a-website-with-chatgpt-CH01_F07_McFedries3.png)

图 1.7 在一些服务中，例如这里展示的 Netlify，部署是一个简单的拖放操作。

![图片](img/build-a-website-with-chatgpt-CH01_F08_McFedries3.png)

图 1.8 ChatGPT 创建的网页已上线。

前几节向您介绍了提示-复制-保存-部署的过程，我认为您会同意，这个过程既令人满意，又出人意料地简单明了。然而，并非所有项目都这么简单，尤其是当你开始创建远不止“Hello World！”的网页时。对于这些更具雄心的项目，你通常会使用两种额外技术：重复提示-复制-保存-部署过程以创建多个页面和页面组件；以及改进和修订你的 ChatGPT 提示。

### 1.4.5 需要时重复

在你的网页制作生涯中，仅通过一个提示创建单个网页的情况相对较少。更有可能的是，你需要多次执行提示-复制-保存-部署的循环，才能最终获得所需的所有内容。这里有两种情况需要考虑：

+   *创建多个页面*——许多网站由单个页面组成，但更常见的情况是网站由多个页面组成。即使是规模较小的网站，也可能包括主页、关于页面（描述你或你的网站）、联系页面（列出网站访客可以联系你的各种方式），以及用于文章、照片和作品集等内容的独立页面。对于这样的网站，你需要为每个页面重复提示-复制-保存-部署的循环。

+   *为单个页面创建多个组件*——大多数现代网页由多个组件组成，例如页眉、导航栏或菜单、内容区域、侧边栏和页脚。你可以在单个提示中包含所有需要的组件，但如果你为每个组件使用单独的提示，你会得到更令人满意的结果。在这种情况下，这个过程变成了一种重复提示-复制-保存循环的部分，每个组件的复制代码被插入到同一个 HTML 文件中。然后你只在添加了所有页面组件之后部署代码。

如果现在这一切看起来有点抽象或令人困惑，不要担心：这本书的其余部分都是关于让你熟悉创建多个页面和页面组件的具体细节。

### 1.4.6 优化和修订你的提示

图 1.3 中描述的 ChatGPT 辅助页面创建过程适用于简单的网页和 ChatGPT 准确满足你的请求的时候。但随着你的网页——以及你的提示——变得更加复杂，你几乎肯定会发现自己需要在这个过程中添加几个额外的步骤。我已经将这些额外步骤包含在图 1.9 中所示的过程图的阴影区域中。

![图片](img/build-a-website-with-chatgpt-CH01_F09_Mcfedries3.png)

图 1.9 优化和修订你的网页提示

初看之下，这可能看起来是一个更复杂的过程，但实际上，这个新过程只需要额外走两条路径。这两条路径以问题的形式出现：

+   *这是你想要的吗？* 你会在 ChatGPT 根据你的提示生成你请求的代码后立即提出这个问题。基本上，你是在检查代码（尽可能好地检查）以确保它为你完成工作。如果答案是“是”，你就继续下一个问题；如果答案是“否”，你以某种方式（例如，使其更具体）改进提示，然后再次尝试。

+   *它工作吗？* 这个问题要求你通过复制代码并将其粘贴到在线测试网页代码的网站上来测试代码，正如我在附录 A 中描述的那样。如果代码通过检查，你可以继续将其保存到 HTML 文件中。如果代码在某些方面有错误，你需要通过以某种方式修订提示并重新提交来修复错误；再次，附录 A 是寻找一些故障排除建议的地方。

当然，如果 ChatGPT 每次都能生成出色的代码那就太好了。而且，ChatGPT 的每个新版本不仅在生产准确代码方面变得更好，而且在创建与模糊或一般提示匹配的代码方面也变得更好。尽管 ChatGPT 可能有一天会例行公事地生成完美的网页代码，但目前它还没有达到那个水平，所以你需要优化和修订你的提示来得到你想要的页面。

## 摘要

+   GPT 代表 *生成*（它被设计用来生成文本），*预训练*（它接触了大量文本以学习语言模式和结构），*转换器*（它分析请求，以给予最重要的组件更高的优先级）。

+   ChatGPT 是一个应用程序，它通过 OpenAI 应用程序在 [`chat.openai.com`](https://chat.openai.com)、通过 Bing Copilot 在 [`bing.com`](https://bing.com)（选择 Copilot 选项卡）或通过 Microsoft Copilot 在 [`copilot.microsoft.com`](https://copilot.microsoft.com) 上，通过 GPT 实现对话访问。

+   GPT 在大量编程代码上进行了训练，包括用于构建网页的代码：HTML、CSS 和 JavaScript。这种训练使 ChatGPT 能够根据简单的英语指令生成网页代码。

+   ChatGPT 最好用于创建不需要或依赖于存储在服务器上的数据的静态网页。

+   ChatGPT 帮助您通过基本的提示-复制-保存-部署周期创建网页，其中 *提示* 是告诉 ChatGPT 您想要哪种类型页面的指令，*复制* 意味着复制 ChatGPT 生成的代码并将其粘贴到文件中，*保存* 意味着将代码保存为 HTML 文件，而 *部署* 意味着将 HTML 文件上传到网络托管提供商。

+   为了获得最佳效果，您通常需要调整您的提示以使网页的结构和内容恰到好处，并且通常需要修改您的提示以修复页面问题。

# 2 创建和部署您的第一个网页

本章涵盖

+   理解创建和部署网页的过程

+   使用 ChatGPT 提示生成完整的网页

+   复制生成的网页代码

+   将代码保存到 HTML 文件

+   将您的网页文件放到网上

您可能觉得这听起来太好了而不真实，您可以让 ChatGPT 帮助您创建一个完全功能性的网站，而无需学习任何网络开发代码。如果您仍然怀疑，我理解您：即使您对 ChatGPT 如何工作有一些了解，整个项目仍然带有不可否认的魔力。毕竟，您不是要求 ChatGPT 告诉您一个敲门笑话或写一首赞美芜菁营养价值的俳句。不，我们谈论的是构建一个真正有用的网页所需的所有代码。这在任何标准下都是一个复杂的要求，所以您剩余的怀疑是完全有理由的。

在本章中，我的目标是向您展示在 ChatGPT 的帮助下创建网页是可能的。我不会通过探索更多的 ChatGPT 理论来做这件事。不，那已经足够了。相反，我会带您通过一个完整的例子，其中我会说服 ChatGPT 创建一个功能网页的代码，到本章结束时，这个网页将在网上有自己的家。为了在一个章节中完成这项工作，网页将不可避免地非常简单，但它会工作，甚至还会提供一些乐趣（取决于您对双关语的品味）。

## 2.1 理解过程

为了创建本章的功能性网页，我将使用我在第一章中介绍过的提示-复制-保存-部署循环（参考图 2.1）：

1.  提示 ChatGPT 生成网页代码。

1.  复制生成的代码。

1.  将代码粘贴到文本编辑器中，然后保存为 HTML 文件。

1.  将 HTML 文件部署到网站托管服务上。

![](img/build-a-website-with-chatgpt-CH02_F01_Mcfedries3.png)

图 2.1 本章中将要使用的提示-复制-保存-部署循环

本章剩余部分的内容将扩展到每个这些步骤。

## 2.2 提示 ChatGPT 生成你的网页代码

要开始，你首先需要将 ChatGPT 显示在屏幕上。你有以下选择：

+   如果你没有 OpenAI 账户，请访问 [`chat.openai.com`](https://chat.openai.com) 使用 GPT-3.5 作为模型。

+   如果你拥有 OpenAI 账户但没有 ChatGPT Plus 订阅，请访问 [`chat.openai.com`](https://chat.openai.com) 使用 GPT-3.5 作为模型。

+   如果你拥有 ChatGPT Plus 订阅，请访问 [`chat.openai.com`](https://chat.openai.com) 并点击 GPT-4 按钮。

+   如果你更喜欢使用 Bing Copilot，请访问 [`bing.com`](https://bing.com)，点击 Copilot，然后点击精确对话风格。

+   如果你拥有 Microsoft 账户，请访问 [`copilot.microsoft.com`](https://copilot.microsoft.com) 并点击精确对话风格。

对于我的提示，我使用了带有 GPT-4 作为模型的 ChatGPT 应用，如图 2.2 所示。

![](img/build-a-website-with-chatgpt-CH02_F02_McFedries3.png)

图 2.2 选择 GPT-4 作为语言模型的 ChatGPT 应用

现在你已经让 ChatGPT 等待执行你的命令，下一步是向模型提供一个提示以生成一些网页代码。在本章中，我想强调的一点是，可以通过单个提示让 ChatGPT 输出功能网页的代码。为了达到这个目标，我们必须极大地简化事情，因此这不能是一个复杂的多功能页面，带有大量的功能。

然而，它也不必是一个最基础的“Hello World！”页面。一般来说，如果你有一个简单的页面想法，只需让 ChatGPT 生成页面的代码，并包括你想要的内容描述。这个描述将根据想法而变化，但你可能希望包括以下内容之一：

+   *目标*——你希望 ChatGPT 生成的（在这种情况下，是一个网页）

+   *数据*——你希望 ChatGPT 使用的数据（如果有的话）

+   *行动*——你希望网页执行的操作，通常是通用的或与指定的数据相关

+   *界面*——你希望用户如何启动操作或与页面交互

这是我想创建的网页的提示（参考图 2.3）：

```py
Create web page code that stores 50 puns and displays a random pun each time the user clicks a button.
```

![](img/build-a-website-with-chatgpt-CH02_F03_McFedries3.png)

图 2.3 准备发送提示的 ChatGPT 应用

这个提示如何符合目标-数据-行动-界面模式：

+   `创建网页代码`——这个提示部分告诉 ChatGPT 生成整个网页的代码。

+   `存储 50 个双关语`——告诉 ChatGPT 创建 50 个双关语作为页面数据。

+   `并显示一个随机双关语`——告诉 ChatGPT 从数据中随机选择一个双关语。

+   `每次用户点击按钮`——告诉 ChatGPT 提供一个按钮，当点击时，显示另一个随机双关语。

将提示输入到 ChatGPT 文本框中，点击发送消息图标，等待结果。

### 2.2.1 检查结果

以下代码显示了从 ChatGPT 收到的第一个响应（ChatGPT 为你生成的代码可能不同）：

```py
<!DOCTYPE html>
<html>
<head>
    <title>Pun Generator</title>                                                    ①   
    <style>
        body {                                                                      ②
            font-family: Arial, sans-serif;                                         ②
        }                                                                           ②
        #displayPun {                                                               ③
            font-size: 24px;                                                        ③
            margin-top: 20px;                                                       ③
        }                                                                           ③
    </style>
</head>
<body>
    <h1>Welcome to Pun Generator!</h1>                                              ④

    <button id="generatePun">Generate Pun</button>                                  ⑤

    <p id="displayPun"></p>                                                         ⑥
    <script>
        var puns = [                                                                ⑦
            "Time flies like an arrow; fruit flies like a banana.",                 ⑦
            "I used to be a baker because I kneaded dough.",                        ⑦
            "I used to play piano by ear, but now I use my hands.",                 ⑦
            // Add the rest of the 50 puns here...                                  ⑦
        ];    
        document.getElementById("generatePun").
addEventListener("click", function() {                                              ⑧
            var randomPunIndex = Math.floor(Math.random() * puns.length);           ⑧
            document.getElementById("displayPun").innerText = puns[randomPunIndex]; ⑧
        });                                                                         ⑧
    </script>
</body>
</html>
```

① 页面标题

② 将 Arial 字体应用于页面

③ 以 24 像素的字体显示每个双关语，顶部有 20 像素的边距

④ 页面的主要标题

⑤ 用户点击以获取新随机双关语的按钮

⑥ 页面中每个随机双关语出现的部分

⑦ （部分）页面数据，这是一个双关语的集合

⑧ 从数据中提取随机双关语的 JavaScript 代码

这里有三点需要注意：

+   尽管这是一个简单的页面，但代码本身相当复杂，所以如果你觉得它像一门外语一样，请不要担心。你不需要知道代码是如何工作的，只需知道它确实可以工作（考虑到我在这份清单中的第三点）。

+   记住，ChatGPT 是非确定性的，这意味着即使你使用相同的提示，它也不会每次都生成相同的代码。因此，如果你在 ChatGPT 中运行我的提示，你很可能得到与列表 2.1 中看到的不同代码。

+   与创建 50 个双关语不同，ChatGPT 只创建了三个双关语，然后推卸责任：

    ```py
    // Add the rest of the 50 puns here...
    ```

这种情况并不总是发生，但你应该知道这是 ChatGPT 非常常见的做法。幸运的是，这并不意味着你陷入了困境。我通过一个简单的提示让 ChatGPT 完成了它的任务：

```py
Can you fill in the rest of the puns for me?
```

ChatGPT 使用完整的双关语集重新生成了代码（尽管我确实在 ChatGPT 卡住时点击了继续生成按钮——参见图 2.4——一次）。这是一大批数据，所以完整的代码出现需要几分钟。

![](img/build-a-website-with-chatgpt-CH02_F04_McFedries3.png)

图 2.4 如果 ChatGPT 卡住了，你可能需要点击继续生成以使其恢复。

理解和自定义代码（可选）

如果你想要理解和/或自定义 ChatGPT 生成的代码（这完全是可选的），以下是一些注意事项：

+   HTML 由称为*标签*的项目集合组成，用于指定页面对象，如段落、标题、项目符号列表和链接。大多数 HTML 标签都是围绕尖括号（`<`和`>`）的字母代码。例如，你用`<p>`标签指定段落的开始，用`</p>`标签指定段落的结束。作为另一个例子，上一节中 ChatGPT 生成的 HTML 代码包括以下行：

    ```py
    <h1>Welcome to Pun Generator!</h1>
    ```

    `<h1>` 和 `</h1>` 标签标记了一级标题（参考第三章了解更多关于标题的信息），因此在这种情况下，文本“欢迎来到双关语生成器！”以这样的标题形式出现在页面上。

+   CSS 由一组称为 *属性* 的项目组成，用于指定应用于页面对象的样式。例如，`font-size` 属性决定了指定对象的文本大小，因此要设置大小为 `24px`（24 像素），你使用以下 CSS 声明：

    ```py
    font-size: 24px;
    ```

    注意属性名后面的冒号（`:`）和结尾的分号（`;`）。CSS 声明被分组到 *规则* 中，这些规则包括应用声明的对象以及用大括号（`{` 和 `}`）包围的声明，如下面从之前显示的 ChatGPT 生成的代码中的例子所示：

    ```py
    #displayPun {
        font-size: 24px;
        margin-top: 20px;
    }    
    ```

    在这个例子中，`#displayPun` 是对 HTML 代码中以下元素的引用：

    ```py
    <p id="displayPun"></p>
    ```

+   `<title>` 和 `</title>` 标签之间的文本是浏览器标签中显示的页面标题。你可以自由编辑这个文本（但不要乱动这些标签）。

+   你可以通过修改 `font-size` 值来更改双关语文本的大小。无论你使用什么值，只需确保后面跟着 `px`（像素）。

+   `<h1>` 和 `</h1>` 标签之间的文本是主页标题。你可以编辑这个文本（但不要触摸这些标签）。

+   用户点击的按钮由 `<button>` 标签指定。该标签和 `</button>` 标签之间的文本就是按钮上显示的文本。如果你愿意，可以编辑这个文本。

+   ChatGPT 将页面数据存储在一个特殊的数据对象中，称为 *数组*。在这种情况下，数组中的每个项目都是文本（具体来说，是一个双关语），由双引号（`""`）包围，后面跟着一个逗号。根据需要，你可以编辑、添加或删除数组项目；只需确保完成时，每个数组项目都由双引号包围，后面跟着一个逗号。另外，不要删除开始和结束数组的方括号（`[` 和 `]`）。

在进行下一步之前，我将花一点时间给你提供一些针对简单单页网站的其它提示建议。

### 2.2.2 检查一些针对单页网站的其它提示

如果你正在跟随并想使用 ChatGPT 的帮助创建自己的单页网站，你可以使用上一节中的我的提示，或者如果你有一个一直想尝试的想法，你可以使用自己的提示。如果你不确定该做什么，这里有一些建议：

注意：ChatGPT 对你提出的问题以及在同一聊天会话中之前生成的内容有一种“记忆”。在尝试以下任何提示之前，请确保开始一个新的聊天，以免 ChatGPT 的结果受到会话早期内容的影响。

+   “创建显示 *Y*（*X* 事物清单，其中 *X* 是一个形容词，例如 *fun* 或 *interesting*，*Y* 是一个城市或地区的名称）”的网页代码。例如：

    ```py
    Create web page code that displays a list of ten entertaining things to do in Miami’s South Beach area.
    ```

+   “生成一个网页代码，提供制作 *X* 的食谱”（其中 *X* 是一道晚餐、甜点或其他可以从头开始烹饪的菜肴）。示例：

    ```py
    Generate the code for a web page that provides a recipe for making panna cotta.
    ```

+   “提供网页代码，列出完成 *X* 所需的步骤”（其中 *X* 是一个项目、维修工作、维护工作或其他任务）。示例：

    ```py
    Provide web page code that lists the steps required to replace a bathroom faucet.
    ```

+   “创建网页代码，解释 *X* 的工作原理”（其中 *X* 是一台机器、小工具、科学原理，或者实际上几乎可以是任何东西）。示例：

    ```py
    Create web page code that explains how a hologram works.
    ```

+   “生成一个网页代码，存储 *X* 并在用户点击按钮时显示随机的 *Y*”（其中 *X* 是一些数据，而 *Y* 是以某种方式组合的数据）。示例：

    ```py
    Generate the code for a web page that stores a dozen each of the following: names, verbs, colors, adjectives, and nouns. When the user clicks a button, the code should assemble and display a random sentence that uses the template "Name verb the color, adjective noun."
    ```

+   “提供网页代码，将 *X* 以列表形式显示并存储与每个 *X* 相关的 *Y*。当用户从列表中选择 *X* 时，页面将显示相关的 *Y*”（其中 *X* 可以是一个单词、人物或物体，而 *Y* 可以是一首诗、传记或描述）。

    ```py
    Provide web page code that displays six rarely used adjectives in a dropdown list and stores a limerick associated with each adjective. When the user chooses an adjective from the list, the page displays the associated limerick.
    ```

您可以自由地使用示例提示语，或者根据您想要的页面进行自定义。

## 2.3 复制 ChatGPT 的网页代码

一旦 ChatGPT 生成了您的代码，您的下一步是复制代码。您如何复制生成的代码取决于您是否使用 ChatGPT 应用程序、Bing Copilot 或 Microsoft Edge 中的 Copilot 侧边栏。每个界面都提供了一种复制代码的功能，形式为一个图标或按钮。有关如何在每个界面中复制代码的完整细节，请参阅附录 A。如果您像我一样使用 ChatGPT 应用程序，代码将出现在一个单独的 HTML 代码窗口中，该窗口右上角有一个复制代码按钮，如图 2.5 所示。

![](img/build-a-website-with-chatgpt-CH02_F05_McFedries3.png)

图 2.5 要在 ChatGPT 应用程序中复制生成的代码，请点击代码窗口右上角的“复制代码”。

复制的代码现在存储在您的计算机剪贴板中，这是一个特殊的内存区域，用于存储最近复制的数据。为了避免在剪贴板中覆盖复制的代码，请确保在您的计算机上执行任何其他操作之前（尤其是复制或剪切其他数据）继续下一步。

### 2.3.1 将网页代码保存为 HTML 文件

现在您已经复制了 ChatGPT 生成的网页代码，您的下一步是将复制的代码粘贴到文本文件中，然后将该文档保存为 HTML 文件。在开始之前，使用文件资源管理器（Windows）或 Finder（macOS）创建一个子文件夹来存储所有您的网页项目。例如，您可能想在用户账户的文档文件夹中创建一个名为 sites 或 public_html 的文件夹。

完成这些操作后，以下是保存复制的 ChatGPT 代码到 HTML 文件的步骤：

1.  打开您的文本编辑器。

1.  开始创建一个新的文本文件。在大多数文本编辑器中，您可以选择文件 > 新建（或者，根据应用程序，您可能需要选择不同的命令，例如新建文件、新建文本文件或新建文档）。您也可以通常按下 Ctrl-N（在 Windows 上）或 Cmd-N（macOS）。

1.  选择编辑 > 粘贴以将复制的代码粘贴到新的文本文件中。您也可以按 Ctrl-V（在 Windows 上）或 Cmd-V（macOS）。

1.  选择文件 > 保存。您也可以按 Ctrl-S（在 Windows 上）或 Cmd-S（macOS）。应用程序显示另存为对话框。

1.  导航到您之前创建的文件夹（命名为 sites 或 public_html 或任何名称）以存储您的网页项目。

1.  点击新建文件夹按钮，然后输入文件夹名称。您将在下一节中将此文件夹上传到网络，因此您使用的名称应仅包含小写字母、数字、破折号（-）和/或下划线（_）。不允许有空格。

1.  对于文件名，键入`index.xhtml`。

1.  点击保存。应用程序保存您的 HTML 文件。图 2.6 显示了保存为 HTML 文件的 Pun Generator 代码。

![图片](img/build-a-website-with-chatgpt-CH02_F06_McFedries3.png)

图 2.6 ChatGPT 生成的代码已保存为 HTML 文件

在图 2.6 的顶部附近，注意我的文本编辑器显示 HTML 文件的路径：

```py
paul/Documents/public_html/pun-generator/index.xhtml
```

此路径表示在我的用户账户的文档文件夹中，我创建了一个名为 public_html 的子文件夹来存放所有我的网站。使用前面的步骤，我首先导航到 public_html，创建了新的 pun-generator 子文件夹，然后在该新文件夹中将代码保存为 index.xhtml。

您现在可以在网页浏览器中测试您的页面。

## 2.4 在浏览器中测试您的网页

当您的网页代码已保存到计算机上的文件中时，在部署之前快速检查页面总是一个好主意。测试网页的最简单方法是使用您最喜欢的网页浏览器打开 HTML 文件。以下是您需要遵循的步骤：

1.  在您的网页浏览器中，显示打开对话框：

    +   Windows 网页浏览器：按 Ctrl-O。

    +   Mac 网页浏览器：选择文件 > 打开文件或按 Cmd-O。

1.  在打开对话框中，导航到上一节中存储您的 HTML 文件的文件夹。

1.  选择 HTML 文件。

1.  点击打开。

网页浏览器打开 HTML 文件并根据 HTML 标签和 CSS 属性显示网页。

从计算机打开网页进行测试运行非常方便，但如果您想在网络上看到您的页面，则需要部署它。

## 2.5 部署您的网页

部署您的页面意味着将 HTML 文件上传到您的网络主机。具体操作取决于主机，因此请查看主机的支持页面以获取具体步骤。以下是在大多数网络主机上遵循的一般步骤：

1. 登录您的网络托管提供商。

2. 导航到上传您的网页文件的页面。

3. 上传您在上一节中创建的子文件夹，包括该文件夹的`index.xhtml`文件。

对于这个例子，我将按照以下步骤将我的 Pun Generator 部署到 Cloudflare（尽管请参考附录 B 以获取更具体的说明）：

4. 在 Cloudflare 仪表板的导航侧边栏中，在 Workers & Pages 下点击概览。

5.  点击图 2.7 所示的创建应用程序按钮。（如果您是第一次在 Cloudflare 上部署，屏幕上不会有创建应用程序按钮。在这种情况下，请跳过此步骤。）

![](img/build-a-website-with-chatgpt-CH02_F07_McFedries3.png)

图 2.7 在概览页面上，点击创建应用程序。

6.  点击页面标签。

7.  滚动到直接上传创建部分，然后点击上传资源。

8.  输入您的项目名称，然后如图 2.8 所示点击创建项目。

![](img/build-a-website-with-chatgpt-CH02_F08_McFedries3.png)

图 2.8 输入项目名称，然后点击创建项目。

9.  使用以下方法之一上传您的网站文件夹：

a)  拖动您的网站文件夹，并将其拖放到上传区域。

b)  点击从计算机选择，然后点击上传文件夹。在出现的对话框中，导航到项目文件夹，然后点击上传。

10.  如果您的网络浏览器要求您确认操作，请点击上传。

11.  点击部署网站。

12.  点击链接在网页浏览器中查看已部署的网站。图 2.9 显示我的 Pun Generator 已部署到[`pun-generator.pages.dev`](https://pun-generator.pages.dev)。

![](img/build-a-website-with-chatgpt-CH02_F09_McFedries3.png)

图 2.9 将 Pun Generator 网站部署到 Cloudflare Pages。

就这样：在 ChatGPT 的帮助下创建的网页，只需几个步骤就部署到了网络上。是的，您创建的页面很简单，但本书的其余部分致力于向您展示如何让 ChatGPT 帮助您构建更复杂、更有用的网站。

## 摘要

+   获取 ChatGPT 帮助构建网页的基本过程是提示-复制-保存-部署周期。

+   在提示 ChatGPT 时，包括目标、所需数据、页面要执行的操作以及用户启动操作的用户界面。

+   如果 ChatGPT 没有给您提供您所要求的所有内容，运行第二个提示以请求缺失的信息。

+   通过点击复制代码图标或按钮来复制生成的代码。

+   使用您的操作系统文件管理应用程序创建一个文件夹，您将在其中存储所有您的网络项目。

+   在您的文本编辑器中，将复制的代码粘贴到新的文本文件中，然后以 index.xhtml 的名称保存该文件，并将其保存在为项目创建的新子文件夹中。

+   通过将项目数据上传到您的网络托管提供商来部署网站。

# 3 使用字体、颜色和标题

本章节涵盖

+   理解字体在网页设计中的作用

+   为您的页面创建颜色方案

+   使用标题使页面更容易阅读

+   提示 ChatGPT 构建个人主页

+   检查和自定义 ChatGPT 代码

在第二章中，我带你从头开始使用相对简单的 ChatGPT 提示创建了一个功能性的网页。生成的页面运行良好，但外观并不吸引人。那个朴素的页面对我来说是合适的，因为我想要保持简单，但如果你打算在网络上建立某种存在，你肯定希望生成的页面看起来很棒。

在本章中，你将通过检查几个可以大大提高任何网页吸引力和可读性的页面格式选项，迈出第一步。这些选项包括字体、字体大小、颜色和标题。在这里，你将了解为什么这些很重要，以及如何让 ChatGPT 帮助你为你的页面做出这些设计选择。所有这些信息都将被整合到一个详细的提示中，然后你将把这个提示传递给 ChatGPT，以生成个人主页的网页代码，让你拥有一片可以称为自己的网络空间。如果你好奇，本章还解释了 ChatGPT 生成的代码，并展示了几个无需再次提示 ChatGPT 即可自定义代码的方法。

## 3.1 环顾本章的项目

在本章中，你将请求 ChatGPT 帮助你完成的项目是一个简单的个人主页，它可能包含以下部分之一或全部：

+   标题（可能是你的名字）

+   副标题（一个总结页面或你自己的标语，供读者参考）

+   简短的传记

+   简短的职业描述

+   你爱好和兴趣的列表

+   你最喜欢的书籍、电影、电视剧、乐队等的列表

图 3.1 展示了你将在 ChatGPT 的帮助下创建的页面类型示例。

![图片](img/build-a-website-with-chatgpt-CH03_F01_McFedries3.png)

图 3.1 ChatGPT 生成的个人主页

当然，这是你的页面，所以请随意添加任何你希望世人了解的信息。你也可以稍微修改这个页面，将其变成一个在线简历或履历。

在具体提示 ChatGPT 生成个人主页代码之前，你可以使用该模型生成一些设计建议，包括网站标题和副标题、字体和配色方案。你将在构建提示时使用这些建议。

## 3.2 构建个人主页

为了帮助你使用 ChatGPT 构建个人主页，接下来的几节将带你了解页面的每个组成部分，从标题到类型再到颜色。在每种情况下，我都会给你一些背景信息，展示相关的 HTML 和/或 CSS（如果有），然后展示如何请求 ChatGPT 生成你需要的内容。

### 3.2.1 获取网站标题和副标题建议

你个人主页最明显的标题就是你的名字。如果你觉得不够有创意，可以让 ChatGPT 帮忙提出不仅是一个网站标题，还可以是一个副标题或标语，出现在标题下方。

提示 ChatGPT 生成标题和副标题的一个有用方法是结合你从事的工作以及一个或多个爱好或兴趣，看看 ChatGPT 能提出什么建议。以下是一个你可以使用的通用提示：

```py
You are a wordsmith that can generate catchy and creative titles and taglines for personal home pages. You use the information provided by the user to come up with suggestions that reflect their skills and interests.

I am *X* and my favorite hobby is *Y*.

First, think of some words or phrases that relate to *X* and *Y*.

Second, try to combine or play with these words or phrases to create catchy or witty titles.

Third, add a tagline that explains or expands on the title.
```

在这个提示中，将 *`X`* 替换为你的工作标题或描述，将 *`Y`* 替换为一个或多个兴趣或爱好。图 3.2 展示了我的结果（使用创意模式中的 Bing Copilot 生成的）。如果你找到一个你喜欢的标题和副标题（它们不必来自同一个建议），请将它们复制到某个地方，以便你可以在提示 ChatGPT 创建主页代码时使用它们。

![](img/build-a-website-with-chatgpt-CH03_F02_McFedries3.png)

图 3.2 提示 ChatGPT 生成页面标题和标语

网页字体是页面文本的样式。这是一个很大的话题，但就我们在这里的目的而言，你可以考虑三个组成部分：字体、字体大小和字体样式。

### 3.2.2 字体样式

*字体* 是任何相关字母、数字和符号集合中常见的独特设计。等一下，我听到你说，那不是 *字体* 吗？两者有什么区别？从实用角度来看，这两个术语是可以互换的。然而，从技术上讲，字体是字体的特定实现，这意味着字体是以特定的尺寸和样式渲染的。Arial 是一种字体；Arial 16 点粗体是一种字体。

你最常遇到的五种字体类别如下：

| *衬线* —*衬线*（与 *sheriff* 发音相似）字体在每个字符的末端包含细小的交叉笔画（称为 *feet*）。这些细微的附加物赋予了字体一种传统、优雅的外观，但在小尺寸的屏幕上显示时可能会丢失。 |
| --- |

![](img/build-a-website-with-chatgpt-CH03_UN01_McFedries3.png)

|

| *无衬线* —*无衬线* 字体在字符的末端不包含交叉笔画。这些字体通常具有干净、现代的外观，非常适合屏幕文本，尤其是在小尺寸时。 |
| --- |

![](img/build-a-website-with-chatgpt-CH03_UN02_McFedries3.png)

|

| *等宽* —*等宽* 字体（也称为 *fixed-width* 字体）为每个字符使用相同的空间，因此像 *i* 和 *l* 这样细长的字母占用与像 *m* 和 *w* 这样较宽的字母一样多的空间。 |
| --- |

![](img/build-a-website-with-chatgpt-CH03_UN03_McFedries3.png)

|

| *手写* —*手写* 字体设计用来模仿手写笔或刷子的书写。 |
| --- |

![](img/build-a-website-with-chatgpt-CH03_UN04_McFedries3.png)

|

| *幻想* —*幻想* 字体通常具有一些极端元素（例如非常厚）的奇异设计。 |
| --- |

![](img/build-a-website-with-chatgpt-CH03_UN05_McFedries3.png)

|

在 CSS 代码中，字体是通过 `font-family` 属性指定的：

```py
font-family: *typeface*;
```

您将*`typeface`*占位符替换为字体名称。（如果字体名称包含一个或多个空格，您需要将名称用引号括起来。）例如，每个之前的字体类别都有自己的 CSS 关键字，所以以下都是合法的 CSS 声明：

```py
font-family: serif;
font-family: sans-serif;
font-family: monospace;
font-family: cursive;
font-family: fantasy;
```

这五个关键字—`serif`、`sans-serif`、`monospace`、`cursive`和`fantasy`—代表了所谓的*通用*字体，这些字体在所有网络浏览器中都是可用的。如果您想在网页的某个组件中使用这些通用字体之一，您可以将适当的字体关键字作为您对 ChatGPT 的指令的一部分：

```py
Style the web page tagline with the generic cursive typeface.
```

还要注意，在单个声明中指定多个字体也是可能的，并且网络浏览器将使用用户设备上安装的第一个字体（从左到右阅读）。这一点很重要，因为 ChatGPT 几乎总是会在其生成的 CSS 中指定多个字体。以下是我们将在本章后面部分检查的网页代码的示例：

```py
font-family: 'Roboto Serif', serif;
```

这个声明意味着网络浏览器将首先尝试加载 Roboto Serif 字体。如果由于某种原因无法加载，它将回退到使用通用的`serif`字体。

您接下来将要处理的主要字体组件是字体大小。

### 3.2.3 设置字体大小

*字体大小*是每个字符的相对大小。字体大小通常以像素（缩写为 px）为单位测量，常规页面文本的默认文本大小是 16 像素（在网页代码中写作`16px`）。

在 CSS 代码中，字体大小是通过`font-size`属性指定的：

```py
font-size: *size*;
```

在这里，将*`size`*替换为您想要的字体大小。例如，许多人发现默认的文本大小 16 px 对于舒适的阅读来说有点小，因此通常指定更大的字体大小，如 20 px：

```py
font-size: 20px;
```

图 3.3 展示了几个常见的字体大小。

![图片](img/build-a-website-with-chatgpt-CH03_F03_McFedries3.png)

图 3.3 一些常见的字体大小

这里是一个向 ChatGPT 指定页面组件字体大小的示例指令：

```py
Style the web page tagline with a font size of 24px.
```

### 3.2.4 与字体样式一起工作

*字体样式*是应用于一个或多个字符或单词的特殊样式。最常见的两种样式是粗体和*斜体*。

对于粗体文本，CSS 使用`font-weight`属性设置为`bold`关键字：

```py
font-weight: bold;
```

这里是一个向 ChatGPT 指定使页面组件加粗的示例指令：

```py
Style the first paragraph with bold.
```

对于斜体，CSS 使用`font-style`属性设置为`italic`关键字：

```py
font-style: italic;
```

这里是一个向 ChatGPT 指定使用斜体样式页面组件的示例指令：

```py
Style the web page tagline with italics.
```

注意：您还可以使用 HTML 标签标记关键词、标题和其他特殊文本，用粗体或斜体表示。您将在第十二章学习这些标签是如何工作的。

只需这三个方面的网络排版——字体、字体大小和字体样式——您就可以在很大程度上使您的页面看起来很棒。当您提示 ChatGPT 时，您可以像刚才展示的那样为字体应用单独的指令，或者您可以将所有内容放在一个单独的指令中，如下例所示：

```py
Style the web page tagline with the Arial typeface, 24px type size, and italics.
```

如果你在你的项目中不确定使用哪种字体，ChatGPT 可以帮助你，就像我在下一节中展示的那样。

### 3.2.5 从 ChatGPT 获取字体建议

我之前提到的通用字体是不错的，但你是否知道有数百种字体可供选择？这是个好消息，因为这意味着你的网页项目可以通过使用有趣的字体脱颖而出，尤其是通过为常规页面文本和标题使用不同的字体。然而，你不能只是随机选择两种字体。因为每种字体都有特定的风格，很容易选择两种在某些方面不匹配的字体，就像选择不匹配的颜色一样。但你怎么才能不仅选择几款字体，还能确保这些字体搭配得当呢？

ChatGPT 就在这里帮助你。特别是，你可以要求 ChatGPT 从 Google Fonts（[`fonts.google.com`](https://fonts.google.com)）生成建议，这是一个包含 1500 多种免费字体的在线仓库。以下是一个通用的提示，你可以用它让 ChatGPT 建议几对兼容的字体（一个用于标题，一个用于正文）：

```py
You are a font aficionado that can generate awesome font combinations for personal home pages. Use the information provided by the user to come up with suggestions that reflect the theme of the personal home page.

My personal home page is related to *X*.

First, using only fonts available at Google Fonts, suggest a *Y* font for the page headings.

Second, using only fonts available at Google Fonts, suggest a compatible *Z* font for the page text.

Third, please do not include Roboto or Open Sans in your suggestions. Be creative and bold in your choices.
```

将*`X`*替换为你个人主页相关的一个词或短语，将*`Y`*和*`Z`*替换为`serif`或`sans serif`。不幸的是，ChatGPT 经常建议 Roboto 和 Open Sans 字体。这些字体无疑是优秀且美丽的，但如果你想要更有趣的字体，确保在你的提示中排除这些常见的字体，就像我那样做。

在图 3.4 中，你可以看到 ChatGPT 为我推荐的字体是 Josefin Sans 和 Roboto Serif（使用 Bing Copilot 在创意模式下生成）。这些是非常好的字体，应该可以很好地搭配在一起。

![图片](img/build-a-website-with-chatgpt-CH03_F04_McFedries3.png)

图 3.4 ChatGPT 的字体建议

如果你使用的是 Bing Copilot，响应可能包括一些推荐的字体示例。如果没有，请点击链接到 Google Fonts（[`fonts.google.com`](https://fonts.google.com)）来检查推荐的字体，以确保你喜欢你所看到的。如果推荐的字体不适合你的设计，请让 ChatGPT 再次尝试：

```py
The suggested typefaces don't work for my personal home page design. Please suggest two different typefaces.
```

一旦你找到了你喜欢的两种字体，你不需要做任何事情，只需写下或记住它们的名称。当你提示 ChatGPT 构建你的网页代码时，你会包括字体名称。

### 3.2.6 生成配色方案

默认情况下，网页使用黑色文字和白色背景。这种颜色组合使文字易于阅读，但不会赢得任何设计奖项。你不需要对颜色做出疯狂的选择，但跳出黑色文字在白色背景上的思维定式，是给读者一点视觉享受的简单方法。

在网络上指定颜色有许多方法，但最简单的是使用网络上的 140 个预定义颜色名称（或关键字）。它们从`aliceblue`到`yellow`不等，不仅包括标准颜色如`red`、`green`和`blue`，还包括一些非常不标准的色调，如`lemonchiffon`、`darkorchid`和`wheat`。

我已经将颜色关键词的完整列表放在我的 Web 设计游乐场网站上[wdpg.io/2/colorkeywords](https://webdesignplayground.io/2/tools/css-color-keywords/)。图 3.5 显示了一个部分列表。

![](img/build-a-website-with-chatgpt-CH03_F05_McFedries3.png)

图 3.5 要查看 Web 设计游乐场上的 CSS 颜色关键词的完整列表，请访问[wdpg.io/2/colorkeywords](https://webdesignplayground.io/2/tools/css-color-keywords/)。

在图 3.5 所示的列表中，你只需要关注颜色列和关键词列。你可以安全地忽略 RGB 值列中的奇怪之处。

CSS 定义了两个与颜色相关的属性。第一个属性是`color`，你用它来为某些文本应用颜色，第二个是`background-color`（有时简称为`background`），你用它来为元素背景应用颜色：

```py
color: *keyword1*;
background-color: *keyword2*;
```

你将*`keyword1`*和*`keyword2`*替换为一个颜色关键词，例如`darkblue`和`lavender`：

```py
color: darkblue;
background-color: lavender;
```

警告：当你为你的网页选择颜色时，你需要确保通过选择具有足够对比度的文本和背景颜色来确保文本的可读性。深色文本在浅色背景上或浅色文本在深色背景上是你想要追求的效果。

你的主页不需要复杂的颜色方案，但你可能想要避免使用黑白搭配，寻找更有趣的方案。以下是一个你可以使用的提示，让 ChatGPT 帮助你为你的主页生成颜色方案：

```py
You are web designer and know how to create beautiful and compelling color schemes. Use the information provided by the user to come up with suggestions that reflect the theme of the personal home page.

My personal home page is related to *X*.

First, design a color scheme for my personal home page. I want the page to be visually appealing and easy on the eyes. I'm thinking of using *Y* as the dominant hue. Suggest two other colors that would go well with *Y*.

Second, show some examples of the suggested color scheme.

Third, when suggesting colors, please use the standard CSS color keywords, such as aliceblue and papayawhip.
```

将*`X`*替换为你个人主页相关的一个词或短语，将*`Y`*替换为你想要用作网站主色调的颜色关键词。我向 ChatGPT 请求了一个以`dodgerblue`为主色调的颜色方案，图 3.6 显示了结果（使用 Bing Copilot 在创意模式下生成）。

![](img/build-a-website-with-chatgpt-CH03_F06_McFedries3.png)

图 3.6 ChatGPT 的颜色方案建议

注意，提示要求 ChatGPT 使用标准的 CSS 颜色关键词来建议颜色。当你要求 ChatGPT 生成你的网页代码时，你将使用这些关键词作为提示的一部分。

你几乎准备好为 ChatGPT 构建主页提示了。你最后的准备工作是理解网页标题的工作方式，这是下一节的主题。

### 3.2.7 理解网页标题

网页*标题*是一个加粗的词或短语，它垂直地从其余文本中突出出来，并作为页面或页面部分的标题。对于大多数网页，只使用三种类型的标题：

+   一个单独的主要标题，它是页面标题

+   有一个或多个二级标题，它们作为每篇主要文章或页面部分的标题

+   在每个二级标题中，有一个或多个三级标题，它们作为子标题

幸运的是，你通常不需要对此过于具体，因为 ChatGPT 几乎总是会自动为你确定标题层次结构。然而，你可能想要控制标题的字体大小以获得你想要的外观。为了给你一个你正在处理的内容的概念，以下是一些关于前三级标题字体大小的说明：

+   *一级标题*——默认字体大小为 32 px。根据标题、长度和想要达到的效果，一级标题（在 HTML 中使用`<h1>`标签指定）可以更大，例如 48 px、72 px，甚至更大。

+   *二级标题*——默认字体大小为 24 px。然而，二级标题（在 HTML 中使用`<h2>`标签指定）略大一些，例如 28 px 或 32 px 并不罕见。

+   *三级标题*——默认字体大小约为 18.2 px。由于这个默认大小仅比正常页面文本（16 px）大一点，你可能更喜欢将三级标题（在 HTML 中使用`<h3>`标签指定）设置为更大，例如 20 px 或 24 px。

再次强调，你不需要深入到网页代码的细节中。对于大多数网页提示，你只需要告诉 ChatGPT 每个标题你想要的字体大小即可，假设默认标题大小不适合你的页面设计。

### 3.2.8 编写提示

现在，你已经拥有了所有你需要提示 ChatGPT 为你提供主页网页代码的东西。你的提示应该开始如下：

```py
I want to build a personal homepage. I don't know how to code, so I need you to provide the code for me.

First, write the HTML code for a simple web page that includes the following:
```

然后你指定页面内容，包括以下内容（参考图 3.7）：

+   包含你的页面标题和副标题的标题（参考第四章）。

+   一个以引言段落开头的主要部分（可能像是对读者的欢迎信息）。

+   一级或多个二级标题后跟一些文本。例如，标题“我喜欢看的电影”可以后面跟着你最喜欢的电影列表。对于每个条目，你不需要提供完整的文本；几个词或第一句话就足够了。你可以在 ChatGPT 生成代码后稍后再完成文本。

![](img/build-a-website-with-chatgpt-CH03_F07_Mcfedries3.png)

图 3.7 个人主页的各个部分

接下来，你要求 ChatGPT 为你生成你想要页面格式的 CSS：

```py
Second, in a separate file please write the CSS code for the following:
```

然后你指定格式，包括以下内容：

+   标题背景颜色（这应该是你的配色方案中的主色）。

+   你想要用于页面标题和副标题的字体大小和颜色（颜色应该是配色方案中的辅助色）。

+   二级标题的字体大小和颜色（颜色应该是配色方案中的主色）。

+   正常页面文本的字体大小。

+   用于标题和正常页面文本的字体。

+   页面的最大宽度。这可以防止文本行过长。对于大多数页面，800 px 的最大长度是合适的。

这是为我主页的示例提示：

```py
I want to build a personal homepage. I don't know how to code, so I need you to provide the code for me.

First, write the HTML code for a simple web page that includes the following:
 * A header that includes the title "Cryptic Writer" and the subtitle "Solving puzzles with words and words with puzzles."
 * A main section where the first paragraph contains the text between the triple quotation marks: 
"""Hi! My name is Paul McFedries. Welcome to my humble web home away from home. I'm so glad you dropped by to learn more about me. Enjoy!""".
 * The second-level heading "What I Do (for Work)" followed by a paragraph that contains the text between the triple quotation marks:
"""I'm a technical writer with over 100 books to my credit..."""
* The second-level heading "What I Do (for Fun)" followed by a paragraph that contains the text between the triple quotation marks:
"""My hobbies and interests include cryptic crosswords, word puzzles, puns, bread baking, typography, Art Deco..."""
* The second-level heading "What I Read" followed by a paragraph that contains the text between the triple quotation marks:
"""I'm currently reading Landlines, by Raynor Winn. Recent reads are The Faraway Nearby by Rebecca Solnit, Journal of a Solitude by May Sarton..."""
* The second-level heading "What I Am" followed by a paragraph that contains the text between the triple quotation marks:
"""Although I was born in Toronto, my parents are both Scottish, which explains my love of both bagpipes and haggis..."""

Second, in a separate file please write the CSS code for the following:
* The header background color is dodgerblue with 20px padding all around. Center the title and subtitle.
 * The title font size is 48px with color whitesmoke.
 * The subtitle font size is 24px with color whitesmoke and formatted as italic.
 * The second-level heading font size is 32px with color dodgerblue.
 * The main section font size is 20px.
 * For the headings, use the Josefin Sans font from Google Fonts. For the rest of the text, use the Roboto Serif font from Google Fonts.
 * The page is centered.
 * The page is responsive with a maximum width of 800px.
```

注意，我包括了居中页面的说明，因为不占用整个浏览器窗口的页面（如本页面在任何宽度超过 800 px 的窗口中都不会这样做）通常在窗口内居中时看起来更好。

ChatGPT 应首先创建 HTML 代码，您可以复制并粘贴到名为 index.xhtml 的文件中。在这段代码中，您应该看到顶部附近类似以下的一行：

```py
<link rel="stylesheet" type="text/css" href="styles.css">
```

这段代码指示网页浏览器在名为 styles.css 的文件中查找 CSS 代码，因此您的下一个任务是复制生成的 CSS 代码，然后将其粘贴并保存到名为 styles.css 的文件中（或您在`<link>`标签中看到的任何名称）。务必将 styles.css 保存到与您的 index.xhtml 文件相同的文件夹中。参考附录 A 了解有关处理 HTML 和 CSS 文件的相关信息。我将此提示提交给 Bing Copilot 的精确模式，它生成的代码产生了图 3.8 所示的页面。

![](img/build-a-website-with-chatgpt-CH03_F08_McFedries3.png)

图 3.8 ChatGPT 生成的我的个人主页

到目前为止，如果您对 ChatGPT 为您制作的个人主页感到满意，您可以跳过本章的其余部分，并按照附录 B 中描述的方式部署代码。但是，如果您想了解更多关于 ChatGPT 生成的代码的信息，请继续阅读下一节。

## 3.3 检查个人主页代码

在本节中，我将为您简要介绍 ChatGPT 为我生成的个人主页代码（以及产生图 3.8 所示页面的代码）。ChatGPT 为您生成的代码可能不会相同，原因有两个：

+   ChatGPT 内置了一定程度的随机性，因此即使相同的提示也可能经常生成略微不同的响应。

+   ChatGPT 生成的网页代码取决于模型的版本（GPT-3.5 与 GPT-4）、使用的应用程序（OpenAI 与 Copilot），以及对于 Copilot，使用的模式（创意、平衡或精确）。

话虽如此，您的个人主页代码可能与我的非常相似，因此如果您对代码是如何工作的感到好奇，下一两个部分的代码注释应该是有用的。

### 3.3.1 检查 HTML

我将从 ChatGPT 为我个人主页生成的 HTML 代码开始，如下所示：

```py
<!DOCTYPE html>
<html>
  <head>
    <link href="https://fonts.googleapis.com/css?family=Josefin+Sans|Roboto+Serif" 
rel="stylesheet">                                                      ①
    <link rel="stylesheet" type="text/css" href="styles.css">          ②
    <title>Cryptic Writer</title>
  </head>
  <body> 
    <header>                                                           ③
      <h1>Cryptic Writer</h1>                                          ④
      <h2>Solving puzzles with words and words with puzzles.</h2>      ⑤
    </header>
    <main>                                                             ⑥
      <p>Hi! My name is Paul McFedries. Welcome to my humble           ⑦
         web home away from home. I'm so glad you dropped by           ⑦
         to learn more about me. Enjoy!</p>                            ⑦
      <h2>What I Do (for Work)</h2>                                    ⑧
      <p>I'm a technical writer with over 100 books to my credit...</p>
      <h2>What I Do (for Fun)</h2>                                     ⑧
      <p>My hobbies and interests include cryptic crosswords, 
         word puzzles, puns, bread baking, typography, Art Deco...</p>
      <h2>What I Read</h2>                                             ⑧
      <p>I'm currently reading Landlines, by Raynor Winn. Recent 
         reads are The Faraway Nearby by Rebecca Solnit, Journal 
         of a Solitude by May Sarton...</p>
      <h2>What I Am</h2>                                               ⑧
      <p>Although I was born in Toronto, my parents are both 
         Scottish, which explains my love of both bagpipes and 
         haggis...</p>
    </main>
  </body>
</html>
```

① 从 Google Fonts 加载 Josefin Sans 和 Roboto Serif 字体

② 告诉网页浏览器在哪里找到 CSS 代码

③ 页面标题

④ 页面标题

⑤ 页面副标题

⑥ 页面主体部分

⑦ 正常文本段落

⑧ 二级标题

注意，特别是告诉网页浏览器在哪里找到 CSS 代码的代码，我将在下一节中描述。

### 3.3.2 检查 CSS

ChatGPT 为我主页生成的 CSS 代码如下所示：

```py
body {
  font-family: 'Roboto Serif', serif;      ①
  max-width: 800px;                        ②
  margin: auto;                            ③
}

header {
  background-color: dodgerblue;            ④
  padding: 20px;                           ⑤
  text-align: center;                      ⑥
}

header h1 {
  font-family: 'Josefin Sans', sans-serif; ⑦
  font-size: 48px;                         ⑧
  color: whitesmoke;                       ⑧
}

header h2 {
  font-family: 'Josefin Sans', sans-serif; ⑦
  font-size: 24px;                         ⑨
  color: whitesmoke;                       ⑨
  font-style: italic;    
}

main {
  font-size: 20px;                         ⑩
}

main h2 {
  font-family: 'Josefin Sans', sans-serif; ⑦
  font-size: 32px;                         ⑪
  color: dodgerblue;                       ⑪
}
```

① 将 Roboto Serif 应用到页面文本上

② 将页面最大宽度设置为 800 px

③ 居中页面

④ 将标题背景设置为 dodgerblue

⑤ 在标题文本周围添加 20 px 的空间

⑥ 在标题内居中文本

⑦ 将 Josefin Sans 应用于标题文本

⑧ 使用 48 px 的字体大小和 whitesmoke 颜色设置标题样式

⑨ 使用 24 px 的字体大小、whitesmoke 颜色和斜体设置副标题样式

⑩ 将常规页面字体大小设置为 20 px

⑪ 使用 32 px 的字体大小和 dodgerblue 颜色设置二级标题样式

如果您喜欢，可以使用这些注释来调整您的网页代码，正如我在下一节中描述的那样。

## 3.4 定制个人主页

如果 ChatGPT 为您生成的个人主页代码不是您想要的，您有两个选择：

+   如果生成的页面与您想要的相差甚远，最好重写您的提示，开始一个新的聊天会话，然后再次尝试。

+   如果生成的页面看起来不错，但只需要一些调整，请让 ChatGPT 为您进行这些调整。确保您在原始提示的同一会话中提交此请求。

对于第二种情况，如果 ChatGPT 生成的代码确实只需要一些小的调整，请考虑根据我在上一节中提供的注释手动修改代码。因为您不知道网页代码，所以最好不要尝试进行任何重大更改。然而，这仍然让您有相当多的方法可以修改代码以获得您想要的页面。

首先，这里是一些 HTML 代码的定制建议：

+   在标题中，您可以编辑标题或副标题。只需确保不要编辑或删除相关的 HTML 标签：`<h1>`和`</h1>`用于标题；`<h2>`和`</h2>`用于副标题。

+   在 HTML 代码的主部分，您可以在每个二级标题（即`<h2>`和`</h2>`标签之间的文本）中添加、删除或编辑文本。确保您不要编辑或删除这些标签）。

+   在 HTML 代码的主部分，您可以在每个段落（即`<p>`和`</p>`标签之间的文本）中添加、删除或编辑文本。确保您不要编辑或删除这些标签）。

+   在 HTML 代码的主部分，您可以通过输入一个`<p>`标签，然后是您的段落文本，最后是`</p>`标签来添加一个新段落。

现在是 CSS 代码的一些定制想法：

+   如果您想使您的首页有不同的最大宽度，将`max-width`值更改为`800px`以外的值。

+   对于任何颜色值，您可以将现有的颜色更改为不同的颜色关键字。

+   对于任何字体大小值，您可以通过更改数字来增加或减少字体大小。只需确保您保留`px`单位即可。

+   为了使您的页面代码更易于访问，考虑将所有 px 测量值转换为 rem 测量值。默认情况下，1 rem 相当于 16 px，因此 20 px 是 1.25 rem，24 px 是 1.5 rem，32 px 是 2 rem，48 px 是 3 rem，依此类推。rem 单位更易于访问，因为它测量的是相对于浏览器用户在其浏览器设置中定义的默认字体大小的字体大小。

## 摘要

+   通过告诉 ChatGPT 一些关于您页面内容的信息，您可以提示它生成有创意的标题和副标题。

+   ChatGPT 可以帮助你处理网页排版的三个关键方面：字体、字体大小和样式。

+   你可以要求 ChatGPT 使用 CSS 提供的 140 个颜色关键词中的任何一个来创建一个配色方案。

+   几乎所有的网页都使用标题：一个一级标题作为页面标题，以及一个或多个二级和三级标题。

+   为了获得最佳效果，你的页面提示应该尽可能具体，包括颜色、字体大小和标题级别。

+   将生成的 HTML 保存到 index.xhtml 文件中，将生成的 CSS 保存到 HTML 代码中 ChatGPT 建议的文件名，通常是 styles.css。

# 4 为页面添加结构

本章涵盖

+   页面标题和页脚的作用

+   在网页中插入图片。

+   添加社交媒体网站的链接。

+   指示 ChatGPT 构建一个读书俱乐部页面。

+   检查和自定义 ChatGPT 网页代码。

在第三章中，你学习了如何让 ChatGPT 帮助你构建一个个人主页。从这个过程中得到的重大启示之一是，你的提示越具体，生成的代码就越能反映你的要求，生成的页面就越接近你的原始页面愿景。

第三章中可能让你感到惊讶的两个方面是最终提示的长度和包含的细节量。然而，长而详细的提示是确保 ChatGPT 生成满足你设计目标的代码的唯一方法。在本章中，你通过添加一些常见的页面结构元素——页面标题和页脚——向 ChatGPT 提供更多细节。你还学习了如何包含一些有用的内容元素：一个或多个图片和一个或多个社交媒体链接。所有这些信息随后将进入一个详细的提示，你将传递给 ChatGPT 以生成一个读书俱乐部页面的代码，为你和其他俱乐部成员提供一个网络家园。

本章还提供了 ChatGPT 生成的代码的高级解释。它甚至提供了一些手动自定义代码的技巧，以获得你想要的一切。

## 4.1 理解本章的项目

在本章中，你将要求 ChatGPT 帮助你为读书俱乐部构建一个简单的网页。生成的页面将包括以下组件：

+   一个包含以下内容的标题元素：

    +   读书俱乐部标志。

    +   读书俱乐部名称

    +   一个描述或总结俱乐部的标语。

+   一个包含以下内容的主元素：

    +   一个介绍性章节，描述读书俱乐部。

    +   一个“我们在读什么”部分，显示关于读书俱乐部当前选择的信息，包括封面、标题和摘要。

    +   一个“下次聚会”部分，显示关于下次俱乐部聚会的信息，包括日期、时间、地点以及一些需要考虑的与书籍相关的问题。

+   一个包含以下内容的页脚元素：

    +   版权声明

    +   链接到俱乐部的社交媒体账户。

图 4.1 展示了你将在 ChatGPT 的帮助下创建的页面类型的一个示例。

对于你自己的页面，你可能想与你的小组成员讨论页面设计，看看是否遗漏了任何内容。你也可以稍微修改这个页面，将其变成阅读小组、讨论小组、文学社团或任何类型的聚会的主页。

![](img/build-a-website-with-chatgpt-CH04_F01_McFedries3.png)

图 4.1 使用 ChatGPT 生成的代码构建的读书俱乐部页面

## 4.2 构建读书俱乐部页面

本章的目标是利用 ChatGPT 的帮助构建一个简单的读书俱乐部页面，该页面演示了网页的基本元素：页眉、页脚和图片。你还学会了如何添加到一个或多个社交媒体账户的链接。在本节结束时，你将所有这些内容组合成一个完整的提示来构建读书俱乐部页面。

### 4.2.1 介绍页面页眉

页面页眉是出现在页面顶部的部分。在几乎所有情况下，页眉会扩展到整个页面的宽度。然而，这里值得指出的是，这并不意味着页眉一定会扩展到整个浏览器窗口的宽度。为什么？因为，正如你将在本章的项目和本书大多数示例页面中看到的那样，通常最好限制网页的宽度，这样文本行就不会太宽，因此也就不会太难阅读。

页眉充当页面的某种介绍，这意味着它通常包括以下一个或多个元素：

+   页面图标或标志

+   页面标题以及可选的标语或副标题

+   社交媒体账户链接

通常（尽管并非必需），可以通过使用不同的背景颜色来设置页眉与页面其余部分的分隔。

当提示 ChatGPT 时，你可以通过包含以下类似的指令来指定页眉及其内容：

```py
Add a header element that includes an image named logo.png, the title "Code & Prose", and the tagline "Diving deep into the narrative side of code".
```

注意：本章中所有的提示都可以在本书的网站上找到（[www.manning.com/books/build-a-website-with-chatgpt](https://www.manning.com/books/build-a-website-with-chatgpt)）和本书的 GitHub 仓库中（[`github.com/paulmcfe/websites-with-chatgpt`](https://github.com/paulmcfe/websites-with-chatgpt)）。

这里有一些示例 HTML 代码，ChatGPT 可能会根据这个指令生成：

```py
<header>
    <img src="logo.png" alt="Code & Prose logo">
    <h1>Code & Prose</h1>
    <p>Diving deep into the narrative side of code</p>
</header>
```

注意，标题是通过标题元素标记的，这意味着标题内容出现在`<header>`和`</header>`标签之间，如本例所示。（我将在本章稍后讨论`<img>`标签；对于`<h1>`标签，请参阅第三章；对于`<p>`标签，请参阅第五章。）图 4.2 展示了在应用了一些 CSS 之后，这段代码可能呈现的样子。页眉的页面底部对应物是页脚，我将在下一节讨论。

![](img/build-a-website-with-chatgpt-CH04_F02_McFedries3.png)

图 4.2 页面页眉

### 4.2.2 介绍页面页脚

页脚是出现在页面底部的一个区域。像页眉一样，页脚几乎总是延伸到页面的整个宽度，页脚的高度取决于其内容。页脚通常相对简单，包括以下一个或两个部分：

+   版权声明

+   社交媒体账户链接

注意，尽管社交媒体链接可以出现在页眉或页脚中，但它们不应该同时出现在两者中。在本章的项目中，社交媒体链接将出现在页脚中。

再次强调，通常通过使用不同的背景颜色来将页脚与页面的其余部分区分开来。通常还会在页脚中包含指向其他主要网站页面的链接，这是我在第七章中讨论的主题。

作为你的 ChatGPT 提示的一部分，你可以通过包含类似于以下指令的说明来指定页脚及其内容：

```py
Add a footer element that includes the text "Copyright" (spelled out, do not include the Copyright symbol), followed by the current year, followed by "Code & Prose".
```

根据这个指令，ChatGPT 可能会生成以下代码：

```py
<footer>
    <p>
        Copyright 2023 Code & Prose
    </p>
</footer>
```

注意，页脚是用`footer`元素标记的，这意味着页脚内容出现在`<footer>`和`</footer>`标签之间，如本例所示。图 4.3 展示了在应用了一些 CSS 之后，浏览器如何渲染这段代码。接下来，你将学习网页上看到的元素的一个关键方面：盒模型。

![图片](img/build-a-website-with-chatgpt-CH04_F03_McFedries3.png)

图 4.3 页脚

### 4.2.3 介绍填充、边框和边距

需要记住的一个重要 HTML 概念是，页面上的每个元素都被一个不可见的框所包围。为什么这很重要呢？因为你可以让 ChatGPT 生成代码来控制这个框的许多方面，包括其内部间距、边框和外部间距。要达到这个目的，你需要熟悉框的各个部分。

图 4.4 给你一个基本框部分的抽象视图，图 4.5 展示了这些相同的部分如何影响实际的页面内容。每个元素框有四个部分：

+   *内容*—这个区域是框的内部矩形，包含框内的内容，例如一些文本或图片。

+   *填充*—这个区域位于内容和边框之间，代表在内容区域的顶部、右侧、底部和左侧边缘外添加的额外空白。

+   *边框*—这部分沿着填充区域的边缘运行，并用线条包围内容和填充。

+   *边距*—这个区域是框的外部矩形，代表在顶部、右侧、底部和左侧边框外添加的额外空白。

![图片](img/build-a-website-with-chatgpt-CH04_F04_Mcfedries3.png)

图 4.4 元素框的主要部分

![图片](img/build-a-website-with-chatgpt-CH04_F05_Mcfedries3.png)

图 4.5 元素框部分与实际页面内容一起出现

内容区域、内边距、边框和边距的组合在 CSS 领域被称为*盒模型*。在尽可能记住所有这些的同时，现在是时候将你的注意力转向那些有用且强大的 CSS 属性，这些属性使你能够操纵任何元素框。首先是改变盒内边距。

添加内边距

在元素框中，内边距是添加到内容上方、下方、左侧和右侧的空白。如果你在元素上添加边框，如下一节所述，内边距是内容与边框之间的空间。内边距给元素在其框中留出一些呼吸空间，确保内容不会被其自身的边框或附近元素拥挤。

你通过将一个或多个边的值应用到内边距来设置内边距：

```py
element {
    padding-top: top-value;
    padding-right: right-value;
    padding-bottom: bottom-value;
    padding-left: left-value;
}
```

每个值都是以像素（px）为单位的测量值。以下是一个例子：

```py
header {
    padding-top: 16px;
    padding-right: 24px;
    padding-bottom: 12px;
    padding-left: 20px;
}
```

你还可以使用一个`padding`简写属性来通过单个声明设置所有内边距值。你可以通过以下简写语法重复前一个示例中的规则：

```py
header {
    padding: 16px 24px 12px 20px;
}
```

如果你只提供一个值，浏览器将把这个值应用到所有四个边。

要让 ChatGPT 设置元素的内边距，你需要在提示的 CSS 部分包含一个类似于以下的指令：

```py
Style the footer with 10px padding all around.
```

根据这个指令，ChatGPT 将生成如下代码：

```py
header {
    padding: 10px;
}
```

盒模型的下一段是边框。

用边框包围一个元素

在元素框中，边框是定义四个边（上、右、下、左）内边距外边缘的线条。这样，边框位于元素的边距和内边距之间。边框是可选的，但通常很有用，可以为读者提供一个视觉指示，表明封装的内容与任何附近的内容是分开的。要创建一个基本的元素边框，请使用如图 4.6 所示的`border`属性。

![图片](img/build-a-website-with-chatgpt-CH04_F06_Mcfedries3.png)

图 4.6 `border`属性的语法

`width`值是以像素（px）为单位的测量值。你也可以将值设置为以下任何关键字：`thin`、`medium`或`thick`。对于`style`值，你可以使用以下任何关键字：`dotted`、`dashed`、`solid`、`double`、`groove`、`ridge`、`inset`、`outset`、`hidden`或`none`。对于`color`参数，你可以使用你在第三章中学到的任何颜色名称。

要让 ChatGPT 在元素周围添加边框，你需要在提示的 CSS 部分包含一个类似于以下的指令：

```py
Style the nav element with a 1px, solid, black border.
```

根据这个指令，ChatGPT 将生成如下代码：

```py
nav {
    border: 1px solid black;
}
```

我在这里要讨论的盒模型的最后一个方面是边距。

与边距一起工作

在元素框中，边距是在边框上方、下方、左侧和右侧添加的空白。边距让你可以控制元素之间的空间。例如，正边距值可以防止页面元素相互碰撞或重叠，并防止元素触及浏览器视口的边缘。另一方面，如果你的设计需要元素重叠，你可以通过使用负边距值来实现这种效果。

你通过设置一个值到元素的一个或多个侧面来应用边距：

```py
element {
    margin-top: top-value;
    margin-right: right-value;
    margin-bottom: bottom-value;
    margin-left: left-value;
}
```

每个边距值是一个以 px 为单位的测量值。以下是一个示例：

```py
footer {
    margin-top: 24px;
    margin-right: 40px;
    margin-bottom: 32px;
    margin-left: 48px;
}
```

与填充一样，一个边距简写属性让你可以使用单个声明来应用边距。你可以通过使用简写语法重写前面的规则，如下所示：

```py
footer {
    margin: 24px 40px 32px 48px;
}
```

如果你只提供一个值，则网络浏览器将该边距值应用于元素的四个侧面。

要让 ChatGPT 设置元素的边距，你可以在提示的 CSS 部分包含一个类似于以下说明的指令：

```py
Style the body with 16px padding all around.
```

根据这个说明，ChatGPT 将生成如下代码：

```py
body {
    padding: 16px;
}
```

之前，你看到了一个包含图片的标题示例。如何在下一节中处理网页图片将介绍。

### 4.2.4 与图片一起工作

尽管大多数网页（无论你如何定义这个术语）都是通过文字来传达信息，但只有文字的页面可能会让人感到有些令人畏惧，而且通常很无聊！当然，你可以（而且应该）使用字体、颜色和文字样式来美化页面（正如我在第三章中描述的那样）。然而，让一个本来看起来单调的文字墙变得生动的一个相对简单的方法是，通过插入一张或两张图片来给你的读者一些视觉享受。这并不是说你的网页图片只是装饰性的。图片是补充你的页面文字、简洁地展示信息和帮助你的读者记住你在页面上阅读的内容的绝佳方式。

图片是一个单独的文件，你可以告诉 ChatGPT 在页面的 HTML 代码中引用它。（有关图片的更详细处理以及它们如何插入到网页中的信息，请参阅第十章。）网络已经标准化了四种格式，这些格式几乎涵盖了所有网络图像，总结在表 4.1 中。

在本章中，我的假设是，你已经有了你想要包含在页面中的图片。对于读书俱乐部项目，你需要两张图片：

+   读书俱乐部的标志；这张图片将放在页面标题中。

+   俱乐部目前正在阅读的书的封面；这张图片将放在页面的主要内容部分。

你需要知道你想要包含在页面中的所有图片文件的名称，因为你在提示中会包含这些名称。

表 4.1 图片文件格式

| 名称 | 扩展名 | 描述 | 用途 |
| --- | --- | --- | --- |
| GIF | .gif | 这是原始的网页图形格式（名称缩写为图形交换格式，发音为“giff”或“jiff”）。GIF 限制为 256 种颜色，可以有透明背景，并且可以组合成简短动画。 | 如果你想将多个图像组合成单个动画图像，请使用 GIF。 |
| JPEG | .jpg, .jpeg | 这种格式（其名称来源于联合图像专家小组，发音为“jay-peg”）支持具有数百万种颜色的复杂图像。JPEG 文件的主要优点是它们被压缩，因此即使是数字化的照片和其他高质量图像也可以是合理的小尺寸，以便更快地下载。然而，请注意，JPEG 压缩是有损的，这意味着它通过丢弃冗余像素来减小图像的大小。压缩程度越高，丢弃的像素越多，图像看起来就越不清晰。 | 如果你有一个照片或类似复杂图像，JPEG 几乎总是最佳选择，因为它提供了最小的文件大小。 |
| PNG | .png | 这种格式（缩写为可移植网络图形，发音为“p-n-g”或“ping”）支持数百万种颜色。它是一种压缩格式，但与 JPEG 不同，PNG 使用无损压缩。图像保持清晰度，但文件大小可能相当大。PNG 还支持透明度。 | 如果你有一个使用纯色或包含大面积近似纯色的插图或图标，PNG 是最好的选择，因为它在保持优秀图像质量的同时提供了合理的小文件大小。如果你需要透明效果，也可以使用 PNG。 |
| SVG | .svg | 这种格式（缩写为可缩放矢量图形）使用矢量而不是像素来生成图像。这些矢量被编码为 XML 格式的指令集，这意味着图像可以在文本编辑器中修改，并且可以操纵以产生动画。 | 如果你有一个标志或图标，并且有一个可以将文件保存为 SVG 格式的图形程序（例如 Adobe Illustrator 或 Inkscape），这种格式是一个不错的选择，因为它可以生成小文件，这些文件可以缩放到任何大小而不会失真。 |

注意：与生成式 AI 模型一起工作的最有趣的部分之一是让他们根据文本提示创建全新的图像。我在第五章中讨论了使用 OpenAI 的 DALL-E 模型从文本生成新图像。

你可能还想为与你的读书俱乐部相关的每个社交媒体账户获取图标，下文将讨论。

### 4.2.5 添加社交媒体链接

在这个现代时代，没有至少几个指向社交媒体网站的链接的网页看起来是不完整的。本章的项目假设你想要链接到 Facebook、X（Twitter）和 Instagram 上的账户。对于每个链接，你需要以下内容：

+   账户用户名

+   社交媒体网站的图标

对于后者，您不需要从网络上下载单独的图像文件（除非您更喜欢这样做）。相反，您将要求 ChatGPT 链接到一个名为 Font Awesome 的图标工具包，它包括所有主要社交媒体网站的图标。（一个例外是 Threads 社交媒体网站，它的图标尚未添加到 Font Awesome 中。）

### 4.2.6 构建提示

如果您已经完成了上一节中的 ChatGPT 提示，那么您现在就有必要提示 ChatGPT 为您生成读书俱乐部页面的代码。您的提示应该开始如下：

```py
I want to build a web page for a book club. I don't know how to code, so I need you to provide the code for me.

First, write the HTML code for a web page that includes the following:
```

然后您指定页面内容，包括以下内容（参见图 4.7）：

+   包含您的俱乐部标志、页面标题和标语的页眉。

+   一个以介绍访客的读书俱乐部部分开始的主体元素。

+   一个显示俱乐部当前阅读的书籍信息的部分，包括封面、标题、摘要和页数。

+   一个显示俱乐部下次聚会的信息的部分，包括日期、时间、地点以及一些供成员提前考虑的问题。

+   包含版权声明和链接到您的俱乐部社交媒体账户的页脚。

接下来，您要求 ChatGPT 生成您想要页面格式的 CSS 代码：

```py
Second, in a separate file please write the CSS code for the following:
```

然后您指定格式设置，包括以下内容：

+   页眉背景颜色（这应该是您配色方案中的主色）。

+   您想要用于页面标题和标语（颜色应该是您配色方案中最浅的颜色）的字体大小和颜色。

+   二级标题的字体大小和颜色（颜色应该是您配色方案中的主色）。

+   正常页面文本的字体大小。

+   用于标题和正常页面文本的字体。

+   页面的最大宽度。这可以防止文本行过长。对于大多数页面来说，800 px 的最大长度是合适的。

![](img/build-a-website-with-chatgpt-CH04_F07_McFedries3.png)

图 4.7 读书俱乐部页面的部分

这里是一个为我自己的读书俱乐部页面提供的示例提示：

```py
I want to build a web page for a book club. I don't know how to code, so I need you to provide the code for me.

First, write the HTML code for a web page that includes the following:
 * A header element that includes an image named logo.png, the title "Code & Prose", and the tagline "Diving deep into the narrative side of code".
 * A main element that contains three sections.
 * The first section contains the second-level heading "Welcome!", followed by a paragraph that contains the text between the triple quotation marks: 
"""Welcome to Code & Prose, the only book club in the world that (we think) reads fiction related to web development.""".
 * A second section that begins with the second-level heading "What We're Reading".
 * In the second section, include the image named book-cover.png, followed by the text between the triple quotation marks, where each word or phrase before a colon is bold:
"""
Title: The Web Designer
Author: Paul McFedries
Pages: 1,576
Summary: At High Falutin High, [etc.]
"""
 * A third section that begins with the second-level heading "Next Meetup".
 * In the third section, include the text between the triple quotation marks, where each word or phrase before a colon is bold:
 """
 Date: August 23
 Time: 6:00pm
 Location: The Coder Cafe
 Questions to ponder: Can Daisy code, or what? Does the book contain too much HTML, or not enough? Why is it so hard for nerds to date?
 """
 * A footer element that includes the text "Copyright" (spelled out, do not include the Copyright symbol), followed by the current year, followed by "Code & Prose". In a separate paragraph, the footer also includes three links to social media accounts: one for Facebook (username: CodeAndProse), Instagram (username: codeandprose), and Twitter (username: codenprose).

Second, in a separate file write the CSS code for the following:
 * The header background color is darkorchid with 10px padding all around. Float the logo to the left and right-align the title and tagline.
 * The title font size is 48px with color lightsteelblue.
 * The tagline font size is 24px with color lightsteelblue and formatted as italic.
 * The second-level heading font size is 30px with color darkorchid and a top margin of 15px.
 * The main element font size is 20px.
 * In the second and third sections, the bold text should use the color mediumseagreen.
 * The image named book-cover.png should be floated to the right.
 * For the title and headings, use the Fira Sans Extra Condensed Bold font from Google Fonts. For the rest of the text, use the Source Code Pro font from Google Fonts.
 * The footer background color is darkorchid with 5px padding all around and a 10px top margin. The text color is lightsteelblue. Center the text and social media links.
 * For the social media links, use the corresponding Font Awesome icons.
 * The entire page is centered in the browser window.
 * The page is responsive with a maximum width of 800px.
```

注意：鉴于这个提示的长度，如果您使用 Bing Copilot 或 Microsoft Copilot，请确保使用精确模式，该模式具有 4,000 个字符的提示限制。

ChatGPT 应首先创建 HTML 代码，您可以复制并粘贴到名为 index.xhtml 的文件中。在这段代码中，您应该看到顶部附近类似以下的一行：

```py
<link rel="stylesheet" type="text/css" href="styles.css">
```

这段代码指示网络浏览器在名为 styles.css 的文件中查找 CSS 代码，因此您的下一个任务是复制生成的 CSS 代码，然后将其粘贴并保存到名为 styles.css 的文件中（或您在`<link>`标签中看到的任何名称）。请确保将 styles.css 保存到与您的 index.xhtml 文件相同的文件夹中。您还需要将图像文件复制到同一文件夹中。有关与网页文件一起工作的更多信息，请参阅附录 A。我使用 OpenAI 的 ChatGPT 应用提交了这个提示，它生成的代码导致了图 4.8 所示的页面。

如果你对你用 ChatGPT 生成的书友会页面满意，你可以跳过本章的其余部分，并按照附录 B 中描述的方式部署代码。然而，如果你想了解更多关于 ChatGPT 生成的代码，下一节将为你提供更详细的了解。

![](img/build-a-website-with-chatgpt-CH04_F08_McFedries3.png)

图 4.8 ChatGPT 生成的我的书友会页面

## 4.3 检查代码

我将为你提供一个简短且相对非技术性的概述，关于 ChatGPT 根据上一节中的提示生成的书友会页面代码（该页面如图 4.8 所示）。你用 ChatGPT 生成的代码将不同于我的，不仅因为你的文本和图片会不同，还因为

+   ChatGPT 的算法包含一些内置的随机性，所以相同的提示每次运行时通常会生成略微不同的代码。

+   ChatGPT 的输出取决于模型（GPT-3.5 与 GPT-4）和应用程序（OpenAI 与 Bing Copilot）。对于 Bing Copilot，输出还取决于对话风格（创意、平衡或精确）。

注意：我生成的书友会 HTML 和 CSS 代码可在本书的网站上（www.manning.com/books/build-a-website-with-chatgpt）和 GitHub 仓库（[`github.com/paulmcfe/websites-with-chatgpt`](https://github.com/paulmcfe/websites-with-chatgpt)）找到。

然而，ChatGPT 的每个版本都应该输出至少与下一两个部分显示的 HTML 和 CSS 代码相似的代码，所以我的代码注释应该能帮助你理解底层发生了什么。

### 4.3.1 检查 HTML

这里展示了 ChatGPT 为我生成的书友会 HTML 代码：

```py
<!DOCTYPE html>
<html>
<head>
    <title>Code & Prose</title>
    <link rel="stylesheet" href="styles.css">                   ①
    <link rel="preconnect" href="https://fonts.gstatic.com">    ②
    <link href="https://fonts.googleapis.com/css2
          ?family=  Fira+Sans+Extra+Condensed:wght@700
          &family=Source+Code+Pro&display=swap" 
          rel="stylesheet">                                     ②
    <link rel="stylesheet" 
          href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2
          /css/all.min.css">
</head>
<body>
    <header>                                                    ③
        <img src="logo.png" alt="Code & Prose logo" id="logo">  ④
        <h1>Code & Prose</h1>                                   ⑤
        <p>Diving deep into the narrative side of code</p>      ⑥
    </header>                                                   ③
    <main>
        <section>                                               ⑦
            <h2>Welcome!</h2>
            <p>Welcome to Code & Prose, the only book 
               club in the world that (we think) 
               reads fiction related to web 
               development.</p>
        </section>                                              ⑧
        <section>                                               ⑨
            <h2>What We're Reading</h2>
            <img src="book-cover.png"                           ⑩
                 alt="Book cover"                               ⑩
                 id="book-cover">                               ⑩
            <p><b>Title:</b> The Web Designer<br>               ⑪
            <b>Author:</b> Paul McFedries<br>                   ⑪
            <b>Pages:</b> 1,576<br>                             ⑪
            <b>Summary:</b> At High Falutin High, [etc.]</p>    ⑪  
        </section>                                              ⑨
        <section>                                               ⑫
            <h2>Next Meetup</h2>
            <p><b>Date:</b> August 23<br>                       ⑬
            <b>Time:</b> 6:00pm<br>                             ⑬
            <b>Location:</b> The Coder Cafe<br>                 ⑬
            <b>Questions to ponder:</b> Can Daisy 
               code, or what? Does the book contain 
               too much HTML, or not enough? Why is 
               it so hard for nerds to date?</p>                ⑬
        </section>                                              ⑫
    </main>
    <footer>                                                    ⑭
        <p>Copyright 2023 Code & Prose</p>                      ⑮
        <p>                                                     ⑯
        <a href=https://www.facebook.com/CodeAndProse
        target="_blank">
        <i class="fab fa-facebook-square"></i></a>              ⑯
        <a href=https://www.instagram.com/codeandprose
        target="_blank">
        <i class="fab fa-instagram"></i></a>
        <i class="fab fa-x-twitter"></i></a>                    ⑯
        </p>                                                    ⑯
    </footer>                                                   ⑭
</body>
</html>
```

① 告诉网页浏览器在哪里找到 CSS 代码

② 从 Google Fonts 加载页面字体

③ 页面页眉

④ 页面标志

⑤ 页面标题

⑥ 页面标语

⑦ 页面的第一部分

⑧ 页面的第一部分

⑨ 页面的第二部分

⑩ 书籍封面图片

⑪ 书籍信息

⑫ 页面的第三部分

⑬ 俱乐部聚会信息

⑭ 页面页脚

⑮ 版权声明

⑯ 社交媒体链接

注意：在我的实验中，ChatGPT 偶尔会生成在页面上添加了不寻常字符的代码。如果你看到不寻常的字符，你几乎总是可以通过在 HTML 文件中的`<head>`标签后立即添加代码`<meta charset="utf-8">`来修复这个问题。这个标签告诉浏览器如何处理某些字符，例如花括号引号（“和”）。

在阅读 HTML 代码时，请注意以下几点：

+   页面的两个图像使用`<img>`标签引用，其中`src`值是图像文件的名称。如果你更改了图像文件的名称，务必更改相应的`src`值。

+   在书籍信息和聚会信息中，`<br>`标签告诉网络浏览器在下一行开始下一个项目，两行之间没有额外空间。如果您的页面在这两行之间有额外空间，这意味着 ChatGPT 使用了`<p>`（段落）标签而不是`<br>`（换行）标签。请在每行的开头删除`<p>`标签，并将每行末尾的`</p>`标签替换为`<br>`。

+   在社交媒体链接中，`target="_blank"`代码告诉网络浏览器在新标签页中打开链接。如果要（首选方法）在同一标签页中打开链接，请从每个链接中删除`target="_blank"`代码。

+   在社交媒体链接中，`class`值引用特定的 Font Awesome 图标以显示为链接文本。例如，`class="fab fa-instagram"`将显示 Instagram 图标。

最后，请注意，HTML 代码中包含以下行：

```py
<link rel="stylesheet" href="styles.css">
```

此标签告诉网络浏览器在哪里找到 CSS 代码，我将在下一节中描述。

### 4.3.2 检查 CSS

ChatGPT 为我书友会页面生成的 CSS 代码如下所示：

```py
body {
    font-family: 'Source Code Pro', monospace;            ①
    color: black;
    max-width: 800px;                                     ②
    margin: auto;                                         ③
}
header {
    background-color: darkorchid;                         ④
    padding: 10px;                                        ⑤
}
header img {
    float: left;                                          ⑥
}
header h1 {
    font-family: 'Fira Sans Extra Condensed', sans-serif; ⑦
    font-size: 48px;                                      ⑧
    color: lightsteelblue;                                ⑧
    text-align: right;    
}
header p {
    font-size: 24px;                                      ⑨
    color: lightsteelblue;                                ⑨
    font-style: italic;                                   ⑨
    text-align: right;                                    ⑨
    clear: right;
}
main {
    font-size: 20px;                                      ⑩
}
h2 {
    font-family: 'Fira Sans Extra Condensed', sans-serif; ⑪
    font-size: 30px;                                      ⑪
    color: darkorchid;                                    ⑪
    margin-top: 15px;                                     ⑪
}
section:nth-child(2) img {
    float: right;                                         ⑫
}
section:nth-child(2) p b,
section:nth-child(3) p b {
    color: mediumseagreen;                                ⑬
}
footer {
    background-color: darkorchid;                         ⑭
    color: lightsteelblue;                                ⑭
    padding: 5px;                                         ⑭
    margin-top: 10px;                                     ⑭
    text-align: center;                                   ⑭
}
footer a {
    margin: 0 10px;                                       ⑮
    color: lightsteelblue;                                ⑮
    text-decoration: none;                                ⑮
}
```

① 将 Source Code Pro 应用于页面文字

② 设置最大页面宽度为 800 px

③ 使页面居中

④ 将页眉背景设置为暗紫色

⑤ 在页眉文字周围添加 10 px 的空间

⑥ 将标志浮动到左侧

⑦ 将 Fira Sans Extra Condensed 字体应用于标题

⑧ 设置标题样式：字体大小 48 px，颜色浅钢蓝色，右对齐

⑨ 设置标语样式：字体大小 24 px，颜色浅钢蓝色，斜体，右对齐

⑩ 将常规页面字体大小设置为 20 px

⑪ 设置二级标题样式：Fira Sans Extra Condensed 字体，字体大小 30 px，颜色暗紫色，顶部边距 15 px

⑫ 将书封浮动到右侧

⑬ 将中等海绿色应用于粗体文字

⑭ 设置页脚样式：背景颜色为暗紫色，文字颜色为浅钢蓝色，内边距 5 px，顶部边距 10 px，文字居中

⑮ 设置页脚链接样式：左右边距 10 px，文字颜色浅钢蓝色，无下划线

如果您愿意，可以使用这些注释来调整您的网页代码，正如我在下一节中描述的那样。

## 4.4 自定义页面

如果由于某种原因 ChatGPT 的书友会页面代码不正确，您有两种方法来修复它：

+   如果页面与您期望的相差甚远，请重新编写提示，开始一个新的聊天会话，并再次尝试。

+   如果页面接近您想要的效果，请要求 ChatGPT 进行必要的调整。确保您在原始提示的同一会话中提交此请求。

对于第二种情况，如果 ChatGPT 生成的代码确实只需要一些小的调整，请考虑根据我在上一节中提供的注释手动修改代码。由于您不了解网页代码，最好不要尝试进行任何重大更改。然而，这仍然留下了一些方法可以修改代码以获得您想要的页面。 

首先，这里有一些对 HTML 代码的定制建议：

+   在页眉中，您可以编辑标题或标语。只是确保不要编辑或删除相关的 HTML 标签：标题使用 `<h1>` 和 `</h1>`；标语使用 `<p>` 和 `</p>`。

+   在 HTML 代码的主要部分，您可以在每个二级标题（即 `<h2>` 和 `</h2>` 标签之间的文本）中添加、删除或编辑文本。确保您不要编辑或删除这些标签。

+   在 HTML 代码的主要部分，您可以在每个段落（即 `<p>` 和 `</p>` 标签之间的文本）中添加、删除或编辑文本。确保您不要编辑或删除这些标签。

+   在 HTML 代码的主要部分，您可以通过输入 `<section>` 标签后跟 `</section>` 标签来添加一个新部分。在这些标签之间，您可以添加一个标题（一些在 `<h2>` 和 `</h2>` 标签之间的文本）和一个段落（一些在 `<p>` 和 `</p>` 标签之间的文本）。

现在，这里有一些 CSS 代码的定制想法：

+   如果您想使您的页面具有不同的最大宽度，将 `max-width` 值更改为 `800px` 以外的值。例如，如果您增加字体大小（如我稍后所述），您可能想增加页面宽度；减小字体大小意味着您可以减小页面宽度。尝试不同的宽度（通常在 600 px 的低端和 1,000 px 的高端之间），直到找到适合您页面的宽度。

+   对于任何颜色值，您可以将现有颜色更改为不同的颜色关键字。请注意，然而，更改单个颜色可能会破坏您的页面配色方案。如果您不喜欢您的页面颜色，请选择一个新的主颜色，然后再次提示 ChatGPT 从该色调创建配色方案。

+   对于任何字体大小值，您可以通过更改数字来增加或减少字体大小。例如，如果您的文本感觉拥挤且难以阅读，尝试通过像素或两个增加字体大小值。只是确保您保留 px 单位。

+   对于任何填充或边距值，您可以通过更改数字来增加或减少填充或边距。例如，如果您的页面内容看起来很拥挤，您可以通过增加填充和/或边距来打开空间。同样，如果您的页面项目看起来彼此不相连，尝试减少边距。在每种情况下，请确保保留 px 单位。

+   要使您的页面代码更易于访问，请考虑将所有 px 测量转换为 rem 测量。默认情况下，1 rem 等于 16 px，因此 20 px 等于 1.25 rem；24 px 等于 1.5 rem；32 px 等于 2 rem；48 px 等于 3 rem；依此类推。rem 单位更易于访问，因为它测量的是相对于浏览器用户在其浏览器设置中定义的默认字体大小的字体大小。

## 摘要

+   几乎所有网页都以包含至少标志、页面标题和页面标语或副标题的页眉开始。

+   大多数网页都以包含至少版权声明和一些社交媒体链接的页脚结束。

+   页面上的每个元素都被一个由四个部分组成的不可见框包围：内容，即框内包含的文本或图像；填充，即内容与边框之间的空白；边框，它沿着填充区域的边缘运行，用线条包围内容和填充；以及外边距，即在顶部、右侧、底部和左侧边框之外添加的额外空白。

+   要在你的页面上包含图像，你需要知道图像文件的名称，并且需要将图像文件存储在与你的网页代码文件相同的文件夹中。

+   要在你的页面上包含社交媒体链接，你需要知道每个社交媒体账户的用户名。

+   为了获得最佳效果，你的页面提示应该尽可能具体，包括颜色、字体大小和标题级别。

+   将生成的 HTML 保存到 index.xhtml 文件中，将生成的 CSS 保存到 ChatGPT 在 HTML 代码中建议的文件名中，通常是 styles.css。

# 5 发布页面帖子

本章涵盖

+   与 ChatGPT 协作发布可折叠的帖子

+   使用 DALL-E 生成新图像

+   指示 ChatGPT 构建在线期刊页面

+   检查和自定义 ChatGPT 网页代码

虽然许多人不喜欢写作，但许多人真正享受将笔尖触及纸张，或者手指敲击键盘的行为。我们中许多人非常喜欢写作，以至于除了我们更“严肃”的写作外，我们还保持着一种定期更新的日记或期刊形式的写作习惯。令人惊讶的是，这些人中有很多人渴望将这些沉思在线发布。事实上，每次我与人谈论构建网页时，最常见的问题无疑是，“我如何开始一个在线期刊/日记/博客？”

幸运的是，如果你已经有一些东西写好了，让 ChatGPT 帮助你创建一个网页，你可以在那里发布你的散文，让全世界都能阅读。你还可以使用 AI 生成网站标志、图标和页面插图等新图像。本章还展示了如何使用 ChatGPT 和 OpenAI 的 DALL-E 图像创建模型组合来生成你页面所需的任何图像。

所有这些信息都包含在一个详细的提示中，你将传递给 ChatGPT 以生成在线期刊页面的代码，你可以在该页面上发布你想要分享的任何写作。本章还提供了对 ChatGPT 生成的代码的高级解释，甚至给出了一些手动定制代码的技巧，以获得你想要的一切。

## 5.1 理解本章的项目

在本章中，你将让 ChatGPT 帮助你构建一个在线期刊的简单网页。最终页面将包括以下组件：

+   包含以下内容的页眉元素：

    +   期刊标志（由 Dall-E 生成）

    +   期刊标题

    +   期刊标语

+   一个主要元素，其中显示期刊条目。每个条目最初只显示其标题，但点击后则显示条目内容。

+   包含版权声明页脚元素。

图 5.1 展示了本章中在 ChatGPT 的帮助下你将构建的页面类型示例。这个页面的简单性意味着你可以轻松地修改它来存储博客或旅行日记的条目、论文、书籍或电影评论、粉丝小说故事，或任何类型的定期写作。

![](img/build-a-website-with-chatgpt-CH05_F01_McFedries3.png)

图 5.1 由 ChatGPT 生成的在线期刊页面

## 5.2 构建在线期刊页面

在为你的在线期刊页面生成代码的提示之前，你需要了解一些关于网页元素手风琴的背景知识，以及如何让 AI 根据文本提示创建新图像。接下来的几个部分将提供详细信息。

### 5.2.1 与手风琴式布局一起工作

本章中你将了解的唯一新网页技术是*手风琴*，这是一个交互式 HTML 元素，使用户能够在仅显示项目标题和项目标题及内容之间切换。手风琴由两个元素组成：

+   *摘要*—一个作为手风琴标题或描述的元素

+   *详细信息*—一个包含手风琴全部内容的元素，包括摘要元素和任何其他你提供的内容（如一篇文章或多个文章、标题、段落、图像等）

手风琴背后的想法是，默认情况下，你首先看到的是摘要元素。例如，图 5.2 显示了一个包含四个手风琴的网页的一部分。每个手风琴目前只显示其摘要元素，如顶部“Hello World!”，这是第一个手风琴的摘要文本。

![](img/build-a-website-with-chatgpt-CH05_F02_McFedries3.png)

图 5.2 一个包含四个手风琴的网页，每个手风琴只显示其摘要文本

注意，每个摘要元素文本左侧的指向右方的箭头。这个箭头表示还有更多内容可用。当你点击一个摘要（或其箭头）时，手风琴展开以显示手风琴的详细信息元素中的所有内容。例如，点击“Hello World!”摘要展开第一个手风琴，如图 5.3 所示。注意，手风琴的箭头现在指向下方，表示手风琴的完整内容已显示。再次点击摘要文本（或箭头）将隐藏详细内容。

![](img/build-a-website-with-chatgpt-CH05_F03_McFedries3.png)

图 5.3 点击第一个摘要元素打开手风琴以显示其全部内容。

要提示 ChatGPT 在你的页面上使用手风琴，你可以包含以下类似的指令：

```py
Include a main section where each entry is an accordion using the HTML summary and details elements. For each entry, the summary text is the entry title and the details include the entry date, followed by the entry text. Please provide four sample entries going back four days from today.
```

使用手风琴的目的在于，你可以在页面上放置相当多的帖子，而不会因为大量内容而使访客感到不知所措。最好的消息是？只需告诉 ChatGPT 你希望在页面上使用手风琴，它就会为你处理所有的 HTML 和 CSS 细节。

### 5.2.2 使用 GPT-4 和 DALL-E 生成图像

GPT-4 能够从相对简单的提示中生成文章、诗歌、电子邮件，当然还有网页代码，这令人愉快且令人惊叹。然而，如果有一个功能使 GPT-4 “难以区分于魔法”（用亚瑟·C·克拉克的话说），那就是模型将自然语言转换为图像的能力。也就是说，给定一个描述某物（场景、物体、人物等）的文本提示，GPT-4 可以使用该描述生成与之匹配的图像。

这项看似神奇的壮举背后的工具是 DALL-E（结合了 *WALL-E* 电影标题和艺术家萨尔瓦多·达利的姓氏），这是一个针对将自然语言文本描述转换为图像进行优化的 OpenAI 模型。

警告 如您在接下来的章节中所学，DALL-E 在将文本转换为图像方面相当出色，但**仅此而已**。它很少会直接生成您可以直接使用的图像。您可能需要自己使用图形程序调整图像，或者请图形专业人士帮助修改 DALL-E 图像，或者将生成的图像作为最终设计的原型。

访问 DALL-E

您有两种方式可以访问 DALL-E：

+   *OpenAI DALL-E 应用程序*—此应用程序通过您的 OpenAI 账户直接访问 DALL-E。有几个方法可以访问该应用程序（如图 5.4 所示）：

    +   访问 [`openai.com`](https://openai.com)，点击菜单，点击登录，然后登录您的 OpenAI 账户。在出现的 OpenAI 工具选择中，点击 DALL-E。

    +   访问 [`openai.com/dall-e-2`](https://openai.com/dall-e-2)，点击“尝试 DALL-E”，然后登录您的 OpenAI 账户。

![图片](img/build-a-website-with-chatgpt-CH05_F04_McFedries3.png)

图 5.4 OpenAI DALL-E 应用程序

+   *协作者图像创建器*—使用 Microsoft Edge，访问 [`www.bing.com/images/create`](https://www.bing.com/images/create)（参见图 5.5）或 [`copilot.microsoft.com/images/create`](https://copilot.microsoft.com/images/create)；或者在 Copilot 中，将您的提示直接指向图像创建器（例如，`Ask Image Creator for an image of a dog running on the moon`）。

![图片](img/build-a-website-with-chatgpt-CH05_F05_McFedries3.png)

图 5.5 协作者图像创建器

注意 通过 Open AI 应用程序使用 DALL-E 是不免费的。要使用它，您需要购买积分，其中一张积分可用于一个 DALL-E 请求。在我写这篇文章的时候，您可以通过您的 OpenAI 账户以 15 美元的价格购买 115 张积分。请注意，通过 Microsoft Copilot 使用 DALL-E 是免费的。

指示 DALL-E

让 DALL-E 生成令人满意的图像本身就是一种艺术。DALL-E 新手犯的最大错误是将应用程序当作聊天机器人，并给它提供您希望它执行的操作的指令。相反，假设您的图像已经存在，您所写的是为盲人或视力有其他障碍的人提供的详细描述，这些障碍使他们无法看到图像。

在您的描述中，不仅要包括您想要在图像中看到的元素，还要包括一个或多个（通常越多越好）关键词，以指定图像的确切风格。以下是一些想法：

+   *情绪*—使用唤起积极情绪（*明亮，* *轻快，* *生动，* *平和*）或消极情绪（*忧郁，* *黑暗，* *柔和，* *忧郁，* *暴风雨*）的关键词。

+   *整体美学*—例如，*哥特式，* *蒸汽朋克，* *赛博朋克，* *后末日，* *非洲未来主义*。

+   *媒介*—例如，*摄影，* *插图，* *绘画，* *卡通*。

+   *媒介的具体细节*—一些示例：

    +   *摄影*—电影类型（*彩色，* *黑白*），环境（*室内，* *室外*），照明，角度（*长，* *中，* *特写*），景深（*浅，* *深*）。

    +   *插图*—媒介（*铅笔，* *墨水，* *炭笔，* *模板，* *蜡笔*等）和风格（*数字艺术，* *拼贴，* *动漫，* *装饰艺术，* *包豪斯*等）。

    +   *绘画*—媒介（*水彩，* *油画*等）和风格（*印象派，* *风格主义，* *象征主义，* *新艺术*等）。

注意：到您阅读本文时，DALL-E 的最新版本（DALL-E 3）应该已经普遍可用。这是个好消息，因为与 DALL-E 的先前版本相比，这个最新版本在渲染文本方面要好得多。如果您的图像需要文本，请将其包含在您的描述中。但是，请仔细检查生成的图像文本，因为 DALL-E 3 经常要么省略一个字母，要么添加一个额外的字母。

为了让您了解如何提示 DALL-E 工作，通过几个示例进行操作是有帮助的。对于我的在线日记页面，我向 Copilot 提示如下：

```py
Please ask image creator to create a cartoon of a cow standing on two legs with a text bubble over the cow's head that says "Moo".
```

图 5.6 展示了我收到的图像。左上角的那个相当不错！

![](img/build-a-website-with-chatgpt-CH05_F06_McFedries3.png)

图 5.6 展示了根据我的提示由 Image Creator 生成的卡通。

以下是一个包含关键词`medium shot`和`fluorescent lighting`的摄影提示示例：

```py
A photograph of a golden retriever browsing in a library, medium shot, fluorescent lighting.
```

图 5.7 展示了 DALL-E 根据这个提示生成的图像。

![](img/build-a-website-with-chatgpt-CH05_F07_McFedries3.png)

图 5.7 DALL-E 生成的摄影图像

以下是一个使用关键词`post-apocalyptic`和`desolate`的数字艺术插图提示：

```py
A digital art illustration of an old-fashioned diner in a post-apocalyptic, desolate street scene.
```

图 5.8 展示了从该提示生成的 DALL-E 图像示例。

![](img/build-a-website-with-chatgpt-CH05_F08_McFedries3.png)

图 5.8 展示了 DALL-E 生成的插图。

以下是一个使用关键词`bright`和`lavish`的插图提示：

```py
A bright, lavish, illuminated manuscript page that includes "Lorem ipsum" text and drawings of cats in the margins.
```

图 5.9 展示了 DALL-E 根据这个提示创建的图像。

![](img/build-a-website-with-chatgpt-CH05_F09_McFedries3.png)

图 5.9 展示了 DALL-E 生成的带有猫的插图。

如果 DALL-E 生成了一个您想要使用的图像（无论是用于编辑还是作为原型），您的下一步是将该图像保存到您的电脑上。

保存生成的图像

一旦您有了想要在网页上使用的图像，您需要将该图像保存到您的电脑上：

+   *OpenAI DALL-E app*—点击图片，点击图片右上角出现的三个点 (...) 按钮，然后点击下载。

+   *Copilot Image Creator*—点击图片，然后点击下载。

无论哪种方式，图片都会出现在您的电脑下载文件夹中。将图片文件移动到包含您的 HTML 和 CSS 文件（您将在下一节中创建）的同一文件夹中，然后使用您首选的文件名重命名图片。

现在您已经知道如何让 ChatGPT 帮助您编写和编辑文本以及生成图像，您就可以构建生成在线期刊网页代码的提示了。

### 5.2.3 构建提示

本章的项目是一个在线期刊页面。在继续之前，您应该有以下准备：

+   页面标志、标题和标语。

+   您想要用于页面标题和页面文本的字体名称。

+   您想要应用于页面背景和文本的颜色名称。

参考第三章了解这些设计元素以及如何提示 ChatGPT 获取标题、字体和颜色建议。

即使您没有要发布的写作，您也可以通过提示 ChatGPT 生成您的在线期刊 HTML 和 CSS 的过程，因为代码将包括您的文本占位符。您需要立即让 ChatGPT 知道您希望它帮助您构建网页，并且您不知道如何编码，因此它将为您生成代码。这一切都是通过以下方式开始的：

```py
I want to build a web page for an online journal. I don't know how to code, so I need you to provide the code for me.

First, write the HTML code for a web page that includes the following:
```

您然后指定页面内容，包括以下内容（参见图 5.10）：

+   包含您的标志、页面标题和标语的头。

+   主要元素，其中每个条目都是一个使用 HTML 的`summary`和`details`元素的折叠面板。

+   对于每个条目，`summary` 文本是条目标题，而`details` 元素包括条目日期和条目文本。

+   包含版权声明的页脚。

![图片](img/build-a-website-with-chatgpt-CH05_F10_McFedries3.png)

图 5.10 在线期刊页面的部分

接下来，您要求 ChatGPT 生成您想要页面格式的 CSS：

```py
Second, in a separate file please write the CSS code for the following:
```

您然后指定格式，包括以下内容：

+   页面背景颜色和文本颜色。

+   您想要用于页面标题和标语的字体大小。

+   `summary` 元素的字体大小。

+   用于标题、摘要和常规页面文本的字体。

+   页面的最大宽度。这可以防止文本行过长。对于大多数页面，850 px 的最大长度是合适的。

这是我自己的在线期刊页面的一个示例提示：

```py
I want to build a web page for an online journal. I don't know how to code, so I need you to provide the code for me.

First, write the HTML code for a web page that includes the following:
 * A header element that includes an image named logo.png, the title "The Moo Point", and the tagline "It's like a cow's opinion, you know, it just doesn't matter. It's moo."
 * A main section where each entry is an accordion using the HTML summary and details elements.
 * For each entry, the summary text is the entry title and the details include the entry date, followed by the entry text.
 * Please provide four sample entries going back four days from today.
 * A footer element that includes the Copyright symbol, followed by the current year, followed by "Paul McFedries".
 * In the page head section, include the tag <meta charset="utf-8">.

Second, in a separate file write the CSS code for the following:
 * The page background color is mintcream.
 * The page text color is slategray.
 * Make the image a maximum width of 150px and floated to the left.
 * The title font size is 48px.
 * The tagline font size is 22px and formatted as italic.
 * The summary font size is 30px.
 * The main section font size is 20px with a top margin of 48px.
 * Make the date of each entry dark blue with font size 18px.
 * For the headings and summary text, use the Lato font from Google Fonts. For the rest of the text, use the Merriweather font from Google Fonts.
 * The footer has 5px padding all around and a 10px top margin.
 * Make the page responsive with a maximum width of 850px.
 * Style the accordions to make them look nicer, including a powderblue background color.
```

ChatGPT 应首先创建 HTML 代码，您可以复制并粘贴到名为 index.xhtml 的文件中。在该代码中，您应该看到类似以下内容的行：

```py
<link rel="stylesheet" type="text/css" href="styles.css">
```

这段代码告诉浏览器在名为 styles.css 的文件中查找 CSS 代码，因此你的下一个任务是复制生成的 CSS 代码，将其粘贴到文件中，并保存为 styles.css（或你在`<link>`标签中看到的任何名称）。确保将 styles.css 保存与你的 index.xhtml 文件相同的文件夹中。你还需要将你的图片文件复制到同一个文件夹。有关更多关于工作网页文件的信息，请参阅附录 A。

我使用 OpenAI 的 ChatGPT 应用向 GPT-4 提交了这个提示。它生成的代码导致了图 5.11 所示的页面。

![](img/build-a-website-with-chatgpt-CH05_F11_McFedries3.png)

图 5.11 ChatGPT 生成的我的在线期刊页面

注意：为了得到图 5.11 所示的页面，我不得不纠正 ChatGPT 在 CSS 代码中犯的一个错误。我将在下一节中讨论这个错误。

如果你喜欢 ChatGPT 为你制作的在线期刊，你可以跳过本章的其余部分，并按照附录 B 中描述的方式部署代码。但是，如果你想更多地了解 ChatGPT 生成的代码，下一节将为你提供更详细的了解。

## 5.3 检查代码

如果你对 ChatGPT 生成的代码感到好奇，在本节中，我将为你提供一个简短且不太技术性的概述，介绍由我上一节提示生成的在线期刊代码（如图 5.11 所示的期刊页面）。你生成的 ChatGPT 代码将不同于我的，不仅因为你的文本和图片不同，还因为

+   ChatGPT 的算法包括一些内置的随机性，因此相同的提示每次运行时通常会生成略微不同的代码。

+   ChatGPT 的输出取决于模型（GPT-3.5 与 GPT-4）和应用（OpenAI 与 Copilot）。对于 Copilot，输出还取决于对话风格（创意、平衡或精确）。

注意：我在线期刊页面的生成 HTML 和 CSS 代码可在本书的网站上找到（[www.manning.com/books/build-a-website-with-chatgpt](https://www.manning.com/books/build-a-website-with-chatgpt)）以及本书的 GitHub 仓库：[`github.com/paulmcfe/websites-with-chatgpt`](https://github.com/paulmcfe/websites-with-chatgpt)。

然而，ChatGPT 的每个版本都应该输出至少与下一两个部分显示的类似的 HTML 和 CSS 代码，因此我的代码注释应该能帮助你理解底层发生了什么。

### 5.3.1 检查 HTML

这里展示了 ChatGPT 为我在线期刊页面生成的 HTML 代码：

```py
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">                                   ①
        <title>The Moo Point</title>
        <link rel="stylesheet" 
              href="styles.css">                                 ②
        <link rel="preconnect" 
              href="https://fonts.googleapis.com">               ③
        <link rel="preconnect"                                   ③
              href=https://fonts.gstatic.com                     ③
              crossorigin>                                       ③
        <link href="https://fonts.googleapis.com/css2?           ③
        family=Lato:wght@400;700&family=Merriweather:            ③
        ital,wght@0,400;0,700;1,400&                             ③
        display=swap" rel="stylesheet">                          ③
    </head>
    <body>
        <header>                                                 ⑦
            <img src="logo.png" alt="Logo">                      ④⑤
            <h1 class="title">The Moo Point</h1>                 ⑤⑦
            <p class="tagline">                                  ⑥⑦
                It's like a cow's opinion, you know, it          ⑦
                just doesn't matter. It's moo.                   ⑦
            </p>                                                 ⑥⑦
        </header>                                                ⑦

        <main>
            <details>                                            ⑪
                <summary class="entry-title">                    ⑧⑪
                    Title of Entry 1                             ⑪
                </summary>                                       ⑧⑪
                <p class="entry-date">24 July 2023</p>           ⑨⑪
                <p class="entry-text">Entry text goes here.</p>  ⑩⑪
            </details>                                           ⑪

            <details>
                <summary class="entry-title">Title of Entry 2</summary>
                <p class="entry-date">25 July 2023</p>
                <p class="entry-text">Entry text goes here.</p>
            </details>

            <details>
                <summary class="entry-title">Title of Entry 3</summary>
                <p class="entry-date">26 July 2023</p>
                <p class="entry-text">Entry text goes here.</p>
            </details>

            <details>
                <summary class="entry-title">Title of Entry 4</summary>
                <p class="entry-date">27 July 2023</p>
                <p class="entry-text">Entry text goes here.</p>
            </details>
        </main>

        <footer>                                                 ⑫
            <p>&copy; 2023 Paul McFedries</p>                    ⑫
        </footer>                                                ⑫
    </body>
</html>
```

① 指定页面字符集

② 告诉浏览器在哪里找到 CSS 代码

③ 从 Google Fonts 加载页面字体

④ 页面标志

⑤ 页面标题

⑥ 页面标语

⑦ 页眉

⑧ 条目摘要（标题）

⑨ 条目日期

⑩ 条目文本

⑪ 详细信息元素

⑫ 页脚

在阅读 HTML 代码时，请注意以下几点：

+   HTML 文件中`<head>`标签之后立即的代码`<meta charset="utf-8">`告诉浏览器页面使用的字符集。您不需要知道这意味着什么，只需知道这个标签是使版权符号正确显示所必需的。如果您在日记条目中使用像破折号（—）和括号引号（“和”）这样的字符，它也会帮助这些字符正确显示。

+   此代码使用占位文本为条目，因此您需要为每个条目添加自己的标题、日期和文本。

+   如果页面的标语听起来很熟悉，那是一句从老电视剧《老友记》中的角色乔伊那里借来的。

最后，请注意 HTML 代码中包含以下行：

```py
<link rel="stylesheet" href="styles.css">
```

这个标签告诉网络浏览器在哪里找到 CSS 代码，我将在下一节中描述。

### 5.3.2 检查 CSS

ChatGPT 为我在线日记页面生成的 CSS 代码如下所示：

```py
body {
    background-color: mintcream;               ①
    color: slategray;                          ①
    font-family: 'Merriweather', serif;        ①
    max-width: 850px;                          ②
    margin: 0 auto;                            ③
}
img {
    max-width: 150px;                          ④
    float: left;                               ④
}
h1 {
    font-size: 48px;                           ⑤
    font-family: 'Lato', sans-serif;           ⑤
}
p.tagline {
    font-size: 22px;                           ⑥
    font-style: italic;                        ⑥
}
main {
    margin-top: 48px;
}
.summary, .entry-title {
    font-size: 30px;                           ⑦
    font-family: 'Lato', sans-serif;           ⑦
}
.date {
    color: darkblue;                           ⑧
    font-size: 18px;                           ⑧
}
footer {
    padding: 5px;
    margin-top: 10px;
}
details {                                      ⑨
    background: powderblue;
    margin: 5px 0;
    border: 1px solid #aaa;
    border-radius: 4px;
    padding: .625em .625em .625em .625em;
    width: 100%;
}
summary {
    font-weight: bold;
    margin: -.625em -.625em 0;
    padding: .625em;
}
details[open] {
    padding: .625em;
    border: 1px solid #aaa;
}
details[open] summary {
    border-bottom: 1px solid #aaa;
    margin-bottom: .625em;
}    #I
```

① 设置页面背景色、文字颜色和字体

② 设置最大页面宽度为 850 px

③ 使页面居中

④ 设置最大标志宽度，并将其浮动到左侧

⑤ 设置页面标题字体大小为 48 px，并应用 Lato 字体

⑥ 使用 22 px 字体大小和斜体样式标语

⑦ 使用 30 px 字体大小和 Lato 字体样式条目标题

⑧ 使用深蓝色和 18 px 字体大小样式条目日期

⑨ 为手风琴应用特殊样式

幸运的是，ChatGPT 在生成 HTML 和 CSS 代码时很少出错，但在这个案例中，它确实犯了错。要查看错误，首先查看以下 HTML 代码中的以下行（每个条目都有类似的行）：

```py
<p class="entry-date">24 July 2023</p>
```

在这个`<p>`标签中，`class`属性指的是应用于段落的 CSS 样式集。在这个例子中，类名是`entry-date`。在 CSS 代码中，类样式通过在类名前添加一个点(`.`)来指定。然而，您可以整天浏览 CSS 代码，但您不会找到任何以`.entry-date`开头的 CSS 规则。最接近的是`.date`，这意味着 ChatGPT 犯了一个错误。（您如何知道？在这种情况下，您会通过查看页面并注意到条目日期没有按照提示中指定的`darkblue`颜色格式化来知道。）在 CSS 中，您可以通过将`.date`更改为`.entry-date`来修复这个问题。

如果您愿意，可以使用本节前面部分的注释来调整您的网页代码，正如我接下来要描述的。

## 5.4 自定义页面

如果您对 ChatGPT 为您生成的页面不满意，一个可能的解决方案是修改您的提示并重新提交。然而，对于相对较小的自定义，手动编辑代码通常更容易。

首先，这里有一些 HTML 代码的自定义建议：

+   在页眉中，您可以编辑标题或标语。只需确保不要编辑或删除相关的 HTML 标签：用于标题的`<h1>`和`</h1>`，以及用于标语的`<p>`和`</p>`。

+   要添加一个新条目（即，一个新的手风琴），请按照以下步骤操作：

a) 在文本编辑器中打开 HTML 文件。

b) 选择一个现有条目。也就是说，选择包括单个`<details>`和`</details>`标签之间的所有内容，如图 5.12 所示。

![图片](img/build-a-website-with-chatgpt-CH05_F12_McFedries3.png)

图 5.12 选择现有的手风琴条目。

c) 复制条目（例如，通过按 Ctrl-C 或 Cmd-C）。

d) 在你想要新条目出现的位置创建一个新行。例如，如果你想新条目出现在现有条目之上，将光标立即放在第一个`<details>`标签之前，然后按 Enter 或 Return。

e) 将光标定位在你刚刚创建的新行上，如图 5.13 所示。

![图片](img/build-a-website-with-chatgpt-CH05_F13_McFedries3.png)

图 5.13 将光标定位在你想要粘贴你复制的代码的位置。

f) 粘贴复制的代码（例如，通过按 Ctrl-C 或 Cmd-C）。

g) 编辑条目标题、日期和文本。

+   如果你的条目文本包含多个段落，你可以通过在开始和结束处分别添加`<p class="entry-text">`标签和`</p>`标签来确保每个段落正确渲染：

    ```py
    <main>
        <details>
            <summary class="entry-title">Title of Entry 1</summary>
            <p class="entry-date">24 July 2023</p>
            <p class="entry-text">Entry text goes here.</p>
            <p class="entry-text">Another paragraph goes here.</p>
            <p class="entry-text">You can keep going if you want.</p>
        </details> 
    ```

+   在 HTML 代码的页脚部分，你可以添加指向你的社交媒体账户的链接，正如我在第四章中描述的那样。

现在，这里有一些 CSS 代码的定制想法：

+   要格式化每个条目的文本，请将`.entry-text { }`添加到你的 CSS 代码底部，并填充你想要的格式。例如，以下代码调整条目字体大小：

    ```py
    .entry-text {
        font-size: 20px;
    }
    ```

+   如果你想你的页面有不同的最大宽度，将`max-width`值更改为`850px`以外的值。

+   对于任何颜色值，你可以将现有颜色更改为不同的颜色关键字。

+   对于任何字体大小值，你可以更改数字以增加或减少字体大小。只需确保保留`px`单位。

+   对于任何填充或边距值，你可以更改数字以增加或减少填充或边距。在每种情况下，务必保留`px`单位。

+   要使你的页面代码更易于访问，考虑将所有 px 测量转换为 rem 测量。默认情况下，1rem 相当于 16px，因此 20px 是 1.25rem，24px 是 1.5rem，32px 是 2rem，48px 是 3rem，依此类推。rem 单位更易于访问，因为它测量的是相对于浏览器用户在其浏览器设置中定义的默认字体大小的字体大小。

## 摘要

+   手风琴是一个特殊的 HTML 功能，它由摘要（手风琴的标题或描述）和细节（手风琴内容的全部）组成。

+   点击手风琴摘要可以切换手风琴内容的隐藏和显示状态。

+   要让 AI 根据文本提示生成图像，可以使用 OpenAI 的 DALL-E 应用或 Copilot 的图像创建器。

+   在请求图像时，使用关键词来唤起整体情绪和美学、媒介以及媒介的具体细节。

+   为了获得最佳效果，你的页面提示应该尽可能具体，包括颜色、字体大小和标题级别。

+   将生成的 HTML 保存到 index.xhtml 文件中，将生成的 CSS 保存到 HTML 代码中 ChatGPT 建议的文件名，通常是 styles.css。

# 6 添加链接和导航

本章涵盖

+   创建到其他网站和页面的链接

+   为你的网站创建导航栏

+   让 ChatGPT 帮助你设计页面

+   指示 ChatGPT 为组织构建信息网站

+   检查和自定义 ChatGPT 的网页代码

在本书中你迄今为止看到的每个网络项目中，你都巧妙地让 ChatGPT 为你提供单个网页的代码。网络上有一大堆单页网站，但一个网站拥有两个或更多页面更为常见。然而，一旦添加了第二个页面，问题很快就会出现：你如何将网站访客从主页引导到其他页面？一旦有人到达那个其他页面，你如何让他们回到主页？如何在一个拥有三页、四页甚至更多页面的网站上解决这个问题呢？

回答这些问题以及类似的问题是本章的主题。在接下来的页面中，你将学习如何通过让 ChatGPT 编写一些网页代码来创建一个可点击的链接到另一个页面，从而让访问你网站的访客能够从一个页面跳转到另一个页面。你还将学习如何让 ChatGPT 创建一个特殊的网页元素，称为导航栏，将所有网站页面的链接汇总到一个方便的位置，以便轻松访问。

所有这些信息都包含在一个详细的提示中，然后你将传递给 ChatGPT 以生成一个非常常见的项目模式的代码：一个提供组织信息的网站。本章还提供了 ChatGPT 生成的代码的高级解释以及手动自定义代码的指南，以获得你想要的一切。

## 6.1 理解本章的项目

在本章中，你将让 ChatGPT 帮助你为组织构建一个简单的信息网站。最终页面将包括以下组件：

+   包含网站标题和标语的头元素

+   包含链接到网站其他页面的导航元素

+   包含网站介绍以及一些吸引读者内容的主要元素

+   包含版权声明的页脚元素

图 6.1 展示了由 ChatGPT 生成的信息网站主页的示例。这种类型的网站可以很容易地修改，用作社区、慈善机构、活动、团队或乐队的信息网站，甚至是一部喜欢的电影或电视剧。

![图片](img/build-a-website-with-chatgpt-CH06_F01_McFedries3.png)

图 6.1 ChatGPT 生成的信息网站主页

## 6.2 构建信息网站主页

信息网站包含多个网页，因此分阶段构建网站是个好主意。我推荐的过程总结如下：

1.  指示 ChatGPT 生成网站主页的 HTML 代码。

1.  提示 ChatGPT 生成网站的 CSS 样式代码。请注意，最好将这两个步骤合并为一个提示。

1.  对于你的其他网站页面，提示 ChatGPT 生成该页面的 HTML 代码。特别是，其他网站页面的提示应包括以下内容：

    +   指示使用与步骤 2 中保存的 CSS 生成的 CSS 文件相同的 CSS 文件。

    +   指示不要生成任何额外的样式，尤其是内联样式（即直接插入 HTML 标签中的 CSS 代码）。ChatGPT 总是希望将其 HTML 输出与 CSS 样式一起包含，因此如果没有这个指示，ChatGPT 几乎肯定会添加额外的样式，这可能会与或覆盖 CSS 文件中的样式。

在你了解所有这些之前，花一分钟时间熟悉本章中介绍的新网页技术。

### 6.2.1 创建链接

HTML（实际上，它是*HTML*中的*H*）的一个显著特征是*超文本*，这只是一个更华丽的词，指的是带你去其他页面的链接，无论这些页面是否存在于你的网站上或互联网上的任何地方。链接通常是一个配置为当有人点击该文本时，网络浏览器会导航到链接配置指定的任何网页的单词或短语。

如果你正在链接到与当前 HTML 文件相同的目录中的网站页面，你可以要求 ChatGPT 提供对该文件名的链接。以下是一些请求名为 about.xhtml 的页面的代码：

```py
Provide the HTML code for a link to a web page named about.xhtml.
```

图 6.2 显示了 ChatGPT 应用输出的结果。以下是 ChatGPT 返回的 HTML 代码：

```py
<a href="about.xhtml">About</a>
```

![图片](img/build-a-website-with-chatgpt-CH06_F02_McFedries3.png)

图 6.2 ChatGPT 为 about.xhtml 页面生成的代码

如代码所示，你用来创建链接的 HTML 标签是`<a>`及其相应的`</a>`闭合标签。在`a`元素中，你使用`href`属性来插入链接的地址——通常称为*URL*（即*统一资源定位符*）——图 6.3 显示了该元素的工作方式。

![图片](img/build-a-website-with-chatgpt-CH06_F03_Mcfedries3.png)

图 6.3 `<a>`标签的语法

如果你想要链接的文件位于你的网站上的不同目录中，你需要在你的提示中包含该目录名：

```py
Provide the HTML code for a link to a web page named index.xhtml in the /faq directory.
```

图 6.4 显示了 ChatGPT 应用输出的结果。以下是 ChatGPT 返回的 HTML 代码：

```py
<a href="/faq/index.xhtml">FAQ</a>
```

![图片](img/build-a-website-with-chatgpt-CH06_F04_McFedries3.png)

图 6.4 ChatGPT 为/faq 目录中的 index.xhtml 页面生成的代码

注意，我在目录名前加了一个斜杠(`/`)，这告诉 AI 指定的目录是从网站根目录开始的。如果你要链接的文件位于当前 HTML 文件所在的目录的子目录中，请在提示中省略斜杠。

对于外部网页，通常最简单的方法是创建一个空链接（即`<a href="">链接文本</a>`），浏览到该页面，复制地址，然后将该地址粘贴到`href`属性值的引号之间。然而，如果页面可以描述——例如，您知道网站的名称，并且可以用几个词独特地描述页面内容——为什么不请您的 AI 助手为您做这项工作呢？以下是一个示例：

```py
Provide the HTML code for a link to the Wikipedia page on rutabagas.
```

图 6.5 显示了 ChatGPT 应用输出的结果。以下是 ChatGPT 返回的 HTML 代码：

```py
<a href="https://en.wikipedia.org/wiki/Rutabaga">Rutabaga</a>
```

![](img/build-a-website-with-chatgpt-CH06_F05_McFedries3.png)

图 6.5 ChatGPT 为维基百科中 rutabagas 页面的链接代码

### 6.2.2 创建导航栏

一个非常常见的网站模式是*导航栏*，它是一组指向网站其他页面（或如果网站很大，则指向网站最重要的页面）的链接。导航栏可以是水平的或垂直的，但最常见的配置是在页眉下方横跨页面的水平条。图 6.6 显示了示例。

![](img/build-a-website-with-chatgpt-CH06_F06_McFedries3.png)

图 6.6 导航栏示例

在 HTML 中，您可以使用`<nav>`和`</nav>`标签创建一个导航栏。在这些标签之间，您添加指向每个网站页面的链接。您可以通过在提示中包含以下指令来要求 ChatGPT 生成一个类似的导航栏：

```py
Create a navigation element that includes five links:
* The text "Home" that links to the file "index.xhtml".
* The text "Blog" that links to the file "blog.xhtml".
* The text "FAQ" that links to the file "faq.xhtml".
* The text "About" that links to the file "about.xhtml".
* The text "Contact" that links to the file "contact.xhtml".
```

根据这个指令，ChatGPT 将生成类似于以下 HTML 代码（这是创建图 6.6 中显示的导航栏的代码）：

```py
<nav>
    <a href="index.xhtml">Home</a>
    <a href="blog.xhtml">Blog</a>
    <a href="faq.xhtml">FAQ</a>
    <a href="about.xhtml">About</a>
    <a href="contact.xhtml">Contact</a>
</nav>
```

您可能会注意到图 6.6 中浏览器渲染列表的两种奇怪之处：

+   列表水平排列，而不是垂直排列。

+   列表项在页面中均匀分布。

浏览器以这种方式渲染导航栏，是因为以下 CSS 代码将一些属性应用于`nav`元素：

```py
nav {
    border-top: 1px solid midnightblue;        ①
    border-bottom: 1px solid midnightblue;     ①
    display: flex;                             ②
    justify-content: space-between;            ③
    margin: 20px 0;                            ④
    padding: 10px 0;                           ④
}
```

① 在`nav`元素上方和下方添加边框

② 将`nav`元素转换为 Flexbox 容器

③ 告诉浏览器均匀分配项目空间

④ 设置`nav`元素的边距和填充

这里需要注意的主要是`display: flex`声明，它将`nav`元素转换为 Flexbox 容器。默认情况下，它水平显示其项目，而不是垂直显示。（您将在第十章中了解更多关于 Flexbox 的内容。）

注意：根据导航栏中元素的数量，该元素可能太宽，无法在小屏幕上良好渲染，尤其是竖屏模式的智能手机屏幕。通常的解决方案是将导航元素转换为图标，当点击或轻触时显示菜单。要了解如何提示 ChatGPT 生成此类菜单的代码，请参阅第十二章。

现在，您已经拥有了创建 ChatGPT 主页提示所需的所有知识。

### 6.2.3 构建主页提示

本章的项目是一个信息网站。在继续展示提示部分之前，请确保您已经具备以下项目：

+   以下之一或全部：页面标志、标题和标语

+   您想要用于页面标题和页面文字的字体名称

+   您想要应用于页面背景和文字的颜色关键词

参考第三章了解这些设计元素以及如何提示 ChatGPT 提供标题、字体和颜色建议。

您现在可以请 ChatGPT 帮助您生成信息网站主页的代码。您的提示应该开始如下：

```py
I want to build a web page for an information website. I don't know how to code, so I need you to provide the code for me.
First, write the HTML code for a web page that includes the following:
```

您随后指定页面的内容，包括以下内容（参见图 6.7）：

+   包含您的网站标题和标语的页眉

+   一个包含链接到其他网站页面（或网站的主要页面）的导航元素

+   一个包含欢迎访问者到网站的引言段落的主体元素

+   一个或多个用于向读者展示引人入胜内容的章节元素

+   包含版权声明的页脚

![](img/build-a-website-with-chatgpt-CH06_F07_McFedries3.png)

图 6.7 信息网站主页的元素

接下来，您要求 ChatGPT 生成您想要页面格式的 CSS：

```py
Second, in a separate file please write the CSS code for the following:
```

您随后指定格式，包括以下内容：

+   页面的背景颜色和文字颜色

+   您想要用于页面标题和标语的字型大小

+   标题和页面文字的字型大小

+   用于标题和常规页面文字的字体

+   页面的最大宽度。这可以防止文字行过长。对于这种类型的网站，800 像素的最大长度是合适的。

这是我自己的信息页面的一个示例提示：

```py
I want to build a home page for an information website. I don't know how to code, so I need you to provide the code for me.

First, write the HTML code for a web page that includes the following:
 * The page title is "Antediluvian Word Preservation Society".
 * A header that includes the title "Antediluvian Word Preservation Society" and the tagline "Preserving words from the past, for the future".
 * After the header, a navigation element that includes five links:
   * The text "Home" that links to the file "index.xhtml".
   * The text "Blog" that links to the file "blog.xhtml".
   * The text "FAQ" that links to the file "faq.xhtml".
   * The text "About" that links to the file "about.xhtml".
   * The text "Contact" that links to the file "contact.xhtml".
 * A main element that includes the following:
   * An introductory paragraph that includes the text "Welcome to the Antediluvian Word Preservation Society, where our goal is to protect, preserve, and promote old words that are in danger of becoming overlooked, outmoded, and obsolete. Stay a while, take a look around, and bask in the burnished sheen of these old and beautiful words."
  * A section element with the second-level heading "Most recent word", followed by a third-level heading with the text "*hullaballoo* (hul·uh·buh·LOO, noun)", followed by a paragraph that includes the text "A great noise or commotion; an uproar. (Example: "After hearing the **hullaballoo** that eight kids hopped up on sugar could make, Rupert decided to never again volunteer to help out at a Halloween party.") [etc.]."
  * Another section element with the second-level heading "This week's challenge" followed by a paragraph that includes the text "Your challenge this week is to use the word *tomfoolery* — foolish or silly behavior — at least once in each of the following: in conversation, in an email message, in a text message, and in a business meeting (virtual or real-world). Good luck and let us know how you make out!"
  * In the above text, make each word that's surrounded by double asterisks bold, and make each word that's surrounded by single asterisks italic. 
 * A footer element that includes the Copyright symbol, followed by the current year, followed by "Antediluvian Word Preservation Society".
 * In the page head section, include the tag <meta charset="utf-8">.

Second, in a separate file write the CSS code for the following:
 * The body element has 25px padding and a background color of oldlace.
 * Make the title 64px, line height 1, color midnightblue, 20px bottom margin, and the Playfair Display typeface from Google Fonts.
 * Make the tagline font size 30px.
 * The navigation element has a top and bottom border colored midnightblue.
 * The navigation element has 20px top and bottom border and 10px top and bottom padding.
 * Style the navigation links with font size 24px;
 * Space the navigation links so that they span the entire width of the body.
 * Style the second-level headings with size 48px, 30px top margin, 10px bottom margin, the color midnightblue, and the Playfair Display typeface from Google Fonts.
 * Style the rest of the page text with size 24px, the color darkslategray, and the Lora typeface from Google Fonts.
 * Style the links with the color steelblue and no underline.
 * The footer has 10px top and bottom padding, a 50px top margin, and a top and bottom border colored midnightblue.
 * The page has a maximum width of 800px and is centered within the browser window.
```

ChatGPT 应首先创建 HTML 代码，您可以复制然后粘贴并保存到一个名为 index.xhtml 的文件中。在这段代码中，您应该看到顶部附近有一行类似于以下的内容：

```py
<link rel="stylesheet" type="text/css" href="styles.css">
```

这段代码告诉网络浏览器在名为 styles.css 的文件中查找 CSS 代码，因此您的下一个任务是复制生成的 CSS 代码，将其粘贴到文件中，并保存为 styles.css（或 `<link>` 标签中显示的任何名称）。请确保将 styles.css 保存与您的 index.xhtml 文件相同的文件夹中。您还需要将您的图像文件复制到同一个文件夹中。参考附录 A 了解更多关于处理网页文件的信息。

我使用 OpenAI 的 ChatGPT 应用程序向 GPT-4 提交了这个提示。它生成的代码导致了图 6.8 所示的页面。

![](img/build-a-website-with-chatgpt-CH06_F08_McFedries3.png)

图 6.8 ChatGPT 生成的我的信息网站主页

如果您喜欢 ChatGPT 为您制作的网站信息，您可以跳过本章的其余部分，并按照附录 B 中描述的方式部署代码。但是，如果您想了解更多关于 ChatGPT 生成的代码的信息，下一节将为您提供一个更详细的了解。

## 6.3 检查主页代码

如果你好奇 ChatGPT 生成的代码，在本节中，我将为你提供一个关于上一节（信息网站主页如图 6.8 所示）提示生成的信息网站代码的简要且非技术性的概述。

注意：本书网站上提供了我的信息网站主页的生成 HTML 和 CSS 代码（[www.manning.com/books/build-a-website-with-chatgpt](https://www.manning.com/books/build-a-website-with-chatgpt)）以及 GitHub 仓库中的代码：[`github.com/paulmcfe/websites-with-chatgpt`](https://github.com/paulmcfe/websites-with-chatgpt)。

ChatGPT 的每个版本都应该输出至少与下一两个部分显示的 HTML 和 CSS 代码相似的代码，因此我的代码注释应该能帮助你理解底层发生了什么。

### 6.3.1 检查 HTML

下面展示了 ChatGPT 为我信息网站主页生成的 HTML 代码：

```py
<!DOCTYPE html>
<html>
<head>
  <title>Antediluvian Word Preservation Society</title>
  <meta charset="utf-8">                                                    ①
  <link href="https://fonts.googleapis.com/css2?
  family= Playfair+Display:wght@400;700&display=swap"
  rel="stylesheet">                                                         ②
  <link href="https://fonts.googleapis.com/css2?
  family=Lora:ital,wght@0,400;0,700;1,400&display=swap"
  rel="stylesheet">                                                         ②
  <link rel="stylesheet" href="styles.css">                                 ③
</head>
<body>
  <header>                                                                  ⑥
    <h1>Antediluvian Word Preservation Society</h1>                         ④⑥
    <p>Preserving words from the past, for the future</p>                   ⑤⑥
  </header>                                                                 ⑥
  <nav>                                                                     ⑦
    <a href="index.xhtml">Home</a>                                           ⑦
    <a href="blog.xhtml">Blog</a>                                            ⑦
    <a href="faq.xhtml">FAQ</a>                                              ⑦
    <a href="about.xhtml">About</a>                                          ⑦
    <a href="contact.xhtml">Contact</a>                                      ⑦
  </nav>                                                                    ⑦
  <main>                                                                    ⑧
    <p>Welcome to the Antediluvian Word Preservation Society,               ⑧
       where our goal is to protect, preserve, and promote old              ⑧
       words that are in danger of becoming overlooked, outmoded,           ⑧
       and obsolete. Stay a while, take a look around, and bask             ⑧
       in the burnished sheen of these old and beautiful words.</p>         ⑧
    <section>                                                               ⑧
      <h2>Most recent word</h2>                                             ⑧
      <h3><em>hullaballoo</em> (hul·uh·buh·LOO, noun)</h3>                  ⑧
      <p>A great noise or commotion; an uproar. (Example: "After hearing    ⑧
         the <strong>hullaballoo</strong> that eight kids hopped up on      ⑧
         sugar could make, Rupert decided to never again volunteer to help  ⑧
         out at a Halloween party.") This is a fun word to use in           ⑧
         conversation, and it's perfect if you need an unusual synonym for  ⑧
         <em>noise</em> or <em>commotion</em>. It's just obscure enough     ⑧
         that it doesn't get overused, but it's not so obscure that most    ⑧
         people won't recognize it and chuckle to themselves.               ⑧
         <em>Hullabaloo</em> began its life as the word <em>halloo</em>,    ⑧
         meaning "to urge or incite with shouts." Then, via the process of  ⑧
         rhyming reduplication, the <em>balloo</em> part was added to form  ⑧
         <em>halloo-balloo</em>, which eventually morphed in                ⑧
         <em>hullabaloo</em>. Some synonyms that register about the same on ⑧
         the fun-meter are <em>brouhaha</em>, <em>hubbub</em>, and          ⑧
         <em>hurly-burly</em>.</p>                                          ⑧
    </section>                                                              ⑧
    <section>                                                               ⑧
      <h2>This week's challenge</h2>                                        ⑧
         <p>Your challenge this week is to use the word <em>tomfoolery</em> ⑧
         -- foolish or silly behavior -- at least once in each of the       ⑧
         following: in conversation, in an email message, in a text         ⑧
         message, and in a business meeting (virtual or real-world).        ⑧
         Good luck and let us know how you make out!</p>                    ⑧
    </section>                                                              ⑧
  </main>                                                                   ⑧
  <footer>                                                                  ⑨
    &copy; 2023 Antediluvian Word Preservation Society                      ⑨
  </footer>                                                                 ⑨
</body>
</html>
```

① 指定页面字符集

② 从 Google Fonts 加载页面字体

③ 告诉网络浏览器 CSS 代码的位置

④ 页面标题

⑤ 页面标语

⑥ 页面页眉

⑦ 导航元素

⑧ 主要元素

⑨ 页脚

在阅读 HTML 代码时，请注意以下几点：

+   HTML 文件中的`<head>`标签中的`<meta charset="utf-8">`代码告诉浏览器页面使用的字符集。你不需要知道这意味着什么，只需知道这个标签是必需的，以便正确显示版权符号。如果你在页面文本中使用类似字符（如破折号—和引号“和”），它也会帮助这些字符正确显示。

+   由于某种原因，ChatGPT 使用两个单独的`<link>`标签引用了两个 Google Fonts 字体样式。不知道为什么，但它有效，所以我就这样做了。

+   在提示中，我要求 ChatGPT 查找被双星号包围的单词（例如，`**hullaballoo**`）并将这些单词加粗。在 HTML 中，ChatGPT 将双星号替换为`<strong>`和`</strong>`标签，这些标签使它们之间的文本加粗。

+   同样，我要求 ChatGPT 查找被单星号包围的单词（例如，`*noise*`）并将这些单词设置为斜体。在 HTML 中，ChatGPT 将星号替换为`<em>`和`</em>`标签，这些标签使它们之间的文本斜体。

注意，HTML 代码中包含以下行：

```py
<link rel="stylesheet" href="styles.css">
```

这个标签告诉网络浏览器在哪里找到 CSS 代码，我将在下一节中描述。

### 6.3.2 检查 CSS

下面展示了 ChatGPT 为我信息网站主页生成的 CSS 代码：

```py
body {
  background-color: oldlace;              ①
  max-width: 800px;                       ②
  margin: 0 auto;                         ③
  padding: 25px;
}
header h1 {                               ④
  font-size: 64px;                        ④
  line-height: 1;                         ④
  color: midnightblue;                    ④
  font-family: 'Playfair Display', serif; ④
  margin-bottom: 20px;                    ④
}                                         ④
header p {
  font-size: 30px;                        ⑤
}
nav {                                     ⑥
  border-top: 1px solid midnightblue;     ⑥
  border-bottom: 1px solid midnightblue;  ⑥
  margin: 20px 0;                         ⑥
  padding: 10px 0;                        ⑥
  display: flex;                          ⑥
  justify-content: space-between;         ⑥
}                                         ⑥
nav a {
    font-size: 24px;                      ⑦
}
a {
  color: steelblue;                       ⑧
  text-decoration: none;                  ⑧
}
h2 {
  font-size: 48px;                        ⑨
  color: midnightblue;                    ⑨
  font-family: 'Playfair Display', serif; ⑨
  margin: 30px 0 0;                       ⑨
}
h3, p, main p {
  font-size: 24px;                        ⑩
  color: darkslategray;                   ⑩
  font-family: 'Lora', serif;             ⑩
  margin-top: 8px;
}
footer {                                  ⑪
  border-top: 1px solid midnightblue;     ⑪
  border-bottom: 1px solid midnightblue;  ⑪
  padding: 10px 0;                        ⑪
  margin-top: 50px;                       ⑪
}                                         ⑪
```

① 设置页面背景颜色

② 设置页面最大宽度为 800 px

③ 居中页面

④ 将页面标题字体大小设置为 64 px，颜色为 midnightblue，并使用 Playfair Display 字体

⑤ 将标语样式设置为字体大小 30 px

⑥ 样式化导航元素（如前所述）

⑦ 将导航链接的大小设置为 24 px

⑧ 样式化页面链接，颜色为 steelblue，无下划线

⑨ 使用 48px 字体大小、深蓝色和中世纪字体样式化二级标题

⑩ 使用 24px 字体大小、深灰色和 Lora 字体样式化常规页面文本

⑪ 样式化页脚

如果您愿意，可以使用这些注释来调整您的网页代码，正如我在下一节中描述的那样。

## 6.4 定制主页

如果 ChatGPT 的信息网站代码由于某种原因出现问题，您有两种方法可以修复：

+   如果页面与您想要的效果相差甚远，请重新编写提示，开始一个新的聊天会话，然后再次尝试。

+   如果页面接近您想要的效果，请让 ChatGPT 为您进行必要的调整。请确保在原始提示的同一会话中提交此请求。

对于第二种情况，如果 ChatGPT 生成的代码只需要一些小的调整，请考虑根据我在上一节中提供的注释手动修改代码。因为您不了解网页代码，所以最好不要尝试进行任何重大更改。然而，这仍然提供了很多方法来修改代码以获得您想要的页面。

首先，这里有一些 HTML 代码的定制化建议：

+   在页眉中，您可以编辑标题或标语。只需确保不要编辑或删除相关的 HTML 标签：标题使用`<h1>`和`</h1>`，标语使用`<p>`和`</p>`。

+   根据需要编辑`section`元素，调整标题和文本。

+   要添加新部分，请按照以下步骤操作：

a) 在文本编辑器中打开 HTML 文件。

b) 选择一个现有的部分。也就是说，选择包括单个`<section>`和`</section>`标签对之间的所有内容，如图 6.9 所示。

![图片](img/build-a-website-with-chatgpt-CH06_F09_McFedries3.png)

图 6.9 选择一个现有的 section 元素。

c) 复制条目（例如，通过按 Ctrl-C 或 Cmd-C）。

d) 在您想要新部分出现的位置创建一个新行。例如，如果您想在页面的第一个部分上方出现新部分，请将光标置于第一个`<section>`标签之前，然后按 Enter 或 Return 键。

e) 将光标置于您刚刚创建的新行上，如图 6.10 所示。

![图片](img/build-a-website-with-chatgpt-CH06_F10_McFedries3.png)

图 6.10 将光标置于您想要粘贴复制的代码的位置。

f) 粘贴复制的代码（例如，通过按 Ctrl-C 或 Cmd-C）。

g) 编辑部分标题和文本。

+   如果您的入口文本包含多个段落，您可以通过在段落前后添加`<p>`标签来确保每个段落都能正确渲染：

    ```py
    <section>
        <h2>Section heading</h2>
        <p>
            First paragraph
        </p>
        <p>
            Second paragraph
        </p>
        <p>
            Third paragraph
        </p>
    </section>
    ```

+   在 HTML 代码的页脚部分，您可以添加指向您的社交媒体账户的链接，正如我在第四章中描述的那样。

现在为您提供了几个 CSS 代码的定制化建议：

+   如果您希望页面具有不同的最大宽度，请将`max-width`值更改为`800px`以外的值。

+   对于任何颜色值，您都可以将现有颜色更改为不同的颜色关键字。

+   对于任何字体大小值，您可以通过更改数字来增加或减少字体大小。只需确保保留`px`单位。

+   对于任何填充或边距值，你可以更改数字以增加或减少填充或边距。在每种情况下，务必保留`px`单位。

+   为了给您的文本提供更多呼吸空间，通过在 CSS 代码的`body`规则中添加声明`line-height: 1.5;`在每行之间创建一些额外空间：

    ```py
    body {
        background-color: oldlace;
        max-width: 800px;
        margin: 0 auto;
        padding: 25px;
        line-height: 1.5;
    }
    ```

+   为了使您的页面代码更易于访问，考虑将所有`px`测量值转换为`rem`测量值。默认情况下，1 `rem`相当于 16 `px`，所以 20 `px`是 1.25 `rem`，24 `px`是 1.5 `rem`，32 `px`是 2 `rem`，48 `px`是 3 `rem`，依此类推。`rem`单位更易于访问，因为它测量的是相对于浏览器用户在浏览器设置中定义的默认字体大小的字体大小。

## 6.5 为其他网站页面构建提示

虽然一些信息网站只包含一个页面，但大多数网站都有几个页面，很多网站甚至有很多页面。如果您的网站也是这样，您的下一个任务就是提示 ChatGPT 生成其他页面的代码。

幸运的是，这些其他页面将与您的首页结构非常相似，唯一的区别是`main`元素将存储每个页面的标题和文本。这意味着您每个子主题页面的提示将与您首页的提示非常相似。请注意，您也不需要为这些子主题页面添加任何新的 CSS，因此您可以跳过提示中的 CSS 部分。

这里有一个通用的提示您可以使用：

```py
I want to build a page for an information website. I don't know how to code, so I need you to provide the code for me.

Write the HTML code for a web page that includes the following:
 * The page title is "[page title]".
 * A header element that includes the title "[site title]" and the tagline "[site tagline]".
* After the header, a navigation element that includes the following links:
[Copy your navigation links here]
* A main element that includes the text between triple quotation marks.
 """
[page content goes here]
 """
 * A footer element that includes the Copyright symbol followed by the current year, followed by "[site title]".
 * In the page head section, include the tag <meta charset="utf-8">.
 * In the page head section, include a reference to a stylesheet file named "styles.css".
 * In the page head section, include a reference to the Google fonts X and Y.
 * Do not add any inline styles.
```

注意对 ChatGPT 的最后一条指示，即不要添加内联样式，这指的是直接添加到 HTML 标签中的 CSS 代码。在没有任何 CSS 相关指示的情况下，ChatGPT 倾向于插入一些以内联样式形式出现的格式建议。因为您需要的所有样式都已经包含在您的 styles.css 文件中，所以您必须告诉 ChatGPT 不要添加任何可能破坏您页面的新样式。图 6.11 显示了 ChatGPT 为我信息网站生成的示例页面。

![](img/build-a-website-with-chatgpt-CH06_F11_McFedries3.png)

图 6.11 ChatGPT 生成的另一个信息网站页面

无论您想突出显示哪种类型的实体——无论是组织、社区、活动、慈善机构、团队还是项目——信息网站都是向世界介绍它的绝佳方式，并帮助人们了解更多。现在，有了 ChatGPT 作为您的编码伙伴，您只需几个提示就可以建立一个完整的网站并使其运行。

## 摘要

+   链接是一个特殊的 HTML 标签，当点击时，会将用户带到指定的网页。

+   导航栏是一组链接，指向网站上的其他页面（或者，如果网站很大，指向网站最重要的页面）。

+   为了获得最佳效果，您的页面提示应尽可能具体，包括颜色、字体大小和标题级别。

+   将生成的 HTML 保存到 index.xhtml 文件中，将生成的 CSS 保存到 ChatGPT 在 HTML 代码中建议的文件名中，通常是 styles.css。

# 7 创建网站内容

本章涵盖

+   与 ChatGPT 协作创建和编辑内容

+   让 ChatGPT 以你的风格写作

+   获取 AI 帮助编辑你的写作

+   添加英雄图片

+   提示 ChatGPT 为兴趣或爱好创建页面

+   检查和自定义 ChatGPT 网页代码

正如我在第一章中解释的，GPT 中的“G”代表“生成”，这意味着你可以使用 ChatGPT 不仅进行对话，还可以创建新事物。正如你在本书中迄今为止所看到的，这些生成内容可以是页面标题和标语的想法，匹配页面主题的字型建议，配色方案推荐，链接，导航栏，当然还有构建最终网页的 HTML 和 CSS 代码。

然而，你的生成内容雄心不必局限于小块的文本和代码。如果你有在网络上展示你真实自我的冲动，那么最好的方法之一就是写关于一个让你着迷或吸引你的兴趣或爱好。如果你不确定写什么，或者你开始有困难，本章将向你展示如何将 ChatGPT 作为合作伙伴引入，以帮助你开始。你将学习如何获取 AI 生成的创意和写作建议，使用 AI 进行研究，甚至使用 ChatGPT 以你的风格写作。

你还将学习如何制作一个详细的提示，将其传递给 ChatGPT 以生成一个专门针对兴趣或爱好页面的代码，在那里你可以发布你与 ChatGPT 共同创建的内容。本章还提供了 ChatGPT 生成的代码的高级解释，甚至提供了一些手动定制代码的技巧，以获得你想要的一切。

## 7.1 理解本章的项目

在本章中，你将创建一个专注于兴趣或爱好的简单网站。你将雇佣 ChatGPT 作为你的写作助手，帮助你构思想法，进行研究，并为网站内容创建初稿。主页将包括以下组件：

+   包含以下内容的页眉元素：

    +   占据整个浏览器窗口宽度和高度的图片

    +   网站标题

    +   网站标语

    +   包含链接到其他网站页面的导航元素

+   包含一些介绍性文本和链接到其他网站页面的主要元素

+   包含版权声明的页脚元素

图 7.1 展示了使用 ChatGPT 生成的代码构建的一个兴趣网站主页的示例。

![图片](img/build-a-website-with-chatgpt-CH07_F01_McFedries3.png)

图 7.1 ChatGPT 生成的兴趣网站主页

其他网站页面将使用类似的结构：

+   包含以下内容的页眉元素：

    +   英雄图片

    +   页面标题

    +   页面副标题

    +   包含链接到其他网站页面的导航元素

+   包含页面文本的主要元素

+   包含版权声明的页脚元素

图 7.2 显示了这样一个页面的示例。这些页面的简单性意味着你可以轻松地根据你想要与世界分享的任何兴趣、爱好或痴迷来定制它们。

![图片](img/build-a-website-with-chatgpt-CH07_F02_McFedries3.png)

图 7.2 一个子主题页面

## 7.2 使用 ChatGPT 生成和编辑文本

如果你不仅想写，还想通过在网络上发布来与他人分享你的写作，你可能会对使用 ChatGPT 作为写作助手或甚至作为一种机器中的幽灵（作者）持谨慎态度。如果你认为写作很重要，那么它也是重要的，这是你的写作，而不是由 AI 制造的东西。

然而，这并不意味着你不能用 ChatGPT 来完成一些与写作相关的繁琐工作。需要一些内容想法吗？ChatGPT 可以帮忙。需要为文章做一些研究？这正是 ChatGPT 擅长的。面对空白的屏幕感到困惑？让 ChatGPT 生成一些东西，任何东西，也许那句话或甚至那个短语就足以激发你的想象力。对你写的东西不满意？让 ChatGPT 看看它，并提出改进建议。

真的没有尽头的方式来让 ChatGPT 充当你的个人写作助手。当然，如果你想的话，甚至可以让 ChatGPT 为你写一切。如果你能这样做并且还能睡得香，嗯，我可不打算试图说服你改变主意。

### 7.2.1 让 ChatGPT 建议写作想法

ChatGPT 擅长许多任务，但其中一项最突出的才能是就几乎任何主题提出写作想法，无论多么晦涩或神秘。也就是说，如果你对你的写作想要追求的主题有一个大致的概念，ChatGPT 可以从多个角度提出内容想法。

你应该从为 ChatGPT 分配一个角色开始你的提示：

```py
You are an expert in [*topic*] and can generate interesting and creative ideas about [*topic*] based on the following question.
```

用一个词或短语替换`[`*`主题`*`]`，描述你想要写的主题或内容。

现在添加一个问题，让 ChatGPT 为你生成一些文章的想法。以下是一些示例，帮助你开始：

```py
What are the pros and cons of [*topic*]?
What are the top ten features of [*topic*]?
What are five things everyone needs to know about [*topic*]?
What are some common myths about [*topic*]?
How does a beginner get started with [*topic*]?
What are half a dozen tips and tricks to get the most out of [*topic*]?
```

同样，在每种情况下，你都用一个词或短语替换`[`*`主题`*`]`，这个词或短语描述了你想要写的主题或内容。例如，图 7.3 显示了 Copilot（在创意模式下）基于以下提示为我生成的一些想法：

```py
You are an expert in bread baking and can generate interesting and creative ideas about bread baking based on the following question.

How does a beginner get started with bread baking?
```

![图片](img/build-a-website-with-chatgpt-CH07_F03_McFedries3.png)

图 7.3 ChatGPT 关于如何开始面包烘焙的想法

这些都是极好的建议，可以作为一篇吸引面包烘焙初学者的文章的起点。请注意，将 ChatGPT 的内容想法视为起点是很重要的。细节的充实取决于你，以创建一篇出色的文章。

### 7.2.2 生成关于如何写主题的想法

在上一节中，你学习了如何使用 ChatGPT 来生成写作想法。ChatGPT 的另一个类似用途是询问它如何就某个特定主题或某个特定主题的特定方法进行写作。

如同往常，首先给你的 ChatGPT 分配一个角色：

```py
You are a writing coach and an expert on [*topic*] and can generate practical and creative advice on how to write about [*topic*] based on the following question.
```

将 `[`*`topic`*`]` 替换为你想要通过写作探索的主题或主题的描述性单词或短语。

接下来，你添加一个问题，以促使 ChatGPT 想出如何撰写你的主题的想法。以下是一些示例：

```py
What are the best ways to introduce a beginner to [*topic*]?
Once someone has learned the basics of [*topic*], what should I teach them next?
How do I get someone who knows nothing about [*topic*] excited about the subject?
What are some ways to write engagingly about [*topic*]?
What types of posts are most suited to writing about [*topic*]?
```

再次，在每个示例中将 `[`*`topic`*`]` 替换为描述你写作主题的文本。例如，图 7.4 显示了 Copilot（在创意模式下）从以下提示中生成的写作想法：

```py
You are a writing coach and an expert on bread baking and can generate practical and creative advice on how to write about bread baking based on the following question.

What are some ways to write engagingly about bread baking?
```

这些建议不仅适用于撰写面包烘焙方面的文章，而且适用于撰写几乎所有其他主题的文章！

![](img/build-a-website-with-chatgpt-CH07_F04_McFedries3.png)

图 7.4 ChatGPT 关于如何引人入胜地撰写面包烘焙文章的建议

### 7.2.3 获取 ChatGPT 帮助研究主题

ChatGPT 背后的 GPT 模型在难以想象的大量数据上进行了训练，这意味着它们对几乎所有你感兴趣的任何主题都有相当的了解。这使得 ChatGPT 成为完美的研究助手，因为你可以要求它帮助你探索你想要撰写的任何主题，你将得到大量有用的提示。

这是你可以用来请求 ChatGPT 研究帮助的提示：

```py
Help me research [*topic*] for a general audience. I'm interested in *A*, *B*, and *C*. Please provide *X*, *Y*, and *Z*. Also, include any interesting trivia or anecdotes that might be engaging for readers. The goal is to provide a depth of information that is accurate and detailed but also easily understood by a broad audience. Please provide links to your sources.
```

如同往常，`[`*`topic`*`]` 是你想要研究的主题的简短描述。以下是一些其他占位符所代表的含义：

+   *`A`*、*`B`*和*`C`*——与整体主题相关的一般主题。

+   *`X`*、*`Y`*和*`Z`*——整体主题的特定方面。

提示：提示中的最后一句话假设你正在使用一个连接到网络的 ChatGPT 版本。我强烈推荐使用网络连接版本，因为生成的链接使你能够核实 ChatGPT 的结果，并为你提供更多研究素材。

这是示例：

```py
Help me research the history of coffee for a general audience. I'm interested in the discovery of coffee, its spread across the globe, and its cultural impact in different societies. Please provide key historical figures and events, notable varieties of coffee, and the evolution of coffee-drinking habits over time. Also, include any interesting trivia or anecdotes that might be engaging for readers. The goal is to provide a depth of information that is accurate and detailed but also easily understood by a broad audience. Please provide links to your sources.
```

图 7.5 显示了 Copilot（在创意模式下）对先前提示的异常长响应的最后一部分。提示假设你是在为普通受众写作，但当然，你应该根据你预期的读者进行修改。

![](img/build-a-website-with-chatgpt-CH07_F05_McFedries3.png)

图 7.5 ChatGPT 对请求帮助研究咖啡历史的提示的最后一部分响应

### 7.2.4 让 ChatGPT 用你的风格写作

ChatGPT 生成写作的一个难以实现的目标是让模型输出的散文听起来像你。当然，ChatGPT 可以轻松（并且，经常是幽默地）生成像詹姆斯·乔伊斯、艾米莉·狄金森和苏斯博士这样的著名作家的风格散文。这是因为 ChatGPT（几乎肯定）是在这些作者的大量写作样本上进行了训练。然而，ChatGPT 可能对你如何写作一无所知。

然而，这不是问题，因为你可以“训练”ChatGPT 模仿你的写作风格。如何做到？通过给 ChatGPT 提供你写作的几个样本，要求它分析这些样本的语气和风格，然后要求它用相同的语气写一些新的内容。

这是提示：

```py
You are an experienced ghostwriter. Given several examples of an author's writing, you are skilled at detecting the tone and style of the writing and emulating that writer's voice to generate new writing. 

Below are several writing samples, with each sample between sets of triple quotation marks.

Examine the samples to determine the writer's unique voice.

Emulate the writer's voice to generate *X*.

"""
*Writing sample #1*
"""

"""
*Writing sample #2*
"""

"""
*Writing sample #3*
"""

"""
*Writing sample #4*
"""

"""
*Writing sample #5*
"""
```

将每个“*写作样本 #n*”实例替换为您自己的写作样本。

注意：理想情况下，您的写作样本应使用您想要用于您想要创建的写作的风格和语气。

您不必包括所有五个样本。您可以使用两个或三个，甚至一个单独的长样本，但请记住，您提供的文本越多，ChatGPT 提供的分析就越准确，提示就越成功。

提示：如果您有一位您钦佩并希望在一定程度上模仿的作者，请将其包含在提示中。例如，要请 ChatGPT 包含 Eudora Welty 的风格和语气的一小部分，请将以下内容添加到提示中：“请也包含大约 10%的 Eudora Welty 的语气和风格”。

在提示中，将*X*替换为您想要 ChatGPT 生成的写作的简要描述。以下是一个示例：

```py
You are an experienced ghostwriter. Given several examples of an author's writing, you are skilled at detecting the tone and style of the writing and emulating that writer's voice to generate new writing. 

Below are several writing samples, with each sample between sets of triple quotation marks.

Examine the samples to determine the writer's unique voice.

Emulate the writer's voice to generate a satirical news story based on the multiple pronunciations of the letters "ough".

"""
Researchers from Aalborg University announced today that they have finally discovered the long sought-after Soup-Nuts Continuum. Scientists around the world have been searching for this elusive item ever since Albert Einstein's mother-in-law proposed its existence in 1922\. "Today is an incredible day for the physics community and for humanity as a whole," said senior researcher Lars Grüntwerk. "Today, for the first time in history, we are on the verge of knowing everything from soup to, well, you know, nuts."
"""

"""
SCHECHENECTADY, NY--After a long and tempestuous marriage, the two senses of the word "oversight" have petitioned for a divorce. Citing irreconcilable differences, the "responsible" sense of the word ("Watchful care or management") and the "irresponsible" sense ("An omission or error") have separated. "It just got to be too much after a while," said responsible oversight. "The other oversight can't be trusted with even the smallest task. It's 'Oops!' this and 'Sorry!' that. I believe in being careful and in making sure that things get done right, so I just can't stand to live with such neglect."
"""

"""
AIEA, Hawaii--Former United Nations Secretary General Boutros-Boutros Ghali and current United Nations Undersecretary for Alphabet Mobilization Yada-Yada Yada announced today the formation of the United Nations International Vowel Assistance Committee. UNIVAC's mandate is "to help the vowel-deprived wherever they may live and to fund vowel relief efforts in the hardest hit areas." "We have a good stockpile of a's, e's, and o's," said Ng Ng, UNIVAC's Letter Distribution Officer. "We hope to have an adequate supply of i's and u's over the next six months. In the meantime, we can use our extra y's in a pinch."
"""

"""
KALAMAZOO, Michigan--A group of disgruntled grammarians calling themselves "Mad, We Are, As Hell" has filed a number of civil lawsuits over the past few weeks. The targets of these suits are writers, raconteurs, and professional man-in-the-street interviewees who, they claim, are inveterate violators of the rules of grammar. The group's spokesperson, Millicent Peevish, Head Shusher at the Kalamazoo District Library, said the grammarians could no longer sit back and allow "the splitting of blameless infinitives and the ending of sentences with evil, evil prepositions." A previous campaign -- called Shock and Appalled -- that focused on writing testy letters to the editors of various local publications, had no discernible effect.
"""

"""
In a scathing report released today, communications experts have declared that the instant messages teenagers exchange with each other are in reality nothing but gibberish. U.S. Chatmaster General Todd Dood, with technical help from the National Security Agency, examined thousands of instant messages. It has long been thought that teen instant messages contained abbreviations (such as LOL for "laughing out loud" and MAIBARP for "my acne is becoming a real problem"), short forms (such as L8R for "later" and R2D2 for "R2D2"), and slang (such as whassup for "what's up" and yo for "Hello, I am pleased to meet your acquaintance. Do you wish to have a conversation?").
"""
```

图 7.6 显示了基于我的写作样本，GPT-4（创意模式下的 Copilot）生成的故事。

![](img/build-a-website-with-chatgpt-CH07_F06_McFedries3.png)

图 7.6 Creative 模式下的 Copilot 生成的故事

这是一次相当不错的尝试：它符合写作样本的语气和风格，它是一个相当不错的创意，并且有一些真正的幽默。然而，它远非完美：

+   它包含一些错误，例如将“匹兹堡”作为一个使用“ough”字母的单词的例子。

+   一些写作比较笨拙，需要大量重写才能达到标准。

+   在这样的讽刺作品中使用真实姓名（如索尼亚·索托马约尔大法官）是一个糟糕的选择。更好的做法是使用基于“ough”字母的虚构名字。

这些问题在 AI 生成的写作中很常见，因此您应该始终仔细校对 ChatGPT 创建的任何内容，并准备好进行大量的重写。

### 7.2.5 重写后文本

在您写了一些文本之后，您可能会想知道您的散文是否可以通过某种方式改进，使其更有趣、更简洁、更冗长、更容易理解、更学术化等等。幸运的是，只要您的文本是在线的，或者以您能够将其加载到网页浏览器中的形式（例如 HTML 文件、文本文件或 PDF 文件），ChatGPT——特别是 Microsoft Copilot 应用——都愿意提供帮助。以下是方法：

1. 在 Microsoft Edge 浏览器中打开 Copilot 侧边栏。

2. 导航到包含您想要重写的文本的页面或打开该文件。

3. 选择您想要重写的文本。

4. 在侧边栏中，您会看到消息“将选定的或复制的文本发送到聊天？”，如图 7.7 所示。

![](img/build-a-website-with-chatgpt-CH07_F07_McFedries3.png)

图 7.7 在当前页面中选择一些文本，Copilot 会询问您是否想将其发送到 AI。

5. 点击发送。Copilot 询问您想对文本做什么。

6. 输入您的指令。以下是一些示例：

—  使其更有趣

—  使其更简洁

—  使其更容易理解

—  使其更具学术性

——  为 10 岁孩子重写

7.  按下 Enter 或 Return 键。Copilot 将根据你在步骤 6 中提供的说明修改选定的文本。

图 7.8 展示了当我要求 Copilot 将图 7.7 中选定的文本重写为 10 岁孩子能理解的形式时的结果。

![图片](img/build-a-website-with-chatgpt-CH07_F08_McFedries3.png)

图 7.8 图 7.7 中选定的文本，为 10 岁孩子重写

你可能已经注意到了我到目前为止生成的所有写作样本。没错：没有 HTML 标签！这些标签很重要，所以你将在下一节中学习如何在 ChatGPT 生成的写作中包含它们。

### 7.2.6 不要忘记 HTML 标签

无论你与 ChatGPT 合作创作什么内容，最终文本都会存在于一个网页中。这意味着文本需要用适当的 HTML 标签进行结构化，尤其是文本标题和段落。为了让 ChatGPT 为你完成这项工作，请在你的写作提示末尾添加以下内容：

```py
Please add HTML tags to the text, but don't generate the code for an entire web page.
```

当你的网站文本准备发布时，是时候让 ChatGPT 帮助你构建主页了。你将在下一节中学习如何操作。

## 7.3 构建主页

因为这个项目是一个多页网站，最好分阶段构建网站组件。基本流程如下总结：

1.  提示 ChatGPT 生成网站主页的 HTML 代码。

1.  提示 ChatGPT 生成网站样式的 CSS 代码。请注意，最好将这两个步骤合并为一个提示。

1.  对于你的其他网站页面，提示 ChatGPT 生成该页面的 HTML 代码。特别是，其他网站页面的提示应包括以下内容：

    +   使用与步骤 2 生成的 CSS 相同的 CSS 文件

    +   指示不要生成任何额外的样式，尤其是内联样式（即直接插入 HTML 标签中的 CSS 代码）

在你开始所有这些之前，花一分钟熟悉本章中介绍的新网页技术。

### 7.3.1 与英雄图片合作

本章中你唯一需要了解的新网页技术是*英雄图片*：当你首次访问页面时，占据整个浏览器窗口宽度（通常也是整个高度）的引人注目照片或插图。图 7.9 展示了包含英雄图片的示例网页。

![面包特写，自动生成的描述](img/build-a-website-with-chatgpt-CH07_F09_McFedries3.png)

图 7.9 带有英雄图片的网页

使用英雄图片时，以下是一些需要注意的要点：

+   图片主题应与你的页面主题相关。

+   图片应具有戏剧性或引人注目的特点。

+   使用高质量且无像素化等扭曲的图片。如果你使用的是照片，它应该构图良好且光线充足。

+   不要使用过小的图像文件，否则当浏览器将其扩展以适应窗口时，它将会变形。宽度为 1,200 像素，宽高比为 16:9 的图像对于大多数较大屏幕（以及横向模式下的较小设备屏幕）是理想的大小。

+   使用不会使你的文本丢失或难以阅读的图像。

+   如你稍后所见，你可以告诉 ChatGPT 稍微加深图像的亮度，所以如果你的图像对于你的文本来说看起来太亮，请不要担心。

+   如果你没有合适的图像，你可以要求 DALL-E 或 Copilot 的图像创建器为你生成一个（如第五章所述）。

要让 ChatGPT 向页面添加英雄图片，你的提示应该包含类似于以下说明的指令：

```py
Include a header that uses the file hero.jpg as a hero image.
```

有趣的是，当你检查 HTML 代码时，你不会看到对图像文件的引用。例如，下面是创建图 7.9 中所示标题的 HTML 代码：

```py
<header>
    <nav>
        <ul>
            <li><a href="index.xhtml">Home</a></li>
            <li><a href="history.xhtml">History</a></li>
            <li><a href="culture.xhtml">Culture</a></li>
            <li><a href="language.xhtml">Language</a></li>
        </ul>
    </nav>
    <h1>Bread in the Bone</h1>
    <p>A half-baked look at the history and culture of bread</p>
</header>    
```

英雄图片嵌入到 CSS 中的`header`元素中，如图 7.9 中用于`header`元素的`header`规则的部分列表所示：

```py
header {
    background: url('hero.jpg') no-repeat center center fixed;
    background-size: cover;
}
```

这段代码告诉网络浏览器将图像文件 hero.jpg 作为`header`元素的背景显示，并且图像应该覆盖整个元素。使用英雄图片是立即吸引访客注意力的好方法，这也是为什么这已经成为过去几年最受欢迎的网页设计趋势之一。

### 7.3.2 构建主页提示

本章的项目是一个关于兴趣或爱好的网站。你几乎准备好为 ChatGPT 构建主页提示了，但首先你需要确保你已经有了以下这些物品：

+   以下内容之一或全部：页面标志、标题和标语

+   你想要用于页面标题和页面文本的字体名称

+   你想要应用于页面背景和文本的颜色关键词

参考第三章了解更多关于这些设计元素以及如何提示 ChatGPT 获取标题、字体和颜色建议的信息。

你的兴趣或爱好网站起点是主页，你可以请 ChatGPT 帮助你构建。你的提示应该开始如下：

```py
I want to build a web page for a website home page. I don't know how to code, so I need you to provide the code for me.

First, write the HTML code for a web page that includes the following:
```

然后指定你页面的内容，包括以下内容（参见图 7.10）：

+   包含你的英雄图片、页面标题和标语以及包含链接到你的其他网站页面的导航栏的标题

+   一个以欢迎访客的介绍段落开始的主体元素

+   对于你网站的每个子主题，一个包含子主题标题、子主题描述和子主题链接的章节元素

+   包含版权声明的页脚

接下来，请让 ChatGPT 生成你想要页面格式的 CSS：

```py
Second, in a separate file please write the CSS code for the following:
```

指定格式，包括以下内容：

+   页面背景颜色和文本颜色。

+   你想要用于页面标题、标语和导航链接的字体大小和颜色。

+   用于标题和常规页面文本的字体。

+   主要元素的最大宽度。这可以防止文本行过长。对于大多数页面，800 px 的最大长度就足够了。

![](img/build-a-website-with-chatgpt-CH07_F10_McFedries3.png)

图 7.10 感兴趣网站主页的各个部分

这里是我的主页的一个示例提示：

```py
I want to build a website home page. I don't know how to code, so I need you to provide the code for me.

First, write the HTML code for a web page that includes the following:
 * A header that uses the file hero.jpg as a hero image.
 * The header also includes the title "Bread in the Bone" and the tagline "A half-baked look at the history and culture of bread".
 * The header should also include four links in the upper-right corner:
   * The text "Home" that links to the file "index.xhtml".
   * The text "History" that links to the file "history.xhtml".
   * The text "Culture" that links to the file "culture.xhtml".
   * The text "Language" that links to the file "language.xhtml".
 * A main element that includes the following five elements:
   * An introductory paragraph that includes the text "Welcome to Bread in the Bone, where I, a bread baker, a bread eater, and an unabashed bread nerd, try to make sense of the historical, cultural, and linguistic significance of that most humble of home staples: the loaf of bread. It's the greatest thing since, well, you know..."
  * A second paragraph that consists of the text "This site is divided into three sections:"
  * The second-level heading "History" followed by a paragraph that includes the text "A potted and probably not very accurate history of bread, from its ancient origins to today's ancient grains." Then the text "Check it out." as a link to "history.xhtml".
  * The second-level heading "Culture" followed by a paragraph that includes the text "A remarkably shallow examination of the cultural significance of bread, from its religious meanings to its social uses." Then the text "Read it." as a link to "culture.xhtml".
  * The second-level heading "Language" followed by a paragraph that includes the text "A not-all-that-deep dive into the linguistic roots and uses of the word bread, from its etymology to its varied metaphors." Put the word "bread" in italics. Then add the text "Go there." as a link to "language.xhtml".
 * A footer element that includes the Copyright symbol, followed by the current year, followed by "Paul McFedries".
  * In the page head section, include the tag <meta charset="utf-8">.

Second, in a separate file write the CSS code for the following:
 * The page background color is wheat.
 * The hero image covers the entire browser window.
 * Add a linear gradient to the header background to darken the hero image slightly.
 * Make all the header text white.
 * Make the title and tagline centered both horizontally and vertically.
 * Make the title 72px.
 * Make the tagline 36px.
 * Make the header links 24px.
 * Style the headings with size 48px, no bottom margin, the color saddlebrown, and the Raleway typeface from Google Fonts.
 * Style the rest of the page text with size 24px, a 20px bottom margin, and the Lato typeface from Google Fonts.
 * Style the main element's links with the color saddlebrown.
 * The main section has 25px padding all around and a maximum width of 800px.
 * The footer has a top border.
```

ChatGPT 应首先创建 HTML 代码，您可以复制并粘贴到名为 index.xhtml 的文件中，然后保存。在这段代码中，您应该看到顶部附近类似以下的一行：

```py
<link rel="stylesheet" type="text/css" href="styles.css">
```

这段代码告诉网络浏览器在名为 styles.css 的文件中查找 CSS 代码，因此您的下一个任务是复制生成的 CSS 代码，将其粘贴到文件中，并保存为 styles.css（或您在`<link>`标签中看到的任何名称）。请确保将 styles.css 保存与您的 index.xhtml 文件相同的文件夹中。您还需要将您的英雄图片文件复制到同一文件夹中。有关更多关于工作网页文件的信息，请参阅附录 A。

我使用 OpenAI 的 ChatGPT 应用提交了这个提示，它生成的代码导致了图 7.11 所示的页面。

![](img/build-a-website-with-chatgpt-CH07_F11_McFedries3.png)

图 7.11 ChatGPT 生成的主页

如果您喜欢 ChatGPT 为您创建的主页，您可以跳过本节的其余部分，并继续到其他页面（请参阅“为其他网站页面构建提示”）。但是，如果您想了解更多关于 ChatGPT 生成的代码的信息，下一节将为您提供更详细的了解。

## 7.4 检查主页代码

我将为您提供一个简短且不太技术性的概述，这是从我上一节提示（如图 7.11 所示的主页）中得到的页面代码。

注意：本书网站上（[www.manning.com/books/build-a-website-with-chatgpt](https://www.manning.com/books/build-a-website-with-chatgpt)）和 GitHub 存储库（[`github.com/paulmcfe/websites-with-chatgpt`](https://github.com/paulmcfe/websites-with-chatgpt)）中提供了我在线日志页面的生成的 HTML 和 CSS 代码。

ChatGPT 的每个版本都应该输出至少与下一两个部分显示的类似的 HTML 和 CSS 代码，因此我的代码注释应该能帮助您理解底层发生了什么。

### 7.4.1 检查 HTML

ChatGPT 为我感兴趣网站的主页生成的 HTML 代码如下所示：

```py
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8">                                              ①
    <title>Bread in the Bone</title>
    <link href="https://fonts.googleapis.com/css2?
        family=Lato:wght@700&family=Raleway:wght@400&
        display=swap"rel="stylesheet">                                  ②
    <link rel="stylesheet" href="styles.css">                           ③
</head>
<body>
    <header>                                                            ④
        <nav>                                                           ④⑤
            <ul>                                                        ④⑤
                <li><a href="index.xhtml">Home</a></li>                  ④⑤
                <li><a href="history.xhtml">History</a></li>             ④⑤
                <li><a href="culture.xhtml">Culture</a></li>             ④⑤
                <li><a href="language.xhtml">Language</a></li>           ④⑤
            </ul>                                                       ④⑤
        </nav>                                                          ④⑤
        <h1>Bread in the Bone</h1>                                      ④⑥
        <p>                                                             ⑦
            A half-baked look at the history                            ⑦
            and culture of bread                                        ⑦
        </p>                                                            ⑦⑧
    </header>                                                           ⑧

    <main>                                                              ⑨
        <p>                                                             ⑨⑩
            Welcome to Bread in the Bone, where I, a bread baker, a     ⑨⑩
            bread eater, and an unabashed bread nerd, try to make       ⑨⑩
            sense of the historical, cultural, and linguistic           ⑨⑩
            significance of that most humble of home staples: the loaf  ⑨⑩
            of bread. It's the greatest thing since, well, you know...  ⑨⑩
        </p>                                                            ⑨⑩
        <p>This site is divided into three sections:</p>                ⑨

        <section>                                                       ⑪⑫
            <h2>History</h2>                                            ⑪⑫
            <p>                                                         ⑪⑫
                A potted and probably not very accurate history of      ⑪⑫
                bread, from its ancient origins to today's ancient      ⑪⑫
                grains. <a href="history.xhtml">Check it out.</a>        ⑪⑫
            </p>                                                        ⑪⑫
        </section>                                                      ⑪⑫

        <section>                                                       ⑫
            <h2>Culture</h2>                                            ⑫
            <p>                                                         ⑫
                A remarkably shallow examination of the cultural        ⑫
                significance of bread, from its religious meanings      ⑫
                to its social uses. <a href="culture.xhtml">Read it.</a> ⑫
            </p>                                                        ⑫
        </section>                                                      ⑫

        <section>                                                       ⑫
            <h2>Language</h2>                                           ⑫
            <p>                                                         ⑫
                A not-all-that-deep dive into the linguistic roots      ⑫
                of bread, from its etymology to its varied metaphors.   ⑫
                <a href="language.xhtml">Go there.</a>                   ⑫
            </p>                                                        ⑫
        </section>                                                      ⑫
    </main>                                                             ⑫

    <footer>                                                            ⑬
        &copy; 2023 Paul McFedries                                      ⑬
    </footer>                                                           ⑬
</body>
</html> 
```

① 指定页面字符集

② 从 Google Fonts 加载页面字体

③ 告诉网络浏览器在哪里找到 CSS 代码

④ 页面页眉

⑤ 导航元素

⑥ 页面标题

⑦ 页面标语

⑧ 页面页眉

⑨ 主要元素

⑩ 页面简介

⑪ 每个部分元素都有一个标题、描述和链接。

⑫ 主要元素

⑬ 页面页脚

注意，HTML 代码中包含以下行：

```py
<link rel="stylesheet" href="styles.css">
```

这个标签告诉网络浏览器在哪里找到 CSS 代码，我将在下一节中描述。

### 7.4.2 检查 CSS

ChatGPT 为我感兴趣网站的主页生成的 CSS 代码如下所示：

```py
* {                                                            ①
    margin: 0;                                                 ①
    padding: 0;                                                ①
    box-sizing: border-box;                                    ①
}                                                              ①
body {                                                         ②
    background: wheat;                                         ②
    font-family: 'Lato', serif;                                ②
    font-size: 24px;                                           ②
    color: #333;                                               ②
}                                                              ②
header {
    background: url('hero.jpg') no-repeat center center fixed; ③
    background-size: cover;                                    ③
    color: white;
    display: flex;                                             ④
    flex-direction: column;                                    ④
    justify-content: center;                                   ④
    align-items: center;                                       ④
    height: 100vh;                                             ④
    position: relative;
    background-image:                                          ⑤
        linear-gradient(rgba(0, 0, 0, 0.5),                    ⑤
        rgba(0, 0, 0, 0.5)),                                   ⑤
        url('hero.jpg');                                       ⑤
}
nav ul {                                                       ⑥
    list-style-type: none;                                     ⑥
    display: flex;                                             ⑥
    gap: 20px;                                                 ⑥
    position: absolute;                                        ⑥
    top: 20px;                                                 ⑥
    right: 30px;                                               ⑥
}                                                              ⑥
nav a {                                                        ⑦
    color: white;                                              ⑦
    font-size: 24px;                                           ⑦
    text-decoration: none;                                     ⑦
}                                                              ⑦
nav a:hover {                                                  ⑧
    text-decoration: underline;                                ⑧
}                                                              ⑧
.title-container {
    text-align: center;
}
h1 {
    font-size: 72px;                                           ⑨
    font-family: 'Raleway', sans-serif;                        ⑨
    margin-bottom: 10px;
}
header p {
    font-size: 36px;                                           ⑩
}
h2 {
    color: saddlebrown;                                        ⑪
    font-size: 48px;                                           ⑪
    font-family: 'Raleway', sans-serif;                        ⑪
    margin-top: 30px;
}
main p {
    margin-bottom: 20px;                                       ⑫
}
main {
    padding: 25px;                                             ⑬
    max-width: 800px;                                          ⑬
    margin: 0 auto;                                            ⑬
}
a {
    color: saddlebrown;                                        ⑭
    text-decoration: none;                                     ⑭
}
a:hover {
    text-decoration: underline;                                ⑮
}
footer {
    margin-top: 50px;                                          ⑯
    text-align: center;                                        ⑯
    padding: 20px 0;                                           ⑯
    border-top: 1px solid black;                               ⑯
} 
```

① 重置一些样式

使用样式设置页面背景颜色、字体、字体大小和文字颜色

设置英雄图片以填充浏览器窗口

使用样式使页眉文本居中

使用样式使英雄图像变暗，以便更容易阅读

使用样式设置导航元素

使用样式设置导航链接

在鼠标悬停时为每个导航链接添加下划线

将页面标题的字体大小设置为 72 px，并应用 Raleway 字体

使用 36 px 的字体大小样式设置标语

使用颜色为 saddlebrown、字体大小 48 px 和 Raleway 字体的样式设置页面标题

为每个主元素段落添加 20 px 的下边距

使用 25 px 的内边距、800 px 的最大宽度和居中对齐样式设置主元素

使用颜色为 saddlebrown 且无下划线的样式设置页面链接

在鼠标悬停时为每个链接添加下划线

使用样式设置页面页脚

如果你愿意，可以使用这些注释来调整你的网页代码，正如我在下一节中描述的那样。

### 7.4.3 自定义首页

如果你不喜欢 ChatGPT 生成的代码生成的首页，请随意调整你的提示并再次尝试。然而，如果你只想进行一些小的调整，考虑手动编辑代码。

首先，这里有一些 HTML 代码的定制建议：

+   在页眉中，你可以编辑标题或标语。只需确保不要编辑或删除相关的 HTML 标签：标题的`<h1>`和`</h1>`，标语的`<p>`和`</p>`。

+   在页眉中，根据你的网站文件需要编辑链接文本和链接文件名。

+   编辑`section`元素，根据需要调整标题、描述和链接。

+   要添加一个新部分，复制一个现有的部分（即单个`<section>`和`</section>`标签之间的所有内容），将代码粘贴到`main`元素中你想要的位置（即在`<main>`和`</main>`标签之间），然后调整标题、描述和链接。（有关添加新`section`元素的更详细说明，请参阅第六章。）

+   在 HTML 代码的页脚部分，你可以添加指向你的社交媒体账户的链接，正如我在第四章中描述的那样。

现在，这里有一些 CSS 代码的定制想法：

+   为了设置英雄图像的暗度，ChatGPT 使用以下代码：

    ```py
    linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)) 
    ```

你可以通过调整两个`rgba`函数中的最后数字（此代码中的`0.5`值）来控制暗度。第一个`rgba`函数控制图像上半部分的暗度，第二个`rgba`函数控制下半部分的暗度。使用接近`0`的值以获得更亮的效果，使用接近`1`的值以获得更暗的效果。以下是一个更暗的示例：

```py
      linear-gradient(rgba(0, 0, 0, 0.75), rgba(0, 0, 0, 0.75))
```

+   为了给你的文字提供更多的呼吸空间，在 CSS 代码的`body`规则中添加声明`line-height: 1.5;`以在每行之间创建一些额外的空间：

    ```py
    body {
        background: wheat;
        font-family: 'Lato', serif;
        font-size: 24px;
        color: #333;
        line-height: 1.5;
    } 
    ```

+   如果你想你的页面有不同的最大宽度，定位 CSS 代码中的`main`规则，并将`max-width`值更改为`800px`以外的值。在以下示例中，我已经将最大宽度更改为`960px`：

    ```py
    main {
        padding: 25px;
        max-width: 960px;
        margin: 0 auto;
    }
    ```

+   对于任何颜色值，您可以将现有的颜色更改为不同的颜色关键字。

+   对于任何字体大小值，您可以通过更改数字来增加或减少字体大小。只需确保您保留`px`单位。

+   对于任何填充或边距值，您可以通过更改数字来增加或减少填充或边距。在每种情况下，请确保保留`px`单位。

+   为了使您的页面代码更易于访问，请考虑将所有`px`测量值转换为`rem`测量值。默认情况下，1 `rem`相当于 16 `px`，因此 20 `px`是 1.25 `rem`，24 `px`是 1.5 `rem`，32 `px`是 2 `rem`，48 `px`是 3 `rem`，依此类推。`rem`单位更易于访问，因为它测量的是浏览器用户在其浏览器设置中定义的默认字体大小。

## 7.5 为其他网站页面构建提示

虽然您的兴趣/爱好网站可能只包含一个页面，但更有可能的是，您将拥有几个页面，每个页面对应于您网站主要主题的每个子主题。如果是这样，您的下一个任务是提示 ChatGPT 生成您其他页面的代码。

幸运的是，这些其他页面将与您的首页结构非常相似，唯一的区别是`main`元素将存储每个页面的标题和文本。这意味着您每个子主题页面的提示将与您首页的提示非常相似。请注意，您也不需要为这些子主题页面添加任何新的 CSS，因此您可以跳过提示中的 CSS 部分。

这里有一个通用的提示您可以使用：

```py
I want to build a website page. I don't know how to code, so I need you to provide the code for me.

Write the HTML code for a web page that includes the following:
 * A header element that includes the title "[page title]" and the tagline "[page tagline]".
 * The header should also include the following links in the upper-right corner:
[Copy your home page links here]
* A main element that includes the text between triple quotation marks.
 """
[page content goes here]
 """
 * A footer element that includes the Copyright symbol, followed by the current year, followed by "[your name]".
 * In the page head section, include the tag <meta charset="utf-8">.
 * In the page head section, include a reference to a stylesheet file named "styles.css".
 * In the page head section, include a reference to the Google fonts X and Y.
 * Do not add any inline styles.
```

注意对 ChatGPT 的最后一条指令，即不要添加内联样式，这指的是直接添加到 HTML 标签中的 CSS 代码。在没有任何 CSS 相关指令的情况下，ChatGPT 倾向于插入一些以内联样式形式出现的格式建议。因为您需要的所有样式已经存在于您的 styles.css 文件中，所以您需要告诉 ChatGPT 不要添加任何可能破坏您页面的新样式。

图 7.12 显示了 ChatGPT 为我感兴趣网站生成的示例页面。无论您的兴趣或爱好是什么，为什么不请 ChatGPT 帮忙与朋友、家人以及任何访问您新网站的人分享您的热情呢？向世界展示您所关心的事情从未如此简单！

![图片](img/build-a-website-with-chatgpt-CH07_F12_McFedries3.png)

图 7.12 ChatGPT 生成的子主题页面

## 摘要

+   英雄图片是一张引人注目的照片或插图，当您首次进入页面时，它将占据整个浏览器窗口的宽度（通常也是整个高度）。

+   您可以使用 ChatGPT 来提出写作想法，提供关于特定主题的写作技巧，并帮助研究主题。

+   要让 ChatGPT 用您的声音写作，请提供您的一些写作示例，要求它分析样本的语气和风格，然后要求它写一些模仿您写作风格的内容。

+   为了获得最佳效果，您的页面提示应尽可能具体，包括颜色、字体大小和标题级别。

+   对于网站主页，将生成的 HTML 保存到 index.xhtml 文件，并将生成的 CSS 保存到 ChatGPT 在 HTML 代码中建议的文件名，通常是 styles.css。

+   对于每个网站子主题页面，请 ChatGPT 仅创建 HTML 代码，并将其保存到你为页面使用的任何文件名。

# 8 生成网站表单

本章涵盖

+   处理文本框和文本区域

+   与复选框和单选按钮一起工作

+   向表单添加选择列表和按钮

+   使用免费的 Getform 服务将表单数据发送给你

+   为构建活动注册页面创建 ChatGPT 提示

+   检查和自定义 ChatGPT 生成的代码

大多数网页——以及本书中迄今为止的所有网页项目——都是只读媒体，这意味着它们的目的是为每位访客提供与页面主题相关的信息。此类页面不需要访客做任何事情，除了他们的时间和注意力（在如此繁忙的时代，这两者都是很大的要求！）。

然而，有许多场景下你可能希望你的页面更加互动，这意味着你需要用户提供一些信息。也许你想要获取关于你网站的反馈。也许你想要向访客展示一份调查或测验。或者，也许你想要为人们提供一种订阅时事通讯或注册即将举行的活动的方式。无论原因如何，你通过提供一个*表单*来征求此类信息，这是一个特殊的网页对象，访客可以在其中填写字段并提交。

在本章中，你将学习表单的工作原理，你可以使用哪些类型的字段，以及如何将表单数据通过电子邮件发送给你。然后，你使用这些信息为 ChatGPT 创建一个详细的提示，以生成活动注册页面所需的代码。本章还提供了 ChatGPT 生成的代码的高级解释以及自定义代码的技巧。

## 8.1 检查本章的项目

本章的项目是一个简单的网页，其中包含一个表单，允许页面访客注册即将举行的活动。最终页面将包括以下组件：

+   包含网站标志、标题和标语的头元素

+   包含活动标题、一些信息和注册活动表单的主要元素

+   包含版权声明的页脚元素

图 8.1 展示了在本章中，在 ChatGPT 的帮助下你将构建的页面类型示例。

![图片](img/build-a-website-with-chatgpt-CH08_F01_McFedries3.png)

图 8.1 由 ChatGPT 生成的活动注册页面

示例表单包括所有主要的表单控件类型，这意味着你可以轻松修改表单以收集其他类型的信息，例如网站反馈或调查或测验。要完成任何这些，你需要了解每种表单控件的一些知识。然而，首先你需要学习如何将表单数据发送给你。

## 8.2 获取发送给你的表单数据

不幸的是，HTML 中并没有内置的方法可以将表单数据发送给您。要获取用户提交的表单数据，您需要与提供此服务的公司设置账户。这类公司有很多，但在这个项目中，我将使用 Getform ([`getform.io`](https://getform.io))。这家公司使您能够创建一个免费的*端点*，这是您的表单提交数据的地址。

虽然 Getform 有订阅计划，但您可能不需要，因为该服务还提供免费层，具有以下限制：

+   仅一个端点。

+   每月最多提交 50 份表格。

+   每个收到的表格提交电子邮件消息都会添加 Getform 品牌。

如果这些限制中的任何一个对您来说是决定性的，请查看 Getform 的付费计划[`getform.io/pricing`](https://getform.io/pricing)（计划起价为每月 19 美元）。

### 8.2.1 设置 Getform 账户

首先，按照以下步骤设置 Getform 账户：

1.  导航到 Getform 主页([`getform.io`](https://getform.io))。

1.  点击“免费生成端点”按钮。（如果您看不到该按钮，请点击“账户”、“注册”或直接导航到[`app.getform.io/register`](https://app.getform.io/register)。）

1.  输入您的姓名、电子邮件和密码，然后点击“注册”。

1.  前往您的电子邮件收件箱，打开 Getform 电子邮件消息，然后点击链接以验证您的账户。

### 8.2.2 创建 Getform 端点

验证您的账户后，登录您的 Getform 账户，然后按照以下步骤设置您的表单提交端点：

1.  在左侧侧边栏中点击“创建”。Getform 显示创建对话框，如图 8.2 所示（已填写）。

1.  确保已选中“表单”选项卡。

1.  使用“表单端点名称”文本框输入您的表单的简短但描述性的名称。

1.  使用时区列表选择您的时区。

1.  点击“创建”。

![图片](img/build-a-website-with-chatgpt-CH08_F02_McFedries3.png)

图 8.2 填写此表单以创建您的 Getform 端点。

Getform 创建您的新端点，然后显示端点的首页，如图 8.3 所示。在这个页面上有几个需要注意的地方：

+   当您提示 ChatGPT 构建您的表单时，您将需要端点地址。为了避免错误，请点击地址右侧的“复制”按钮，然后将地址粘贴到您的提示中。

+   为了防止垃圾邮件，示例表单包括以下代码：

    ```py
    <input type="hidden" name="_gotcha" style="display:none !important">
    ```

    这是一个*诱饵字段*的例子，这是一个用户看不到（因此不会填写）但垃圾邮件机器人会填写并提交的字段。（它被称为诱饵字段，因为垃圾邮件机器人无法抗拒它。）填写的诱饵字段告诉 Getform 服务器提交必须是垃圾邮件。当您稍后构建 ChatGPT 提示时，您会要求 ChatGPT 将此代码包含在您的表单中。

+   您可以点击页面顶部的“收件箱”以监控您的表单提交。但请记住，Getform 也会将每个表单提交发送到您的电子邮件地址。

![](img/build-a-website-with-chatgpt-CH08_F03_McFedries3.png)

图 8.3 当你的 Getform 端点创建后，你会看到它的主页。

## 8.3 构建表单

表单是一组特殊的 HTML 元素，它允许你从用户那里收集信息，然后将这些信息发送到某个地方。这些特殊 HTML 元素被称为*控件*，在接下来的几节中，你将了解最常见和最有用的六种表单控件。了解每个控件的功能以及它设计用来收集的信息类型，将使你能够设置提示，以便 ChatGPT 可以构建你需要的表单。

在此过程中，我将为你提供每种控件类型的示例 ChatGPT 提示。在每个示例中，假设在提示中已经包含了以下类似的指令：

```py
Include the code for an HTML form that has the following specifications:
```

### 8.3.1 指定表单的端点

在本章的示例中，你将学习如何使用名为 Getform 的服务来获取发送给你的表单数据。此服务为你提供一个唯一的地址，称为*端点*，它是一个远程脚本，用于处理表单数据。当你指示 ChatGPT 构建 HTML 表单时，第一个规范就是这个端点地址。（参考第 8.2 节了解如何生成用于表单的唯一端点地址。）以下是一个示例说明：

```py
In the form element, set the action attribute to "*endpoint*" and the method attribute to "POST".
```

在此提示中，将`endpoint`替换为 Getform 服务提供的地址。指令中提到的`method`属性告诉浏览器如何发送表单数据。

在完成这些之后，现在是时候更仔细地查看最常见的表单控件了。第一种控件类型是文本框，接下来将讨论。

### 8.3.2 使用文本框收集文本

最常见的表单控件类型是*文本框*，它是一个矩形区域，用于存放用户输入的文本。HTML 提供了一大批文本框输入类型，每种都设计用来存放特定类型的信息。以下是四种最常见的输入类型：

+   *Text*—可以存放任何类型的文本，可以是字母、数字和符号的任意组合。以下是在你的表单提示中要包含的示例说明：

    ```py
    A text box.
    ```

+   *Number*—仅包含数字数据。示例说明：

    ```py
    A text box for numeric data.
    ```

+   *Email*—仅包含电子邮件地址。该控件还会检查用户是否输入了有效的电子邮件地址。以下是一个给 ChatGPT 的示例说明：

    ```py
    A text box for an email address.
    ```

+   *URL*—包含一个网页地址。示例说明：

    ```py
    A text box for a web address.
    ```

图 8.4 展示了每种输入类型的示例。请注意，数字字段包括上箭头和下箭头，用户可以点击它们来增加和减少（分别）当前字段值。

![](img/build-a-website-with-chatgpt-CH08_F04_McFedries3.png)

图 8.4 四种主要的文本框输入类型

tIP 要让 ChatGPT 生成配置你的表单的代码，其中左侧是文本，右侧是文本框，请在你的提示中包含以下内容：“将表单设置为两列网格容器，第一列包含标签，第二列包含控件。”

当提示 ChatGPT 在表单中包含文本框时，你可以控制每个文本框的以下内容：

+   你可以通过指定字符大小来设置框的宽度。例如，在图 8.4 中，每个文本框宽度为 30 个字符。示例提示：

    ```py
    A text box that is 25 characters wide.
    ```

+   你可以指定一个初始值。此值默认显示在文本框中，尽管用户可以自由编辑或替换此默认值。示例提示：

    ```py
    A numeric text box with the initial value 42.
    ```

+   你可以指定一个*占位符*，这是一种暂时出现在文本框中的文本，简要告诉用户应该在文本框中输入什么。一旦用户开始输入，占位符文本就会消失。示例提示：

    ```py
    An email text box with the placeholder text "Type your email address".
    ```

+   你可以指定最大和/或最小长度（以字符为单位）：

    ```py
    A text box with a minimum length of 3 and a maximum length of 10.
    ```

+   如果你指定文本框是“必需的”，则用户在提交表单之前必须填写一个值：

    ```py
    An email text box that is required.
    ```

你可能想知道如何让 ChatGPT 为每个控件命名（例如，图 8.4 中每个控件左侧显示的名称）。如果你不指定名称，ChatGPT 会为你生成一个。指定自己的控件名称是下一节的主题。

### 8.3.3 为每个控件添加标签

如果你检查上一节中的图 8.4，你可以看到项目分为两列：控件在右侧列，左侧列包含描述每个控件的简短文本。这些简短文本被称为*标签*，除了下面的按钮控件外，你需要为每个字段包含一个标签。你的标签应该足够短，以免占用太多页面空间，但描述性足够强，以便用户知道他们应该在每个字段中输入什么。

当你构建 ChatGPT 的表单提示时，最好在说明其余控件规格的同时说明你想要的标签：

```py
An email address text box. Make the text box 30 characters wide and give it the label "Email address".
```

### 8.3.4 使用文本区域处理更多文本

文本框对于收集用户相对较短的信息片段非常有用，例如他们的姓名、电子邮件地址或最喜欢的数字。然而，有时你的表单可能需要收集更长的文本输入，如反馈、建议、问题或甚至用户的个人简介。对于这些较长的输入，你可以添加一个*文本区域*，这是一个支持多行输入的表单字段。图 8.5 显示了文本区域的示例。

![图片](img/build-a-website-with-chatgpt-CH08_F05_McFedries3.png)

图 8.5 文本区域的示例

当提示 ChatGPT 在表单中包含文本区域时，你可以按以下方式自定义文本区域：

+   你可以通过指定行数来设置文本区域框的高度。例如，在图 8.5 中，文本区域的高度为六行。示例指令给 ChatGPT：

    ```py
    A text area with the label "Suggestions" and a height of six rows.
    ```

注意：无论文本区域的高度如何，用户都可以自由输入超过指定行数的文本。如果文本量超过文本区域的高度，用户可以垂直滚动文本区域或通过拖动框的右下角来调整其大小。

+   你可以通过指定列数来设置文本区域框的宽度：

    ```py
    A text area with a width of 30 columns.
    ```

+   文本区域允许用户输入他们想要的任何长度的条目。然而，如果你担心会被过多的文本淹没，你可以指定字符的最大输入大小：

    ```py
    A text area with a maximum length of 240 characters.
    ```

+   如果需要，你还可以指定字符的最小输入大小：

    ```py
    A text area with a minimum length of 20 characters.
    ```

+   如果你希望用户在提交表单之前必须填写一个值，可以将文本区域设置为“必填”：

    ```py
    A text area that is required.
    ```

在某种程度上，与文本密集的文本区域相反的情况是当你需要用户在两个简单的可能性之间进行选择时：是/否、开/关等。不要使用文本区域或文本框来处理这种情况——HTML 提供了一个特殊的控制来处理这些非此即彼的选择，这是下一节的主题。

### 8.3.5 使用复选框获取是/否信息

一种常见的信息收集情况是当用户有一个选择，他们要么接受要么拒绝。同样，根据选项的措辞和意图，用户可能会说“是”或“否”，或者他们可能会打开或关闭。对于所有这些场景——接受/拒绝、是/否、开/关——你可以在你的表单中包含一个称为复选框的控制。这是一个显示小方框的控制。如果用户想要为复选框提交一个肯定响应（接受或“是”或“开”），他们点击复选框以在其中添加勾选标记；如果用户想要为复选框提交一个否定响应（拒绝或“否”或“关”），他们点击复选框以移除其勾选标记。

图 8.6 展示了几个复选框的示例。顶部的复选框未勾选，这意味着（在这种情况下）用户不想被通知未来的事件。底部的复选框已勾选，这意味着（再次，在这种情况下）用户确实想订阅该网站的通讯。以下是在你的表单提示中包含的示例指令：

```py
A checkbox with the label "Get notified about future events".
```

![](img/build-a-website-with-chatgpt-CH08_F06_McFedries3.png)

图 8.6 一些示例复选框

当提示 ChatGPT 在表单中包含复选框时，你可以通过指定复选框是否初始勾选来自定义复选框，如下例所示：

```py
A checkbox with the label "Subscribe to our newsletter" that is initially checked.
```

如果你希望你的用户在超过两个选项之间进行选择，HTML 提供了一些解决方案，首先是下一节将要讨论的单选按钮。

### 8.3.6 使用单选按钮选择多个选项之一

在上一节中，你学习了如何通过提供复选框来启用用户在两种状态之间进行选择。然而，通常情况下，你希望用户从三个或四个可能性中选择一个。例如，如果事件发生在周五、周六和周日，你可能希望用户只选择这些日子中的一个。同样，对于免费 T 恤赠送，你可能要求用户选择他们想要的尺码：小号、中号、大号或加大号。

当你需要你的访客在三个或四个选项中选择一个时，你可以在你的表单中添加一组单选按钮，这是一个具有以下特征的 HTML 元素集：

+   每个按钮都是一个小的圆圈。

+   一次只能选择一个按钮。

+   当前选中的按钮的圆圈被填充。

+   所有未选中的按钮都有空圆圈。

+   当用户单击未选中的按钮时，该按钮的圆圈会被填充，而之前选中的按钮的圆圈变为空。

图 8.7 展示了单选按钮组的示例。Medium 单选按钮当前被选中。

![](img/build-a-website-with-chatgpt-CH08_F07_McFedries3.png)

图 8.7 一组单选按钮

当您准备构建用于表单的 ChatGPT 提示时，您可以使用如下指令：

```py
A group of radio buttons with the following options: "Small", "Medium", "Large", and "Extra Large".
```

您可以按照以下方式自定义您的单选按钮：

+   您可以指定哪个单选按钮最初被选中：

    ```py
    A group of radio buttons with the following options: "Small", "Medium", "Large", and "Extra Large". The "Medium" radio button is initially selected.
    ```

+   您可以用“图例”元素包围您的单选按钮组，并为该图例指定一个“标题”。图 8.7 中的单选按钮组有一个带有标题`选择 T 恤尺寸`的图例。ChatGPT 倾向于自动包含图例元素，但您可以使用如下指令来指定您想要的标题：

    ```py
    A group of radio buttons with the following options: "Small", "Medium", "Large", and "Extra Large". Include a legend element with the caption "Choose a t-shirt size".
    ```

如果您需要用户从超过四个选项中进行选择，您应该将这些选项放入选择列表，正如我在下一节中描述的那样。

### 8.3.7 使用列表提供更多选择

理论上，您可以为用户提供单选按钮的数量没有合理的限制。然而，实际上，拥有大量单选按钮可能会让用户感到困惑，并且会占用过多的页面空间。一般规则是，在任何单选按钮组中最多有四个选项。

然而，向用户提供五个或更多选项并不罕见。也许您希望用户从一周的七天中选择一天（从星期一到星期日）。或者您可能要求访客选择一个州或国家（例如，收集用户的邮寄地址）。

对于这些较大的选择集合，您可以将您想要向用户展示的所有选项放入一个*选择列表*中，默认情况下，它以下拉列表的形式显示，如图 8.8 所示。单击列表将显示用户可用的选项菜单，如图 8.9 所示。

![](img/build-a-website-with-chatgpt-CH08_F08_McFedries3.png)

图 8.8 显示，选择列表最初以下拉列表的形式出现。

![](img/build-a-website-with-chatgpt-CH08_F09_McFedries3.png)

图 8.9 单击选择列表将显示可用的选项。

这里是一个您可以包含在表单提示中的示例指令：

```py
A selection list that includes the following items: "None", "Cat", "Dog", "Ferret", "Fish", "Hamster", "Parrot", "Peeve", and "Snake".
```

当您创建 ChatGPT 表单提示时，您可以按照以下方式自定义您的选择列表：

+   您可以指定哪个列表项最初被选中：

    ```py
    A selection list with the following options: "Happy", "Content", "Neutral", "Melancholy", and "Sad." Make "Neutral" the initially selected option. 
    ```

+   您可以指定用户是否可以选中多个列表项（通过在 Windows 上按 Ctrl 或 macOS 上按 Cmd 并单击每个项）：

    ```py
    A selection list with the label "Philosophers You've Read" and the following options: "Plato", "Aristotle", "Blaise Pascal", "Friedrich Nietzsche", and "Jean-Paul Sartre." Allow the user to make multiple selections.
    ```

+   您可以指定行数的大小。这会将下拉列表转换为显示您指定行数的常规列表框。如果显示的行数少于列表中的项目数，用户可以垂直滚动列表框。以下是一个示例指令：

    ```py
    A selection list with the label "Dream Vacation" and the options "Beach getaway", "Long-distance hike", "Mountain resort", "Urban exploration", and "Staycation". Give the list a height of five rows.
    ```

现在您已经熟悉了所有基本表单控件，您就可以了解用户如何提交表单了。

### 8.3.8 使用按钮提交表单

当您在电脑上处理对话框时，您会填写（如果有）字段，然后点击一个按钮（通常标有“确定”）来告诉您的应用程序或操作系统您已经完成了对话框，它应该处理对话框数据。从某种意义上说，HTML 表单是网页对话框的等价物，这意味着您的表单需要一种方式让用户告诉浏览器他们已经完成了表单，浏览器应该处理它。用户通过点击一个按钮来完成这个操作，这个按钮是一个 HTML 元素，其外观和行为与电脑对话框中的“确定”按钮非常相似。图 8.10 显示了带有“发送它”按钮的表单示例。

![图片](img/build-a-website-with-chatgpt-CH08_F10_McFedries3.png)

图 8.10 带有“发送它”按钮的表单

当您要求 ChatGPT 生成表单代码时，ChatGPT 总是会包括一个名为“提交”的按钮。为了指定您首选的按钮名称，以下是一个可以包含在您整体表单提示中的 ChatGPT 示例指令：

```py
A submit button element with the name "Send It".
```

在表单元素中点击按钮被称为“提交”表单，在下一节中，您将学习如何将表单数据发送给您。

好的，现在您已经知道了成功提示 ChatGPT 构建工作表单所需的所有信息，正如我在下一节中描述的那样。

## 8.4 撰写活动注册页面的提示语

本章的项目是一个包含表单的单页，该表单允许用户注册参加当地搭建谷仓活动。该表单本身将使用我在本章前面讨论的六种类型的控件：一个文本框、一个电子邮件字段、一个文本区域、一个复选框、一个单选按钮组、一个选择列表和一个提交表单的按钮。

在继续之前，您应该已经拥有网站标题、标语和页面标题。您还应该知道您想要用于页面文本的 Google Fonts 字体类型以及您想要应用的配色方案。请参阅第三章了解如何获取 ChatGPT 在标题、字体和颜色方面的帮助。

您的提示语首先告诉 ChatGPT 您希望它帮助您构建一个网页，并且您不知道如何编写代码，因此它将不得不为您生成代码：

```py
I want to build a web page that enables page visitors to use a form to sign up for an event. I don't know how to code, so I need you to provide the code for me.

First, write the HTML code for a web page that includes the following:
```

然后，您指定页面的内容，包括以下项目（参见图 8.11）：

+   包含您的标志、网站标题和标语的头

+   一个主元素，它从页面标题开始，后面跟着一些介绍性文本

+   用户可以提交以注册您活动的表单

+   包含版权声明的页脚

接下来，您指导 ChatGPT 生成页面格式的 CSS：

```py
Second, in a separate file please write the CSS code for the following:
```

然后，您指定格式，包括以下内容：

+   页面背景颜色和文字颜色。

+   您希望用于网站标题、标语、页面标题、页面文字和表单控件的字体大小。

+   用于标题和常规页面文字的字体。

+   页面的最大宽度。这可以防止文字行过长。本页面的最大长度为 800 px。

![](img/build-a-website-with-chatgpt-CH08_F11_McFedries3.png)

图 8.11 事件注册页面元素

这是我自己的事件注册页面的一个示例提示：

```py
I want to build a web page for an event sign-up page. I don't know how to code, so I need you to provide the code for me.

First, write the HTML code for a web page that includes the following:
 * A header element that includes an image named barn.png, the title "Barnstormers!", and the tagline "Building old-fashioned barns the new-fangled way".
 * A main section with the heading "Our Next Barn-Raising".
 * A paragraph with the text "We're looking for volunteers to help with our next barn-raising, which takes place Saturday August 23 and Sunday August 24\. If you want to help, please fill out and submit the form below.".
  * Include the code for an HTML form that has the following specifications:
    * In the form element, set the action attribute to "https://getform.io/f/dbb986ea-ee50-42ba-abe7-5c304a087444" and the method attribute to "POST".
    * A text box with the label "Name", a width of 30 characters, and the placeholder "Your name".
    * An email field with the label "Email", a width of 30 characters, and the placeholder "Your email address".
    * A text area with the label "Skills", 3 rows, and 30 columns.
    * A checkbox with the label "Get notified about future barn-raisings".
    * A radio button group with the options "Saturday", "Sunday", and "Both". Select the "Saturday" option. Add a legend element with the caption "Day(s) you can attend".
    * A selection list with the label "Select your free gift" and the options "None", "Baseball cap", "Coffee mug",  "Poster", "T-shirt", and "Tote bag".
    * The following code: <input type="hidden" name="_gotcha" sty1e="display:none !important">
    * A button element with the name "Sign Me Up!".
    * Use paragraphs to separate each form control, except for the radio buttons, which should be separated by line breaks.
  * A footer element that includes the Copyright symbol, followed by the current year, followed by "Barnstormers!".
 * In the page head section, include the tag <meta charset="utf-8">.
 * In the page head section, include the tag <meta name="viewport" content="width=device-width, initial-scale=1">.

Second, in a separate file write the CSS code for the following:
 * The page has a 24px margin.
 * The page background color is cornsilk. 
 * The page text color is saddlebrown.
 * Make the header image a maximum width of 150px and floated to the left.
 * The title is 48px, aligned to the right, and with no bottom margin.
 * The tagline is 26px, formatted as italic and small caps, aligned to the right, and with no top margin.
 * The main section has a top margin of 75px.
 * The main section heading font size is 30px.
 * The main section font size is 20px.
 * The form width is 400px and the left margin is 32px.
 * The form, input, textarea, select, and button font size is 20px.
 * The button text color is saddlebrown.
 * For all the page text, use the Bitter font from Google Fonts.
 * The footer has 5px padding all around, 50px top margin, and a saddlebrown top border.
 * Give the page a maximum width of 800px.
```

ChatGPT 首先生成 HTML 代码，您可以复制并粘贴到名为 index.xhtml 的文件中保存。在这段代码中，您应该看到顶部附近有一行类似于以下内容：

```py
<link rel="stylesheet" type="text/css" href="styles.css">
```

此代码告诉网络浏览器在名为 styles.css 的文件中查找 CSS 代码，因此您的下一个任务是复制生成的 CSS 代码，然后粘贴并保存到名为 styles.css 的文件中（或您在`<link>`标签中看到的任何名称）。请确保将 styles.css 文件保存到与 index.xhtml 文件相同的文件夹中。您还需要将您的页眉图像文件复制到同一文件夹中。有关更多关于工作网页文件的信息，请参阅附录 A。

我使用 OpenAI 的 ChatGPT 应用将提示提交给 GPT-4。生成的代码产生了如图 8.12 所示的页面。

![](img/build-a-website-with-chatgpt-CH08_F12_McFedries3.png)

图 8.12 我的注册页面

如果您对 ChatGPT 生成的页面和表单满意，您可以自由跳过本章的其余部分并将代码部署到网络上（有关详细信息，请参阅附录 B）。但是，如果您想了解更多关于生成的网页代码，请继续下一节以进行更深入的查看。

## 8.5 检查事件注册页面代码

您不需要了解 ChatGPT 生成的网页代码是如何工作的。但是，如果您想深入了解，接下来的几节将简要介绍由上一节提示（如图 8.12 所示的页面）生成的事件注册页面代码，这不是过于技术性的描述。

注意：本书网站上（[www.manning.com/books/build-a-website-with-chatgpt](https://www.manning.com/books/build-a-website-with-chatgpt)）和 GitHub 存储库（[`github.com/paulmcfe/websites-with-chatgpt`](https://github.com/paulmcfe/websites-with-chatgpt)）提供了我事件注册页面的生成 HTML 和 CSS 代码。

希望我的代码注释能帮助您理解底层发生的事情，并帮助您调整或自定义自己的代码。

### 8.5.1 检查 HTML

这是 ChatGPT 为我事件注册页面生成的 HTML 代码：

```py
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <meta name="viewport" 
          content="width=device-width, initial-scale=1">         ①
    <title>Barnstormers!</title>
    <link rel="stylesheet" 
          type="text/css" href="styles.css">                     ②
</head>
<body>
    <header>                                                     ⑥
        <img src="barn.png" alt="Barnstormers logo">             ③⑥
        <h1>Barnstormers!</h1>                                   ④⑥
        <p>Building old-fashioned barns the new-fangled way</p>  ⑤⑥
    </header>                                                    ⑥
    <main>
        <h2>Our Next Barn-Raising</h2>
        <p>We're looking for volunteers to help with our next 
           barn-raising, which takes place Saturday August 23 
           and Sunday August 24\. If you want to help, please 
           fill out and submit the form below.</p>
        <form action="https://getform.io/f/                      ⑦
              dbb986ea-ee50-42ba-abe7-5c304a087444"              ⑦
              method="POST">                                     ⑦
            <p>
                <label>Name:                                     ⑧
                <input type="text"                               ⑧
                       name="name"                               ⑧
                       size="30"                                 ⑧
                       placeholder="Your name">                  ⑧
                </label>                                         ⑧
            </p>
            <p>
                <label>Email:                                    ⑨
                <input type="email"                              ⑨
                       name="email"                              ⑨
                       size="30"                                 ⑨
                       placeholder="Your email address">         ⑨
                </label>                                         ⑨
            </p>
            <p>
                <label>Skills:                                   ⑩
                <textarea name="skills"                          ⑩
                          rows="3"                               ⑩
                          cols="30">                             ⑩
                </textarea>                                      ⑩
                </label>                                         ⑩
            </p>
            <p>
                <label>                                          ⑪
                <input type="checkbox"                           ⑪
                       name="notify">                            ⑪
                Get notified about future barn-raisings          ⑪
                </label>                                         ⑪
            </p>
            <fieldset>                                           ⑫
                <legend>Day(s) you can attend</legend>           ⑫
                <label>                                          ⑫
                <input type="radio"                              ⑫
                       name="day"                                ⑫
                       value="Saturday"                          ⑫
                       checked>                                  ⑫
                Saturday                                         ⑫
                </label>                                         ⑫
                <br>                                             ⑫
                <label>                                          ⑫
                <input type="radio"                              ⑫
                       name="day"                                ⑫
                       value="Sunday">                           ⑫
                Sunday                                           ⑫
                </label>                                         ⑫
                <br>                                             ⑫
                <label>                                          ⑫
                <input type="radio"                              ⑫
                       name="day"                                ⑫
                       value="Both">                             ⑫
                Both                                             ⑫
                </label>                                         ⑫
            </fieldset>                                          ⑫
            <p>
                <label>Select your free gift:                    ⑬
                <select name="gift">                             ⑬
                    <option value="">None</option>               ⑬
                    <option value="cap">Baseball cap</option>    ⑬
                    <option value="mug">Coffee mug</option>      ⑬
                    <option value="poster">Poster</option>       ⑬
                    <option value="shirt">T-shirt</option>       ⑬
                    <option value="bag">Tote bag</option>        ⑬
                </select>                                        ⑬
                </label>                                         ⑬
            </p>
            <input type="hidden"                                 ⑭
                   name="_gotcha"                                ⑭
                   style="display:none !important">              ⑭
            <p>
                <button type="submit">Sign Me Up!</button>       ⑮
            </p>
        </form>
    </main>
    <footer>© 2023 Barnstormers!</footer>                        ⑯
</body>
</html>
```

① 帮助页面在移动设备上正确显示

② 告诉网络浏览器在哪里找到 CSS 代码

③ 网站标志

④ 网站标题

⑤ 网站标语

⑥ 页面页眉

⑦ 表单元素指定端点

⑧ 名称文本框

⑨ 电子邮件文本框

⑩ 技能文本区域

⑪ 复选框

⑫ 单选按钮组文本框

⑬ 选择列表

⑭ 隐藏的“诱饵”字段

⑮ 提交按钮

⑯ 页面页脚

在阅读 HTML 代码时，请注意以下几点：

+   在`form`元素中，请注意`action`属性设置为 Getform 端点的地址。（注意，我已经更改了真实地址，因此请不要尝试在自己的表单中使用此地址，因为它不会工作。）

+   对于每个表单控件（除了按钮），请注意 ChatGPT 也包含一个`name`属性。网络浏览器使用这些`name`属性值在提交表单时识别每个字段。图 8.13 显示了示例提交。请注意，每个字段的名称——`name`、`email`、`skills`、`day`、`gift`和`notify`——与表单中的`name`属性值相匹配。

![图片](img/build-a-website-with-chatgpt-CH08_F13_McFedries3.png)

图 8.13 表单提交出现在您的 Getform 页面上。

+   注意，每个单选按钮和选择列表选项都有自己的`value`属性。当浏览器提交表单时，它会发送当前选中的单选按钮和列表项的值。例如，在图 8.13 中，提交给`day`字段（单选按钮组）的值是`Saturday`，提交给`gift`字段（选择列表）的值是`shirt`（即列表中的 T 恤项）。

+   在`button`元素之前是一个`input`元素，其`type`属性设置为`hidden`，其`name`属性设置为`_gotcha`。该字段用于检测垃圾邮件机器人，当它们提交此表单时，被编程为填写每个字段，包括这个隐藏字段。如果 Getform 服务收到一个包含此隐藏字段已填写的表单提交，它知道它正在处理垃圾邮件并丢弃该提交。

最后，请注意 HTML 代码中包含以下行：

```py
<link rel="stylesheet" href="styles.css">
```

此标签告诉网络浏览器在哪里找到 CSS 代码，我将在下一节中描述。

### 8.5.2 检查 CSS

这是 ChatGPT 为我生成的事件注册页面 CSS 代码：

```py
@import url('https://fonts.googleapis.com/css2?
    family=Bitter:ital, wght@0,400;0,700;1,400
    display=swap');                                  ①

body {
    margin: 24px;
    background-color: cornsilk;                      ②
    color: saddlebrown;                              ②
    font-family: 'Bitter', serif;                    ②
    max-width: 800px;                                ③
    margin-left: auto;                               ④
    margin-right: auto;                              ④
}

header img {
    max-width: 150px;                                ⑤
    float: left;                                     ⑤
}

header h1 {
    font-size: 48px;                                 ⑥
    text-align: right;                               ⑥
    margin-bottom: 0;
}

header p {
    font-size: 26px;                                 ⑦
    font-style: italic;                              ⑦
    font-variant-caps: small-caps;                   ⑦
    text-align: right;    
    margin-top: 0;
}

main {
    margin-top: 75px;                                ⑧
}

main h2 {
    font-size: 30px;                                 ⑨
}

main p, form {
    font-size: 20px;                                 ⑩
}

form {
    width: 400px;                                    ⑪
    margin-left: 32px;
}

form input, form textarea, form select, form button {
    font-size: 20px;                                 ⑫
}

form button {
    color: saddlebrown;                              ⑬
}

footer {
    padding: 5px;
    margin-top: 50px;
    border-top: solid saddlebrown;
}
```

① 从 Google Fonts 加载 Bitter 字体

② 设置页面背景颜色、文本颜色和字体

③ 将最大页面宽度设置为 800 px

④ 使页面居中

⑤ 设置最大标志宽度，并将其浮动到左侧

⑥ 将页面标题字体大小设置为 48 px，并右对齐

⑦ 使用 26 px 字体大小、斜体、小写字母和右对齐设置标语样式

⑧ 在主要元素顶部添加边距

⑨ 设置主要标题的字体大小

⑩ 设置常规页面文本的字体大小

⑪ 设置表单的宽度

⑫ 设置表单控件文本的字体大小

⑬ 将文本颜色应用于按钮

如果您喜欢，可以使用这些注释来帮助定制您的网页代码，正如我在下一节中描述的那样。

## 8.6 定制事件注册页面

如果 ChatGPT 生成的表单代码甚至接近您想要的结果，您最好开始一个新的聊天会话并提交一个修订的提示。然而，如果表单代码接近您所寻找的，可能更容易自行修改它。

首先，这里有一些针对 HTML 代码的定制建议：

+   随意编辑页面上的任何文本，例如标题、标语、简介文本或任何表单标签。请注意，不要编辑或删除围绕每段文本的 HTML 标签（例如括号表单标签的`<label>`和`</label>`标签）。

+   如果你想要包含第二个简介段落，请将编辑光标放在现有简介段落结束的`</p>`标签之后。按 Enter 或 Return 键开始新行，输入一个`<p>`标签，输入你的段落文本，并以`</p>`标签结束。

+   在表单代码中，你可以编辑一些标签属性值。例如，对于文本框，你可以修改`size`和`placeholder`属性值；对于文本区域，你可以修改`rows`和`cols`属性值；并且你可以修改任何`value`属性字符串。在这些所有情况下，确保只修改双引号之间的文本。此外，不要更改任何`type`或`name`属性值。

+   在 HTML 代码的页脚部分，你可以添加指向你的社交媒体账户的链接，正如我在第四章中描述的那样。

现在，这里有一些针对 CSS 代码的定制想法：

+   要给你的页面设置不同的背景颜色，为`body`元素的`background-color`属性使用不同的颜色关键字。

+   要为页面文本指定不同的颜色，为`body`元素的`color`属性指定不同的颜色关键字。

+   CSS 代码在其他两个地方使用了页面文字颜色：`form button`元素的`color`属性和`footer`元素的`border-top`属性。为了保持颜色的一致性，你需要将这些颜色值替换为在上一项中使用的颜色关键字。

+   如果你希望你的页面有不同的最大宽度，将`max-width`值更改为`800px`之外的其他值。

+   如果你希望将页眉标志放在右侧，并将文本和标语对齐在左侧，你需要进行三个更改：

    +   在`header img`元素中，将`float`值更改为`right`。

    +   在`header h1`元素中，将`text-align`值更改为`left`。

    +   在`header p`元素中，将`text-align`值更改为`left`。

+   对于任何字体大小值，你可以更改数字以增加或减少字体大小。只需确保保留`px`单位。

+   对于任何填充或边距值，你可以更改数字以增加或减少填充或边距。在每种情况下，确保保留`px`单位。

+   要使你的页面代码更易于访问，考虑将所有 px 测量值转换为 rem 测量值。默认情况下，1 rem 相当于 16 px，因此 20 px 是 1.25 rem，24 px 是 1.5 rem，32 px 是 2 rem，48 px 是 3 rem，依此类推。rem 单位更易于访问，因为它测量的是相对于浏览器用户在其浏览器设置中定义的默认字体大小的字体大小。

## 摘要

+   表单是一组特殊的 HTML 元素，它允许你收集信息，然后将这些信息发送到某个地方（例如你的电子邮件地址）。

+   表单的终点是当用户提交表单时，网络浏览器发送表单数据的目标地址。

+   文本框是一个矩形区域，用于容纳用户输入的文本。您可以设置文本框以存储特殊数据类型，例如电子邮件地址、数字和 URL。

+   标签是描述特定控件文本。

+   文本区域是一个表单字段，支持较长的多行文本输入。

+   对于是/否或开/关类型的数据，请使用复选框。

+   要使用户能够从三个或四个选项中选择一个，请使用单选按钮组。

+   要使用户能够从五个或更多选项中选择，请使用选择列表。

+   在表单中包含一个按钮，以便用户可以提交表单数据。

+   为了获得最佳效果，您的页面提示应尽可能具体，包括颜色、字体大小和标题级别。

# 9 向您的页面添加列表

本章涵盖

+   指示 ChatGPT 构建项目符号列表

+   要求 ChatGPT 生成编号列表

+   自定义您的列表

+   为构建食谱页面制作 ChatGPT 提示

+   检查和自定义 ChatGPT 生成的代码

“内容为王”是网络早期的一个古老（而且遗憾的是，带有性别歧视）的谚语。它的意思是，每个网页上最重要的东西就是它所包含的内容。换句话说，如果你发布了优质的内容，全世界都会蜂拥而至你的网站门口。

这可能在 20 世纪 90 年代是真实的，当时人们对自己访问的每个网页期望不多。然而，如今，如果你展示得不好，即使有优质的内容也毫无意义。如果你已经完成了前几章中的任何网络项目，你可能会对 ChatGPT 的提示如此具体感到惊讶（但希望不是失望）。这种详细程度是必要的，因为否则，ChatGPT 将生成页面代码，这些页面明显不吸引人：单调、拥挤且布局不佳。是的，你有想要分享的精彩内容，但为了防止访客在到达后几秒钟内离开，你需要以引人入胜的方式展示这些内容。

在本章中，你将学习两种使你的内容更容易阅读、更容易理解并更吸引读者的技术。这两种技术是项目符号列表和编号列表，它们是现代网页中最常见的模式之一，也是当今一些最受欢迎网站的基础。然后你将运用你新学到的列表知识，为 ChatGPT 创建一个详细的提示，以生成食谱页面的代码。本章还提供了 ChatGPT 生成的代码的高级解释以及自定义它的技巧。

## 9.1 检查本章的项目

在本章中，你将得到 ChatGPT 为你创建的项目，这是一个基本的网页，引导读者了解制作坚果棒的食谱。最终页面将包括以下组件：

+   包含网站标志、标题和标语的头元素

+   一个以食谱标题和介绍开始的主体元素

+   几个包含食谱成分的项目符号列表

+   食谱步骤的编号列表

+   包含版权声明页脚元素

图 9.1 展示了你将在本章中说服 ChatGPT 为你生成的页面类型的一个示例。

![图片](img/build-a-website-with-chatgpt-CH09_F01_McFedries3.png)

图 9.1 ChatGPT 生成的食谱页面

示例页面包括两个项目符号列表和一个单独的编号列表（带编号的子列表），但你可以轻松地修改这个项目，只包含项目符号列表、只包含编号列表，或者包含这两种类型的多个列表。这意味着你可以创建包含内容如前十名列表、教程、文档、旅行指南、产品评论、你最喜欢的书籍、电影、电视节目、游戏、冰淇淋口味、计算机书籍作者等的页面。在你做到所有这些之前，你需要了解每种列表类型的一些信息。

## 9.2 创建项目符号列表

项目符号列表是一组 HTML 元素，它们以垂直列表的形式展示多个项目，其中每个项目都稍微缩进，并在前面有一个称为*项目符号*的小黑圆圈。当你想要展示多个项目但项目的顺序不是列表的必要组成部分时，你会使用项目符号列表。图 9.2 展示了项目符号列表的一个示例。

![图片](img/build-a-website-with-chatgpt-CH09_F02_McFedries3.png)

图 9.2 项目符号列表的示例

这是如何指导 ChatGPT 生成此类列表的代码：

```py
Generate the HTML code for a bulleted list that includes the following items: "Francis", "Haden", "Honey", "Keitt", "Kent", and "Tommy Atkins".
```

这是生成的代码：

```py
<ul>
    <li>Francis</li>
    <li>Haden</li>
    <li>Honey</li>
    <li>Keitt</li>
    <li>Kent</li>
    <li>Tommy Atkins</li>
</ul>
```

该代码有两个主要组成部分：

+   整个内容被`<ul>`和`</ul>`标签包围（其中`ul`是*无编号列表*的缩写）。

+   每个列表项都被`<li>`和`</li>`标签包围（其中`li`是*列表项*的缩写）。

对于短项目（一个单词或短语），在每项周围加上引号是可以的。如果你的列表包含较长的文本项，你将想要使用我在下一节中讨论的方法。

### 9.2.1 处理较长的列表项

项目符号列表项不一定是单个单词或短语。你可以在每个项中包含你需要的任意多的文本。（尽管如此，如果你的列表项内容太长——比如说，超过几句话——你的列表就会变得难以阅读和扫描。）对于较长的列表项，你的提示应该清晰地分隔各项，这样 ChatGPT 就不会感到困惑。以下是一个示例指令：

```py
Generate the HTML code for a bulleted list that includes the following items:
- "Sailing Alone Around the Room," by Billy Collins. The former U.S. poet laureate at the top of his game.
- "Blue Horses," by Mary Oliver. Each poem in this collection is a gem.
- "Human Wishes," by Robert Hass. If prose poetry is more your thing, you owe yourself these stunning examples of the form.
- "The Carrying," by Ada Limón. The current U.S. poet laureate at the top of *her* game.
- "All of Us," by Raymond Carver. The complete poetical works of the master of quiet desperation.
- "What the Living Do," by Marie Howe. A searingly honest search for hope amidst overwhelming grief. Highly recommended.
```

注意到指令在每个列表项前都加上了破折号（`-`）。ChatGPT 理解破折号代表一个新的列表项（加号[`+`]同样有效）。图 9.3 展示了从该指令生成的 ChatGPT 代码在网页浏览器中的显示方式。

![图片](img/build-a-website-with-chatgpt-CH09_F03_McFedries3.png)

图 9.3 带有较长列表项的项目符号列表

如果你的某个项目符号本身需要有一个项目符号列表？这将在下一节中介绍。

### 9.2.2 嵌套项目符号列表

常见的项目符号列表模式是其中一个项目包含其自己的项目符号列表。这被称为*嵌套*项目符号列表，它使您可以将页面信息分成多个层次，这可以使复杂的数据对读者来说更加清晰和易于理解。

以下是一个示例指令，说服 ChatGPT 生成一个项目符号列表，其中一个项目是嵌套的项目符号列表：

```py
Generate the HTML code for a bulleted list with the following items:
- Bread
- Milk
- Fruit
 - Bananas
 - Oranges
 - Papayas
- Chocolate
```

注意，在“水果”项目下，三个项目缩进了一个空格。这种缩进足以让 ChatGPT 知道您希望这些项目以嵌套项目符号列表的形式呈现。图 9.4 显示了 ChatGPT 在网页浏览器中生成的代码。

![](img/build-a-website-with-chatgpt-CH09_F04_McFedries3.png)

图 9.4 带有嵌套项目符号列表的项目符号列表

这是此列表背后的代码：

```py
<ul>
    <li>Bread</li>
    <li>Milk</li>
    <li>Fruit
        <ul>
            <li>Bananas</li>
            <li>Oranges</li>
            <li>Papayas</li>
        </ul>
    </li>
    <li>Chocolate</li>
</ul>
```

为了帮助读者区分嵌套列表和主列表，网页浏览器做了两件事：

+   将嵌套列表项缩进得比主列表项更多

+   使用空心圆圈而不是填充圆圈作为项目符号

那个空心圆圈让您知道有不同类型的项目符号可用。下一节将向您展示如何为您的列表指定不同的项目符号类型。

### 9.2.3 更改项目符号类型

默认情况下，网页浏览器以填充圆圈（也称为*圆点*）作为项目符号来渲染项目符号列表。然而，这种默认的项目符号类型并不是固定不变的。以下是一个通用的提示，指示 ChatGPT 使用不同的项目符号类型：

```py
Generate the HTML code for a bulleted list with the items below. Use a *type* as the bullet.
- Item 1
- Item 2
- etc.
```

在您的指令中，您将*`type`*替换为以下之一：

+   使用单词`circle`以空心圆圈作为项目符号。

+   使用单词`square`以填充方框作为项目符号。

+   任何表情符号字符的名称，例如勾号、星号、心形、箭头或笑脸。

+   任何其他 Unicode 字符的名称，例如黑色右指三角形、右箭头或白色菱形。（查看[www.unicode.org/charts](https://www.unicode.org/charts)以查看可用的字符——全部 144,000 个！）

图 9.5 显示了一个使用勾号表情符号字符而不是常规项目符号的项目符号列表。

![](img/build-a-website-with-chatgpt-CH09_F05_McFedries3.png)

图 9.5 使用勾号表情符号作为项目符号的项目符号列表

项目符号列表在网络上很常见，但它们并不是唯一的列表游戏。编号列表是下一节的主题。

## 9.3 构建编号列表

我之前提到，您在列表项的顺序不是列表的必要组成部分时使用项目符号列表。然而，对于许多项目集合，顺序*是*重要的，并且您的网页可以使用编号列表显示这些项目。

例如，如果您提供一组逐步指令，则程序必须从第一步开始，然后按顺序进行到最后一步。同样，对于前十名排名，您可能希望第十名排在第一位，然后是第九名，一直排到排名第一的项目，它最后出现。

图 9.6 展示了编号列表的示例。以下是指导 ChatGPT 生成该代码的方法：

```py
Generate the HTML code for a numbered list with the following items:
-Inflatable Dartboard
-Water-Resistant Sponge
-Helium-Filled Paperweight
-Teflon Bath Mat
-Flame-Retardant Firewood
```

![图片](img/build-a-website-with-chatgpt-CH09_F06_McFedries3.png)

图 9.6 编号列表的示例

注意，你需要在列表中的每一项前加上一个破折号（`-`）。你也可以使用加号（`+`）、星号（`*`），甚至数字 1 后跟一个句点（`1.`）。下面是生成的代码：

```py
<ol>
    <li>Inflatable Dartboard</li>
    <li>Water-Resistant Sponge</li>
    <li>Helium-Filled Paperweight</li>
    <li>Teflon Bath Mat</li>
    <li>Flame-Retardant Firewood</li>
</ol>
```

这个代码有两个主要组成部分：

+   整个列表被`<ol>`和`</ol>`标签包围（其中`ol`是*ordered list*的缩写）。

+   每个列表项都被`<li>`和`</li>`标签包围（其中`li`是*list item*的缩写）。

网页浏览器总是将编号列表的第一个项目渲染为数字 1，但有两种方法可以自定义列表顺序。首先，在下一节中，你将学习如何反转列表顺序。

### 9.3.1 反转列表顺序

当你在一个教程、产品文档或食谱中使用编号列表时，你希望读者从步骤 1 开始，继续到步骤 2，并按顺序继续，直到最后一步。然而，并非每个编号列表都符合这种模式。例如，一个前 10 名的列表通常从第 10 开始，然后是第 9，以此类推，直到第 1。

为了让 ChatGPT 创建这样的列表，指导它生成一个*倒序编号列表*，如下例所示：

```py
Generate the HTML code for a reversed numbered list with the following items:
-U.C. Santa Cruz Banana Slugs
-Delta State Fighting Okra
-Kent State Golden Flashes
-Evergreen State College Geoducks
-New Mexico Tech Pygmies
-South Carolina Fighting Gamecocks
-Southern Illinois Salukis
-Whittier Poets
-Western Illinois Leathernecks
-Delaware Fightin' Blue Hens
```

图 9.7 显示了 ChatGPT 根据这个指令生成的代码在网页浏览器中的渲染效果。

![图片](img/build-a-website-with-chatgpt-CH09_F07_McFedries3.png)

图 9.7 一个倒序编号列表

你可以用来改变编号列表顺序的另一种方法是指定列表的起始编号，这是下一节的主题。

### 9.3.2 改变列表的起始编号

默认情况下，常规编号列表从数字 1 开始，倒序编号列表从列表项数相等的位置开始。然而，你可以指定任何你喜欢的起始值。你为什么要这样做呢？一个常见的例子是当你展示一个更大的列表的一部分（例如，一份合同）时，如果这部分列表从第 4 开始，那么你向读者展示的编号列表也应该从第 4 开始。

另一个常见的例子是当你开始一个编号列表，有一个文本部分，然后有一个新的编号列表，它应该作为第一个列表的延续。图 9.8 显示了在浏览器中发生的情况。

![图片](img/build-a-website-with-chatgpt-CH09_F08_McFedries3.png)

图 9.8 一个被打断的列表

这里的问题是第二个列表从步骤 1 开始，而它应该从步骤 5 继续。幸运的是，你可以在提示中包含`starting at` *X* 来告诉 ChatGPT 编号列表的起始值，其中*X*是你想要的起始值。以下是一个示例：

```py
Generate the HTML code for a numbered list starting at 5 with the following items:
-Wait for the water to boil: You'll know the water is boiling when you see bubbles rising to the surface rapidly. This could take anywhere from a few minutes to over ten minutes, depending on how much water you're boiling and how powerful your stove is.
-Turn off the stove: Once your water has reached a rolling boil (or once it's heated to your desired temperature), carefully turn off the stove.
```

图 9.9 显示了 ChatGPT 根据这个指令生成的代码现在正确地将第二个列表渲染为第一个列表的延续。

![图片](img/build-a-website-with-chatgpt-CH09_F09_McFedries3.png)

图 9.9 第二个列表现在是第一个列表的适当延续。

需要在嵌套列表中有一个项目拥有自己的编号列表吗？下一节将告诉你所有你需要知道的内容。

### 9.3.3 嵌套编号列表

有时，你需要在编号列表中包含“子步骤”。例如，在教程中，你可能希望将某个特定项目分解成多个子项目以提高清晰度或精确度。同样，法律文本中常见的编号条款和子条款也是如此。较大编号列表中的子步骤集合称为*嵌套编号列表*。

这里有一个示例提示，要求 ChatGPT 生成一个编号列表，其中两个主要步骤都有多个子步骤：

```py
Generate the HTML code for a numbered list with the following items:
-Get into the starting position:
 -Place two balls in your dominant hand, one in front of the other.
 -Hold the third ball in your other hand.
 -Let your arms dangle naturally and bring your forearms parallel to the ground (as though you were holding a tray).
-Make the first toss:
 -Of the two balls in your dominant hand, toss the front one toward your left hand in a smooth arc.
 -Make sure the ball doesn't spin too much.
 -Make sure the ball goes no higher than about eye level.
```

注意，在每种情况下，三个子项目都缩进了一个空格。这种缩进告诉 ChatGPT 你希望这些项目以嵌套编号列表的形式呈现。图 9.10 显示了 ChatGPT 在网页浏览器中生成的代码。

![图片](img/build-a-website-with-chatgpt-CH09_F10_McFedries3.png)

图 9.10 一个包含两个嵌套编号列表的编号列表

这里是这个列表背后的代码：

```py
<ol>
    <li>Get into the starting position:
        <ol style="list-style-type: lower-roman;">
            <li>Place two balls in your dominant hand, 
                one in front of the other.</li>
            <li>Hold the third ball in your other hand.</li>
            <li>Let your arms dangle naturally and bring 
                your forearms parallel to the ground (as 
                though you were holding a tray).</li>
        </ol>
    </li>
    <li>Make the first toss:
        <ol style="list-style-type: lower-roman;">
            <li>Of the two balls in your dominant hand, 
                toss the front one toward your left hand 
                in a smooth arc.</li>
            <li>Make sure the ball doesn't spin too much.</li>
            <li>Make sure the ball goes no higher than 
                about eye level.</li>
        </ol>
    </li>
</ol>
```

为了帮助读者区分嵌套列表和主列表，网络浏览器将嵌套项目比主列表项目缩进更多。然而，这种处理嵌套编号列表的默认方式有点令人困惑，因为嵌套项目使用与主编号列表相同的编号方案（1，2，3 等）。幸运的是，正如你在下一节中学习的，你可以指定不同的编号样式。

### 9.3.4 更改编号样式

默认情况下，网络浏览器使用十进制数字（1，2，3 等）来渲染编号列表。然而，你可以使用几种不同的编号样式，例如罗马数字。这里有一个通用的指令，要求 ChatGPT 使用不同的编号样式：

```py
Generate the HTML code for a numbered list with the items below. Use *style* as the numbering style.
- Item 1
- Item 2
- etc.
```

在你的指令中，你将*`style`*替换为以下之一：

+   术语“十进制前导零”用于根据需要使用前导零填充的十进制数字（01，02，03 等）

+   术语“上标罗马数字”用于使用大写罗马数字（I，II，III 等）

+   术语“下标罗马数字”用于使用小写罗马数字（i，ii，iii 等）

+   术语“上标字母”用于使用大写字母（A，B，C 等）

+   术语“下标字母”用于使用小写字母（a，b，c 等）

这里是上一节中 ChatGPT 指令的修订版，要求嵌套编号列表中使用小写罗马数字：

```py
Generate the HTML code for a numbered list with items below. Use lower roman as the numbering style for the nested numbered lists.
-Get into the starting position:
 -Place two balls in your dominant hand, one in front of the other.
 -Hold the third ball in your other hand.
 -Let your arms dangle naturally and bring your forearms parallel to the ground (as though you were holding a tray).
-Make the first toss:
 -Of the two balls in your dominant hand, toss the front one toward your left hand in a smooth arc.
 -Make sure the ball doesn't spin too much.
 -Make sure the ball goes no higher than about eye level.
```

图 9.11 显示了使用小写罗马数字的更新后的编号列表和嵌套编号列表。

![图片](img/build-a-website-with-chatgpt-CH09_F11_McFedries3.png)

图 9.11 嵌套编号列表现在使用小写罗马数字。

到目前为止，你已经知道了成功提示 ChatGPT 构建食谱页面的所有要求。下一节将带你通过这个过程。

## 9.4 构建食谱页面的提示

本章的项目是一个网页，为读者提供了一个使用多个列表的食谱：

+   两套成分的两份列表项

+   指令的编号列表（包含嵌套编号列表）

到目前为止，你应该已经有了网站标题、标语和页面标题，在这个例子中，页面标题将是食谱的名称。如果你知道你想要用于页面文本的 Google Fonts 字体类型和想要使用的颜色，这将很有帮助。查看第三章了解如何提示 ChatGPT 获取建议的标题、字体和颜色。

要开始你的提示，告诉 ChatGPT 你想要构建一个网页，并且希望它为你生成代码：

```py
I want to build a web page for a recipe. I don't know how to code, so I need you to provide the code for me.

First, write the HTML code for a web page that includes the following:
```

现在详细说明页面内容，包括以下内容（参考图 9.12）：

+   包含你的标志、网站标题和标语的页眉

+   一个以页面标题开始并跟随着一些介绍性文本的主要元素

+   详细说明食谱成分的列表项

+   一个或多个编号列表，引导读者通过食谱步骤

+   包含版权声明的页脚。

![](img/build-a-website-with-chatgpt-CH09_F12_McFedries3.png)

图 9.12 食谱页面的元素

接下来，要求 ChatGPT 生成 CSS：

```py
Second, in a separate file please write the CSS code for the following:
```

然后你指定页面格式，包括以下内容：

+   页面背景颜色和文本颜色。

+   你想要用于网站标题、标语、页面标题和页面文本的字体大小。

+   用于标题和常规页面文本的字体。

+   页面的最大宽度。这可以防止文本行过长。对于这个页面，800 像素的最大长度是合适的。

这里是我自己食谱页面的一个示例提示：

```py
I want to build a web page for a recipe. I don't know how to code, so I need you to provide the code for me.

First, write the HTML code for a web page that includes the following:
 * A header element that includes an image named super-baker.png, the title "The Super Baker", and the tagline "The ultimate guide to super-powered baking. Learn how to make delicious treats that will boost your energy, strength, and speed.".
 * A main section with the heading "Super-Energy Nut Bars".
 * A paragraph with the text "Looking for an energy boost, either first thing in the morning or during that mid-afternoon lull? Look no further than these tasty and nutritious nut bars, which turn the energy dial up to 11\. Packed full of delicious and take-you-all-the-way-to-dinner nuts and dried fruit, all combined with a give-me-energy-now hit of honey and maple syrup, these bars just might be the perfect superhero snack."
  * Add the third-level heading "Dry Ingredients" followed by a bulleted list with the following items:
    -200g rolled oats
    -100g peanuts
    -100g almonds
    -50g pumpkin seeds
    -50g sesame seeds
    -100g dates or other dried fruit
  * Add the third-level heading "Wet Ingredients" followed by a bulleted list with the following items:
    -120g honey
    -80g maple syrup
    -1 tsp vanilla extract
    -¼ tsp sea salt
  * Add the third-level heading "Preparation" followed by a numbered list with the following items:
    -Preheat the oven to 350°F. Place one rack on the bottom shelf and another rack in the middle.
    -Cover two baking sheets with parchment paper.
    -Spread out the nuts and seeds evenly on one baking sheet.
    -Spread out the rolled oats evenly on the other baking sheet.
    -Place the nuts and seeds on the bottom rack and the oats on the middle rack.
    -Bake for 8 minutes, then remove the nuts and seeds; continue baking the oats for another 7 minutes. 
    -Allow the oats, nuts, and seeds to cool. (Don't throw out the parchment paper sheets.)
    -Chop the cooled nuts.
    -Chop the dates.
    -Combine all the dry ingredients in a large bowl.
    -Prepare an 8x10 or 7x11 pan:
     -Line the pan with one of the sheets of parchment paper from the bake.
     -Coat the parchment paper with oil (such as sunflower oil).
     -Oil one side of the other sheet of parchment paper.
    -Add the wet ingredients to a small saucepan.
    -Cook the wet ingredients on the stovetop, stirring constantly, until a quick-read thermometer inserted into the liquid reads 260°F.
    -Add to cooked liquid to the dry ingredients and mix thoroughly.
    -Add the mixture to the prepared pan.
    -Place the oiled side of the second sheet of parchment paper down on the mixture and use a spoon and/or potato masher to press the mixture into place.
    -Cool the mixture in the refrigerator for 30-60 minutes.
    -Remove from the fridge and let sit for 30-60 minutes. (You want the mixture to be warm enough that it doesn't shatter when you try to cut it.)
    -Cut into 24 pieces.
  * A footer element that includes the Copyright symbol, followed by the current year, followed by "The Super Baker".
 * In the page head section, include the tag <meta charset="utf-8">.
 * In the page head section, include the tag <meta name="viewport" content="width=device-width, initial-scale=1">.

Second, in a separate file write the CSS code for the following:
 * The page has background color azure, a 24px margin, and a line height of 1.5.
 * The header has text color darkred and 12px padding.
 * Make the header image a maximum width of 250px and floated to the left.
 * The title is 48px, centered, and with no bottom margin.
 * The tagline is 26px, italic, centered, and with no top margin.
 * The main section has a top margin of 75px.
 * The main section heading font size is 30px.
 * The main section font size is 20px.
 * For the page headings, use the Merriweather Sans font from Google Fonts. For the page text, use the Merriweather font from Google Fonts.
 * For the nested numbered list, use lower roman numerals.
 * The footer has 5px padding all around, 50px top margin, and a darkred top border.
 * Give the page a maximum width of 800px and center the body element within the browser window.
```

ChatGPT 首先生成 HTML 代码，你可以复制并粘贴到名为 index.xhtml 的文件中。在这段代码中，你应该看到顶部附近类似以下的一行：

```py
<link rel="stylesheet" type="text/css" href="styles.css">
```

这段代码指示网络浏览器在名为 styles.css 的文件中查找 CSS 代码，因此你的下一个任务是复制生成的 CSS 代码，并将其粘贴并保存到名为 styles.css 的文件中（或 `<link>` 标签中显示的任何名称）。务必将 styles.css 保存到与你的 index.xhtml 文件相同的文件夹中。你还需要将你的页眉图像文件复制到同一个文件夹中。参考附录 A 了解更多关于工作网页文件的信息。

我使用 OpenAI 的 ChatGPT 应用将我的提示提交给 GPT-4。生成的代码生成了图 9.13 所示的页面。

![](img/build-a-website-with-chatgpt-CH09_F13_Mcfedries3.png)

图 9.13 我的食谱页面

如果你喜欢 ChatGPT 提供的页面，你可以跳过本章的其余部分，并将代码部署到网络上（有关部署细节，请参阅附录 B）。然而，如果你想了解生成的网页代码，请继续阅读以获得更详细的了解。

## 9.5 检查食谱页面代码

本书的一个主要前提是 ChatGPT 在编写网页代码方面足够出色，即使那些不想深入了解网页开发的人也可以通过信任 ChatGPT 来完成代码部分的工作，从而将网页发布到网络上。尽管如此，尝试理解 ChatGPT 生成的代码所做的工作并没有什么规则。为此，下一两个部分将揭开面纱，检查上一节中我提出的提示所生成的食谱页面代码（该页面如图 9.13 所示）。

注意：本食谱页面的生成 HTML 和 CSS 代码可在本书的网站上找到（[www.manning.com/books/build-a-website-with-chatgpt](https://www.manning.com/books/build-a-website-with-chatgpt)）以及本书的 GitHub 仓库：[`github.com/paulmcfe/websites-with-chatgpt`](https://github.com/paulmcfe/websites-with-chatgpt)。

下面的代码注释将帮助您理解幕后发生的事情，并调整或自定义您自己的代码。

### 9.5.1 检查 HTML

这是 ChatGPT 为我食谱页面生成的 HTML 代码：

```py
<!DOCTYPE html>
<html>
<head>
    <title>The Super Baker</title>
    <meta charset="utf-8">
    <meta name="viewport" 
        content="width=device-width, initial-scale=1">                         ①
    <link href="https://fonts.googleapis.com/css2?
        family=Merriweather&family=Merriweather+Sans&
        display=swap" rel="stylesheet">                                        ②
    <link rel="stylesheet" type="text/css" href="styles.css">                  ③
</head>
<body>
    <header>                                                                   ⑦
        <img src="super-baker.png" alt="The Super Baker Logo">                 ④⑦
        <h1>The Super Baker</h1>                                               ⑤⑦
        <p>The ultimate guide to super-powered baking. Learn how to            ⑥⑦
           make delicious treats that will boost your energy,                  ⑥⑦
           strength, and speed.</p>                                            ⑥⑦
    </header>                                                                  ⑦

    <main>
        <h2>Super-Energy Nut Bars</h2>                                         ⑧
        <p>                                                                    ⑨
            Looking for an energy boost, either first thing in the             ⑨
            morning or during that mid-afternoon lull? Look no further         ⑨
            than these tasty and nutritious nut bars, which turn the           ⑨
            energy dial up to 11\. Packed full of delicious and                 ⑨
            take-you-all-the-way-to-dinner nuts and dried fruit, all           ⑨
            combined with a give-me-energy-now hit of honey and maple          ⑨
            syrup, these bars just might be the perfect superhero snack.       ⑨
        </p>                                                                   ⑨
        <h3>Dry Ingredients</h3>
        <ul>                                                                   ⑩
            <li>200g rolled oats</li>                                          ⑩
            <li>100g peanuts</li>                                              ⑩
            <li>100g almonds</li>                                              ⑩
            <li>50g pumpkin seeds</li>                                         ⑩
            <li>50g sesame seeds</li>                                          ⑩
            <li>100g dates or other dried fruit</li>                           ⑩
        </ul>                                                                  ⑩

        <h3>Wet Ingredients</h3>
        <ul>                                                                   ⑪
            <li>120g honey</li>                                                ⑪
            <li>80g maple syrup</li>                                           ⑪
            <li>1 tsp vanilla extract</li>                                     ⑪
            <li>¼ tsp sea salt</li>                                            ⑪
        </ul>                                                                  ⑪

        <h3>Preparation</h3>                                                   ⑫
        <ol>                                                                   ⑫
            <li>Preheat the oven to 350°F. Place one rack on the bottom        ⑫
                 shelf and another rack in the middle.</li>                    ⑫
            <li>Cover two baking sheets with parchment paper.</li>             ⑫
            <li>Spread out the nuts and seeds evenly on one baking sheet.</li> ⑫
            <li>Spread out the rolled oats evenly on the other baking          ⑫
                sheet.</li>                                                    ⑫
            <li>Place the nuts and seeds on the bottom rack and the oats on    ⑫
                the middle rack.</li>                                          ⑫
            <li>Bake for 8 minutes, then remove the nuts and seeds; continue   ⑫
                baking the oats for another 7 minutes.</li>                    ⑫
            <li>Allow the oats, nuts, and seeds to cool. (Don't throw out the  ⑫
                parchment paper sheets.)</li>                                  ⑫
            <li>Chop the cooled nuts.</li>                                     ⑫
            <li>Chop the dates.</li>                                           ⑫
            <li>Combine all the dry ingredients in a large bowl.</li>          ⑫
            <li>Prepare an 8x10 or 7x11 pan:</li>                              ⑫
            <ol>                                                               ⑫⑬
                <li>Line the pan with one of the sheets of parchment paper     ⑫⑬
                    from the bake.</li>                                        ⑫⑬
                <li>Coat the parchment paper with oil (such as sunflower       ⑫⑬
                    oil).</li>                                                 ⑫⑬
                <li>Oil one side of the other sheet of parchment paper.</li>   ⑫⑬
            </ol>                                                              ⑫⑬
            <li>Add the wet ingredients to a small saucepan.</li>              ⑫
            <li>Cook the wet ingredients on the stovetop, stirring constantly, ⑫
                until a quick-read thermometer inserted into the liquid reads  ⑫
                260°F.</li>                                                    ⑫
            <li>Add to cooked liquid to the dry ingredients and mix            ⑫
                thoroughly.</li>                                               ⑫
            <li>Add the mixture to the prepared pan.</li>                      ⑫
            <li>Place the oiled side of the second sheet of parchment paper    ⑫
                down on the mixture and use a spoon and/or potato masher to    ⑫
                press the mixture into place.</li>                             ⑫
            <li>Cool the mixture in the refrigerator for 30-60 minutes.</li>   ⑫
            <li>Remove from the fridge and let sit for 30-60 minutes. (You     ⑫
                want the mixture to be warm enough that it doesn't shatter     ⑫
                when you try to cut it.)</li>                                  ⑫
            <li>Cut into 24 pieces.</li>                                       ⑫
        </ol>                                                                  ⑫
    </main>

    <footer>                                                                   ⑭
        &copy; 2023 The Super Baker                                            ⑭
    </footer>                                                                  ⑭
</body>
</html>
```

① 帮助页面在移动设备上正确显示

② 从 Google Fonts 加载 Merriweather 和 Merriweather Sans 字体

③ 告诉网络浏览器在哪里找到 CSS 代码

④ 网站标志

⑤ 网站标题

⑥ 网站标语

⑦ 页面页眉

⑧ 食谱标题

⑨ 食谱简介

⑩ 干燥成分的列表项

⑪ 湿成分的列表项

⑫ 食谱准备步骤的编号列表

⑬ 嵌套编号列表

⑭ 页面页脚

注意，HTML 代码中包含以下行：

```py
<link rel="stylesheet" href="styles.css">
```

这个标签告诉网络浏览器在哪里找到 CSS 代码，我将在下一节中描述。

### 9.5.2 检查 CSS

这是 ChatGPT 为我食谱页面生成的 CSS 代码：

```py
body {
    background-color: azure;                       ①
    margin: 24px;                                  ①
    line-height: 1.5;                              ①
    font-family: 'Merriweather', serif;            ①
    max-width: 800px;                              ②
    margin-left: auto;                             ③
    margin-right: auto;                            ③
}

header {
    color: darkred;                                ④
    padding: 10px;                                 ④
    text-align: center;                            ④
}

header img {
    max-width: 250px;                              ⑤
    float: left;                                   ⑤
}

header h1 {
    font-size: 48px;                               ⑥
    margin-bottom: 0;                              ⑥
    font-family: 'Merriweather Sans', sans-serif;  ⑥
}

header p {
    font-size: 26px;                               ⑦
    margin-top: 0;                                 ⑦
    font-style: italic;                            ⑦
}

main {
    margin-top: 75px;                              ⑧
    font-size: 20px;                               ⑧
}

main h2 {
    font-size: 30px;                               ⑨
    font-family: 'Merriweather Sans', sans-serif;  ⑨
}

ol ol {
    list-style-type: lower-roman;                  ⑩
}

footer {
    padding: 5px;                                  ⑪
    margin-top: 50px;                              ⑪
    border-top: 1px solid darkred;                 ⑪
} 
```

① 设置页面背景颜色、边距、行高和字体

② 设置最大页面宽度为 800 px

③ 居中页面

④ 设置页眉文本颜色、填充和对齐

⑤ 设置最大标志宽度，并将其浮动到左侧

⑥ 设置页面标题字体大小、底部边距和字体

⑦ 设置标语字体大小、顶部边距和斜体

⑧ 在主元素顶部添加边距，并设置字体大小

⑨ 设置食谱标题的字体大小和字体

⑩ 将嵌套编号列表样式设置为小写罗马数字

⑪ 设置页脚填充、顶部边距和顶部边框

如果您喜欢，可以使用这些注释来帮助自定义您的网页代码，正如我在下一节中描述的那样。

## 9.6 自定义食谱页面

如果您真的不喜欢 ChatGPT 为您创建的页面，请尝试修改您的提示并提交一个新的聊天会话。如果页面接近您所寻找的内容，请考虑自己调整代码。

我将从修改 HTML 的一些建议开始：

+   编辑页面文本是安全的，包括标题、标语、标题或引言文本以及任何项目符号或编号列表项。只需确保你不会意外地编辑或删除文本两侧的 HTML 标签（例如包围项目符号或编号列表项的`<li>`和`</li>`标签）。

+   随意添加一个或多个引言段落。对于每个新的段落，请遵循以下步骤：

a) 在你的文本编辑器中，将光标置于结束现有引言段落的`</p>`标签之后。

b) 按 Enter 或 Return 键开始新的一行。

c) 输入一个`<p>`标签，然后按 Enter 或 Return 键。大多数文本编辑器会自动插入一个`</p>`标签。

d) 输入你的段落文本。

e) 如果你的文本编辑器尚未这样做，输入一个`</p>`标签以完成你的段落元素。

+   如果你正在围绕食谱（或类似内容）构建网站，你将需要一个导航元素，以便访客可以轻松找到你的其他页面。查看第六章了解如何提示 ChatGPT 获取链接和导航栏。

+   在 HTML 代码的页脚部分，你可以添加指向你的社交媒体账户的链接，正如我在第四章中描述的那样。

这里有一些 CSS 代码的定制想法：

+   如果你希望嵌套编号列表使用另一种编号方案，将`ol`元素的`list-style-type`属性值更改为另一个关键字，例如`lower-alpha`。

+   为了改变背景颜色，将`body`元素的`background-color`属性的值替换为另一个颜色关键字。

+   为了改变标题文本颜色，将`header`元素的`color`属性的值替换为另一个颜色关键字。

+   如果你希望你的页面有不同的最大宽度，将`max-width`的值更改为`800px`以外的值。

+   如果你希望将标题标志放在右侧，在`header img`元素中，将`float`值更改为`right`。

+   对于任何字体大小值，你可以改变数字来增加或减少字体大小。只需确保保留`px`单位。

+   对于任何填充或边距值，你可以改变数字来增加或减少填充或边距。在每种情况下，确保保留`px`单位。

+   为了使你的页面代码更易于访问，考虑将所有 px 测量值转换为 rem 测量值。默认情况下，1 rem 相当于 16 px，因此 20 px 是 1.25 rem，24 px 是 1.5 rem，32 px 是 2 rem，48 px 是 3 rem，依此类推。rem 单位更易于访问，因为它测量的是相对于浏览器用户在其浏览器设置中定义的默认字体大小的字体大小。

## 摘要

+   项目符号列表是一组 HTML 元素，将多个项目作为垂直列表展示，其中每个项目从左边缘略微缩进，并 precede by a small black circle called a bullet。

+   当你想展示多个项目但项目顺序不是列表的必要组成部分时，使用项目符号列表。

+   有序列表是一组 HTML 元素，它们以垂直列表的形式展示多个项目，其中每个项目都稍微缩进，并且通常在左边距前有一个数字。

+   当你想展示多个项目，并且这些项目的顺序是列表的一个基本组成部分时，你使用有序列表。

+   位于另一个项目符号或有序列表内部的列表称为嵌套在该列表内。

+   为了获得最佳效果，你的页面提示应该尽可能具体，包括颜色、字体大小和标题级别。

+   将生成的 HTML 保存到 index.xhtml 文件中，将生成的 CSS 保存到 ChatGPT 在 HTML 代码中建议的文件名中，通常是 styles.css。

# 10 设置照片库

本章涵盖

+   在网页上使用图像

+   使用图像的缩略图版本

+   在相册中显示图像

+   使用 Flexbox 布局页面

+   为构建照片库页面制作 ChatGPT 提示

+   检查和自定义 ChatGPT 生成的代码

在你学习了第四章的一些图像基础知识之后，本书中的项目大多只包含一个图像：页面页眉中的网站标志。这是一个很好的开始，但你无疑知道，从你自己的在线活动来看，图像在网络上无处不在。一个放置得当且选择恰当的图片或艺术品可以真正让页面焕发活力，并为疲惫的访客提供一些受欢迎的视觉享受。

在本章中，你将了解更多关于图像在网页上如何工作的信息，这将使你能够将额外的图像添加到你的页面中。正如俗话所说——要么做大，要么回家，所以本章通过展示如何构建一个可以用来展示你的摄影技巧的工作照片库，以及如何使用现代布局技术让你的页面看起来很棒，来大张旗鼓地介绍图像。然后，你将所有这些图像和布局知识应用到实践中，为 ChatGPT 创建一个详细的提示，以生成照片库的代码。

本章还提供了 ChatGPT 生成的 HTML 和 CSS 的注释版本，以帮助你理解照片库是如何工作的。你还得到了一些有用的提示，用于自定义代码。

## 10.1 检查本章的项目

如我在引言中提到的，本章的项目是一个单页照片库。最终页面将包括以下组件：

+   包含网站标志和标题的页眉元素

+   一个以相册标题和使用说明开始的主体元素

+   九个缩小尺寸的图片版本，点击其中一张图片将显示该图片的大尺寸版本

+   包含版权声明的页脚元素

图 10.1 显示了由 ChatGPT 提供的代码创建的示例相册。你可以使用这种布局来展示其他类型的内容，包括产品目录、艺术家作品集、设计样本或当前或已完成的项目、团队成员、即将举行的活动、客户评价或客户。这些项目的共同点是它们由一系列图片（可能还有一些文本）组成，因此你需要了解更多关于图片在网页上如何工作的信息。

![](img/build-a-website-with-chatgpt-CH10_F01_McFedries3.png)

图 10.1 由 ChatGPT 生成的相册

## 10.2 深入了解图片

如果你使用过文字处理程序或演示文稿程序，你可能已经创建了许多包含图片的文档。在每种情况下，应用程序都提供类似插入图片的命令，允许你选择你想要的图片，并将其直接添加到你在文档中选择的地点。

令人惊讶的是，网页代码的工作方式并不相同。没有 HTML 等价于插入图片命令，可以直接将图片嵌入页面。相反，你需要将图片作为单独的文件上传到你的网站，然后在页面文本中插入一个特殊的 HTML 标签，告诉浏览器图片的位置。当浏览器遇到这个标签时，它会从服务器检索图片文件，并在你指定的位置在页面上显示图片。

### 10.2.1 检查 `<img>` 标签

获取浏览器将图片添加到网页的特殊标签是 `<img>` 标签，它使用图 10.2 中显示的部分语法。

![](img/build-a-website-with-chatgpt-CH10_F02_McFedries3.png)

图 10.2 使用 `<img>` 标签将图片插入网页。

这个版本的 `img` 元素有两个属性：

+   `src="`*`file`*`"`—对于 `src`（简称 *源*）属性，你将 *`file`* 替换为图片文件的位置。为了简化，我只将展示两种最常见的情况：

    +   如果图片文件与 HTML 文件位于同一目录下，将 *`file`* 替换为图片文件的名称。例如，如果你的图片文件是 logo.png，你的 `<img>` 标签将看起来像这样：

        ```py
        <img src="logo.png" alt="">
        ```

    +   如果图片在子目录中，将 *`file`* 替换为图片的目录名和文件名，用反斜杠（`/`）分隔。例如，如果你创建了一个名为 images 的子目录，并且你的图片文件是 logo.png，你的 `<img>` 标签将看起来像这样：

        ```py
        <img src="images/logo.png" alt="">
        ```

+   `alt="`*`description`*`"`—对于 `alt`（简称 *替代*）属性，你将 *`description`* 替换为一个描述图片的词或短语；如果图片文件无法显示，可以使用此文本代替图片。Alt 文本（通常如此称呼）也被屏幕阅读器和盲文应用用来向用户传达图片的大致内容。以下是一个示例：

    ```py
    <img src="images/logo.png" alt="Ampersand Photography logo">
    ```

    从技术上讲，除非每个`<img>`标签都有一个存在的`alt`属性，否则你的网页是无效的。一个无效的页面意味着你的网页可能在网络浏览器中无法正确渲染，但主要意味着你的页面对使用辅助技术（如屏幕阅读器）的人的可用性会降低。幸运的是，ChatGPT 生成的`<img>`标签通常包括`alt`属性，但描述几乎总是微不足道的且无帮助。因此，你应该始终在你的提示中包含你想要的`alt`文本。以下是一个向 ChatGPT 的示例指令：

    ```py
    Add an image named "old-road-marker.jpg", which is stored in the "images" subdirectory. For the alt attribute, use the following: "A photo with a very old road marker in the foreground that reads 'Appleby 12 Miles'".
    ```

    这里是一个 ChatGPT 根据这样的提示生成的`<img>`标签的例子：

    ```py
    <img src="images/old-road-marker.jpg" 
         alt="A photo with a very old road marker in the 
         foreground that reads 'Appleby 12 Miles'">
    ```

提示：如果你的页面使用了装饰性或其他非必需的图片，请将`alt`属性设置为空字符串（`""`）。这样，你的页面仍然有效，但不会让使用辅助技术（如屏幕阅读器）的人感到烦恼，他们可能不想听到纯装饰性图片的描述。

如果你还没有你想要使用的图片，但知道图片的最终尺寸，你可以插入一个占位符图片来占据页面上的相同空间，直到图片准备好使用。本节提供了详细信息。

### 10.2.2 添加占位符图片

你可能知道，在文本的世界里，一个*占位符*是一些临时标记某个永久单词或短语最终将出现位置的文本。例如，在前一节中，`<img>`标签的语法使用了占位符*`file`*和*`description`*分别作为`src`和`alt`属性值的占位符。

你还可以使用占位符与图片一起使用。在这种情况下，占位符图片占据与最终将添加到页面上的永久图片相同的空间，如果你想在页面中构建内容但还没有所需的图片（或图片），这非常有用。

你有几种方法可以添加占位符图片，但最简单的是使用占位符服务器，例如[`placehold.co`](https://placehold.co)。以下是一个向 ChatGPT 添加占位符图片的示例指令：

```py
Insert a placeholder image from placehold.co. The image dimensions are width 300px and height 200px.
```

这里是一个 ChatGPT 根据这个提示生成的`<img>`标签的例子：

```py
<img src="https://placehold.co/300x200" alt="Placeholder image" width="300" height="200">
```

图 10.3 显示了这种占位符在网页上的显示方式。

![](img/build-a-website-with-chatgpt-CH10_F03_McFedries3.png)

图 10.3 来自 placehold.co 的一个示例占位符图片

### 10.2.3 与图像缩略图一起工作

要真正展示你的照片，你需要以相对较大的尺寸显示它们。然而，根据文件格式（参考第四章）和其他因素，例如你使用的相机，完整尺寸的文件可以相当大——至少几兆字节。对于单个图片来说已经足够糟糕了，但你的照片画廊将包含多张图片（本项目中有九张）；要求画廊访客下载如此大量的数据确实太过分了。（这对于通过慢速互联网连接或有限的数据计划来到你页面的人来说尤其如此。）

对于像照片库这样的项目，对所有用户来说，最初显示每个照片的缩小版本（在业界称为“缩略图”）是一个更好的策略。目的是设置您的页面，以便点击缩略图将临时显示照片的大尺寸版本。（用户看到的尺寸取决于浏览器窗口的尺寸。）

注意：关于缩略图的大小没有硬性规定。一个可以容纳数十张图片的页面可能只使用宽度为 50 或 75 像素的缩略图，而对于像本章中 ChatGPT 帮助您构建的相册这样的照片库，宽度约为 300 像素的缩略图效果较好。

在继续之前，您应该创建您照片的缩略图版本。首先，是 Windows 的说明。

使用 Windows 照片应用创建缩略图

如果您使用的是 Windows 11，您可以复制原始照片文件，然后使用照片应用将副本调整到您首选的缩略图尺寸。在本项目中，我假设您的缩略图版本包含文件名中的文本“-thumbnail”。例如，如果完整尺寸版本命名为 image01.jpg，则其缩略图版本应命名为 image01-thumbnail.jpg。

按照以下步骤使用照片应用创建照片的缩略图版本：

1. 使用文件资源管理器找到您要处理的照片。

2. 点击文件，点击工具栏中的“复制”，然后点击“粘贴”以创建照片的副本。

3. 点击复制的文件，点击“重命名”（或按 F2 键），然后编辑文件名以删除 Windows 添加的“-Copy”文本，并将其替换为`-thumbnail`。（因此，您最终应该得到一个类似 image01-thumbnail.jpg 的文件名。）

4. 双击复制并重命名的图像文件，将图像加载到照片应用中。

5. 点击工具栏中的“查看更多”（三个点），然后点击“调整大小图像”以打开图 10.4 所示的“调整大小”对话框。

![](img/build-a-website-with-chatgpt-CH10_F04_McFedries3.png)

图 10.4 使用“调整大小”对话框创建照片的缩略图版本。

6. 确保已选择“像素”选项。

7. 使用“宽度”文本框设置缩略图的宽度（像素）。（请注意，高度值会自动更改以保持宽高比——即图像宽度与其高度的比例——这是您想要的。或者，您也可以设置高度值，宽度将自动更改。）

8. 点击保存。

如果您使用的是 Mac 而不是 Windows PC，您的步骤版本如下。

使用 macOS 预览应用创建缩略图

如果您正在运行 macOS，您可以使用 Finder 复制原始照片文件，然后使用预览应用将副本调整到您首选的缩略图宽度和高度。本项目假设缩略图副本的文件名中包含文本“-thumbnail”。例如，如果完整尺寸的照片文件名为 image01.jpg，则缩略图版本应命名为 image01-thumbnail.jpg。

按照以下步骤在 macOS 中创建照片的缩略图版本：

1. 使用 Finder 定位并点击你想要处理的照片。

2. 选择“编辑”>“复制”，然后选择“编辑”>“粘贴”以创建照片的副本。

3. 点击复制的文件，按 Enter 键，然后编辑文件名以移除 Finder 添加的*copy*文本，并替换为`-thumbnail`。（因此，你应该得到一个类似 image01-thumbnail.jpg 的文件名。）

4. 双击复制并重命名的图像文件，将图像加载到预览中。

5. 选择“工具”>“调整大小”以打开图 10.5 所示的对话框。

![](img/build-a-website-with-chatgpt-CH10_F05_McFedries3.png)

图 10.5 使用此对话框创建照片的缩略图版本。

6. 确保在“宽度”和“高度”文本框右侧的列表中选中了“像素”项。

7. 使用“宽度”文本框设置缩略图的宽度（以像素为单位）。（注意，高度值会自动改变以保持宽高比——即图像宽度与高度的比率，这是你想要的。或者，你也可以设置高度值，宽度会自动改变。）

8. 点击“确定”。

接下来，你将学习如何通过一些说明性文字来增强缩略图版本。

### 10.2.4 添加图像说明

你可能更喜欢你的相册只显示每张图像的缩略图版本。然而，如果你为每张图像提供简短的说明，可以让你访客的体验更加友好。说明不必过于复杂：只需一个简短的标题或照片描述即可。

你可以通过多种方式添加说明文字，但最直接的方式是让 ChatGPT 将你的图像转换为**图**，然后提供**图说明**。以下是 ChatGPT 生成的通用 HTML 代码：

```py
<figure>
    <img src="*file*" alt="*description*">
    <figcaption>*Caption text*</figcaption>
</figure>
```

在这里，*`Caption text`* 是说明文字，它出现在图像下方。以下是对 ChatGPT 的示例指令：

```py
Add an image named "old-road-marker.jpg", which is stored in the "images" subdirectory. Make it a figure with a caption. For the alt attribute, use the following: "A photo with a very old road marker in the foreground that reads 'Appleby 12 Miles'". For the caption, use the following: "An old road marker".
```

以下是一个示例图和说明，由 ChatGPT 从这样的提示生成：

```py
<figure>
    <img src="images/old-road-marker.jpg" 
         alt="A photo with a very old road marker in the 
              foreground that reads 'Appleby 12 Miles'">
    <figcaption>An old road marker</figcaption>
</figure>
```

图 10.6 显示了它在浏览器中的样子。

![](img/build-a-website-with-chatgpt-CH10_F06_McFedries3.png)

图 10.6 带有说明的图

在创建好缩略图版本并编写好说明文字后，你就可以查看访客如何看到每张照片的大尺寸版本了。

## 10.3 实现灯箱覆盖

稍后你将了解到（参考第 10.5 节），当有人访问相册时，页面最初显示九个缩略图图像的网格。用户如何看到照片的大尺寸版本？

解决这个问题有很多方法。例如，你可以将每个缩略图图像设置为链接，点击链接后加载照片的大尺寸版本。这种方法是可行的，但点击链接会将用户从相册中移出，所以他们需要导航回来查看更多照片。相信我，没有人那么想看你的照片！

一个更好的解决方案是让 ChatGPT 创建一个**灯箱**，这是一个具有以下特性的特殊元素：

+   它是即时创建的。

+   它占据了浏览器窗口的整个宽度和高度。

+   它略微透明。

+   它显示在现有网页之上，这就是为什么它被称为“覆盖层”。

例如，图 10.7 显示了一个包含三个缩略图的简单相册版本。当用户点击缩略图时，以下事情会发生：

1.  创建了灯箱元素。

1.  新的灯箱元素被赋予了一个`img`元素。

1.  那个`img`元素被填充了照片的大尺寸版本。

1.  通过在页面上覆盖它来显示灯箱。

![](img/build-a-website-with-chatgpt-CH10_F07_McFedries3.png)

图 10.7 一个包含三个缩略图的简单相册

结果是，用户现在看到的是照片的大尺寸版本，它填充了整个或大部分浏览器窗口。例如，如果我点击图 10.7 中最右侧的缩略图，浏览器将显示照片的较大版本，如图 10.8 所示。注意，相册在灯箱左右的空间中显得微弱。这使用户知道他们还没有离开相册。要返回相册，用户只需在页面的任何地方点击一下，这将移除灯箱并重新显示相册。

![](img/build-a-website-with-chatgpt-CH10_F08_McFedries3.png)

图 10.8 点击缩略图显示灯箱，其中包含照片的较大版本。

如果所有这些都看起来像是编码起来会非常复杂，请记住，你不必做任何事，只需准备你的缩略图图像。你可以要求 ChatGPT 使用类似以下指令来实现所有灯箱功能：

```py
Please provide the HTML, CSS, and JavaScript code to implement a lightbox-style overlay for the images on this page. The thumbnails have names such as image01-thumbnail.png, image02-thumbnail.png, image03-thumbnail.png, and so on. Each full-size image uses the same name as its thumbnail but without "-thumbnail", as in image01.png, image02.png, image03.png, and so on. All the image files are stored in the "images" subdirectory.
```

留意细节的读者会注意到这个提示中要求提供“JavaScript 代码”。这是怎么回事？下一节将解开这个谜团。

## 10.4 灯箱：由 JavaScript 驱动

到这本书的这一部分，你已经看到，仅使用 HTML 和 CSS 就可以走得很远。这些是强大的技术，当通过 ChatGPT 的详细提示成功生成时，可以产生吸引人且实用的网页。

然而，HTML 和 CSS 虽然强大，但仍然有很多事情做不到。灯箱就是一个很好的例子。是的，你可以使用 HTML 和 CSS 来创建和样式化灯箱，但一旦点击缩略图，HTML 和 CSS 就会失败：

+   他们无法创建新元素。

+   他们无法将点击的缩略图的全尺寸版本加载到灯箱`img`元素中。

+   他们无法显示隐藏的灯箱。

+   用户点击时无法移除灯箱。

幸运的是，还有一种主要的网页技术可以处理这些类型的任务以及更多：JavaScript。这是一种内置在网页浏览器中的编程语言，旨在为其他方面静止的网页元素添加交互性和动态性。在这个项目中，JavaScript 基本上做两件事：

+   它为每个图像添加了一个“点击”事件处理程序。*事件处理程序*是当指定事件发生时自动运行的 JavaScript 代码。在这种情况下，事件是用户在照片画廊中点击图像。

+   在事件处理程序中，JavaScript 构建并显示相框。

幸运的是，这就是你需要知道的所有关于它的内容。ChatGPT 将处理其余部分。

## 10.5 使用 Flexbox 布局画廊

当你在网页上添加项目时，大多数元素的默认布局行为是垂直排列在页面中，一个元素接一个。这在本书中你看到的迄今为止的项目中效果很好，但这对照片画廊来说不起作用。为什么？因为你的图像被渲染为图，它们也会垂直排列在页面中，一个接一个。

当然，这并不是世界末日，但这看起来并不好，而且对访问你页面的人来说也不方便。图 10.9 展示了照片画廊的一种版本，其中照片以这种方式显示。

你可以通过要求 ChatGPT 使用一种称为*Flexbox*的网页技术来布局照片画廊来防止这种默认行为。这是一个复杂的技术，但你现在需要知道的是，当你将网页元素转换为 Flexbox 容器时，项目会失去其刚性的默认布局行为，并适应浏览器当前的大小。对于这个项目，你可以通过简单的指令提示 ChatGPT 使用 Flexbox：

```py
Make the gallery a Flexbox container. Center the content and enable it to wrap.
```

要查看此指令的结果，请查看稍后出现的最终照片画廊布局，如图 10.10 所示。

到目前为止，你已经知道了成功提示 ChatGPT 构建照片画廊所需的所有内容。下一节将带你通过这个过程。

![图片](img/build-a-website-with-chatgpt-CH10_F09_McFedries3.png)

图 10.9 默认情况下，你的照片图将垂直排列在页面中，一个接一个。

## 10.6 为照片画廊制作提示

本章的项目是一个照片画廊页面，它显示九个照片缩略图，每个缩略图在被点击时都会显示照片的大尺寸版本。我假设你已经有了网站标志和标题，知道你想要用于页面标题和文本的字体，并且已经准备好了要应用的颜色方案。返回第三章学习如何提示 ChatGPT 提供标题、字体和颜色建议。

要开始你的提示，告诉 ChatGPT 你想要构建一个网页，并且你想要它为你生成代码：

```py
I want to build a web page for a photo gallery. I don't know how to code, so I need you to provide the code for me.

First, write the HTML code for a web page that includes the following:
```

现在逐项概述页面内容，包括以下内容（参见图 10.10）：

+   包含你的标志和网站标题的页眉

+   一个以页面标题开始的主体元素，后面跟着一些指令

+   照片缩略图画廊

+   包含版权声明的页脚

![图片](img/build-a-website-with-chatgpt-CH10_F10_McFedries3.png)

图 10.10 照片画廊页面的元素

接下来，请 ChatGPT 生成 CSS：

```py
Second, in a separate file please write the CSS code for the following:
```

然后你指定页面格式，包括以下内容：

+   页面背景颜色和文本颜色

+   你想要用于标题和页面文本的字体大小。

+   用于标题和常规页面文本的字体。

+   哪些元素应该是 Flexbox 容器（在本项目中，这些将是页眉、相册和灯箱覆盖层）。

最后，你指示 ChatGPT 提供用于显示大尺寸照片的灯箱样式覆盖层的 HTML、CSS 和 JavaScript 代码。

这里是我为我的照片画廊的示例提示：

```py
I want to build a web page for a photo gallery. I don't know how to code, so I need you to provide the code for me.

First, write the HTML code for a web page that includes the following:
 * A header element that includes an image named logo.png, which is stored in the "images" subdirectory, and the title "Ampersand Photography".
 * A main section with the heading "Photo Gallery".
 * A paragraph with the text "Click each thumbnail to see the full version of the image. To return to the gallery, click anywhere on the page."
 * A gallery element that contains the following images, each of which is stored in the "images" subdirectory, and with each image rendered as a figure with the specified alt text and caption:
  * An image named "image01-thumbnail.jpg" with the alt text "Macro photograph of a cactus" and the caption "Cactus close-up".
  * An image named "image02-thumbnail.jpg" with the alt text "A blurry reflection of a passing streetcar and a person walking" and the caption "Street(car) scene".
  * An image named "image03-thumbnail.jpg" with the alt text "A photo with a very old road marker in the foreground that reads 'Appleby 12 Miles'" and the caption "An old road marker".
  * An image named "image04-thumbnail.jpg" with the alt text "A photo taken from the top of a Lake District fell looking down on a town and a lake" and the caption "Lake District scene".
  * An image named "image05-thumbnail.jpg" with the alt text "A Montreal tower shot from below through a hole" and the caption "Montreal architecture".
  * An image named "image06-thumbnail.jpg" with the alt text "The ornate ceiling of a church in Florence, Italy" and the caption "Church ceiling in Florence".
  * An image named "image07-thumbnail.jpg" with the alt text "A cheerful, bright, sky-blue umbrella sitting improbably on a dingy, dirty balcony." and the caption "A dash of color".
  * An image named "image08-thumbnail.jpg" with the alt text "A large, ornate, Zeus-like head over the words 'Brazen Head'" and the caption "Coffee shop sign".
  * An image named "image09-thumbnail.jpg" with the alt text "A metal bird sculpture with its head peeking out of a snow bank" and the caption "Peek-a-boo bird".
 * A footer element that includes the Copyright symbol, followed by "Ampersand Photography".
 * In the page head section, include the tag <meta charset="utf-8">.
 * In the page head section, include the tag <meta name="viewport" content="width=device-width, initial-scale=1">.

Second, in a separate file write the CSS code for the following:
 * The page has background color black and no margin.
 * The page text uses font size 20px, the color gold, and the Libre Baskerville font from Google Fonts.
 * The header has background color maroon and 24px padding.
 * Make the header a Flexbox container with centered content.
 * The title is 64px, centered, uses the generic "cursive" font, and has 16px padding on the left.
 * The main section has centered text and a 24px margin.
 * The main section heading has font size 30px and uses the Montserrat font from Google Fonts.
 * Make the gallery a Flexbox container. Center the content and enable it to wrap.
 * The footer has background color maroon, 24px padding, and centered text.

Third, provide the HTML, CSS, and JavaScript code to implement a lightbox-style overlay for the images in the gallery. Each full-size image uses the same name as its thumbnail, but without "-thumbnail". For example, for the image01-thumbnail.jpg thumbnail file, the full-size image filename is image01.jpg.
```

在我使用此提示进行的每次测试中，ChatGPT 都分四个阶段生成了此代码：

1.  ChatGPT 生成了一些——但关键的是，并非全部——HTML 代码。在生成`figure`元素时，ChatGPT 仅生成了第一个图标的代码，随后是一个类似于以下注释的代码：

    ```py
    <!-- repeat for each image -->
    ```

    我不这么认为！后来，我使用了以下提示来要求 ChatGPT 提供完整的 HTML 代码：

    ```py
    Please provide the complete HTML code, including all the images specified in the original prompt.
    ```

    完成这些后，我将完整的 HTML 代码保存为 index.xhtml。在该文件中，你应该看到两个对外部文件的引用：

    +   首个引用位于`head`部分，是为 CSS 文件设置的；引用是一个`<link>`标签，其外观可能如下所示：

        ```py
        <link rel="stylesheet" type="text/css" href="styles.css">
        ```

    +   第二个引用位于 HTML 代码的底部附近，是为 JavaScript 文件设置的；引用是一个`<script>`标签，其外观可能如下所示：

        ```py
        <script src="script.js"></script>
        ```

1.  ChatGPT 生成了 CSS 代码，你需要将其保存到与`<link>`标签中出现的相同文件名（通常是 styles.css）。

1.  ChatGPT 生成了 JavaScript 代码，你需要将其保存到与`<script>`标签中出现的相同文件名（通常是 script.js）。

1.  ChatGPT 为灯箱覆盖层生成了更多的 CSS 代码。你需要复制该代码并将其粘贴到 CSS 文件的底部。

我使用 OpenAI 的 ChatGPT 应用将我的提示提交给 GPT-4。生成的代码产生了图 10.11 所示的页面。点击缩略图将生成图像的较大版本，如图 10.12 所示。

![](img/build-a-website-with-chatgpt-CH10_F11_McFedries3.png)

图 10.11 我的照片画廊

![](img/build-a-website-with-chatgpt-CH10_F12_McFedries3.png)

图 10.12 点击缩略图将显示照片的较大版本。

如果你对自己的页面满意，可以自由地跳过本章的其余部分并将代码部署到网络上（参考附录 B 了解如何部署你的页面）。然而，如果你想了解生成的网页代码，请继续阅读以获得更详细的了解。

## 10.7 检查照片画廊代码

如果你想要至少对 ChatGPT 为你生成的代码有一个大致的了解，接下来的三个部分为你提供了对之前图 10.11 中显示的照片画廊页面背后的 HTML 和 CSS 代码的简要查看，以及启用图 10.12 中演示的灯箱覆盖层的 JavaScript 代码。

注意：本书网站上（[www.manning.com/books/build-a-website-with-chatgpt](https://www.manning.com/books/build-a-website-with-chatgpt)）和 GitHub 存储库（[`github.com/paulmcfe/websites-with-chatgpt`](https://github.com/paulmcfe/websites-with-chatgpt)）中提供了我的照片画廊生成的 HTML 和 CSS 代码。

下面的代码注释应该有助于您理解照片画廊的工作原理，并使修改或自定义您自己的代码变得更加容易。

### 10.7.1 检查 HTML

这里是 ChatGPT 为我照片画廊生成的 HTML 代码的注释版本：

```py
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <meta name="viewport" 
        content="width=device-width, initial-scale=1">                     ①
    <link href="https://fonts.googleapis.com/css?                          ②
        family=Montserrat|                                                 ②
        Libre+Baskerville&display=swap"                                    ②
        rel="stylesheet">                                                  ②
    <link rel="stylesheet" href="styles.css">                              ③
    <title>Ampersand Photography</title>
</head>
<body>
    <header>                                                               ⑥
        <img src="images/logo.png"                                         ⑥
             alt="Ampersand Photography Logo">                             ④⑥
        <h1>Ampersand Photography</h1>                                     ⑤⑥
    </header>                                                              ⑥
    <main>
        <h2>Photo Gallery</h2>                                             ⑦
        <p>                                                                ⑧
            Click each thumbnail to see the full version of the image.     ⑧
            To return to the gallery, click anywhere on the page.          ⑧
        </p>                                                               ⑧
        <div class="gallery">                                              ⑫
            <figure>                                                       ⑪⑫
                <img src="images/image01-thumbnail.jpg"                    ⑨⑪⑫
                     alt="Macro photograph of a cactus"                    ⑨⑪⑫
                     class="thumbnail">                                    ⑨⑪⑫
                <figcaption>Cactus close-up</figcaption>                   ⑩⑪⑫
            </figure>                                                      ⑪⑫
            <figure>                                                       ⑫
                <img src="images/image02-thumbnail.jpg"                    ⑫
                     alt="A blurry reflection of a passing streetcar       ⑫
                         and a person walking"                             ⑫
                     class="thumbnail">                                    ⑫
                <figcaption>Street(car) scene</figcaption>                 ⑫
            </figure>                                                      ⑫
            <figure>                                                       ⑫
                <img src="images/image03-thumbnail.jpg"                    ⑫
                     alt="A photo with a very old road marker in the       ⑫
                         foreground that reads 'Appleby 12 Miles'"         ⑫
                     class="thumbnail">                                    ⑫
                <figcaption>An old road marker</figcaption>                ⑫
            </figure>                                                      ⑫
            <figure>                                                       ⑫
                <img src="images/image04-thumbnail.jpg"                    ⑫
                     alt="A photo taken from the top of a Lake District    ⑫
                         fell looking down on a town and a lake"           ⑫
                     class="thumbnail">                                    ⑫
                <figcaption>Lake District scene</figcaption>               ⑫
            </figure>                                                      ⑫
            <figure>                                                       ⑫
                <img src="images/image05-thumbnail.jpg"                    ⑫
                     alt="A Montreal tower shot from below through a hole" ⑫
                     class="thumbnail">                                    ⑫
                <figcaption>Montreal architecture</figcaption>             ⑫
            </figure>                                                      ⑫
            <figure>                                                       ⑫
                <img src="images/image06-thumbnail.jpg"                    ⑫
                     alt="The ornate ceiling of a church in Florence,      ⑫
                         Italy"                                            ⑫
                     class="thumbnail">                                    ⑫
                <figcaption>Church ceiling in Florence</figcaption>        ⑫
            </figure>                                                      ⑫
            <figure>                                                       ⑫
                <img src="images/image07-thumbnail.jpg"                    ⑫
                     alt="A cheerful, bright, sky-blue umbrella sitting    ⑫
                         improbably on a dingy, dirty balcony."            ⑫
                     class="thumbnail">                                    ⑫
                <figcaption>A dash of color</figcaption>                   ⑫
            </figure>                                                      ⑫
            <figure>                                                       ⑫
                <img src="images/image08-thumbnail.jpg"                    ⑫
                     alt="A large, ornate, Zeus-like head over the words   ⑫
                         'Brazen Head'"                                    ⑫
                     class="thumbnail">                                    ⑫
                <figcaption>Coffee shop sign</figcaption>                  ⑫
            </figure>                                                      ⑫
            <figure>                                                       ⑫
                <img src="images/image09-thumbnail.jpg"                    ⑫
                     alt="A metal bird sculpture with its head peeking     ⑫
                         out of a snow bank"                               ⑫
                     class="thumbnail">                                    ⑫
                <figcaption>Peek-a-boo bird</figcaption>                   ⑫
            </figure>                                                      ⑫
        </div>                                                             ⑫
    </main>
    <footer>                                                               ⑬
        &copy; Ampersand Photography                                       ⑬
    </footer>                                                              ⑬

    <script src="script.js"></script>                                      ⑭
</body>
</html>
```

① 帮助页面在移动设备上正确显示

② 从 Google Fonts 加载 Montserrat 和 Libre Baskerville 字体

③ 告诉网络浏览器 CSS 代码的位置

④ 网站标志

⑤ 网站标题

⑥ 页面页眉

⑦ 页面标题

⑧ 指示段落

⑨ 图像标题

⑩ 图像标题

⑪ 照片画廊图像

⑫ 照片画廊

⑬ 页面页脚

⑭ 告诉网络浏览器 JavaScript 代码的位置

注意 HTML 代码中包含以下行：

```py
<link rel="stylesheet" href="styles.css">
```

这个标签告诉网络浏览器 CSS 代码的位置，我将在下一节中描述。

### 10.7.2 检查 CSS

这里是 ChatGPT 为我照片画廊生成的 CSS 代码的注释版本：

```py
body {                                        ①
    background-color: black;                  ①
    margin: 0;                                ①
    font-size: 20px;                          ①
    color: gold;                              ①
    font-family: 'Libre Baskerville', serif;  ①
}                                             ①

header {
    background-color: maroon;                 ②
    padding: 24px;                            ②
    display: flex;                            ③
    justify-content: center;                  ③
    align-items: center;                      ③
}

h1 {
    font-size: 64px;                          ④
    font-family: cursive;                     ④
    padding-left: 16px;                       ④
}

h2 {
    font-size: 30px;                          ⑤
    font-family: 'Montserrat', sans-serif;    ⑤
}

main {
    margin: 24px;                             ⑥
    text-align: center;                       ⑥
}

.gallery {
    display: flex;                            ⑦
    flex-wrap: wrap;                          ⑦
    justify-content: center;                  ⑦
    align-items: center;                      ⑦
}

footer {
    background-color: maroon;                 ⑧
    padding: 24px;                            ⑧
    text-align: center;                       ⑧
}
.overlay {                                    ⑬
    position: fixed;                          ⑨⑬
    top: 0;                                   ⑨⑬
    left: 0;                                  ⑨⑬
    width: 100%;                              ⑩⑬
    height: 100%;                             ⑩⑬
    background-color: rgba(0, 0, 0, 0.8);     ⑪⑬
    display: flex;                            ⑫⑬
    justify-content: center;                  ⑫⑬
    align-items: center;                      ⑫⑬
}                                             ⑬

.overlay img {
    max-width: 90%;                           ⑭
    max-height: 90%;                          ⑭
}
```

① 设置页面背景颜色、边距、文本大小、文本颜色和字体

② 设置页眉背景颜色和填充

③ 将页眉设置为具有居中文本的 Flexbox 容器

④ 设置页面标题的字体大小、字体和左填充

⑤ 设置页面标题的字体大小和字体

⑥ 使用边距样式主元素，并居中文本

⑦ 将相册设置为具有居中文本和换行的 Flexbox 容器

⑧ 设置页脚背景颜色和填充，并居中文本

⑨ 定位于窗口的左上角

⑩ 占据全宽度和高度

⑪ 略微透明

⑫ 带有居中文本的 Flexbox 容器

⑬ 设置相册覆盖层的样式

⑭ 设置较大图像使用 90%的相册宽度和高度

在本章前面部分的 HTML 代码列表中，注意以下接近底部的一行：

```py
<script src="script.js"></script>
```

这个标签告诉网络浏览器 JavaScript 代码的位置，我将在下一节中注释。

### 10.7.3 检查 JavaScript

如果您小心操作，可以对 HTML 和 CSS 代码进行一些小的调整。然而，我强烈建议您不要修改 ChatGPT 的 JavaScript 代码。代码很复杂，不恰当的编辑可能会使相册无法使用。

然而，如果您知道一点 JavaScript，您可能会对 ChatGPT 解决相册问题感兴趣，所以这里有一个 ChatGPT 为我照片画廊生成的 JavaScript 代码的注释版本：

```py
document.addEventListener('DOMContentLoaded', 
    function () {                                              ①

    const thumbnails = document.querySelectorAll(
        '.thumbnail');                                         ②

    thumbnails.forEach((thumbnail) => {                        ③

        thumbnail.addEventListener('click', 
            function (e) {                                     ④

            const imageName = e.target.src.split('/')
                .pop().replace('-thumbnail', '');              ⑤

            const overlay = document.createElement('div');     ⑥

            overlay.classList.add('overlay');                  ⑦

            const img = document.createElement('img');         ⑧

            img.src = `images/${imageName}`;                   ⑨

            overlay.appendChild(img);                          ⑩

            document.body.appendChild(overlay);                ⑪

            overlay.addEventListener('click', function () {    ⑫
                document.body.removeChild(overlay);            ⑫
            });                                                ⑫
        });
    });
});
```

① 页面加载后运行后续的函数代码

② 存储所有缩略图

③ 遍历缩略图

④ 为当前缩略图添加“点击”事件处理器

⑤ 提取全尺寸图像的文件名

⑥ 创建用于相册覆盖层的新元素

⑦ 将覆盖类添加到新元素

⑧ 创建一个新的`img`元素

⑨ 将全尺寸图片文件名设置为新图片的源

⑩ 将图片添加到灯箱覆盖层

⑪ 将灯箱覆盖层添加到页面

⑫ 为灯箱添加一个“点击”事件处理器，从页面上移除灯箱

如果你愿意，可以使用前两节中的 HTML 和 CSS 注释来帮助定制你的网页代码，正如我在下一节中描述的那样。

## 10.8 定制照片库

以前几节的注释为指导，我将带你通过一些相对简单的代码定制，你可以在文本编辑器中打开 HTML 和 CSS 文件来实现。然而，如果你的页面离你想要的效果还差很远，你最好重写你的提示并将其提交给 ChatGPT 的新会话。

对于 HTML 代码，这里有一些建议的定制：

+   你可以编辑页面上的一些文本，包括标题、标题和说明文本。只需确保你只编辑文本，而不是围绕文本的 HTML 标签（如每个图例周围的`<figcaption>`和`</figcaption>`标签）。

+   随意更改任何图像的替代文本，只需编辑该`img`标签的`alt`属性值。确保你不会意外删除围绕`alt`值的双引号。

+   如果你想包含一个第二段简介，请将编辑光标放置在结束现有简介的`</p>`标签之后。按 Enter 或 Return 键开始新行，输入一个`<p>`标签，输入你的段落文本，并以`</p>`标签结束。

+   你可能想通过创建多个照片库（或其他内容），每个页面专注于特定的主题或类别来构建你的网站。请 ChatGPT 一次创建一个页面，根据需要修改你的提示。如果你选择这条路，你将需要一个导航元素，使用户能够访问每个页面。参考第六章了解如何提示 ChatGPT 获取链接和导航栏。

+   在 HTML 代码的页脚部分，你可以添加指向你的社交媒体账户的链接，正如我在第四章中描述的那样。

现在，这里有一些 CSS 代码的定制想法：

+   要使用其他页面背景颜色，为`body`元素的`background-color`属性指定不同的颜色关键字。

+   要为页眉和页脚使用其他背景颜色，为`header`和`footer`元素的`background-color`属性指定一个新的颜色关键字。

+   要使用不同的颜色显示页面文本，为`body`元素的`color`属性指定不同的颜色关键字。

+   要调整灯箱覆盖层的透明度，编辑`.overlay`类的`background-color`属性。具体来说，修改`rgba()`函数中的最后一个值，其中`1.0`是完全不透明，`0.0`是完全透明。

+   对于任何字体大小值，你可以通过改变数字来增加或减少字体大小。只需确保保留`px`单位。

+   对于任何填充或边距值，你可以更改数字以增加或减少填充或边距。在每种情况下，务必保留 `px` 单位。

+   为了使你的页面代码更易于访问，考虑将所有 px 测量值转换为 rem 测量值。默认情况下，1 rem 等于 16 px，因此 20 px 等于 1.25 rem，24 px 等于 1.5 rem，32 px 等于 2 rem，48 px 等于 3 rem，依此类推。rem 单位更易于访问，因为它测量的是相对于浏览器用户在其浏览器设置中定义的默认字体大小的字体大小。

## 摘要

+   在 HTML 中，你使用 `img` 元素告诉网络浏览器将外部图像文件插入到页面中。

+   在 `<img>` 标签中，使用 `src` 属性告诉浏览器在哪里找到图像文件；使用 `alt` 属性添加一个简短的短语来描述图像，尤其是对于使用屏幕阅读器和盲文应用的人。

+   当处理图像缩略图时，最好创建一个具有你想要使用的较小尺寸的单独缩略图文件。

+   要包含标题，将 `img` 元素包裹在 `figure` 元素中，并将标题添加到 `figcaption` 元素中。

+   轻量级覆盖层是一种动态创建的网页元素，用于显示点击的缩略图的大尺寸版本。

+   当你不想在页面上垂直排列页面元素时，将元素转换为 Flexbox 容器。

+   为了获得最佳效果，你的页面提示应尽可能具体，包括颜色、字体大小和标题级别。

+   将生成的 HTML 保存到 index.xhtml 文件，并将生成的 CSS 保存到 ChatGPT 在 HTML 代码中建议的文件名，通常是 styles.css。

# 11 创建作品集页面

本章涵盖

+   构建用户界面卡片

+   添加阴影效果

+   圆角卡片

+   使页面响应式

+   为构建作品集页面创建 ChatGPT 提示

+   检查和自定义 ChatGPT 生成的代码

在网上建立家园的最好理由之一是展示你的个人作品或团队、部门或公司的作品。本书中的许多项目都是为了实现这一目标：个人主页（第三章）、在线日志（第五章）、兴趣或爱好网站（第七章）和照片画廊（第十章）。

在本章中，你将学习另一种用于推广个人、团体或组织活动的页面结构：作品集页面。这个页面使用图像、标题和文本来创建一个高效且流行的页面组件，旨在展示你希望其他人看到的内容。你还将学习各种自定义此组件的方法和一些可以使你的作品集看起来最佳的技术，不仅在大型显示器上，也在较小的屏幕上——甚至智能手机上。然后，你将运用所有这些新的 HTML 和 CSS 知识来创建一个详细的提示，使 ChatGPT 能够生成你的作品集页面的网页代码。

本章提供了 ChatGPT 生成的 HTML 和 CSS 的注释版本，以帮助您理解投资组合页面是如何工作的。您还可以获得一些自定义代码的实用技巧。

## 11.1 了解本章的项目

本章的项目是一个投资组合页面。最终页面将包括以下组件：

+   包含标志和标题的**页眉元素**

+   以投资组合标题开始的**主要元素**

+   六张卡片，每张卡片展示投资组合中的一个项目

+   包含版权声明的**页脚元素**

图 11.1 展示了使用 ChatGPT 提供的代码创建的投资组合页面示例。

![](img/build-a-website-with-chatgpt-CH11_F01_McFedries3.png)

图 11.1 ChatGPT 生成的投资组合页面

示例页面是一个书籍设计师的投资组合，但您可以使用这种布局来展示许多其他类型的内容：

+   **艺术**——绘画、照片、插图、时尚、建筑、室内设计、写作

+   **工作**——项目、产品、事件、新闻、关键指标、教育课程

+   **人物**——团队成员、客户、用户资料、推荐信

简而言之，这是一个非常灵活的布局，您将在下一节开始学习如何构建它。

## 11.2 构建投资组合页面

如果您从事创意工作——插画、写作、音乐、美术——您应该为自己和您的职业生涯而自豪，向世界展示您的才华。您该如何做到这一点？如今，社交媒体是吹嘘自己的标准方式。这很好，但当你使用他人的平台来吹嘘自己时，你正在放弃对自己展示方式的许多控制权。始终控制自己的信息会更好，而做到这一点最好的方式是建立自己的在线存在。对于创意人士来说，这种在线存在应该包括一个展示您最好或最新作品的**投资组合页面**。

**投资组合页面**是一个网页，旨在展示您的一些（甚至全部）创意作品。它是那些多年来从赞助人到赞助人、从雇主到雇主拖着硬拷贝投资组合的饥饿艺术家的在线等价物。投资组合页面的主要目的是向可能想要购买或雇佣您进行创意工作的人展示您的创意作品。

然而，即使您不是艺术家，投资组合页面也是一个展示许多不同类型项目的绝佳布局，例如产品、课程和员工。投资组合页面的主要组件是卡片，您将在下一节了解它。

### 11.2.1 构建卡片

**卡片**——有时也称为**用户界面卡片**或**UI 卡片**——是一组特殊的 HTML 标签和 CSS 属性，旨在简洁高效地传达关于某物的信息，这可能是一件艺术品、一个事件、一个项目、一个人或您投资组合中的任何项目。典型的卡片包括以下一些或全部内容：

+   **图像**——一张照片、插图或其他图像，提供了项目的预览或表示

+   *标题*—项目的标题或名称

+   *文本*—对项目的简要描述

+   *按钮或链接*—允许读者了解更多关于项目或执行操作（如订阅或购买项目）的元素

组织卡片信息的方式有很多种，但两种布局比较常见。第一种常见布局是图片位于顶部，然后是标题、文本，最后是按钮或链接。图 11.2 展示了示例。

![图片](img/build-a-website-with-chatgpt-CH11_F02_McFedries3.png)

图 11.2 一个典型的卡片布局，信息从卡片顶部延伸到卡片底部

要提示 ChatGPT 创建使用此布局的卡片，你可以使用类似以下指令：

```py
Generate the code for a card with a maximum width of 350px. At the top of the card add the image portfolio01.jpg from the images subfolder. Below the image add the second-level heading "I Fell In Love With ChatGPT", followed by the text "I designed this book for Moughton-Hifflin's new line of AI-themed romance books", followed by a "Learn more" link to the file portfolio01.xhtml. Center the text in the card.
```

第二种常见布局是图片位于一侧（可以是左侧或右侧），而标题、文本和按钮或链接位于另一侧。图 11.3 展示了示例。

![图片](img/build-a-website-with-chatgpt-CH11_F03_McFedries3.png)

图 11.3 一个典型的卡片布局，图片位于左侧，文本位于右侧

要提示 ChatGPT 创建使用此布局的卡片，你可以使用如下指令：

```py
Generate the code for a card with a maximum width of 500px. On the left side of the card, add the image portfolio01.jpg from the images subfolder. On the right side of the card,  add the second-level heading "I Fell In Love With ChatGPT", followed by the text "I designed this book for Moughton-Hifflin's new line of AI-themed romance books", followed by a "Learn more" link to the file portfolio01.xhtml.
```

如果你对你周围图片的空白区域不满意，你将在下一节中学习如何修复它。

### 11.2.2 使图片延伸至卡片边缘

一个常见且吸引人的卡片调整是让图片延伸至卡片边缘：

+   *如果图片位于卡片顶部*—图片延伸至顶部、左侧和右侧边缘。

+   *如果图片位于卡片左侧*—图片延伸至顶部、左侧和底部边缘。

+   *如果图片位于卡片右侧*—图片延伸至顶部、右侧和底部边缘。

你可以通过在上一节中卡片提示中添加如下内容来请求 ChatGPT 配置卡片：

```py
Make sure there is no margin or padding around the image so that it extends all the way to the top, left, and right edges of the card.
```

此指令适用于顶部有图片的卡片，并生成如图 11.4 所示的卡片。

![图片](img/build-a-website-with-chatgpt-CH11_F04_McFedries3.png)

图 11.4 一个图片延伸至卡片边缘的卡片布局

另一个有用的卡片自定义选项是阴影效果，将在下一节中讨论。

### 11.2.3 添加阴影

注意图 11.2、11.3 和 11.4 中的每个卡片都有一个细微的阴影效果。这被称为*阴影效果*，因为它使卡片看起来像是稍微抬离页面，因此有一个“落下”到背景的阴影。关于这些阴影效果的例子有两点需要注意：

+   即使你的提示没有指定阴影效果，ChatGPT 也会自动添加阴影效果。如果你不希望有阴影效果，你需要在你的提示中包含如下指令：

    ```py
    Don't add a drop-shadow to the card.
    ```

+   ChatGPT 创建的阴影很吸引人，但可能不符合你的口味。例如，你可能更喜欢阴影延伸到卡片右侧的长度与延伸到卡片下方的长度相同。

创建阴影效果的 CSS 属性称为`box-shadow`，其语法在图 11.5 中显示。这里有四个你可以调整的值：

+   *`x-offset`*—阴影相对于卡片向右（任何正数）或向左（任何负数）移动的像素量

+   *`y-offset`*—阴影相对于卡片向下（任何正数）或向上（任何负数）移动的像素量

+   *`blur`*—阴影模糊的像素量，其中`0`表示无模糊，更高的值会使阴影逐渐模糊

+   *`alpha`*—一个介于 0 和 1 之间的值，用于定义阴影的透明度，其中`0`表示完全透明，`1`表示完全不透明

![](img/build-a-website-with-chatgpt-CH11_F05_McFedries3.png)

图 11.5 `box-shadow`属性的语法

这是向 ChatGPT 添加自定义阴影到卡片的一个示例指令：

```py
Add a drop-shadow effect to the card where both the x and y offset are 8px, the blur is 4px, and the transparency is 0.5.
```

注意：尽管在本章中你只将阴影应用到投资组合卡片上，但在实践中，你可以将阴影添加到任何创建块状元素的页面元素上，包括段落、标题、`div`元素或项目符号或编号列表。

此指令将生成类似于以下内容的阴影声明：

```py
box-shadow: 8px 8px 4px rgba(0, 0, 0, 0.5);
```

注意：有时 ChatGPT 生成的`box-shadow`值在*`blur`*数字和`rgba()`函数之间包含一个额外的数字（通常是 0）。这个额外的参数决定了阴影的*扩散*，这是阴影相对于卡片的大小（其中`0`表示阴影与卡片大小相同，更高的像素值会扩大阴影的大小）。

你还可以应用到你的卡片上的另一个效果是圆角处理，这是下一节的主题。

### 11.2.4 圆角处理

检查图 11.2、11.3 和 11.4，注意每个卡片的角落都是圆角化的，这使卡片看起来更柔和、更易于接近。关于这些圆角需要注意两点：

+   即使你的提示没有要求，ChatGPT 也会自动将卡片角落圆角化。如果你不希望有圆角，你需要在你的提示中包含如下指令：

    ```py
    Don't round the corners of the card.
    ```

+   曲率的量是可变的，你也可以只将曲率应用到特定的角落。

使角落圆角的 CSS 属性称为`border-radius`，其语法在图 11.6 中显示。

![](img/build-a-website-with-chatgpt-CH11_F06_McFedries3.png)

图 11.6 `border-radius`属性的语法

你可以调整四个值：

+   *`top-left`*—应用于卡片左上角的曲率量（以像素或百分比表示）

+   *`top-right`*—应用于卡片右上角的曲率量（以像素或百分比表示）

+   *`bottom-right`*—应用于卡片右下角的曲率量（以像素或百分比表示）

+   *`bottom-left`*—应用于卡片左下角的曲率量（以像素或百分比表示）

小贴士：ChatGPT 常生成的一个简短指令是 `border-radius:` *`value`*，其中 *`value`* 是应用于卡片四个角的所有曲率的量（以像素或百分比表示）。

这是一个向 ChatGPT 添加自定义圆角到卡片的示例指令：

```py
Round only the top-left and top-right corners of the card by 10px.
```

此指令将生成一个类似于以下内容的 `box-shadow` 声明：

```py
border-radius: 10px 10px 0 0;
```

对于作品集页面，你需要调查的最后一个设计想法是确保页面在任何尺寸的屏幕上都能良好显示，这是下一节的主题。

### 11.2.5 使你的页面响应式

如第十章所述，对于类似头部、页脚、导航区域、标题和段落这样的盒状网页元素，其默认布局行为是垂直向下流动：第二个元素位于第一个元素下方，第三个元素位于第二个元素下方，依此类推。作品集示例中的每个项目也将是这些盒状元素之一：`div` 元素。这意味着如果你满足于默认布局，你的作品集项目将以垂直堆叠的形式显示，这不是最吸引人或最有效率的视觉效果。

第十章中我提出的解决方案是使用 Flexbox，它将网页元素转换为 Flexbox 容器：该容器中的项目会失去其刚性的默认布局行为，并适应浏览器当前尺寸。对于这个项目，你可以通过一个简单的指令来提示 ChatGPT 使用 Flexbox：

```py
Make the portfolio container a Flexbox container. Enable the content to wrap and give each card a minimum width of 250px and a maximum width of 300px.
```

注意，这个提示包括设置卡片的最小和最大宽度的指令，因为你不希望它们变得过大或过小。

启用 Flexbox 容器中的内容——即你的作品集卡片——以换行，这意味着你的布局将根据浏览器窗口的当前尺寸自适应。能够做到这一点的布局被称为 *响应式*，这意味着你的作品集将在从大显示器到小巧的手机屏幕上的任何设备上看起来都很好。

然而，为了使你的页面在小屏幕上看起来最佳，你的 HTML 代码需要在 `<head>` 和 `</head>` 标签之间包含以下标签：

```py
<meta name="viewport" content="width=*device-width*, initial-scale=1">
```

此标签做两件事：

+   通过设置 `width=device-width`，你是在告诉浏览器将页面的宽度设置为与显示页面的设备宽度相同。

+   通过设置 `initial-scale=1`，你是在告诉浏览器最初显示页面时不要放大或缩小。

为了确保此标签包含在代码中，你的 ChatGPT 提示应该包含类似于以下内容的指令：

```py
In the page head section, include the tag <meta name="viewport" content="width=*device-width*, initial-scale=1">
```

之后，在我向你展示最终的页面布局（参见图 11.7）之后，我还会向你展示页面在平板电脑（图 11.8）和智能手机（图 11.9）上的显示效果，以验证页面确实是响应式的。

注意：你还可以使用一个特殊的 CSS 属性，称为 *媒体查询*，来使你的页面对不同屏幕尺寸的响应性更强。你将在第十二章学习如何使用媒体查询。

现在您知道如何提示 ChatGPT 构建投资组合页面，如以下章节所述。

## 11.3 构建投资组合页面的提示

本章的项目是一个投资组合页面，展示了一个虚构的书籍设计师的作品。在继续之前，我假设您已经准备好了以下内容：

+   以下之一或多个：页面标志、标题和标语

+   您想要用于页面标题和页面文本的字体名称

+   您想要应用于页面背景和文本的颜色名称

参考第三章了解每个设计元素以及如何提示 ChatGPT 进行标题、字体和颜色建议。

要开始您的提示，告诉 ChatGPT 您想要构建一个网页，并且希望它为您生成代码：

```py
I want to build a portfolio web page. I don't know how to code, so I need you to provide the code for me.

First, write the HTML code for a web page that includes the following:
```

现在逐项检查页面内容，包括以下内容（参见图 11.7）：

+   包含您的标志和标题的页眉

+   从页面标题开始的主元素

+   投资组合容器

+   投资组合卡片

+   包含版权声明的页脚

![](img/build-a-website-with-chatgpt-CH11_F07_McFedries3.png)

图 11.7 投资组合页面的部分

接下来，请让 ChatGPT 生成 CSS：

```py
Second, in a separate file please write the CSS code for the following:
```

您然后指定页面格式，包括以下内容：

+   页面背景颜色和文本颜色

+   您想要用于标题和页面文本的字体大小

+   用于标题和常规页面文本的字体

+   哪些元素应该是 Flexbox 容器（在这个项目中，这些将是页眉和投资组合容器）

这是我自己的投资组合页面的一个示例提示：

```py
I want to build a web page for a photo gallery. I don't know how to code, so I need you to provide the code for me.

First, write the HTML code for a web page that includes the following:
 * A header element that includes an image named logo.png, which is stored in the "images" subdirectory, and the title "Cover Me Book Design".
 * A main section with the heading "My Latest Book Designs".
 * A container with six UI cards, each of which has an image at the top, followed by a second-level heading, followed by some text. Here are the specifics for each of the six cards:
   * Card 1: The image portfolio01.jpg in the images subfolder; the heading "I Fell In Love with ChatGPT"; the text "I designed this book for Moughton-Hifflin's new line of AI-themed romance books."
   * Card 2: The image portfolio02.jpg in the images subfolder; the heading "The Shakespeare Time Machine"; the text "Maggie O'Farrell meets H.G. Wells in this historical fiction book I designed for Juxtaposition Publishing."
   * Card 3: The image portfolio03.jpg in the images subfolder; the heading "Our New ChatBot Overlords"; the text "A dystopian AI future awaits us all in this science fiction title I designed for H. J. Simpson Press."
   * Card 4: The image portfolio04.jpg in the images subfolder; the heading "Yo, Yossarian!"; the text "A biography of the character John Yossarian from Joseph Heller's novel Catch-22; designed for Hyperbole Editions."
   * Card 5: The image portfolio05.jpg in the images subfolder; the heading "The Mystery of the Missing Sock"; the text "A perennial mystery gets solved in this whodunit, which I designed for The Butler Did It Publications."
   * Card 6: The image portfolio06.jpg in the images subfolder; the heading "The Old Person's Guide to TikTok"; the text "I designed the cover of this TikTok how-to guide for Old People Are People, Too Press."
 * A footer element that includes the Copyright symbol, followed by "Cover Me Book Design".
 * In the page head section, include the tag <meta charset="utf-8">.
 * In the page head section, include the tag <meta name="viewport" content="width=device-width, initial-scale=1">.

Second, in a separate file write the CSS code for the following:
 * The page has background color mintcream and no margin.
 * The page text uses font size 20px and the Nunito font from Google Fonts.
 * The header has background color coral and 24px padding.
 * Make the header a Flexbox row container with centered content and allow the content to wrap.
 * The title is 64px, uses the Poppins font from Google Fonts, and has 16px padding on the left.
 * The main section has centered text and a 24px margin.
 * The main section heading has font size 30px and uses the Poppins font from Google Fonts.
 * Make the portfolio a Flexbox container. Enable the content to wrap and add a gap between items of 16px.
 * Give each card a minimum width of 200px and a maximum width of 350px.
 * For each card image, make sure there is no margin or padding around the image so that it extends all the way to the top, left, and right edges of the card.
 * Add 16px padding to the left and right of the card text.
 * Style the cards with a drop-shadow where both the x and y offsets are 8px, the blur is 4px, and the transparency is 0.3.
 * Style the cards with a border radius of 20px.
 * The footer has background color coral, 16px padding, and centered text.
```

我使用 OpenAI 的 ChatGPT 应用将我的提示提交给 GPT-4。生成的代码产生了图 11.8 所示的页面。

![](img/build-a-website-with-chatgpt-CH11_F08_McFedries3.png)

图 11.8 我的投资组合页面

图 11.8 显示了在桌面显示器上的页面外观。为了确保您的页面具有响应性，您需要使用一些较小的屏幕进行测试。例如，图 11.9 显示了在平板尺寸屏幕上的页面投资组合部分：投资组合通过降低到两列布局以适应较小的屏幕尺寸。

![](img/build-a-website-with-chatgpt-CH11_F09_McFedries3.png)

图 11.9 页面的投资组合部分在平板屏幕上使用两列布局。

当然，您还应该在智能手机屏幕上测试您的页面，如图 11.10 所示。在这种情况下，投资组合通过将其减少到单列布局以适应更小的屏幕尺寸。

![](img/build-a-website-with-chatgpt-CH11_F10_McFedries3.png)

图 11.10 页面的投资组合部分在智能手机屏幕上使用单列布局。

如果 ChatGPT 为您生成的代码完成了工作，您可以跳过本章的其余部分并将代码部署到网络上（如附录 B 中所述）。但是，如果您想了解投资组合页面代码，请继续阅读以获得更详细的了解。

## 11.4 检查投资组合页面代码

如果你好奇 ChatGPT 生成的代码，或者如果你想更好地理解它以便进行微调，下一两节提供了对之前在图 11.8-11.10 中展示的作品集页面背后的 HTML 和 CSS 代码的注释指南。

注意：我的作品集页面的生成 HTML 和 CSS 代码可在本书的网站上找到（[www.manning.com/books/build-a-website-with-chatgpt](https://www.manning.com/books/build-a-website-with-chatgpt)）以及本书的 GitHub 仓库：[`github.com/paulmcfe/websites-with-chatgpt`](https://github.com/paulmcfe/websites-with-chatgpt)。

我将在下一节开始介绍 HTML 代码。

### 11.4.1 检查 HTML

这是 ChatGPT 为我作品集页面生成的 HTML 代码的注释版本：

```py
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <meta name="viewport"                                                 ①
          content="width=device-width, initial-scale=1">                  ①
    <link rel="stylesheet" href="styles.css">                             ②
    <title>Cover Me Book Design</title>
</head>
<body>
    <header>                                                              ③
        <img src="images/logo.png"                                        ③
             alt="Cover Me Book Design Logo">                             ④③
        <h1>Cover Me Book Design</h1>                                     ⑤③
    </header>                                                             ③

    <main>
        <h1>My Latest Book Designs</h1>                                   ⑥
        <div class="portfolio">                                           ⑦
                                                                          ⑦
            <div class="card">                                            ⑧⑦
                <img src="images/portfolio01.jpg"                         ⑨⑧⑦
                     alt="I Fell In Love with ChatGPT"                    ⑧⑦
                     class="card-image">                                  ⑧⑦
                <h2>I Fell In Love with ChatGPT</h2>                      ⑩⑧⑦
                <p>I designed this book for Moughton-Hifflin's new        ⑪⑧⑦
                    line of AI-themed romance books.                      ⑪⑧⑦
                </p>                                                      ⑧⑦
            </div>                                                        ⑧⑦
                                                                          ⑦
            <div class="card">                                            ⑦
                <img src=»images/portfolio02.jpg»                         ⑦
                     alt="The Shakespeare Time Machine"                   ⑦
                     class="card-image">                                  ⑦
                <h2>The Shakespeare Time Machine</h2>                     ⑦
                <p>Maggie O'Farrell meets H.G. Wells in this historical   ⑦
                    fiction book I designed for Juxtaposition Publishing. ⑦
                </p>                                                      ⑦
            </div>                                                        ⑦
                                                                          ⑦
            <div class="card">                                            ⑦
                <img src=»images/portfolio03.jpg»                         ⑦
                     alt="Our New ChatBot Overlords"                      ⑦
                     class="card-image">                                  ⑦
                <h2>Our New ChatBot Overlords</h2>                        ⑦
                <p>A dystopian AI future awaits us all in this science    ⑦
                    fiction title I designed for H. J. Simpson Press.     ⑦
                </p>                                                      ⑦
            </div>                                                        ⑦
                                                                          ⑦
            <div class="card">                                            ⑦
                <img src=»images/portfolio04.jpg»                         ⑦
                     alt="Yo, Yossarian!"                                 ⑦
                     class="card-image">                                  ⑦
                <h2>Yo, Yossarian!</h2>                                   ⑦
                <p>A biography of the character John Yossarian from       ⑦
                    Joseph Heller's novel Catch-22, designed for          ⑦
                    Hyperbole Editions.                                   ⑦
                </p>                                                      ⑦
            </div>                                                        ⑦
                                                                          ⑦
            <div class="card">                                            ⑦
                <img src=»images/portfolio05.jpg»                         ⑦
                     alt="The Mystery of the Missing Sock"                ⑦
                     class="card-image">                                  ⑦
                <h2>The Mystery of the Missing Sock</h2>                  ⑦
                <p>A perennial mystery gets solved in this whodunit,      ⑦
                    which I designed for The Butler Did It Publications.  ⑦
                </p>                                                      ⑦
            </div>                                                        ⑦
                                                                          ⑦
            <div class="card">                                            ⑦
                <img src=»images/portfolio06.jpg»                         ⑦
                     alt="The Old Person's Guide to TikTok"               ⑦
                     class="card-image">                                  ⑦
                <h2>The Old Person's Guide to TikTok</h2>                 ⑦
                <p>I designed the cover of this TikTok how-to guide for   ⑦
                    Old People Are People, Too Press.                     ⑦
                </p>                                                      ⑦
            </div>                                                        ⑦
        </div>                                                            ⑦
    </main>

    <footer>                                                              ⑫
        <p>&copy; Cover Me Book Design</p>                                ⑫
    </footer>                                                             ⑫
</body>
</html>
```

① 帮助页面在移动设备上正确显示

② 告诉网络浏览器在哪里找到 CSS 代码

③ 页面页眉

④ 网站标志

⑤ 网站标题

⑥ 页面标题

⑦ 作品集

⑧ 作品集卡片

⑨ 卡片图片

⑩ 卡片标题

⑪ 卡片文本

⑫ 页面页脚

注意，HTML 代码中包含以下行：

```py
<link rel="stylesheet" href="styles.css">
```

这个标签告诉网络浏览器在哪里找到 CSS 代码，我将在下一节中进行描述。

### 11.4.2 检查 CSS

这是 ChatGPT 为我作品集页面生成的 CSS 代码的注释版本：

```py
@import url('https://fonts.googleapis.com/css2?]family=Nunito&family=Poppins&display=swap');      ①

body {
    background-color: mintcream;                  ②
    margin: 0;                                    ②
    font-size: 20px;                              ②
    font-family: 'Nunito', sans-serif;            ②
}

header {
    background-color: coral;                      ③
    padding: 24px;                                ③
    display: flex;                                ④
    justify-content: center;                      ④
    align-items: center;                          ④
    flex-wrap: wrap;                              ④
}

header h1 {
    font-size: 64px;                              ⑤
    font-family: 'Poppins', sans-serif;           ⑤
    padding-left: 16px;                           ⑤
}

main {
    text-align: center;                           ⑥
    margin: 24px;                                 ⑥
}

main h1 {
    font-size: 30px;                              ⑦
    font-family: 'Poppins', sans-serif;           ⑦
}

.portfolio {
    display: flex;                                ⑧
    flex-wrap: wrap;                              ⑧
    justify-content: center;                      ⑧
    gap: 24px;                                    ⑧
}

.card {
    min-width: 200px;                             ⑨
    max-width: 350px;                             ⑨
    box-shadow: 8px 8px 4px rgba(0, 0, 0, 0.3);   ⑩
    border-radius: 20px;                          ⑪
    overflow: hidden;                             ⑫
}

.card img {
    width: 100%;                                  ⑬
    margin: 0;                                    ⑬
    padding: 0;                                   ⑬
}

.card h2, .card p {
    padding: 0 16px;                              ⑭
}

footer {
    background-color: coral;                      ⑮
    padding: 16px;                                ⑮
    text-align: center;                           ⑮
}
```

① 从 Google Fonts 导入 Nunito 和 Poppins 字体

② 设置页面背景颜色、边距和文本大小及字体

③ 设置页眉背景颜色和填充

④ 将页眉设置为具有居中、换行内容的 Flexbox 容器

⑤ 设置页面标题的字体大小、字体和左内边距

⑥ 使用边距样式设计主要元素，并居中文本

⑦ 设置页面标题的字体大小和字体

⑧ 将作品集设置为具有换行、居中内容和项目之间间隙的 Flexbox 容器

⑨ 为每个卡片设置最小和最大宽度

⑩ 为卡片设置阴影效果

⑪ 以圆角样式设计卡片

⑫ 确保图片的角落也是圆角

⑬ 为每个卡片图片设置延伸到卡片边缘的样式

⑭ 为卡片文本添加 16 px 的左右填充

⑮ 设置页脚背景颜色和填充，并居中文本

你可以参考前两节中的 HTML 和 CSS 注释，以帮助自定义你的网页代码，正如我在下一节中描述的那样。

## 11.5 自定义作品集页面

这里有一些 HTML 代码的自定义建议：

+   在页眉中，你可以编辑标题。只需确保不要编辑或删除相关的 HTML 标签`<h1>`和`</h1>`。

+   如果你正在构建包含多个作品集的网站，你将需要一个导航区域，以便访客可以轻松找到你的其他页面。请参考第六章了解如何提示 ChatGPT 获取链接和导航栏。

+   在主要部分，你可以编辑页面标题，但不要修改相关的 HTML 标签`<h1>`和`</h1>`。

+   如果你想包含一个或多个额外的引言段落，请将它们添加到`main`元素中的`<h1>`标签下方。确保每个段落都能正确渲染，通过在段落开头和结尾处分别使用`<p>`标签和`</p>`标签来实现：

    ```py
    <main>
        <h1>My Latest Book Designs</h1>
        <p>
            Type your introductory paragraph text here.
        <p>
        <div class="portfolio">
        etc.
    ```

+   在 HTML 代码的页脚部分，你可以添加指向你的社交媒体账户的链接，正如我在第四章中描述的那样。

现在，这里有一些 CSS 代码的定制想法：

+   如果你不喜欢阴影效果，你可以通过查找以下代码并删除`box-shadow`声明来移除它：

    ```py
    .card {
        min-width: 200px;
        max-width: 350px;
        box-shadow: 8px 8px 4px rgba(0, 0, 0, 0.3);
        border-radius: 20px;
        overflow: hidden;
    }
    ```

+   如果你没有使用阴影效果，你仍然需要某种方法让你的卡片从页面背景中脱颖而出。最简单的方法是在卡片周围添加一个边框（参考第五章）。在 CSS 代码中，在`box-shadow`声明出现的位置添加`border`声明，如下所示（根据你的个人作品集调整值）：

    ```py
    .card {
        min-width: 200px;
        max-width: 350px;
        border: 5px solid coral;
        border-radius: 20px;
        overflow: hidden;
    }
    ```

+   如果你更喜欢你的卡片文本左对齐，你可以通过在 CSS 中找到以下代码并将`text-align`值从`center`更改为`left`来更改它：

    ```py
    main {
        text-align: center;
        margin: 24px;
    }
    ```

+   对于任何颜色值，你可以将现有的颜色更改为不同的颜色关键字。

+   对于任何字体大小值，你可以通过改变数字来增加或减少字体大小。只需确保保留`px`单位。

+   对于任何填充或边距值，你可以通过改变数字来增加或减少填充或边距。在每种情况下，务必保留`px`单位。

+   为了使你的页面代码更易于访问，考虑将所有 px 测量值转换为 rem 测量值。默认情况下，1 rem 相当于 16 px，所以 20 px 是 1.25 rem，24 px 是 1.5 rem，32 px 是 2 rem，48 px 是 3 rem，依此类推。rem 单位更易于访问，因为它测量的是相对于浏览器用户在浏览器设置中定义的默认字体大小的字体大小。

## 摘要

+   卡片是一组特殊的 HTML 标签和 CSS 属性的特殊集合，旨在有效地传达关于物品的信息：一件艺术品、一个事件、一个项目、一个人等等。

+   大多数卡片都包括物品的图片、物品的标题或名称、物品的简要描述，以及一个按钮或链接，允许读者了解更多关于物品的信息或执行与物品相关的操作。

+   两种最常见的卡片布局是垂直布局，其中卡片元素从上到下排列（图片、标题、文本、链接），和水平布局，其中卡片元素从左到右排列（通常图片在左侧，文本在右侧）。

+   你可以使用`box-shadow`属性为卡片添加阴影效果。

+   你可以使用`border-radius`属性来使卡片的角落变得圆润。

+   为了获得最佳效果，你的页面提示应该尽可能具体，包括颜色、字体大小和标题级别。

+   将生成的 HTML 保存到 index.xhtml 文件，将生成的 CSS 保存到 HTML 代码中 ChatGPT 建议的文件名，通常是 styles.css。

# 12 构建文章页面

本章涵盖

+   文章页面的结构

+   使用 CSS Grid 布局页面

+   使文章在智能手机屏幕上看起来更好

+   为构建文章页面编写 ChatGPT 提示

+   检查和自定义 ChatGPT 生成的代码

建立网页的原因和想要建立某种网络存在感的人一样多。然而，这些原因中的大多数都可以归纳为两大类：自我表达和信息共享。到目前为止，在这本书中，你已经完成了几个与自我表达相关的项目：个人主页（第三章）、在线日记（第五章）、照片画廊（第十章）和作品集页面（第十一章）。你同样也完成了与信息共享相关的项目：读书俱乐部页面（第四章）、信息网站（第六章）、兴趣或爱好网站（第七章）、活动报名页面（第八章）和食谱页面（第九章）。

本章将向您介绍另一种信息共享页面结构：文章页面。这个页面使用常见的 HTML 结构，如页眉、导航栏、侧边栏和页脚，所有这些都被安排在页面的中心：一篇包含几个部分的长文章。本章将比之前的项目更加“动手实践”，因为手动添加部分、标题和段落以及标记文本（即添加适当的 HTML 标签）比依赖 ChatGPT 来完成所有工作要容易得多。不过，不用担心：你仍然会利用 ChatGPT 的编码知识来创建文章页面的基本结构，并添加一些额外的功能，使你的文章脱颖而出。

## 12.1 了解本章的项目

本章的项目是一个文章页面。最终页面将包括以下组件：

+   包含标志、标题和口号的页眉元素

+   包含链接到网站其他部分的导航栏

+   包含标题的文章元素的主元素

+   文章中包含多个部分元素，每个部分都有自己的标题和段落

+   包含相关信息的侧边栏元素

+   包含版权声明的页脚元素

图 12.1 展示了使用 ChatGPT 提供的代码和文本创建的（部分）示例文章页面。

![](img/build-a-website-with-chatgpt-CH12_F01_McFedries3.png)

图 12.1 由 ChatGPT 生成的文章页面

示例页面是一篇虚构的旅行文章，来自一部文学作品（纳尼亚，C.S.路易斯的幻想系列《纳尼亚传奇》的主要背景），但你也可以使用文章布局来展示许多其他类型的内容：新闻条目、论文、博客文章、评论、传记、历史记载等等。你将在下一节中开始学习如何构建文章布局。

## 12.2 构建文章页面

你如何知道一篇文章的页面布局是你需要的？检查你想要在页面上显示的主要内容，并问自己以下问题：

+   写作是否专注于单一主题？

+   写作是否被分为多个子主题？

如果两个问题的答案都是“是”，那么在本章中你学到的文章布局将是你写作的一个很好的展示。

在你学习如何将页面布局为文章之前，你应该稍微退后一步，回顾你在本书早期章节中遇到的 HTML 页面布局元素。这将帮助你理解文章页面的整体布局。

### 12.2.1 回顾 HTML 页面布局元素

在本书的大部分项目中，ChatGPT 生成的 HTML 使用了以下元素之一或全部来布局页面：

+   `header`—定义一个包含介绍性内容的页面区域。此内容通常是网站标题（应使用标题元素，如`h1`进行标记），但它也可以包括网站标志和标语。以下是一个示例（来自第九章）：

    ```py
    <header>
        <img src="super-baker.png" alt="The Super Baker Logo">
        <h1>The Super Baker</h1>
        <p>The ultimate guide to super-powered baking. Learn how to 
            make delicious treats that will boost your energy, 
            strength, and speed.</p>
    </header>
    ```

+   `nav`—定义一个包含导航内容的页面区域，例如指向网站其他部分的链接。此元素可以在页面的任何位置，但通常出现在页面的`header`元素之后。以下是一个示例（来自第六章）：

    ```py
    <nav>
        <a href="index.xhtml">Home</a>
        <a href="blog.xhtml">Blog</a>
        <a href="faq.xhtml">FAQ</a>
        <a href="about.xhtml">About</a>
        <a href="contact.xhtml">Contact</a>
    </nav>
    ```

+   `main`—为当前页面独特的内容创建一个容器。与`header`、`nav`和`footer`元素通常是网站所有或大多数页面的共同元素不同，`main`元素旨在标记独特的内容。每个页面只能有一个`main`元素。它通常出现在`header`和`nav`元素之后，如下所示（来自第六章）：

    ```py
    <header>
        <h1>Antediluvian Word Preservation Society</h1>
        <p>Preserving words from the past for the future</p>
    </header>
    <nav>
        <a href="index.xhtml">Home</a>
        <a href="blog.xhtml">Blog</a>
        <a href="faq.xhtml">FAQ</a>
        <a href="about.xhtml">About</a>
        <a href="contact.xhtml">Contact</a>
    </nav>
    <main>
        *Unique page content goes here*
    </main>
    ```

+   `section`—包含你希望在页面大纲中看到的页面任何部分。也就是说，如果页面的某个部分由一个标题元素（如`h2`或`h3`）和一些文本组成，你将使用`<section>`和`</section>`标签包围标题及其文本，如下所示（来自第六章）：

    ```py
        <section>
          <h2>This week's challenge</h2>
          <p>
              Your challenge this week is to use the word tomfoolery 
              — foolish or silly behavior — at least once in each 
              of the following: in conversation, in an email message, 
              in a text message, and in a business meeting (virtual or 
              real-world). Good luck and let us know how you make out!
          </p>
        </section>
    ```

+   `p`—将一大块文本标记为段落。`section`元素通常由一个或多个段落组成，尽管你也可以将段落添加到任何其他元素中，特别是`header`、`main`和`footer`元素。

+   `footer`—定义一个包含结尾内容的页面区域，例如版权声明、地址和联系方式。以下是一个示例（来自第四章）：

    ```py
    <footer>
        <p>Copyright 2023 Code & Prose</p>
        <p>
            <a href="https://www.facebook.com/CodeAndProse">
            <i class="fab fa-facebook-square"></i></a>
            <a href="https://www.instagram.com/codeandprose">
            <i class="fab fa-instagram"></i></a>
            <a href="https://twitter.com/codenprose">
            <i class="fab fa-twitter-square"></i></a>
        </p>
    </footer>
    ```

图 12.2 显示了一个抽象页面布局，展示了这些元素在页面上的显示方式。注意，它包括我在本节中没有涵盖的两个 HTML 页面布局元素：`article`和`aside`。不出所料，`article`元素在本章的文章页面布局中起着至关重要的作用，因此我将在下一节中详细介绍它。

![](img/build-a-website-with-chatgpt-CH12_F02_McFedries3.png)

图 12.2 包含基本 HTML 布局元素的概念布局

### 12.2.2 使用文章元素

你使用`article`元素来标记一个完整、自包含的组成。这里的模型是一篇报纸或杂志文章，但这个元素也可以应用于评论、博客条目、论坛帖子或论文。大多数页面都有一个`article`元素嵌套在`main`元素中。那个`article`元素通常包含以下内容：

+   标题，通常标记为二级标题（即`h2`元素）

+   一个或多个介绍性的`p`元素（段落）

+   一个或多个`section`元素

+   在每个`section`元素内部，一个第三级标题（即`h3`元素）后跟一个或多个`p`元素

以上内容并非一成不变。例如，一个`article`元素只包含标题和一个或多个段落是完全可行的。然而，为了本章的目的，文章页面布局使用这些元素。以下是你会使用的通用结构：

```py
<main>
    <article>
        <h2>Article Title</h2>
        <p>Introductory paragraph</p>
        <section>
            <h3>Section 1 heading</h3>
            <p>
                Section 1 paragraph 1
            </p>
            <p>
                Section 1 paragraph 2
            </p>
            <p>
                etc.
            </p>
        </section>
        <section>
            <h3>Section 2 heading</h3>
            <p>
                Section 2 paragraph 1
            </p>
            <p>
                Section 2 paragraph 2
            </p>
            <p>
                etc.
            </p>
        </section>
        <section>
            <h3>Section 3 heading</h3>
            <p>
                Section 3 paragraph 1
            </p>
            <p>
                Section 3 paragraph 2
            </p>
            <p>
                etc.
            </p>
        </section>
    </article>
</main>
```

通常，你可以通过在提示中包含类似于以下指令来让 ChatGPT 生成`article`元素的代码：

```py
In the main section, add an article element where the article title is "[*title*]" as a second-level heading.
```

在图 12.2 中较早展示的第二个新的 HTML 页面布局元素是`aside`，你将在下一部分了解它。

### 12.2.3 在你的页面上包含侧边栏

你使用`aside`元素来标记一个包含与页面独特内容间接相关的内容的页面侧边栏区域（在本章的布局中，这个独特内容指的是在`article`元素中显示的内容）。以下是一些此类侧边栏的用例：

+   与页面主要内容相关的网站页面链接列表

+   最新网站新闻

+   社交媒体动态

+   一个或多个广告

`aside`元素可以出现在`main`元素中的任何位置（可以在页面上多次出现）。在本章的文章页面布局中，`aside`元素出现在页面的`article`元素之后，如下例所示：

```py
<main>
    <article>
        <h2>Article Title</h2>
        <p>Introductory paragraph</p>
        <section>
            <h3>Section 1 heading</h3>
            <p>
                Section 1 paragraph 1
            </p>
            <p>
                Section 1 paragraph 2
            </p>
            <p>
                etc.
            </p>
        </section>
        <section>
            <h3>Section 2 heading</h3>
            <p>
                Section 2 paragraph 1
            </p>
            <p>
                Section 2 paragraph 2
            </p>
            <p>
                etc.
            </p>
        </section>
        <section>
            <h3>Section 3 heading</h3>
            <p>
                Section 3 paragraph 1
            </p>
            <p>
                Section 3 paragraph 2
            </p>
            <p>
                etc.
            </p>
        </section>
    </article>
    <aside>
        <h3>Aside heading</h3>
        <p>
            Aside paragraph 1
        </p>
        <p>
            Aside paragraph 2
        </p>
        <p>
            etc.
        </p>
    </aside>
</main>
```

通常，为了让 ChatGPT 生成`aside`元素的代码，你需要在提示中包含类似于以下指令的指令：

```py
At the bottom of the main section, add an aside element where the aside title is "[*title*]" as a third-level heading.
```

作为本章更实用的方法的一部分，在接下来的几个部分中，你将学习如何向你的页面添加新项目，而不是让 ChatGPT 生成这些项目。

### 12.2.4 向文章添加新部分

文章可以是短篇或长篇。对于短篇文章，将文本和标题包含在 ChatGPT 提示中，让模型为你做大部分工作是没有问题的。然而，这种方法对于长篇文章来说并不那么有效，因为你的提示最终会变得非常长。这种长度可能导致两个问题：

+   你可能超过提示中允许的最大字符数。

+   提示越长，ChatGPT 在生成回复时迷失方向的可能性就越大。

由于这些原因，在本章的项目中，你只需要让 ChatGPT 创建页面布局的骨架。然后，你将手动添加剩余的文章内容，为这些骨架添加血肉。

ChatGPT 返回的 HTML 代码部分看起来像这样：

```py
<main>
    <article>
        <h2>Travel Guide to Narnia</h2>
        <!-- Article content goes here -->
    </article>
</main>
```

添加新`section`元素到文章的步骤如下：

1. 在文本编辑器中打开 HTML 文件。

2. 将光标置于`<!-- Article content goes here -->`文本占位符之后，如图 12.3 所示。

![图片](img/build-a-website-with-chatgpt-CH12_F03_McFedries3.png)

图 12.3 将光标置于此处所示的位置。

3. 按下 Enter 或 Return 键开始新行。

4. 输入`<section>`。如果您使用的是代码编辑器，它应该自动添加`</section>`标签（尽管您可能需要按 Tab 键来实现这一点）。如果不是，请输入`</section>`并将光标置于`<section>`和`</section>`标签之间。

5. 按下 Enter 或 Return 键。现在您有一个新的`section`元素准备使用，如图 12.4 所示。

![图片](img/build-a-website-with-chatgpt-CH12_F04_McFedries3.png)

图 12.4 新的`section`元素，准备填充

6. 输入`<h3>`。如果您使用的是代码编辑器，它应该自动添加`</h3>`标签（尽管您可能需要按 Tab 键来实现这一点）。如果不是，请输入`</h3>`并将光标置于`<h3>`和`</h3>`标签之间。

7. 输入部分标题或标题，如图 12.5 所示。（您现在还没有添加段落。我将在下一节中介绍这一点。）

![图片](img/build-a-website-with-chatgpt-CH12_F05_McFedries3.png)

图 12.5 为新部分输入标题或标题

8. 要添加更多部分，将光标置于您刚刚添加的`section`元素的`</section>`标签之后，然后按照步骤 3 到 7 进行操作。

您的新`section`元素有标题但没有文本。您将在下一节中解决这个问题。

### 12.2.5 在文章、部分或旁白中添加新段落

无论您是在处理页面的`article`元素、任何`section`元素还是`aside`元素，您通常都需要添加另一个段落。以下是完成此操作的步骤：

1. 在文本编辑器中打开 HTML 文件。

2. 将光标置于您想添加段落的元素的结束标签之后。例如，如果您在一个当前只包含`h3`元素标题的`section`元素中工作，您将光标置于`</h3>`标签之后，如图 12.6 所示。

![图片](img/build-a-website-with-chatgpt-CH12_F06_McFedries3.png)

图 12.6 将光标置于您想添加段落的元素的结束标签之后。

3. 按下 Enter 或 Return 键开始新行。

4. 输入`<p>`。如果您使用的是代码编辑器，它应该自动添加`</p>`标签（尽管您可能需要按 Tab 键来实现这一点）。如果不是，请输入`</p>`并将光标置于`<p>`和`</p>`标签之间。

5. 按下 Enter 或 Return 键。现在您有一个新的`p`元素准备输入文本，如图 12.7 所示。

![图片](img/build-a-website-with-chatgpt-CH12_F07_McFedries3.png)

图 12.7 新的`p`元素，准备输入文本

6. 输入段落文本，如图 12.8 所示。

![图片](img/build-a-website-with-chatgpt-CH12_F08_McFedries3.png)

图 12.8 为新部分输入标题或标题。

7. 对于你想要添加的每个新段落，将光标置于当前段落的 `</p>` 标签之后，然后按照步骤 3 到 6 进行操作。

当你输入段落文本时，你可能会遇到你想要网页浏览器以粗体或斜体显示的特殊单词或短语。你将在下一节中学习如何做到这一点。

### 12.2.6 标记特殊单词和短语

你的文本中的某些单词或短语在某种意义上是“特殊”的，因为它们以某种方式与文本的其余部分区分开来。例如，你可能想要强调某个特定的单词，你通常会通过使用斜体格式化单词来实现这一点。同样，一个特定的短语可能很重要，为了确保读者不会错过它，你通常会使用粗体格式化短语。

虽然当然可以指示 ChatGPT 在需要的地方添加斜体和粗体，但在许多情况下可能会出现问题：

+   你的文本可能多次使用一个单词或短语。

+   你可能只想标记单词或短语的第一实例。

+   你的文本可能包含许多你想要标记的不同的单词或短语。

在每种情况下，你都需要找到一种方法来确保 ChatGPT 标记了你想要的文本，这在实践中并不容易做到。相反，实际上在你输入文本时手动进行标记要简单得多。接下来的几节将提供详细信息。

标记重要文本

在你的网页上，你可能想要确保读者看到某个特定的单词、短语或句子，因为它很重要。这段文本可能是一个重要的指令、一个关键条件或类似的具有重大意义的段落，需要从普通文本中突出显示，因为你不希望读者错过它。在 HTML 中，你通过使用 `strong` 元素来标记文本为重要：

```py
<strong>*important text goes here*</strong>
```

所有浏览器都会将 `<strong>` 和 `</strong>` 标签之间的文本以粗体字体显示。以下示例展示了带有重要段落并使用 `strong` 元素标记的网页代码，图 12.9 显示了在网页浏览器中显示的粗体文本：

```py
<p>
    As you enter the room, notice the big, red button to your right.
    <strong>Never press that button!</strong>
</p>
```

![](img/build-a-website-with-chatgpt-CH12_F09_McFedries3.png)

图 12.9 使用 `strong` 元素标记的文本在浏览器中显示为粗体。

类似的标记场景是关键词，将在下文讨论。

标记关键词

在某些情况下，你想要引起对某个单词或短语的关注，并不是因为它本身很重要，而是因为相关的文本在某种角色上使其与普通文本不同。这种文本可能是一个产品名称、公司名称或界面元素，例如与复选框或命令按钮相关的文本。再次强调，你正在处理的文本本身并不重要，但它以某种方式不同，因此你希望它看起来与普通页面文本不同。

小贴士：网页关键词的其他候选包括人名（例如出现在名人八卦专栏中的臭名昭著的“粗体名字”）以及文章的前几个单词或开头句子。

这些每一项都表示一个*关键词*（或*关键短语*），它具有超出常规页面文本的意义。在 HTML 中，这种类型的项目通过使用`b`元素进行标记：

```py
<b>*keyword*</b>
```

网络浏览器将`<b>`和`</b>`标签之间的文本以粗体字体显示，如下面的示例和图 12.10 所示：

```py
<p>
    To save your work, pull down the <b>File</b> menu 
    and then click <b>Save</b>.
</p>
```

![](img/build-a-website-with-chatgpt-CH12_F10_McFedries3.png)

图 12.10 使用`b`元素标记的关键词在浏览器中显示为粗体。

到目前为止，我想你可能正在挠头，想知道`strong`元素和`b`元素之间的区别，因为两者都显示为粗体文本。这是一个合理的观点，我必须承认区别是微妙的。我应该说是*语义的*，因为 HTML 使用这两个不同的元素来区分重要文本和关键词。为什么要这么做呢？因为预计将来屏幕阅读器和其他辅助设备将使用这种语义区分来帮助视障人士理解网页。

标记强调文本

在页面上强调某些单词或短语通常很重要。这种强调告诉读者要以加重的语气阅读或说出文本。在 HTML 中，您可以通过使用`em`（表示强调）元素来标记单词或短语以添加强调：

```py
<em>*text*</em>
```

网络浏览器将`<em>`和`</em>`标签之间的文本以斜体显示，如下面的示例和图 12.11 所示：

```py
<p>
    When mixing pie pastry, it's <em>vital</em> that 
    your butter is as cold as possible.
</p>
```

![](img/build-a-website-with-chatgpt-CH12_F11_McFedries3.png)

图 12.11 使用`em`元素标记的文本在浏览器中显示为斜体。

注意：`strong`元素和`em`元素之间的区别是什么？当问题中的文本对读者来说本质上至关重要时，您使用`strong`；当问题中的文本需要增强强调以传达观点时，您使用`em`。

标记替代文本

在散文中，通常需要标记单词或短语以表明它具有与常规文本不同的声音、语气或角色。常见的替代文本例子包括书籍和电影标题。在 HTML 中，这种语义文本通过使用`i`（表示斜体）元素进行标记：

```py
<i>*text*</i>
```

注意：替代文本的其他例子包括出版物名称、技术术语、外语短语以及一个人的想法。

网络浏览器将此类文本以斜体显示，如下面的示例和图 12.12 所示：

```py
<p>
    Let's visit the land of Narnia, first introduced to us by 
    C.S. Lewis in <i>The Lion, the Witch, and the Wardrobe</i> (1950).
</p>
```

![](img/build-a-website-with-chatgpt-CH12_F12_McFedries3.png)

图 12.12 使用`i`元素标记的替代文本在浏览器中显示为斜体。

你可以在其他文本级元素内嵌套这些文本级元素以产生额外效果。例如，你可以通过使用`strong`元素来标记一个句子为重要，并在那个句子中，你可以通过使用`em`元素来标记一个词以强调，浏览器将渲染该词为粗体和斜体。

### 12.2.7 以滴管首字母开始文章

你可以通过在文章开头使用*滴管首字母*（第一段的第一字母，格式化后看起来比段落其他文本大得多，并定位在文本基线之下，向下“滴落”几行）来让你的文章脱颖而出。要使 ChatGPT 为你创建滴管首字母，在你的提示中包含类似以下指令：

```py
Create the HTML and CSS code that renders the following text as a paragraph with a dark red drop cap: "Starting an article doesn't have to be boring! Get your text off to a great beginning by rocking the opening paragraph with a giant first letter. You can use either a <i>raised cap</i> (also called a <i>stick-up cap</i> or simply an <i>initial</i>) that sits on the baseline, or you can use a <i>drop cap</i> that sits below the baseline and nestles into the text."
```

这是 ChatGPT 生成的 HTML：

```py
<p>
    <span class="drop-cap">S</span>tarting an article doesn't have to be 
    boring! Get your text off to a great beginning by rocking the opening 
    paragraph with a giant first letter. In particular, you can use a 
    <i>drop cap</i> that sits below the baseline and nestles into the text.
</p>
```

关键是包围段落第一字母的`<span>`和`</span>`标签。`span`元素使用`drop-cap`类，在 CSS 代码中看起来如下：

```py
.drop-cap {
    float: left;                 ①
    font-size: 4em;              ②
    line-height: 0.8em;          ③
    padding: 0.1em 0.1em 0 0;    ④
    color: darkred;              ⑤
}
```

① 将字母从常规页面流程中移除

② 使字母变大

③ 调整滴管首字母的位置

④ 给滴管首字母留出一些空间

⑤ 设置滴管首字母的颜色

图 12.13 展示了在浏览器中滴管首字母的显示效果。

![](img/build-a-website-with-chatgpt-CH12_F13_McFedries3.png)

图 12.13 带有滴管首字母的文章开头段落

滴管首字母是给网页增添专业风格的好方法。只需记住，你只为文章第一段的第一字母使用滴管首字母。

### 12.2.8 使用 CSS Grid 布局文章

当我在第十章介绍 Flexbox 时，我提到，默认情况下，网络浏览器通过堆叠它们来布局 HTML 块级元素，包括`header`、`nav`、`main`、`section`、`aside`、`footer`和`p`元素。第一个块在顶部，第二个块位于其下方，第三个块位于第二个块下方，依此类推。这不是一个非常鼓舞人心的外观！

Flexbox 使你能够在一个维度（水平或垂直）中跳出默认布局，但如果你想在两个维度（水平和垂直）中布局你的页面，你需要转向另一种称为 CSS Grid 的布局技术。

CSS Grid 的好消息是，你可以在提示的 CSS 部分包含一个简单指令，让 ChatGPT 为你生成所有必需的代码：

```py
The header is a two-column CSS Grid container with the logo in the left column and the site title and tagline in the right column.
```

就这些！然而，为了本章项目的目的，我会提到 ChatGPT 生成的 CSS Grid 代码的一个重要方面。如果你参考图 12.2，注意以下两点：

+   在`main`元素内部，`aside`元素被布局在`article`元素的右侧。

+   `article`元素比`aside`元素占用更多的水平空间。

这一切都是通过 CSS Grid 完成的。要了解它是如何工作的，首先检查 HTML：

```py
<main>
    <article>
        *Article content goes here*
    </article>

    <aside>
        *Aside content goes here*
    </aside>
</main>
```

通常，网络浏览器会将`article`元素堆叠在`aside`元素之上，并且两者都会是`main`元素的全宽。你可以通过向 ChatGPT 发出类似以下指令来打破这种默认布局：

```py
The main element is a two-column CSS Grid container where the article element column is twice the width of the aside element column.
```

在这种情况下，生成的 CSS Grid 代码将`aside`元素放置在`article`元素的右侧，并通过为`main`元素定义一个两列网格来调整元素的宽度：

```py
main {
    display: grid;                     ①
    grid-template-columns: 2fr 1fr;    ②
}
```

① 将主元素设置为网格容器

② 将网格容器分为两列

`article`元素在 HTML 中排在第一位，因此被分配到左侧列，而`article`元素被分配到右侧列。关键在于`grid-template-columns`属性的`2fr 1fr`值。这个看起来奇怪的值定义了两个列的相对宽度如下：

1.  将`main`元素所有可用的水平空间全部占用。

1.  将那个水平空间平均分成三部分。

1.  将其中两部分分配给第一列。

1.  将剩余的部分分配给第二列。

这给你一些自由度来调整这些相对宽度以适应你自己的页面。例如，如果你希望`article`元素有三个可用空间单位，而`aside`元素只有一个单位，你可以按如下方式修改规则：

```py
main {
    display: grid;
    grid-template-columns: 3fr 1fr;
}
```

正如你在下一节中学习的那样，尽管 CSS Grid 可以使你的页面对浏览器窗口大小的变化做出响应，但它并不足以使文章页面在所有屏幕上显示良好。

### 12.2.9 调整小屏幕上的文章页面布局

我在上一节中引入的`fr`单位被称为*相对*测量，因为例如`1fr`的值取决于网格容器中可用的宽度（假设你在使用网格列）。这使得你的页面具有响应性，因为当网格容器的宽度改变时（可能是因为浏览器窗口的宽度改变），列的宽度会自动相对于新的宽度进行改变。

这对于相对较大的屏幕（例如平板电脑、笔记本电脑和台式机）来说效果很好，但在小屏幕上，例如纵向模式的智能手机上，可能会出现问题。为了理解我的意思，请查看图 12.14，这是本章的文章页面在智能手机上的显示。特别注意，两列都很窄，这使得文本难以阅读。

![图片](img/build-a-website-with-chatgpt-CH12_F14_McFedries3.png)

图 12.14 在智能手机屏幕上，文本列可能会变得太窄，难以舒适阅读。

这可能看起来像是一个无法解决的问题，但使用 CSS 你可以创建一个所谓的*自适应布局*，这是一种根据设备屏幕的某些特性（如宽度）改变其属性的布局。通过自适应布局，你可以通过询问浏览器视口（浏览器窗口中显示网页的部分）的宽度来解决问题，如图 12.14 所示。

例如，您可能会问：“视口宽度小于 500 像素吗？”如果答案是“否”，则保持布局不变；如果答案是“是”，您可以告诉浏览器将文章显示为单列，其中`aside`元素位于`article`元素之后，但两者都占据整个屏幕宽度。

您可以通过在 CSS 中定义媒体查询来提出这些以及其他许多类型的问题。一个*媒体查询*是一个表达式，后面跟着一个包含一个或多个样式规则的代码块。该表达式询问屏幕的某些特性，例如其宽度。如果该表达式对当前设备为真，则浏览器应用媒体查询的样式规则；如果表达式为假，则浏览器忽略媒体查询的规则。

媒体查询的一般语法如下：

```py
@media (*expression*) { 
    *Rules to apply if* expression *is true go here*
}
```

`expression`通常为`min-width`或`max-width`，后面跟一个冒号和一个值。例如，如果您想要在屏幕宽度不超过指定值的情况下应用样式，请使用`max-width`。以下代码告诉浏览器，当屏幕宽度小于或等于 500 px 时，将`main`元素显示为单列网格：

```py
@media (max-width: 500px) {
    main {
        display: grid;
        grid-template-columns: 1fr;
    }
}
```

要让 ChatGPT 在您的 CSS 代码中包含媒体查询，您可以在提示中包含如下指令：

```py
For screens with width less than or equal to 500px, make the main element a one-column grid.
```

类似地，如果您想要在屏幕宽度至少等于指定值的情况下应用样式，请使用`min-width`。以下代码在屏幕宽度大于或等于 1,024 px 时设置`h1`元素的字体大小：

```py
@media (min-width: 1024px) {
    h1 {
        font-size: 72px;
    }
}
```

要让 ChatGPT 在您的 CSS 代码中包含此媒体查询，您可以在提示中包含如下指令：

```py
For screens with width greater than or equal to 1024px, make the h1 element font size 72px.
```

之后，在我向您展示最终的文章页面布局（参见图 12.16）之后，我还会向您展示页面在智能手机上的显示方式（图 12.17），以验证页面确实通过切换到单列布局来适应较小的屏幕。

现在您已经知道如何提示 ChatGPT 构建文章页面，如以下章节所述。

### 12.2.10 为文章页面制作提示

本章的项目是一个显示文学作品中某个地方旅行指南的文章页面。在继续之前，我假设您已经准备好了以下内容：

+   头部内容，例如网站标志、标题和标语

+   您想要用于标题和文本的 Google Fonts 字体样式

+   您想要用于页面背景和文本的颜色关键词

参考第三章以了解更多关于这些设计元素的信息，以及如何提示 ChatGPT 获取标题、字体和颜色建议。

要开始您的提示，告诉 ChatGPT 您想要构建一个网页，并且希望它为您生成代码：

```py
I want to build a web page for an article. I don't know how to code, so I need you to provide the code for me.

First, write the HTML code for a web page that includes the following:
```

现在逐项检查页面内容，包括以下内容（参见图 12.15）：

+   包含您的网站标志、标题和标语的头像

+   包含指向网站其他区域的链接的导航元素

+   包含一个`article`元素和一个`aside`元素，这两个元素排列在两列中的主元素

+   包含版权声明的页脚

![图片](img/build-a-website-with-chatgpt-CH12_F15_McFedries3.png)

图 12.15 文章页面的部分

注意，在这个项目中，你不会在你的提示中包含页面内容——即构成文章的章节和段落以及构成侧边的段落。相反，一旦你有了图 12.15 所示的页面骨架，你将手动添加内容，正如我在第 12.3 节中解释的那样。

接下来，要求 ChatGPT 生成 CSS：

```py
Second, in a separate file please write the CSS code for the following:
```

然后你指定页面格式，包括以下内容：

+   页面背景颜色和文本颜色

+   你想要用于标题和页面文本的字体大小

+   用于标题和常规页面文本的字体

+   布局应使用 CSS Grid

+   布局应适应较小的屏幕

这里是一个为我自己的文章页面提供的示例提示：

```py
I want to build a web page for an article. I don't know how to code, so I need you to provide the code for me.

First, write the HTML code for a web page that includes the following:
 * A header element that includes an image named logo.png, which is stored in the "images" subdirectory, the site title "Dream Vacations" and the site tagline "Travel guides to imaginary places".
 * A navigation element that includes the following links:
  * Home (links to index.xhtml)
  * Sci-Fi (links to sci-fi.xhtml)
  * Fantasy (links to fantasy.xhtml)
  * Children's (links to childrens.xhtml)
  * Literary (links to literary.xhtml)
 * A main section that contains an article element and an aside element.
 * The article element title is the second-level heading "Travel Guide to Narnia".
 * The aside element title is the third-level heading "Related Guides".
 * A footer element that includes the Copyright symbol, followed by "Dream Vacations, LLC".
 * In the page head section, include the tag <meta charset="utf-8">.
 * In the page head section, include the tag <meta name="viewport" content="width=device-width, initial-scale=1">.

Second, in a separate file write the CSS code for the following:
 * The page text uses font size 20px and the Baskerville font from Google Fonts.
 * The header has background color lightblue and 24px padding.
 * The site title is 64px and uses the Raleway font from Google Fonts.
 * The site tagline is 32px and uses the Raleway font from Google Fonts.
 * The second-level heading is 36px and uses the Raleway font from Google Fonts.
 * The third-level headings are 24px and use the Raleway font from Google Fonts.
 * The article title and the aside title have a 10px top margin.
 * The aside has a 1px, solid, lightblue border.
 * The nav, article, aside, and footer elements have 10px padding.
 * The footer has a 1px, lightblue top border and a 10px top margin.
 * The page has a maximum width of 800px and is centered within the browser window.
 * Style all links with color midnightblue and no underline.
 * Lay out the page as follows:
  * The header is a two-column CSS Grid container with the logo in the left column and the site title and tagline in the right column.
  * The navigation bar is a row Flexbox container.
  * The main element is a two-column CSS Grid container; the article element column is twice the width of the aside element column; there is a gap of 10px between the columns.
 * For screens with width less than or equal to 500px, do the following:
  * Convert each two-column grid into a one-column grid.
  * Make the site title 40px and the site tagline 24px.
  * Give the site logo a maximum width of 150px.
  * Center the header content.
```

我使用 Copilot 的精确模式提交了我的提示。生成的代码生成了图 12.16 所示的页面。

![图片](img/build-a-website-with-chatgpt-CH12_F16_McFedries3.png)

图 12.16 添加内容前的我的文章页面

图 12.16 显示了在桌面显示器上的页面外观。为了检查提示中的媒体查询是否正常工作，你需要使用智能手机浏览器加载页面，如图 12.17 所示。在这种情况下，媒体查询已按以下方式调整页面：

+   现在的页眉是一个一列的网格容器。

+   网站标志的最大尺寸已被减小。

+   网站标题和标语标签的字体大小已被减小。

+   主元素现在是一个一列的网格容器。

![图片](img/build-a-website-with-chatgpt-CH12_F17_McFedries3.png)

图 12.17 通过媒体查询将文章骨架调整为智能手机屏幕

将骨架文章页面的代码复制到你的文本编辑器后，你的下一个任务是填写缺失的内容。

## 12.3 向页面添加内容

ChatGPT 生成的 HTML 代码包括基本的页面标签和文本，但它缺少最重要的部分：`article`和`aside`元素的内容。为了完成你的页面，你需要将 index.xhtml 加载到你的文本编辑器中，然后手动添加内容。

首先，为了添加你的文章内容，检查 HTML 代码以查找以下标签：

```py
<article>
    <h2>Travel Guide to Narnia</h2>
    <!-- Article content goes here -->
</article>
```

这里的关键行是`<!-- Article content goes here -->`，这是文章内容的占位符。（标签`<!--`和`-->`创建了一个*注释*，这是描述 HTML 代码的文本，但在浏览器中显示页面时不会出现。）你将在该行下方输入你的内容。在大多数情况下，你将添加以下内容：

+   在文章标题（`h2`元素）下方的一组`<p>`和`</p>`标签以及你的文章介绍在这些标签之间的文本。根据需要，你可以添加两个或更多这样的段落。

+   在引言段落（或段落）之后，添加一个或多个`section`元素，每个元素都有一个三级（`h3`）标题，后面跟着一个或多个段落（每个段落都位于一对`<p>`和`</p>`标签之间）。

一旦你的文章完成，添加你的侧边栏内容。首先，检查 HTML 代码以查找以下标签：

```py
<aside>
    <h3>Related Guides</h3>
    <!-- Related guides go here -->
</aside>
```

再次强调，这里的重要行是`<!—相关指南放在这里 -->`（你的文本将根据你在提示中使用的标题而有所不同）。这一行是`aside`内容的占位符。你可以在该行下方输入你的内容，你的内容可能是一系列段落、链接列表或其他与文章相关的信息。根据需要，你可以自由添加新的`h3`元素。图 12.18 显示了添加了内容的文章页面的顶部部分。

![](img/build-a-website-with-chatgpt-CH12_F18_McFedries3.png)

图 12.18 我的文章页面，现在已添加了内容

如果你对自己的文章页面满意，你可能更喜欢跳过本章的其余部分，并将你的页面部署到网络上（如附录 B 中所述）。如果你想了解更多关于文章页面代码的信息，请继续阅读。

## 12.4 检查文章页面代码

下一两个部分提供了对之前在图 12.16 和 12.17 中显示的文章骨架页面的 HTML 和 CSS 代码的注释指南。我将在下一节中从 HTML 代码开始。 

注意：我文章页面的生成的 HTML 和 CSS 代码可在本书的网站上找到（[www.manning.com/books/build-a-website-with-chatgpt](https://www.manning.com/books/build-a-website-with-chatgpt)）以及本书的 GitHub 仓库中：[`github.com/paulmcfe/websites-with-chatgpt`](https://github.com/paulmcfe/websites-with-chatgpt)。

### 12.4.1 检查 HTML

这里是 ChatGPT 为我文章页面生成的 HTML 代码的注释版本：

```py
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <meta name="viewport"                                     ①
          content="width=device-width, initial-scale=1">      ①
    <title>Dream Vacations</title>
    <link rel="stylesheet" type="text/css" href="styles.css"> ②
</head>
<body>
    <header>                                                  ③
        <img src="images/logo.png" alt="Logo">                ③④
        <div>                                                 ③
            <h1>Dream Vacations</h1>                          ③⑤
            <p>Travel guides to imaginary places</p>          ③⑥
        </div>                                                ③
    </header>                                                 ③
    <nav>                                                     ⑦
        <a href="index.xhtml">Home</a>                         ⑦
        <a href="sci-fi.xhtml">Sci-Fi</a>                      ⑦
        <a href="fantasy.xhtml">Fantasy</a>                    ⑦
        <a href="childrens.xhtml">Children's</a>               ⑦
        <a href="literary.xhtml">Literary</a>                  ⑦
    </nav>                                                    ⑦
    <main>                                                    ⑧
        <article>                                             ⑧⑨
            <h2>Travel Guide to Narnia</h2>                   ⑧⑨⑩
            <!-- Article content goes here -->                ⑧⑨⑪
        </article>                                            ⑧⑨
        <aside>                                               ⑧⑫
            <h3>Related Guides</h3>                           ⑧⑫⑬
            <!-- Related guides go here -->                   ⑧⑫⑭
        </aside>                                              ⑧⑫
    </main>                                                   ⑧
    <footer>                                                  ⑮
        © Dream Vacations, LLC                                ⑮
    </footer>                                                 ⑮
</body>
</html>
```

① 帮助页面在移动设备上正确显示

② 告诉网络浏览器在哪里找到 CSS 代码

③ 页面标题

④ 网站标志

⑤ 网站标题

⑥ 网站标语

⑦ 导航栏

⑧ 主元素

⑨ 文章元素

⑩ 文章标题

⑪ 文章内容占位符

⑫ 侧边栏元素

⑬ 侧边栏标题

⑭ 侧边栏内容占位符

⑮ 页脚

注意，HTML 代码中包含以下行：

```py
<link rel="stylesheet" href="styles.css">
```

这个标签告诉网络浏览器在哪里找到 CSS 代码，我将在下一节中描述。

### 12.4.2 检查 CSS

这里是 ChatGPT 为我文章页面生成的 CSS 代码的注释版本：

```py
@import url('https://fonts.googleapis.com/css2?family=         ①
➥Baskerville:wght@400&family=Raleway:wght@400&display=swap'); ①

body {
    font-size: 20px;                                           ②
    font-family: 'Baskerville', serif;                         ②
    max-width: 960px;                                          ②
    margin: 0 auto;                                            ②
}

header {
    display: grid;                                             ③
    grid-template-columns: auto 1fr;                           ③
    background-color: lightblue;                               ④
    padding: 24px;                                             ④
}

header h1 {
    font-size: 64px;                                           ⑤
    font-family: 'Raleway', sans-serif;                        ⑤
}

header p {
    font-size: 32px;                                           ⑥
    font-family: 'Raleway', sans-serif;                        ⑥
}

nav {
    display: flex;                                             ⑦
    justify-content: space-between;                            ⑦
}

a {
    color: midnightblue;                                       ⑧
    text-decoration: none;                                     ⑧
}

main {
    display: grid;                                             ⑨
    grid-template-columns: 2fr 1fr;                            ⑨
    gap: 10px;                                                 ⑨
}

article h2, aside h3 {
    margin-top: 10px;                                          ⑩
}

aside {
    border: 1px solid lightblue;                               ⑪
}

nav, article, aside, footer {
    padding: 10px;                                             ⑫
}

h2 {
    font-size: 36px;                                           ⑬
    font-family: 'Raleway', sans-serif;                        ⑬
}

h3 {
    font-size: 24px;                                           ⑭
    font-family: 'Raleway', sans-serif;                        ⑭
}

footer {
    border-top: 1px solid lightblue;                           ⑮
    margin-top: 10px;                                          ⑮
}

@media (max-width: 500px) {                                    ⑯
    header {                                                   ⑯
        grid-template-columns: 1fr;                            ⑯
        text-align: center;                                    ⑯
    }                                                          ⑯
                                                               ⑯
    header img {                                               ⑯
        max-width: 150px;                                      ⑯
        margin-left: auto;                                     ⑯
        margin-right: auto;                                    ⑯
        display: block;                                        ⑯
    }                                                          ⑯
                                                               ⑯
    header h1 {                                                ⑯
        font-size: 32px;                                       ⑯
    }                                                          ⑯
                                                               ⑯
    header p {                                                 ⑯
        font-size: 24px;                                       ⑯
    }                                                          ⑯
                                                               ⑯
    main {                                                     ⑯
        grid-template-columns: 1fr;                            ⑯
}                                                              ⑯
```

① 从 Google Fonts 导入 Baskerville 和 Raleway 字体

② 样式化文本大小和字体，设置最大宽度，并居中页面

③ 设置标题为两列网格

④ 样式化标题背景颜色和填充

⑤ 样式化网站标题的字体大小和字体

⑥ 样式化网站标语字体大小和字体

⑦ 将导航设置为具有均匀间隔项的 Flexbox 容器

⑧ 设置链接颜色并移除下划线

⑨ 将主元素设置为两列网格

⑩ 在文章和侧边栏标题上方添加边距

⑪ 为侧边栏添加边框样式

为导航、文章、侧边栏和页脚元素添加填充

⑬ 设置 h2 字体大小和字体

⑭ 设置 h3 字体大小和字体

⑮ 为页脚添加顶部边框和边距

⑯ 为宽度小于或等于 500 像素的屏幕设置媒体查询

您可以参考前两个部分中的 HTML 和 CSS 注释，以帮助您定制网页代码，正如我在下一节中描述的那样。

## 12.5 定制文章页面

下面是一些针对 HTML 代码的定制建议：

+   如果您希望侧边栏在左侧，您需要同时更改 HTML 和 CSS。首先，在 HTML 代码中，将 `aside` 元素移动到 `article` 元素之前：

    ```py
    <main>
        <aside>
            <h3>Related Guides</h3>
            <!-- Related guides go here -->
        </aside>
        <article>
            <h2>Travel Guide to Narnia</h2>
            <!-- Article content goes here -->
        </article>
    </main>
    ```

    第二，在 CSS 中，将 `main` 元素的 `grid-template-columns` 值从 `2fr 1fr` 更改为 `1fr 2fr`，如下所示：

    ```py
    main {
        display: grid;
        grid-template-columns: 1fr 2fr;
        gap: 10px;
    }
    ```

+   在页眉中，您可以编辑标题和标语。只需确保不要编辑或删除相关的 HTML 标签，`<h1>` 和 `</h1>` 以及 `<p>` 和 `</p>`。

+   在主要内容区域，您可以编辑文章标题，但不要修改相关的 HTML 标签，`<h2>` 和 `</h2>`。

+   在 HTML 代码的页脚部分，您可以添加指向您社交媒体账户的链接，正如我在第四章中描述的那样。

现在，这里有一些针对 CSS 代码的定制想法：

+   对于任何颜色值，您可以将现有颜色更改为不同的颜色关键字。

+   对于任何字体大小值，您可以更改数字以增加或减少字体大小。只需确保保留 `px` 单位。

+   对于任何填充或边距值，您可以更改数字以增加或减少填充或边距。在每种情况下，请确保保留 `px` 单位。

+   为了使您的页面代码更具可访问性，考虑将所有 px 测量值转换为 rem 测量值。默认情况下，1 rem 等于 16 px，因此 20 px 等于 1.25 rem，24 px 等于 1.5 rem，32 px 等于 2 rem，48 px 等于 3 rem，依此类推。rem 单位更具可访问性，因为它测量的是相对于浏览器用户在其浏览器设置中定义的默认字体大小的字体大小。

## 摘要

+   如果写作内容聚焦于单一主题并且可以划分为多个子主题，请使用文章布局。

+   主要的 HTML 页面布局元素包括 `header`、`nav`、`main`、`article`、`aside`、`footer` 和 `p`。

+   使用 `article` 元素标记一个完整、自包含的组成，类似于报纸或杂志文章。此元素也可以应用于评论、博客条目、论坛帖子或论文。

+   使用 `aside` 元素标记包含与页面独特内容间接相关的内容的页面侧边栏区域，例如相关网站页面的链接列表、最新网站新闻、社交媒体源或广告。

+   使用 `strong` 元素标记重要文本，使用 `b` 元素标记关键词，使用 `em` 元素为文本添加强调，并使用 `i` 元素标记替代文本。

+   使用 CSS 网格在二维空间中布局页面。

+   为了获得最佳效果，您的页面提示应尽可能具体，包括颜色、字体大小和标题级别。

+   将生成的 HTML 保存到 index.xhtml 文件，将生成的 CSS 保存到 ChatGPT 在 HTML 代码中建议的文件名，通常是 styles.css。

# 13 编写交互式课程目录

本章涵盖

+   准备 Excel 数据以便在网页上使用

+   了解 JSON 数据格式

+   使用 ChatGPT 将 Excel 数据转换为 JSON

+   使用 JSON 数据使网页交互式

+   为课程目录页面制作 ChatGPT 提示

+   检查和自定义 ChatGPT 生成的代码

本书迄今为止看到的这些项目已经产生了有用且相当吸引人的网页。然而，您可能已经注意到一个共同点，那就是您使用 ChatGPT 帮助构建的页面：没错，它们只是静静地在那里。当然，如果页面提供有用、信息丰富或有趣的信息，那么一个不做很多事情的页面并没有什么问题。然而，如果页面以某种方式是交互式的，这真的可以增加页面的吸引力。在这里，“交互式”的意思是读者可以操作页面来更改显示的数据。例如，在一个包含大量数据的页面上，您可能包括允许用户仅显示数据子集或搜索数据的控件。

在本章中，您首先学习如何在无需配置 Web 服务器的情况下将数据放入网页，这是一个令人厌恶的复杂任务，您会庆幸自己可以跳过。特别是，本章向您展示了如何从 Excel 文件中提取数据并将其转换为可以加载到页面上的格式。示例数据是一组大学课程，目标是创建一个允许访客搜索、排序和筛选这些数据的页面。然后，您将所有这些应用到创建一个详细的提示，以便 ChatGPT 生成课程目录网页的代码。

本章提供了 ChatGPT 生成的 HTML、CSS 和 JavaScript 的注释版本，以帮助您理解课程目录的工作原理。您还可以获得一些有用的提示，以自定义代码。

## 13.1 检查本章的项目

正如我在引言中提到的，本章的项目是一个虚构大学的单页课程目录。最终页面将包括以下组件：

+   包含网站标志和标题的页眉元素

+   以过滤、排序和搜索目录的控件开始的主体元素

+   对于每门课程，一个垂直元素——有时称为*tile*——用于显示课程图片、标题、ID、讲师、系、学期和描述

+   包含版权声明的页脚元素

图 13.1 展示了使用 ChatGPT 提供的代码创建的一个示例课程目录。示例页面是一系列瓷砖，每个瓷砖都包含一个大学课程的信息，这种布局可以用于其他类型的内容，如产品目录、可用服务列表、客户订单或几乎任何类型的有结构化数据。在这些项目中，共同点是原始的网页数据最初存储在一个 Excel 电子表格文件中，因此你需要知道如何将数据从 Excel 转换为网页浏览器可以理解的形式。

![图片](img/build-a-website-with-chatgpt-CH13_F01_McFedries3.png)

图 13.1 ChatGPT 生成的课程目录

## 13.2 从 Excel 获取数据

当你想要在网页上展示数据时，最常见的问题之一就是数据格式与网页不兼容。这些数据可能存在于文字处理文档中的表格、演示文稿、文本文件中的文本，或者笔记应用中散乱的笔记。在这个项目中，我假设数据存储在一个 Excel 文件中，而准备这些数据是下一节的主题。

### 13.2.1 准备你的 Excel 数据

由于 Excel 对大多数人来说都很熟悉，数据录入相对简单，且工作表的行和列格式与大多数数据所需的行和列格式相匹配，因此 Excel 是满足轻量级数据库需求的一个非常常见应用。要在网页上使用 Excel 数据，你需要将其转换为合适的格式。我很快就会介绍这种转换，但首先，你需要确保你的 Excel 数据已经准备好。在这里，“准备好”意味着 Excel 数据必须是以下特征之一：

+   数据是一个范围，或者是一个已转换为表格的范围。

+   如果数据是一个范围（即，不是一个表格），以下条件之一必须成立：

    +   工作表上没有其他数据。

    +   数据位于一个命名范围内。

+   数据的每一列都有一个独特的标题。

图 13.2 展示了本项目作为示例将使用的 Excel 数据。这些数据是大学课程的集合，并为每个课程存储以下信息：

+   课程 ID

+   课程标题

+   课程描述

+   课程讲师的姓名

+   提供该课程的系名

+   提供该课程的学期

数据位于一个常规的 Excel 范围内；工作表中没有其他数据，并且每一列都有一个独特的标题。

在你学习如何将此类 Excel 数据转换为可用格式之前，你需要了解该格式，这是下一节的主题。

![图片](img/build-a-website-with-chatgpt-CH13_F02_McFedries3.png)

图 13.2 本项目将使用的 Excel 数据

### 13.2.2 了解 JSON 数据格式

您将在本章后面看到，驱动数据驱动的网页的是 JavaScript，它可以抓取文件的内容，处理文件包含的数据，在网页上显示这些数据，并允许您设置控件以执行搜索、筛选和其他数据操作。所有这一切的起点是 JavaScript 读取的文件。JavaScript 可以处理多种文件类型，但对我们来说最容易和最方便的是 JSON（JavaScript 对象表示法）格式。JSON（发音类似于名字 *Jason*）是网页上处理数据最常见的方式之一。

JSON 之所以如此受欢迎的主要原因之一是数据是纯文本，因此可以使用普通的文本或代码编辑器创建和编辑它。在接下来的两个部分中，您将学习如何说服 ChatGPT 自动从 Excel 文件创建 JSON 数据，这样您就不需要在这个项目中直接处理 JSON 代码。然而，如果您想了解如何直接处理 JSON 数据，本节的其余部分提供了详细信息。

正如我提到的，JSON 数据是纯文本。然而，该文本必须使用正确的 JSON 语法进行配置。以下是对 JSON 数据语法的总体概述：

```py
{
    "*property1*": *value1*,
    "*property2*": *value2*,
    ...
    "*propertyX*": *valueX*
}
```

您这里有一组一个或多个属性-值对。对于这个项目，属性-值对来自原始 Excel 数据，如下所示：

+   每个属性的名称来自 Excel 数据范围内的列标题。

+   分配给属性的值来自 Excel 范围内的单行。

+   每个属性名称被双引号（`"`）包围。

+   每个值通常是一个被双引号包围的字符串，但它也可以是一个数字或任何其他 JavaScript 数据类型。

+   属性-值对由逗号分隔。

+   属性-值对的块被大括号（`{` 和 `}`）包围。

这里有一些示例 JSON 数据，对应于图 13.2 中较早显示的 Excel 数据的第一个行。

```py
{
    "Course ID": "AI101",
    "Title": "The Art of Chatting: Building Conversational AIs",
    "Description": "Dive into the quirky world of chatbots and virtual companions. Learn how to design AIs that can outwit humans in a battle of banter, negotiate pizza toppings, and philosophically ponder the existence of the internet.",
    "Instructor": "Prof. Kaitlyn Wong",
    "Department": "Artificial Intelligence",
    "Semester": 1
}
```

这只是原始 Excel 范围内的单行。对于有多个行的范围，ChatGPT 将生成一个 JSON 对象的数组：每个 JSON 对象由逗号分隔，整个数据集被方括号（`[` 和 `]`）包围。以下是一个部分示例：

```py
[
    {
        "Course ID": "AI101",
        "Title": "The Art of Chatting: Building Conversational AIs",
        "Description": "Dive into the quirky world of chatbots and virtual companions. Learn how to design AIs that can outwit humans in a battle of banter, negotiate pizza toppings, and philosophically ponder the existence of the internet.",
        "Instructor": "Prof. Kaitlyn Wong",
        "Department": "Artificial Intelligence",
        "Semester": 1
    },
    {
        "Course ID": "AI102",
        "Title": "Robot Overlords 101: An Introduction to AI Ethics",
        "Description": "Explore the moral dilemmas of our future robot overlords. From deciding who gets the last piece of cake to governing a small island, this course tackles the hard ethical questions.",
        "Instructor": "Prof. Thiago Silva",
        "Department": "Artificial Intelligence",
        "Semester": 2
    },
    {
        "Course ID": "AI103",
        "Title": "Dreaming in Code: AI for Creative Minds",
        "Description": "Unleash the power of AI to create art, music, and literature. Learn how algorithms can be inspired by dreams and how to interpret the surreal artworks produced by silicon brains.",
        "Instructor": "Prof. Anika Singh",
        "Department": "Artificial Intelligence",
        "Semester": 3
    },
...
    {
        "Course ID": "AI402",
        "Title": "Ghost in the Machine: AI and Paranormal Research",
        "Description": "Investigate the uncanny valley with AI. Learn how artificial intelligence is used to explore paranormal activities, communicate with spirits, and debunk or prove age-old myths.",
        "Instructor": "Prof. Sven Eriksson",
        "Department": "Artificial Intelligence",
        "Semester": 1
    }
]
```

当然，ChatGPT 需要一些数据来工作，因此上传您的 Excel 数据是下一节的主题。

### 13.2.3 将您的 Excel 文件上传到 ChatGPT

将您的 Excel 数据转换为 JSON 格式的第一步是将 Excel 电子表格文件上传到 ChatGPT。

注意：在我写这篇文章的时候，上传文件的功能仅限于 ChatGPT Plus 订阅者。

这里是您需要遵循的步骤：

1. 登录您的 ChatGPT Plus 账户。

2. 启动一个新的 ChatGPT 4 聊天会话。

3. 在消息文本框的左侧，单击附件图标（回形针；参见图 13.3）以显示打开对话框。

![](img/build-a-website-with-chatgpt-CH13_F03_McFedries3.png)

图 13.3 点击“附件文件”（回形针图标）上传您的 Excel 文件。

4. 定位并选择包含您想要转换的数据的 Excel 文件。

5. 点击“打开”。ChatGPT 上传文件，并在您的聊天中显示文件图标，如图 13.4 所示。

![](img/build-a-website-with-chatgpt-CH13_F04_McFedries3.png)

图 13.4 上传的 Excel 文件在聊天记录中显示为图标。

将您的 Excel 文件附加到聊天中后，您就可以提示 ChatGPT 将数据转换为 JSON 格式。

### 13.2.4 使用提示将 ChatGPT 的 Excel 数据转换为 JSON

ChatGPT——至少，您通过 ChatGPT Plus 订阅获得的聊天机器人版本——具有优秀且强大的数据处理能力。这些包括

+   从 Excel 电子表格文件中提取数据

+   将这些数据转换为 JSON 格式

+   将转换后的数据写入 JSON 文件（使用.json 文件扩展名）

与所有 ChatGPT 功能一样，您使用提示来启用这些功能。当您准备好编写提示时，请注意有几个常见的场景需要考虑：

+   *您想要转换为 JSON 的 Excel 数据位于命名范围或命名表中。* 在这种情况下，您可以在提示中使用范围或表名：

    ```py
    In the uploaded Excel file, please convert the range named "Crypto" to JSON format and output the result as a JSON file.
    ```

+   *Excel 文件包含单个工作表，并且该工作表中除了您想要转换为 JSON 的数据范围之外没有其他内容。* 在这种情况下，以下类似的提示应该可以解决问题：

    ```py
    In the uploaded Excel file, please convert the range to JSON format and output the result as a JSON file.
    ```

    这是您可以使用本章示例文件中的示例 Excel 文件的提示。

+   *Excel 文件包含多个工作表，但您想要转换的范围位于第一个工作表中。* 当您没有指定工作表时，ChatGPT 会自动转换第一个工作表中的范围，因此您可以使用以下类似的提示：

    ```py
    In the uploaded Excel file, please convert the range to JSON format and output the result as a JSON file.
    ```

+   *Excel 文件包含多个工作表，而您的范围不在第一个工作表中。* 在这种情况下，您的提示需要指定包含您数据的工作表名称：

    ```py
    In the uploaded Excel file, please convert the range in the worksheet named "My Data" to JSON format and output the result as a JSON file.
    ```

当您提交提示时，ChatGPT 开始分析 Excel 文件，提取数据，并将数据转换为 JSON 格式。当这项工作完成后，ChatGPT 会通知您并提供下载结果的 JSON 文件的链接，如图 13.5 所示。点击链接将 JSON 文件下载到您的计算机。

![](img/build-a-website-with-chatgpt-CH13_F05_McFedries3.png)

图 13.5 当 ChatGPT 将您的 Excel 数据转换为 JSON 后，它会提供一个下载 JSON 文件的链接。

在此阶段，快速查看下载的 JSON 文件以确保 ChatGPT 正确处理数据是个好主意。双击文件将其加载到您计算机上默认的该文件类型应用程序中。您应该看到您的数据以 JSON 格式显示；图 13.6 显示了示例。

![](img/build-a-website-with-chatgpt-CH13_F06_McFedries3.png)

图 13.6 在确保 ChatGPT 正确处理数据之前，查看您的 JSON 数据是个好主意。

如果 JSON 文件包含错误数据，最可能的问题是 ChatGPT 处理了你的 Excel 文件中的错误范围。创建一个新的提示，使用更具体的标识信息来描述数据，例如工作表名称或范围或表名称。如果这不起作用，请在 Excel 中打开电子表格文件，为范围定义一个名称，然后将修订后的 Excel 文件上传到 ChatGPT 聊天，然后编写一个引用你定义的范围名称的提示。一旦你有了你的 JSON 数据文件，就是时候学习如何提取这些数据并在你要创建的网页上显示它们了。

## 13.3 获取并显示 JSON 数据

目前你有一个 JSON 文件，稍后你将有一个由 ChatGPT 创建的网页。你如何将 JSON 数据放到那个网页上？这是一个 JavaScript 任务，所以当你要提示 ChatGPT 为你的网页 JavaScript 代码时，你开始以下请求：

```py
Fetch the contents of the file *filename*.
```

这告诉 ChatGPT 生成代码，提取名为 *`filename`* 的文件中的内容。例如，对于这个项目的 `college_courses.json` 文件，提示将看起来像这样：

```py
Fetch the contents of the file college_courses.json.
```

注意：提取文件内容的 JavaScript 方法称为 `fetch`，所以在请求中使用动词 *fetch* 是故意的。

生成的 JavaScript 代码将所有 JSON 数据加载到内存中，所以下一步是要求 ChatGPT 生成将数据写入网页的 JavaScript 代码。例如，假设你的网页代码包括一个空的 `article` 元素，你希望所有数据都显示在该元素中。一个常见的场景是将数据中的每个记录显示为一个单独的 `section` 元素。所以，你的提示将开始如下：

```py
For each record fetched from the JSON file, add a section element to the article element and populate the section element with the following:
```

你将指定你想要用于显示数据的元素。例如，如果你有一个记录的标题，你可以使用三级标题。同样，如果你有一个长文本项，你可能使用段落元素。

这是本章项目的提示：

```py
For each record fetched from the JSON file, add a section 
element to the article element and populate the section 
element with the following three elements:
 * A third-level heading that includes the record's "Title" text.
 * A div element with the text "Course ID: ", the record's "Course ID" value, a line break, the text "Instructor: ", the record's "Instructor" value, a line break, the text "Department: ", the record's "Department" value, a line break, the text "Semester: ", the record's "Semester" value, and a line break.
 * A paragraph element that includes the record's "Description" value.
```

生成的 JavaScript 代码将遍历所有检索到的 JSON 记录，并将它们中的每一个写入页面。

一旦你获取并显示了你的 JSON 数据，就是时候学习如何在你要创建的网页上操作所有这些数据了。

## 13.4 搜索、排序和过滤课程目录

完全有可能你只想在网页上显示你的 JSON 数据，然后就这样。这可能是在你的数据库相对较小的情况下，比如说几十项或更少的情况。但如果你的数据由几十、几百甚至几千条记录组成，只是简单地将所有这些信息扔到网页上是不够的。为什么？因为这对试图查看它的人来说，几乎不可能有用，而且很可能令人沮丧。

如果你有很多数据，你需要对你的访客表示同情，提供以下一种或多种方式来操作数据：搜索、排序和过滤。接下来的三个部分将详细介绍这些内容。

### 13.4.1 搜索数据

在搜索时，用户输入一个或多个单词或短语来表示他们想要查看的数据。提交搜索文本后，整个数据库将仅替换为包含与搜索词或短语匹配的文本的记录。

网页搜索组件几乎总是包含一个文本框。因此，在你的 ChatGPT 提示中请求 HTML 代码时，你需要包括这样的文本框。以下是一个示例：

```py
A text box with the ID "Search" and the placeholder "Search".
```

在这里，一个占位符是一个出现在文本框中的单词或短语，用来告知用户他们应该输入什么。一旦用户开始在框中输入文本，占位符就会消失。请注意，为组件包含 ID 值可以使 JavaScript 代码更容易阅读。

当你提示 ChatGPT 生成 JavaScript 代码时，你需要包括你想要代码如何处理搜索文本。通常，你会要求 JavaScript 监控搜索字段，并在用户开始输入时，用仅匹配输入文本的记录替换显示的 JSON 记录。以下是一个示例提示：

```py
When the user types text in the "Search" text box, 
repopulate the article element with just the records 
that include the search text in any field.
```

此示例假设你想要将搜索文本应用于你的 JSON 数据中的每个字段。你可能需要考虑一些例外情况：

+   如果有字段你不想包含在搜索中（例如包含数字数据的字段），请在提示的末尾添加`except the` *`X`* `and` *`Y`* `fields`（其中*`X`*和*`Y`*是你想要排除的字段的名称）。

+   如果你只想将搜索应用于一个或多个字段，请在提示中将`any field`替换为`the` *`A`* `and` *`B`* `fields`（其中*`A`*和*`B`*是你想要搜索的字段的名称）。

搜索可能是最常见（并且可以说是最有用）的数据操作功能，但你还需要了解另外两个功能，第一个是过滤。

### 13.4.2 过滤数据

使用过滤，用户可以通过选择特定字段中出现的唯一值之一来显示 JSON 数据的子集。例如，在本章的项目中，用户可以根据`Department`和`Instructor`字段中的唯一值过滤课程数据。

网页过滤组件通常是一个包含特定字段唯一项的下拉列表，因此在你请求 HTML 代码的提示中，你需要要求这样的组件。以下是本章项目中使用的两个提示：

```py
A drop-down list with the ID "Department" and the initial value "Department (All)".
A drop-down list with the ID "Instructor" and the initial value "Instructor (All)".
```

注意，提示为每个列表应用 ID 值，并为每个列表填充一个初始值。在这两种情况下，从列表中选择此初始值将重新填充网页，以包含完整数据库。

当你要求 ChatGPT 生成你的 JavaScript 代码时，首先需要包括你想要你的下拉列表由对应数据字段中的唯一值填充。例如，以下是一个用`Department`字段中的唯一值填充`Department`下拉列表的提示：

```py
Extract all the unique "Department" values and use them to populate the "Department" drop-down list.
```

接下来，你指定代码如何处理用户从列表中选择一个项。一般思路是 JavaScript 监视列表，当用户选择一个项时，代码将显示的 JSON 记录替换为仅匹配所选列表项的记录。以下是针对 `Department` 字段的示例提示：

```py
When the user selects an item from the "Department" list, repopulate the article element with just the records that match the selected department. If the user selects the first item in the list, repopulate the article element with every record imported from the JSON file.
```

最终的数据处理技术是排序，这将在下一节中介绍。

### 13.4.3 排序数据

通过排序，用户可以控制显示记录的顺序，通常是通过以某种方式指定一个字段。然后页面将记录按字母顺序（如果字段包含文本）或按数字顺序（如果字段包含数字）重新排序。在这个项目中，用户可以在 `Department` 和 `Title` 字段上对课程目录进行排序。

网页排序组件通常是一个包含可排序字段名称的下拉列表。当你要求 ChatGPT 生成你网页的 HTML 代码时，你需要请求这样一个组件。以下是本章项目的一个示例：

```py
A drop-down list with the ID "Sort" and the values: "Sort by Department" and "Sort by Title".
```

当你要求 ChatGPT 生成 JavaScript 代码时，你需要包括你希望代码如何处理用户从该列表中选择一个项的情况。一般思路是 JavaScript 确定哪个项被选中，根据该字段对记录进行排序，然后将在页面上重新显示排序后的记录。以下是我们的项目中的一个示例提示：

```py
When the user selects "Sort by Title" from the "Sort" list, sort the displayed records on the "Title" field and then repopulate the article element with the sorted records. When the user selects "Sort by Department" from the "Sort" list, sort the displayed records on the "Department" field and then repopulate the article element with the sorted records.
```

到目前为止，你已经知道了成功提示 ChatGPT 构建课程目录所需的所有内容。下一节将带你了解这个过程。

## 13.5 为课程目录构建提示

本章的项目是一个课程目录页面，它从单独的 JSON 文件中获取并显示所有数据。该页面包括用于过滤、排序和搜索数据的控件。该项目假设你已经有一个标题、副标题和标志；知道你想要用于页面标题和文本的字体；并且已经准备好要应用的颜色方案。回到第三章学习如何请求 ChatGPT 提供标题、字体和颜色建议。

要开始你的提示，告诉 ChatGPT 你想要构建一个网页，并且你希望它为你生成代码：

```py
I want to build a web page for a course catalog. I don't know how to code, so I need you to provide the code for me.

First, write the HTML code for a web page that includes the following:
```

现在逐项概述页面内容，包括以下内容（参见图 13.7）：

+   一个包含左侧图片、右侧标志和中间标题和副标题的页眉

+   一个包含两个用于过滤的下拉列表、一个用于排序的下拉列表和一个用于搜索的文本框的导航元素

+   一个包含一个空 `article` 元素的主体元素

+   包含版权声明的页脚

![](img/build-a-website-with-chatgpt-CH13_F07_McFedries3.png)

图 13.7 在数据渲染之前课程目录页面的元素

图 13.7 没有显示数据，因为，正如我即将讨论的，空的 `article` 元素仅通过你要求 ChatGPT 生成的 JavaScript 代码来填充。

接下来，要求 ChatGPT 生成 CSS：

```py
Second, in a separate file please write the CSS code for the following:
```

然后，你指定页面格式，包括以下内容：

+   页面背景颜色和文本颜色。

+   你想要用于标题和页面文本的字体大小。

+   用于标题和常规页面文本的字体。

+   哪些元素应该是 Flexbox 容器。在这个项目中，这些将是页眉、导航元素、文章元素以及每个部分元素。

最后，你指示 ChatGPT 提供 JavaScript 代码：

```py
Third, in a separate file, write the JavaScript code for the following:
```

然后，你详细说明你希望 JavaScript 执行的操作，包括以下内容：

+   获取 JSON 文件的内容。

+   从特定字段获取唯一值的下拉列表。

+   使用你指定的文本和 HTML 组件将所有 JSON 数据写入网页。

+   处理来自过滤下拉列表的选择。

+   处理来自排序下拉列表的选择。

+   处理搜索框中输入的文本。

我使用 OpenAI 的 ChatGPT 应用将我的提示提交给 GPT-4。生成的代码生成了图 13.8 所示的页面。

![](img/build-a-website-with-chatgpt-CH13_F08_McFedries3.png)

图 13.8 我的课程目录

如果你喜欢你的页面外观，你可以跳过本章的其余部分，并将代码部署到网络上（有关部署说明，请参阅附录 B）。然而，如果你想了解生成的网页代码，请继续阅读以获得更详细的了解。

## 13.6 检查课程目录代码

如果你想知道 ChatGPT 代表你生成的至少一些内容，接下来的三个部分为你提供了对图 13.8 所示的课程目录页面背后的 HTML 和 CSS 代码的简要了解，以及填充页面数据和处理各种数据操作控制的 JavaScript 代码。

注意：本书的网站（[www.manning.com/books/build-a-website-with-chatgpt](https://www.manning.com/books/build-a-website-with-chatgpt)）和 GitHub 存储库（[`github.com/paulmcfe/websites-with-chatgpt`](https://github.com/paulmcfe/websites-with-chatgpt)）上提供了我的课程目录的生成 HTML 和 CSS 代码。

下面的代码注释应该有助于你理解课程目录的工作原理，并使修改或自定义你自己的代码变得更加容易。

### 13.6.1 检查 HTML

这是 ChatGPT 为我生成的课程目录的 HTML 代码的注释版本：

```py
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <meta name="viewport" 
        content="width=device-width, initial-scale=1">                 ①
    <title>University of the Future</title>
    <link href="https://fonts.googleapis.com/css?family=               ②
        Roboto:400,700&display=swap" rel="stylesheet">                 ②
    <link rel="stylesheet" href="styles.css">                          ③
    <title>Ampersand Photography</title>
</head>
<body>
    <header>                                                           ④
        <img src="images/header.png" alt="Header Image">               ④⑤
        <div>                                                          ④
            <h1>University of the Future</h1>                          ④⑥
            <h2>Where tomorrow starts today</h2>                       ④⑦
        </div>                                                         ④
        <img src="images/logo.png" alt="University Logo">              ④⑧
    </header>                                                          ④
    <nav>                                                              ⑨
        <select id="Department">                                       ⑨⑩
            <option value="all">Department (All)</option>              ⑨⑩
        </select>                                                      ⑨⑩
        <select id="Instructor">                                       ⑨⑪
            <option value="all">Instructor (All)</option>              ⑨⑪
        </select>                                                      ⑨⑪
        <select id="Sort">                                             ⑨⑫
            <option value="department">Sort by Department</option>     ⑨⑫
            <option value="title">Sort by Title</option>               ⑨⑫
        </select>                                                      ⑨⑫
        <input type="text" id="Search" placeholder="Search">           ⑨⑬
    </nav>                                                             ⑨
    <main>
        <article></article>                                            ⑭
    </main>
    <footer>                                                           ⑮
        &copy; University of the Future                                ⑮
    </footer>                                                          ⑮
    <script src="script.js"></script>                                  ⑯
</body>
</html>
```

① 帮助页面在移动设备上正确显示

② 从 Google Fonts 加载 Roboto 字体

③ 告诉网页浏览器在哪里找到 CSS 代码

④ 页眉

⑤ 网站的页眉图片

⑥ 网站标题

⑦ 页面标题

⑧ 网站标志

⑨ 导航元素

⑩ 部门过滤器下拉列表

⑪ 教师过滤器下拉列表

⑫ 排序下拉列表

⑬ 搜索文本框

⑭ 空文章元素

⑮ 页脚

⑯ 告诉网页浏览器在哪里找到 JavaScript 代码

注意，HTML 代码中包含以下行：

```py
<link rel="stylesheet" href="styles.css">
```

这个标签告诉网页浏览器在哪里找到 CSS 代码，我将在下一节中描述。

### 13.6.2 检查 CSS

这是 ChatGPT 为我生成的课程目录的 CSS 代码的注释版本：

```py
body {                                 ①
    margin: 0;                         ①
    background-color: white;           ①
    font-family: 'Roboto', sans-serif; ①
    font-size: 20px;                   ①
    color: black;                      ①
}                                      ①
header {
    display: flex;                     ②
    justify-content: space-between;    ②
    align-items: center;
    max-height: 200px;
}
header img:first-of-type {
    height: 100%;                      ③
}
header img:last-of-type {
    max-height: 150px;                 ④
}
header h1 {                            ⑤
    font-size: 48px;
    text-align: center;
}    
header h2 {                            ⑥
    font-size: 28px;                   ⑥
    font-style: italic;                ⑥
    text-align: center;                ⑥
}                                      ⑥
nav {
    display: flex;                     ⑦
    flex-wrap: wrap;                   ⑦
    justify-content: space-between;    ⑦
    background-color: lightgray;
    padding: 10px;
}
article {
    display: flex;                     ⑧
    flex-wrap: wrap;                   ⑧
    gap: 20px;                         ⑧
    justify-content: flex-start;       ⑧
    margin: 20px;
}
section {
    display: flex;                     ⑨
    flex-direction: column;            ⑨
    justify-content: space-between;    ⑨
    flex-grow: 1;                      ⑨
    flex-basis: 200px;                 ⑨
    max-width: 300px;
}
h3 {
    font-size: 24px;                   ⑩
}
footer {                               ⑪
    background-color: navy;            ⑪
    padding: 24px;                     ⑪
    text-align: center;                ⑪
    color: white;                      ⑪
}                                      ⑪
```

① 样式化页面背景颜色、边距、文本大小、颜色和字体

② 样式化页眉为 Flexbox 容器

③ 左侧页眉图像占据整个页眉高度。

④ 设置右侧页眉图像的最大高度

⑤ 样式化页面标题的字体大小、样式和对齐方式

⑥ 样式化页面副标题的字体大小、样式和对齐方式

⑦ 样式化导航元素为 Flexbox 容器

⑧ 将文章元素样式设置为 Flexbox 容器

⑨ 样式化章节元素为 Flexbox 容器

⑩ 设置课程标题的字体大小

⑪ 样式化页脚

在本章前面部分提供的 HTML 代码列表中，注意以下接近底部的一行：

```py
<script src="script.js"></script>
```

这个标签告诉网络浏览器在哪里找到 JavaScript 代码，我将在下一节中对其进行注释。

### 13.6.3 检查 JavaScript

如果您小心操作，对 HTML 和 CSS 代码进行一些小的调整是可以的。然而，我强烈建议您不要修改 ChatGPT 的 JavaScript 代码。代码很复杂，不恰当的编辑可能会使课程目录无法使用。

然而，如果您知道一点 JavaScript，您可能会对 ChatGPT 如何编码获取、显示和操作 JSON 数据感兴趣，所以这里有一个 ChatGPT 为我课程目录生成的 JavaScript 代码的注释版本：

```py
document.addEventListener('DOMContentLoaded', () => {                                   ①
    fetch('college_courses.json')                                                       ②
        .then(response => response.json())
        .then(data => {
            populateDropdowns(data);                                                    ③
            populateArticles(data);                                                     ④
        });

    document.getElementById('Department')                                               ⑤
        .addEventListener('change', function() {                                        ⑤
        filterData();                                                                   ⑤
    });                                                                                 ⑤

    document.getElementById('Instructor')                                               ⑥
        .addEventListener('change', function() {                                        ⑥
        filterData();                                                                   ⑥
    });                                                                                 ⑥

    document.getElementById('Sort')                                                     ⑦
       .addEventListener('change', function() {                                         ⑦
        sortData();                                                                     ⑦
    });                                                                                 ⑦

    document.getElementById('Search')                                                   ⑧
        .addEventListener('input', function() {                                         ⑧
        searchData(this.value.trim());                                                  ⑧
    });                                                                                 ⑧
});                                                                                     ⑨

function populateDropdowns(data) {                                                      ⑩
    const departments = new Set(data.map(course => course.Department));                 ⑩
    const instructors = new Set(data.map(course => course.Instructor));                 ⑩
                                                                                        ⑩
    departments.forEach(department => {                                                 ⑩
        document.getElementById('Department')                                           ⑩
            .add(new Option(department, department));                                   ⑩
    });                                                                                 ⑩
                                                                                        ⑩
    instructors.forEach(instructor => {                                                 ⑩
        document.getElementById('Instructor')                                           ⑩
            .add(new Option(instructor, instructor));                                   ⑩
    });                                                                                 ⑩
}                                                                                       ⑩

function populateArticles(data) {                                                       ⑪
    const article = document.querySelector('article');                                  ⑪
    article.innerHTML = '';                                                             ⑪
    data.forEach(course => {                                                            ⑪
        const section = document.createElement('section');                              ⑪
        section.innerHTML = `                                                           ⑪
            <h3>${course.Title}</h3>                                                    ⑪
            <div>                                                                       ⑪
                Course ID: ${course['Course ID']}<br>                                   ⑪
                Instructor: ${course.Instructor}<br>                                    ⑪
                Department: ${course.Department}<br>                                    ⑪
                Semester: ${course.Semester}<br>                                        ⑪
            </div>                                                                      ⑪
            <p>${course.Description}</p>                                                ⑪
        `;                                                                              ⑪
        article.appendChild(section);                                                   ⑪
    });                                                                                 ⑪
}                                                                                       ⑪

function filterData() {                                                                 ⑫
    fetch('college_courses.json')
        .then(response => response.json())
        .then(data => {
            const departmentValue = document
.getElementById('Department').value;
            const instructorValue = document.
getElementById('Instructor').value;

            let filteredData = data;
            if (departmentValue !== 'all') {
                filteredData = filteredData
.filter(course => course.Department===departmentValue);
            }
            if (instructorValue !== 'all') {
                filteredData = filteredData.
filter(course => course.Instructor===instructorValue);
            }
            populateArticles(filteredData);
        });
}                                                                                       ⑬

function sortData() {                                                                   ⑭
    fetch('college_courses.json')                                                       ⑭
        .then(response => response.json())                                              ⑭
        .then(data => {                                                                 ⑭
            const sortValue = document.getElementById('Sort').value;                    ⑭
            data.sort((a, b) => {                                                       ⑭
                if (sortValue === 'title') {                                            ⑭
                    return a.Title.localeCompare(b.Title);                              ⑭
                } else {                                                                ⑭
                    return a.Department.localeCompare(b.Department);                    ⑭
                }                                                                       ⑭
            });                                                                         ⑭
            populateArticles(data);                                                     ⑭
        });                                                                             ⑭
}                                                                                       ⑭

function searchData(searchText) {                                                       ⑮
    if (!searchText) {                                                                  ⑮
        fetch('college_courses.json')                                                   ⑮
            .then(response => response.json())                                          ⑮
            .then(data => {                                                             ⑮
                populateArticles(data);                                                 ⑮
            });                                                                         ⑮
        return;                                                                         ⑮
    }                                                                                   ⑮
                                                                                        ⑮
    fetch('college_courses.json')                                                       ⑮
        .then(response => response.json())                                              ⑮
        .then(data => {                                                                 ⑮
            const filteredData = data.filter(course =>                                  ⑮
                course.Title.toLowerCase().includes(searchText.toLowerCase()) ||        ⑮
                course['Course ID'].toLowerCase().includes(searchText.toLowerCase()) || ⑮
                course.Instructor.toLowerCase().includes(searchText.toLowerCase()) ||   ⑮
                course.Department.toLowerCase().includes(searchText.toLowerCase()) ||   ⑮
                course.Description.toLowerCase().includes(searchText.toLowerCase())     ⑮
            );                                                                          ⑮
            populateArticles(filteredData);                                             ⑮
        });                                                                             ⑮
}                                                                                       ⑮
```

① 页面加载后运行后续的功能代码

② 从 JSON 文件中获取数据

③ 运行填充下拉列表的功能

④ 运行填充文章的功能

⑤ 监听部门下拉菜单的变化

⑥ 监听讲师下拉菜单的变化

⑦ 监听排序下拉菜单的变化

⑧ 监听搜索文本框的文本输入

⑨ 页面加载后运行后续的功能代码

⑩ 用那些字段的唯一值填充部门和讲师下拉菜单

⑪ 用课程数据填充文章元素

⑫ 当用户在部门或讲师列表中选择一个项目时，过滤数据

⑬ 当用户在部门或讲师列表中选择一个项目时，过滤数据

⑭ 当用户在排序列表中选择一个项目时，对数据进行排序

⑮ 当用户在搜索文本框中输入某些内容时，搜索数据

如果您愿意，可以使用前两节中的 HTML 和 CSS 注释来自定义您的网页代码，正如我在下一节中描述的那样。

## 13.7 自定义课程目录

以前节的注释为指导，这里我将带您通过一些相对简单的代码自定义，您可以通过在文本编辑器中打开 HTML 和 CSS 文件来实现。然而，如果您的页面与您想要的不太接近，您最好重新编写提示并将其提交给 ChatGPT 进行新的会话。

由于此项目中的 HTML 代码最少，因为大部分页面是通过 JavaScript 生成的。因此，我只有一些建议：

+   随意添加更多排序字段，只需在排序下拉列表中添加新项目即可。只需记住提示 ChatGPT 生成处理新字段的 JavaScript 代码。

+   在 HTML 代码的页脚部分，你可以添加指向你的社交媒体账户的链接，正如我在第四章中描述的那样。

现在，这里有一些 CSS 代码的定制想法：

+   要使用不同的页面背景颜色，请为 `body` 元素的 `background-color` 属性指定不同的颜色关键字。

+   要为页眉和页脚使用不同的背景颜色，请为 `header` 和 `footer` 元素的 `background-color` 属性指定新的颜色关键字。

+   要为页面文本使用不同的颜色，请为 `body` 元素的 `color` 属性指定不同的颜色关键字。

+   对于任何字体大小值，你可以通过改变数字来增加或减少字体大小。只需确保保留 `px` 单位。

+   对于任何填充或边距值，你可以通过改变数字来增加或减少填充或边距。在每种情况下，都要确保保留 `px` 单位。

+   要使你的页面代码更易于访问，考虑将所有 px 测量转换为 rem 测量。默认情况下，1 rem 等于 16 px，所以 20 px 是 1.25 rem，24 px 是 1.5 rem，32 px 是 2 rem，48 px 是 3 rem，依此类推。rem 单位更易于访问，因为它测量的是相对于浏览器用户在其浏览器设置中定义的默认字体大小的字体大小。

## 13.8 接下来去哪里

我在这本书中的目标一直是向你展示，尽管看起来神奇，ChatGPT 可以根据请求生成复杂的网页代码，但真正的秘密是将你的网页愿景转化为详细和具体的提示，告诉 ChatGPT 你确切想要什么。你在本书中看到了许多这样的提示示例，并且在过程中，你学习了关于网页构建和设计所需知道的一切。这是个好消息，因为它意味着你现在拥有创建几乎所有你想要在网页上的知识和经验。当你准备好构建一些大胆而美丽的东西时，ChatGPT 将会为你将梦想变为现实。这一切都只是一个提示的距离。

## 摘要

+   将 Excel 数据转换为 JSON 时，请确保数据位于一个范围或表中，并且每个列都有一个唯一的标题。

+   JSON 是一组由逗号分隔的属性-值对，用大括号 `{` 和 `}` 包围，其中属性名用双引号包围。文本值也用双引号包围。

+   如果你有一个 ChatGPT Plus 账户，你可以将你的 Excel 文件上传到聊天中，然后提示 ChatGPT 将你的数据转换为 JSON，并将结果作为可以下载的文件输出。

+   你让 ChatGPT 生成一个空元素（如 `article` 元素）的网页代码；然后你使用 JavaScript 来填充它，使用 JSON 数据。

+   网页上最常见的数据处理技术包括搜索、过滤和排序。您可以通过提示 ChatGPT 生成实现每种技术的 JavaScript 代码。

+   为了获得最佳结果，您的页面提示应尽可能具体，包括颜色、字体大小和标题级别。

+   将生成的 HTML 保存到 index.xhtml 文件中，将生成的 CSS 保存到 ChatGPT 在 HTML 代码中建议的文件名中，通常是 styles.css，将生成的 JavaScript 代码保存到 ChatGPT 在 HTML 代码中建议的文件名中，通常是 script.js。

# 附录 A. 使用 ChatGPT 准备构建网页

除了第一章的介绍性材料外，本书的重点是向您展示如何说服 ChatGPT 帮助您构建网页，而无需学习如何自己编码。我希望您会发现本书的网页想法和用于生成它们的提示对您有用，无论是直接使用还是作为您自己探索的起点。

将 ChatGPT 用作网页编码助手，其复杂程度远不及自己学习编码页面，但它确实需要一些设置和基础设施。本附录旨在向您介绍您需要了解的少数事项以及您需要完成的少数任务，以便您能够成功地将 ChatGPT 用于将您的网站想法变为现实。在经过一个仁慈的简短需求清单后，您将学习如何设置可选的 ChatGPT 或 Microsoft 账户。您还将学习如何在部署代码之前测试您的代码，以及如何处理 HTML 和其他网页文件。

## A.1 开始所需准备

使用 ChatGPT 帮助您创建网页的最好之处之一是，您只需极少的条件，并且无需花费您辛苦赚来的任何一分钱（除非您愿意）。实际上，我可以将您需要启动的所有内容总结成一个只有四项的清单：

+   *互联网接入*—尽管您可以使用 ChatGPT 移动应用离线使用，但 OpenAI 应用([`chat.openai.com`](https://chat.openai.com))、Bing Copilot([`bing.com`](https://bing.com)然后点击 Copilot)和 Microsoft Copilot([`copilot.microsoft.com`](https://copilot.microsoft.com))——您需要使用其中任何一个来轻松访问 ChatGPT 生成的代码——都是在线服务，因此您需要互联网接入。

+   *网页浏览器*—您可以使用任何主流浏览器的最新版本（如 Chrome、Safari、Edge 或 Firefox）访问 OpenAI 应用和 Bing Copilot。但为了使用 Microsoft Copilot，您需要使用 Chrome 或 Microsoft Edge，目前 Firefox 和 Safari 也在开发中。

+   *文本编辑器*—在您复制 ChatGPT 生成的代码后，您需要将其粘贴到某个地方，而这个地方几乎总是打开在文本编辑器中的文件。是的，您可以使用您电脑自带的默认文本编辑器（Windows 的记事本或 macOS 的 TextEdit），但这里有一些适合代码的编辑器可以考虑：

    +   *Notepad++*—仅适用于 Windows，且是免费的：[`notepad-plus-plus.org`](https://notepad-plus-plus.org)

    +   *Nova*—适用于 Mac，价格为 99 美元，但提供免费试用：[`nova.app`](https://nova.app)

    +   *Sublime Text*—适用于 Windows 和 Mac，价格为 99 美元，但提供免费试用：[www.sublimetext.com](https://www.sublimetext.com)

    +   *Visual Studio Code*—适用于 Windows 和 Mac，而且这个也是免费的：[`code.visualstudio.com`](https://code.visualstudio.com)

+   *Web hosting account*—一旦你将 ChatGPT 生成的代码保存到网页文件中，你的最后一步就是将文件部署到网络上。为此，你需要一个网络托管服务提供商的账户。我在附录 B 中更详细地讨论了如何设置网络托管账户以及部署你的网络代码。如果你没有网络托管服务，你仍然可以通过使用网络浏览器的文件 > 打开命令来打开每个保存的 HTML 文件，在本地查看你的页面。

注意：如果你打算在你的网页上使用自己的照片（查看第十章），你可能需要一个用于裁剪、增强颜色、更改图像大小和文件格式的照片编辑应用程序。Windows 和 macOS 附带的照片应用程序可以处理这些简单操作，但对于更深入的任务，你可能需要高端软件，如 Adobe Photoshop ([www.adobe.com/products/photoshop.xhtml](https://www.adobe.com/products/photoshop.xhtml)) 或 GIMP ([www.gimp.org](https://www.gimp.org))，后者是免费的。

是的，这真的是你需要的全部，而且这些物品都不需要额外付费（假设即使你不使用 ChatGPT 创建网页，你也会支付互联网接入费用）。唯一可能需要付费的情况是购买 ChatGPT 订阅，我将在下一节中讨论这一点。

## A.2 理解 ChatGPT 账户访问

ChatGPT 是 OpenAI 的产品，由 Microsoft 支持。因此，似乎合理的预期是，你需要一个 OpenAI 账户或 Microsoft 账户才能与 ChatGPT 进行对话。这是真的吗？令人惊讶的是，答案是否定的，除非你想要一个。那么，你应该为 ChatGPT 访问获取一个账户吗？以下是需要考虑的场景：

+   *Maximizing privacy (no account)*—许多人不愿意将私人数据发送给大型企业（如 OpenAI 和 Microsoft），因此在不使用账户的情况下访问 ChatGPT 可以使整个过程更加私密。你可以不使用账户访问 Open AI ChatGPT 应用程序，但你被限制使用 GPT 3.5。要无 Microsoft 账户使用 ChatGPT，你需要通过 Bing 访问 Copilot。注意，然而，如果没有 Microsoft 账户，你每场会议的限制是 ChatGPT 只有 10 个回复（相对于使用 Microsoft 账户时每场会议的 30 个回复）。

+   *获取 GPT-4 的免费访问权限（Microsoft 账户）*—GPT-4（至少在我写这篇文章的时候）是 OpenAI 最新的、最强大的大型语言模型（LLM），因此是大多数人想要使用的模型，尤其是用于生成网页代码。你可以付费给 OpenAI 来获取 GPT-4 的访问权限（如我在这些要点中的最后一个所述），但另一种方法是导航到 Microsoft Copilot，它使用 GPT-4 作为其 LLM。为了充分利用 Bing Copilot（以及访问独立的 Microsoft Copilot 网站），创建一个 Microsoft 账户并使用它登录——或者如果你是 Windows 用户，使用你现有的 Microsoft 账户。要创建一个 Microsoft 账户，请访问 [`account.microsoft.com`](https://account.microsoft.com)，点击“登录”，然后按照步骤操作。

+   *获取 GPT-3.5 的免费访问权限（免费 OpenAI 账户）*—GPT-3.5 是一个出色的 AI 模型，能够生成可靠且有用的网页代码。如果你想要免费访问 GPT-3.5，但出于某种原因无法（或不想）使用 Copilot 来获取 GPT-4 的免费访问权限（如前一个要点所述），你可以设置一个免费的 OpenAI 账户。拥有账户可以让你访问一些 ChatGPT 的额外功能，这些功能对于没有账户使用 ChatGPT 的人来说是不可用的（如第一个要点所述）。要创建一个免费的 OpenAI 账户，请访问 [`openai.com`](https://openai.com)，点击“注册”，然后按照步骤操作。

+   *获取 GPT-4 的付费访问权限（ChatGPT Plus 订阅）*—如果你想要使用 GPT-4，但出于某种原因无法（或不想）使用 Bing Copilot 或 Microsoft Copilot 来获取 GPT-4 的免费访问权限（如前一个要点所述），你需要设置一个 ChatGPT Plus 的订阅，按照我写这篇文章时的价格，这将花费你每月 20 美元。要设置一个 ChatGPT Plus 订阅，创建一个免费的 OpenAI 账户（如前一个要点所述），访问 ChatGPT 应用程序 ([`chat.openai.com`](https://chat.openai.com))，在左下角点击“升级”（参考图 A.1），然后按照步骤操作。

![图片](img/build-a-website-with-chatgpt-APPA_F01_McFedries3.png)

图 A.1 要设置 ChatGPT Plus 订阅，请点击 ChatGPT 应用程序侧边栏中的“升级”按钮。

## A.3 测试你的代码

ChatGPT 在难以想象的巨大数量的编程代码上进行了训练，这就是为什么它通常在生成你要求的网页小部件方面表现得如此出色。但 ChatGPT 并非完美无缺，这意味着它有时会生成 HTML、CSS 或 JavaScript 代码，这些代码要么没有按照你的要求执行，要么在某些方面存在错误。一个专业的程序员通常可以检查生成的代码，并不仅理解“代码是错误的”，而且还能理解“为什么代码是错误的”。你之所以在阅读这本书，是因为你不是专业的程序员，那么你将如何知道 ChatGPT 是否产生了错误的代码？

答案是，你让网络浏览器渲染代码，然后检查结果以查看代码是否按预期工作（或者根本不起作用）。让网络浏览器渲染 ChatGPT 代码的一种方法是通过运行完整的提示-复制-保存-部署周期。这个过程并不特别繁重，但也不是微不足道，所以如果你只是想知道，比如说，ChatGPT 生成的表单代码是否按预期工作，这似乎有些过度。

更好且更快的方法是仅测试 ChatGPT 生成的代码，你可以通过复制代码然后将其粘贴到可用的在线编码沙盒中来实现。接下来的两个部分将提供详细信息。

### A.3.1 从 ChatGPT 复制数据

一旦 ChatGPT 完成生成你的代码，你的第一步是将该代码复制到你的电脑剪贴板。（剪贴板是电脑用来存储你最近复制的项目的特殊内存区域。）你如何操作取决于你使用哪种方法访问 ChatGPT：

+   *OpenAI ChatGPT 应用*——点击代码窗口右上角的“复制代码”按钮（如图 A.2 所示）。

![](img/build-a-website-with-chatgpt-APPA_F02_McFedries3.png)

图 A.2 在 OpenAI ChatGPT 应用中，点击代码窗口的“复制代码”按钮以复制生成的代码。

+   *Microsoft Copilot*——点击代码上方和右侧出现的“复制”按钮（如图 A.3 所示）。

![](img/build-a-website-with-chatgpt-APPA_F03_McFedries3.png)

图 A.3 在 Copilot 中，点击“复制”按钮以复制生成的代码。

警告：你的电脑剪贴板一次只能存储一个复制的项目。如果你在粘贴你的 ChatGPT 代码之前复制了其他内容（如我在下一节中描述的），那么该代码将从内存中清除，你将不得不重新全部复制。

### A.3.2 将数据粘贴到在线编码沙盒中

将你的 ChatGPT 生成的代码复制到你的电脑剪贴板后，下一步（也是最后一步）是将代码粘贴到在线网页编码沙盒中。*沙盒* 是一个接受 HTML、CSS 以及通常 JavaScript 代码的网站，然后显示该代码在网页浏览器中的渲染效果。通过使用沙盒来测试你的代码，你可以避免将代码保存到文件中，然后将文件部署到网络主机上的麻烦，当你只是想查看页面部分或组件是否正常工作时，这会显得过于繁琐。

这里有一些可以查看的网页编码沙盒：

+   *网页设计沙盒*——这是我的书 *网页设计沙盒* 的配套网站，该书教授初学者 HTML 和 CSS。如图 A.4 所示，该网站提供了一个“沙盒”，其中包括 HTML 和 CSS 编辑器，你可以将 ChatGPT 生成的 HTML 和 CSS 代码粘贴进去。点击“运行代码”，底部结果区域将显示代码在浏览器中的样子。导航到 [`webdesignplayground.io/new`](https://webdesignplayground.io/new) 尝试使用它。

![自动生成中等置信度的聊天截图](img/build-a-website-with-chatgpt-APPA_F04_McFedries3.png)

图 A.4 Web Design Playground 提供 HTML 和 CSS 编辑器，你可以将 HTML 和 CSS 代码粘贴到这些编辑器中以进行测试。

+   *WebDev Workbench*——这是一个我建立的游乐场，旨在帮助网页开发者测试 HTML、CSS 和 JavaScript 代码。如图 A.5 所示，Workbench 提供了 HTML、CSS 和 JavaScript 标签，你可以将 ChatGPT 提供的 HTML、CSS 和 JavaScript 代码粘贴到这些标签中。点击运行，底部结果区域将显示代码在浏览器中的外观。导航到[`webdevworkshop.io/wb`](https://webdevworkshop.io/wb)查看。

![图片 A.5](img/build-a-website-with-chatgpt-APPA_F05_McFedries3.png)

图 A.5 WebDev Workbench 提供 HTML、CSS 和 JavaScript 标签，你可以将 ChatGPT 代码粘贴到这些标签中以进行测试。

+   *CodePen*——这是一个测试网页代码的流行网站。你创建一个包含 HTML、CSS 和 JavaScript 代码编辑器的“笔”，如图 A.6 所示。粘贴后几秒钟，渲染结果会自动出现在下方的框架中。导航到[`codepen.io`](https://codepen.io)并点击开始编码来尝试。

![图片 A.6](img/build-a-website-with-chatgpt-APPA_F06_McFedries3.png)

图 A.6 CodePen 提供 HTML、CSS 和 JavaScript 的编辑器。将你的 ChatGPT 代码粘贴到相应的编辑器中以测试代码。

所有这些游乐场以更多或更少相同的方式工作：

1.  复制你的 ChatGPT 代码。

1.  导航到游乐场。

1.  点击对应于你要测试的代码类型的编辑器内部（例如，使用 HTML 编辑器来编辑 HTML 代码）。

1.  点击运行代码的按钮（或者，在 CodePen 的情况下，只需等待几秒钟）。

注意：如果 ChatGPT 生成的 HTML 代码还包含 CSS 代码（位于`<style>`和`</style>`标签之间），最好单独复制 CSS 代码（忽略`<style>`和`</style>`标签）并将其粘贴到游乐场的 CSS 编辑器中。同样，如果 ChatGPT 生成的 HTML 代码还包含 JavaScript 代码（位于`<script>`和`</script>`标签之间），则单独复制 JavaScript 代码（省略`<script>`和`</script>`标签）并将其粘贴到 JavaScript 编辑器中。为了避免从生成的 HTML 代码中提取 CSS 和 JavaScript 的额外工作，请在你的提示中包含你想要 ChatGPT 分别输出 HTML、CSS 和 JavaScript 的要求。ChatGPT 应该将 HTML 代码放在 HTML 窗口中，CSS 代码放在单独的 CSS 窗口中，JavaScript 代码放在单独的 JavaScript 窗口中。

当你与 ChatGPT 一起工作时，保持你最喜欢的游乐场在其自己的浏览器标签中打开是个好主意。这样，一旦 ChatGPT 为你生成新的代码，你就可以立即复制并粘贴代码到游乐场以检查它是否工作。

## A.4 与网页文件一起工作

虽然您的大部分时间将用于提示 ChatGPT 生成您想要放在线上的网页代码和文本，但您需要在某个时候将此代码放入一个或多个可以部署的文件中。为了帮助完成提示-复制-保存-部署循环中的“保存”部分，本附录的其余部分将告诉您需要了解的内容。

### A.4.1 理解不同类型的网页文件

网页的一个令人惊讶和令人惊奇的事情是，从最简陋的首页到最强大的超大型企业网站，您所看到的一切，其底层都是简单的文本。我怎么会知道？因为每个网页都由一个或多个文件组成，而所有受网页支持的文件类型都是基于文本文件主题的变体。（在这里，我忽略了图像、视频和音频文件，它们是单独交付的。）事实上，大多数网页都是由以下三种文件类型的一些组合组成的：

+   *HTML*—这些文件使用.xhtml（有时是.htm）扩展名，并提供网页的基本结构。所有网站至少包含一个 HTML 文件（通常命名为 index.xhtml）。

+   *CSS*—这些文件使用.css 扩展名，通过定义字体、颜色、边框和布局等样式规则来提供网页的整体外观。

+   *JavaScript*—这些文件使用.js 扩展名，并为网页添加交互性。

当您以这种方式使用单独的文件时，您需要从 HTML 文件中引用它们，您将在不久后学习如何做到这一点。不过，现在您需要学习如何将 ChatGPT 生成的代码粘贴到网页文件中。

### A.4.2 将 ChatGPT 数据粘贴到 HTML 文件中

一个简单的网页可能只使用一个包含 CSS 和 JavaScript 代码的 HTML 文件。CSS 代码位于页面的特殊标题部分中的`<style>`和`</style>`标签之间，JavaScript 代码位于`<script>`和`</script>`标签之间，通常在 HTML 文件的底部附近。以下是这样一种 HTML 文件的一般布局：

```py
<!DOCTYPE html>
<html>
<head>
    <style>
                   ①
    </style>
</head>
<body>
                   ②
    <script>
                   ③
    </script>
</body>
</html>
```

① 将 CSS 代码放在这里。

② 将 HTML 标签和文本放在这里。

③ 将 JavaScript 代码放在这里。

您可以将此代码作为所有简单网页项目的起点。（您将在第六章学习如何让 ChatGPT 生成类似的模板。）有了这个模板，接下来您就可以粘贴 ChatGPT 生成的代码了：

+   *CSS*—将以下代码粘贴到`<style>`标签下方但`</style>`标签上方。

+   *HTML*—将代码粘贴到`<body>`标签下方但`</script>`标签上方。页面上的各种组件需要按照您希望在页面上显示的顺序出现在文件中。我在生成页面组件的章节中提供了更具体的放置说明。

+   *JavaScript*—将代码粘贴到`<script>`标签下方但`</script>`标签上方。

然而，请记住，这种所有代码都在一个文件中的方法实际上仅适用于最简单的网页。当您的页面稍微复杂一些时，您将想要创建单独的 CSS 和 JavaScript 文件，正如我接下来要描述的那样。

### A.4.3 在 HTML 文件中引用 CSS 和 JavaScript 文件

将 CSS 和 JavaScript 代码放入单独的文件会使 HTML 文件更加简单和整洁，并且还允许你将相同的 CSS 和 JavaScript 代码应用于多个网页，这可以节省大量时间。假设你已经将 CSS 和 JavaScript 代码分别保存在单独的.css 和.js 文件中，那么在你想使用 CSS 和/或 JavaScript 代码的任何 HTML 文件中添加对文件的引用：

```py
<!DOCTYPE html>
<html>
<head>
    <link href="styles.css" rel="stylesheet">  ①
</head>
<body>
    *HTML tags and text go here*
    <script src="code.js"></script>            ②
</body>
</html>
```

① 使用`<link>`标签来引用 CSS 文件。

② 使用`<script>`标签来引用 JavaScript 文件。

下面是具体细节：

+   *CSS*——在`<head>`标签和`</head>`标签之间添加一个`<link>`标签，并将`href`属性设置为包围在引号中的 CSS 文件名。

+   *JavaScript*——在`</body>`标签上方，添加一个`<script>`标签，并将其`src`属性设置为包围在引号中的 JavaScript 文件名，然后添加一个`</script>`标签。

要在多个 HTML 文件中重用 CSS 或 JavaScript 文件，将这些文件中的相同`<link>`标签或`<script>`标签包含在内。

### A.4.4 保存你的工作

一旦你对 HTML、CSS 或 JavaScript 文件进行了任何更改，你应该立即保存你的更改以避免丢失工作。在第一次保存新文件时，请注意以下几点：

+   一定要使用正确的文件扩展名：HTML 文件使用.xhtml 扩展名，CSS 文件使用.css 扩展名，JavaScript 文件使用.js 扩展名。

+   如果你的网站由单个 HTML 页面组成，那么将该页面命名为 index.xhtml。如果你的网站由多个页面组成，那么将主页或主页面命名为 index.xhtml。

+   不要在文件名中使用空格或特殊符号。仅使用字母数字字符、破折号(-)或下划线(_)。

+   对于大多数网站托管服务，文件名是区分大小写的，这意味着例如 index.xhtml、Index.xhtml 和 INDEX.xhtml 都会被视为不同的文件。在文件名中坚持使用全部小写字母是最好的做法。

+   尽可能保持文件名尽可能短，同时不要使其变得晦涩。about.xhtml 的名称比 a-few-words-about-this-project.xhtml 更好，但 nlsup.xhtml 比 newsletter-signup.xhtml 更差。

+   确保保存与单个网站相关的所有文件——这意味着不仅包括所有的 HTML、CSS 和 JavaScript 文件，还包括所有的图片、视频和音频文件——在一个单独的文件夹中。当部署你的网站时，这会使你的生活变得更加容易，正如我在附录 B 中描述的那样。

# 附录 B. 部署你的网站

当我说一个网站的关键特征是“web”这个词的部分时，我并没有泄露任何重大秘密或宣扬任何深奥的知识。也就是说，尽管你可以在电脑上创建和预览尽可能多的 HTML 文件，但这些文件只有在部署到网络上供你的朋友、家人甚至陌生人查看时，才真正构成一个网站。将 HTML、CSS、JavaScript 和其他文件从你的电脑传输到网站托管服务被称为*部署*你的网站。

关于你在本书中学到的网站类型的好消息——即，仅使用静态 HTML 文件且不需要访问完整网络服务器的网站——是这些文件的简单性意味着有一些网络托管商会免费部署你的网站。这些网站从大型企业和专业网络开发者那里赚钱，因此托管一个基本的个人网站对他们来说无关紧要。在本附录中，你将学习如何将你的网站部署到两个这样的网络托管商：Netlify 和 Cloudflare。为了保险起见，我还为你提供了将文件部署到其他网络托管提供商的通用说明。

## B.1 部署到 Netlify

Netlify 是一家为大型企业和专业开发者提供基于云的开发平台的公司，用于构建和部署网络应用程序。令人高兴的是，Netlify 还通过提供免费层支持个人和爱好者，使任何人都能轻松地搭建一个或几个页面。唯一的限制是，你最多只能拥有 500 个网站和 100 GB 的带宽。（*带宽* 是每月你的网站传输到网络浏览器中的数据量。100 GB 是 *很多* 带宽。）

### B.1.1 设置 Netlify 账户

要开始使用 Netlify，你需要一个账户。以下是需要遵循的步骤：

1.  将你喜欢的网络浏览器发送到 [`netlify.com`](https://netlify.com)。

1.  点击“注册”。

1.  点击“使用电子邮件注册”。

1.  输入你的电子邮件地址，输入你想要使用的密码，然后点击“注册”。Netlify 会向你的电子邮件地址发送验证消息。

1.  打开你的电子邮件应用程序，点击 Netlify 验证消息，然后点击验证链接。Netlify 验证你的账户，然后显示一系列问题。

1.  答完问题后，点击“继续部署”，然后点击“现在跳过此步骤”。

Netlify 会将你带到团队概览页面。从这里，你可以使用两种方法之一上传你的文件：拖放或对话框。接下来的两个部分将带你了解这两种方法。

### B.1.2 通过拖放上传你的文件

通常，将你的网站文件快速发送到 Netlify 的最快方法是使用鼠标将网站文件夹拖放到上传区域。以下是需要遵循的步骤：

1. 在你的电脑上，打开文件资源管理器（Windows）或 Finder（macOS）。

2. 导航到包含你想要上传的子文件夹的文件夹。

3. 登录 Netlify（如果你还没有这样做），然后在左侧侧边栏中点击“网站”。

4. 调整浏览器窗口和文件资源管理器（或 Finder）窗口，使它们并排显示（或者至少你可以看到浏览器中的上传区域和文件资源管理器或 Finder 中的你想要上传的子文件夹）。

5. 从文件资源管理器（或 Finder）拖动子文件夹，将鼠标指针移到浏览器窗口中的上传区域（如图 B.1 所示），然后放下子文件夹。Netlify 上传子文件夹及其内容，然后部署网站。

![](img/build-a-website-with-chatgpt-APPB_F01_McFedries3.png)

图 B.1 将网站文件夹拖动到 Netlify 上传区域。

6. 在“部署成功！”对话框（如图 B.2 所示）中，点击“开始”。Netlify 显示您的账户概览页面。

![图片](img/build-a-website-with-chatgpt-APPB_F02_McFedries3.png)

图 B.2 Netlify 在您的网站部署后显示“部署成功！”对话框。

7. 在页面上的“站点”部分，点击您的新站点。Netlify 显示网站概览页面。

8. 点击链接在网页浏览器中查看已部署的站点。

### B.1.3 使用对话框上传您的文件

如果您的屏幕相对较小或您的鼠标技能不够，拖放方法可能不是最佳选择。没关系，因为 Netlify 还允许您使用对话框上传您的网站文件夹。以下是操作步骤：

1.  登录 Netlify（如果您尚未这样做），然后点击左侧边栏中的“站点”。

1.  点击浏览以上传。

1.  在出现的对话框中，选择项目文件夹，然后点击上传。

1.  如果您的网络浏览器要求您确认操作，请点击上传。Netlify 上传子文件夹及其内容。

1.  在“部署成功！”对话框中，点击“开始”。Netlify 显示您的账户概览页面。

1.  在页面上的“站点”部分，点击您的新站点。Netlify 显示网站概览页面。

1.  点击链接在网页浏览器中查看已部署的站点。

### B.1.4 更改您的站点子域名或域名

默认情况下，Netlify 为您的部署网站提供了一个自定义域名，格式为*wacky-name-a1b2c3*.netlify.app（图 B.3 展示了示例）。您可以在网站概览页面上看到您的站点名称。要从任何 Netlify 页面访问该页面，请点击左侧边栏中的“站点”，然后点击该站点。

![图片](img/build-a-website-with-chatgpt-APPB_F03_McFedries3.png)

图 B.3 网站概览页面显示了 Netlify 分配给您的站点名称。

您可能喜欢 Netlify 随机提供的古怪名称，但如果您希望域名反映您网站的内容，您需要使用以下方法之一来更改域名：

+   *更改子域名*——如果您想保留 netlify.app 域名，只需更改子域名（即 wacky-name-a1b2c3 部分），请打开网站概览页面，点击“域名设置”，在“生产域名”部分点击“选项”，然后点击“编辑站点名称”。输入您首选的子域名，然后点击“保存”。如果 Netlify 告诉您该站点名称已被占用，请尝试使用不同的名称。

+   *更改域名*——如果您已经有一个域名或想通过 Netlify 购买一个新的域名，请打开网站概览页面，点击“域名设置”，然后在“生产域名”部分点击“添加域名”。输入您现有的或新的域名，点击“验证”，然后按照出现的说明操作。

## B.2 部署到 Cloudflare

Cloudflare 最出名的是一家专注于帮助大型网站避免或摆脱网络攻击的网络公司，例如向网站发送大量垃圾数据的*分布式拒绝服务*（DDOS）攻击。但 Cloudflare 还通过名为 Pages 的服务提供网站托管。这项服务表面上针对的是网站开发者，但对我们这样的人也开放。最好的是，Pages 账户是免费的，并且对网站数量和带宽使用量没有限制。

### B.2.1 设置 Cloudflare Pages 账户

要开始使用 Cloudflare Pages，你首先需要按照以下步骤设置账户：

1.  导航到[`pages.cloudflare.com`](https://pages.cloudflare.com)。

1.  点击“注册”。

1.  输入你的电子邮件地址，输入你想要使用的密码，然后点击“注册”。Cloudflare 会向你的电子邮件地址发送验证邮件。

1.  打开你的电子邮件应用程序，点击 Cloudflare 验证消息，然后点击验证链接。

Cloudflare 验证你的账户，然后显示你的 Cloudflare 仪表板。你已准备好创建一个新的 Cloudflare 应用程序，如下一节所述。

### B.2.2 创建新的 Cloudflare 应用程序

在 Cloudflare 中，一个 Pages 网站被称为*应用程序*，你将其作为 Cloudflare Pages 功能的一部分进行部署。你通过创建一个新的 Pages 应用程序开始部署，以下步骤将概述：

1. 如果你还没有这样做，请登录 Cloudflare。

2. 在左侧的导航菜单中，在“Workers & Pages”下点击“概览”。出现概览页面。如果你还没有部署 Pages 项目，请跳到步骤 4；否则，继续步骤 3。

3. 点击图 B.4 所示的“创建应用程序”按钮。出现“创建应用程序”页面。

![](img/build-a-website-with-chatgpt-APPB_F04_McFedries3.png)

图 B.4 在 Cloudflare 的“Workers & Pages 概览”页面，点击“创建应用程序”。

4. 如图 B.5 所示，点击“Pages”标签页。

![包含文本、字体、屏幕截图的图片，描述自动生成](img/build-a-website-with-chatgpt-APPB_F05_McFedries3.png)

图 B.5 在“创建应用程序”页面，点击“Pages”标签页。

5. 滚动到“使用直接上传创建”部分，然后点击“上传资产”（参见图 B.6）。出现“通过上传项目部署网站”页面。

![云的屏幕截图，描述自动生成，置信度低](img/build-a-website-with-chatgpt-APPB_F06_McFedries3.png)

图 B.6 点击“上传资产”。

6. 为你的项目输入一个名称，然后点击“创建项目”（参见图 B.7）。当你的项目准备就绪（需要几分钟）时，Cloudflare 会显示上传区域。

![白色背景上的蓝色线条，描述自动生成，置信度低](img/build-a-website-with-chatgpt-APPB_F07_McFedries3.png)

图 B.7 为你的项目命名，然后点击“创建项目”。

从这里，您可以通过两种方法之一上传文件：拖放或对话框。接下来的两个部分将向您介绍这两种方法。

### B.2.3 通过拖放上传您的文件

通常，将您的文件从计算机传输到 Cloudflare 最简单的方法是使用鼠标将网站文件夹拖放到上传区域。以下是操作步骤：

1. 在您的计算机上，打开文件资源管理器（Windows）或 Finder（macOS）。

2. 导航到包含您想要上传的子文件夹的文件夹。

3. 调整浏览器窗口和文件资源管理器（或 Finder）窗口，使它们并排显示（或者至少您可以在浏览器中看到上传区域，在文件资源管理器或 Finder 中看到您想要上传的子文件夹）。

4. 将子文件夹从文件资源管理器（或 Finder）拖动，将鼠标指针移入浏览器窗口并覆盖上传区域，然后放下子文件夹。Cloudflare 会上传子文件夹及其内容。

最后一步是将网站部署，如 B.2.5 节所述。

### B.2.4 使用对话框上传您的文件

如果您正在使用小屏幕或鼠标技能不是那么熟练，您可能更喜欢使用对话框将文件上传到 Cloudflare。以下是操作方法：

1. 在 Cloudflare 的上传区域中，点击从计算机选择。

2. 点击上传文件夹。

3. 在出现的对话框中，选择项目文件夹，如图 B.8 所示，然后点击上传。

![计算机截图，描述由中等置信度自动生成](img/build-a-website-with-chatgpt-APPB_F08_McFedries3.jpg)

图 B.8 选择网站文件夹。

4. 如果您的网络浏览器要求您确认操作，请点击上传。Cloudflare 会上传子文件夹及其内容。

最后一步是将网站部署，如下一节所述。

### B.2.5 部署网站

文件上传完成后，您就可以部署新网站了。您可以通过点击部署网站按钮来完成此操作。Cloudflare 会部署网站，然后显示成功！消息，如图 B.9 所示。点击链接在网页浏览器中查看已部署的网站。

![网页截图，描述由低置信度自动生成](img/build-a-website-with-chatgpt-APPB_F09_McFedries3.png)

图 B.9 当您的网站部署时，Cloudflare 显示成功！消息。

### B.2.6 更改您的网站域名

Cloudflare 为您部署的网站提供了一个自定义域名，格式为 *folder-name*-*a1b2*.pages.dev（其中 *folder-name* 来自您上传的网站文件夹名称）。您可以通过以下方式更改此名称为自己的域名：

+   *从 Cloudflare 购买的域名*—在左侧侧边栏中，点击域名注册，点击注册域名，输入您想要使用的新域名，点击搜索，然后按照指示操作。购买完成后，按照下一项指示将新域名分配给 Pages 网站。

+   *你已拥有的域名*—从“工作与页面概览”页面，点击你想要工作的网站，点击“自定义域名”选项卡，点击“设置自定义域名”，输入你拥有的域名（如果你通过 Cloudflare 购买了域名，请输入该域名），点击“继续”，然后按照指示操作。

## B.3 部署到其他网络托管服务

其他服务可以托管你的网站；它们将你的文件存储在称为*Web 服务器*的特殊计算机上，该服务器接受并响应 Web 浏览器对页面及其相关文件的请求。要使用此类服务，你需要注册一个提供其服务器空间的服务。因为该服务实际上充当了你的文件的主机，所以它被称为*网络托管提供商*或*网络托管服务*。

### B.3.1 在选择网络托管服务时应该注意什么

当你评估网络托管服务时，应该使用哪些标准？答案取决于你想要设置的网站类型，但以下标准是最常见的：

+   *最大带宽*—托管服务每月将传输到 Web 浏览器的最大数据量。在大多数情况下，超出月度最大数据量的数据需要额外付费。一些网络托管服务提供无限带宽。

+   *总磁盘空间*—你在 Web 服务器上获得的硬盘存储空间。至少，总磁盘空间通常是几百兆字节，对于简单的网站来说已经足够了。

+   *网站数量*—你可以设置的根文件夹数量。

+   *电子邮件地址数量*—包含在托管服务中的电子邮件地址数量。

+   *域名托管*—网络托管服务是否也托管了你之前从域名注册商那里购买的域名。一些托管商销售域名，而另一些则提供免费子域名，形式为*yourdomain*.*webhostdomain*.com。

+   *FTP 支持*—对*文件传输协议*（FTP）的支持，这是你用来将文件传输到网络托管服务的互联网服务。几乎所有的网络托管服务都支持 FTP，但有些只提供专有的文件传输服务。

通常情况下，网络托管服务越便宜，可用的这些功能就越少。在你开始寻找网络托管服务之前，列出一个这些功能的清单，并决定你需要什么以及什么是可以选择的。对于像最大带宽这样的功能可能比较困难，因为带宽部分取决于你的网站有多受欢迎，但你现在可以尽力为每个功能做出最佳猜测。当你寻找网络托管服务时，你有三个主要选择：

+   *你的互联网服务提供商*（ISP）—你用来访问互联网的公司或机构也可能提供网络托管服务。许多 ISP 为简单的个人网站提供免费网络托管服务，并且一些组织网络包括你可以使用的 Web 服务器。在大多数情况下，托管服务包括带宽和磁盘空间等低端功能。

+   *免费网络托管提供商*—许多服务会免费托管您的网页。但是，您通常对大多数托管功能有相当严重的限制，尤其是带宽和磁盘空间，并且您几乎总是只能获得一个网站。一些免费网络托管商也会显示广告，尽管现在这种情况越来越少了。

+   *商业网络托管提供商*—如果您希望为您的网络存在提供合理的一套功能，您需要支付费用来租用商业网络托管提供商的空间。请注意，我并不是在谈论大笔的钱。流行的提供商，如 Bluehost ([www.bluehost.com](https://www.bluehost.com))、GoDaddy ([www.godaddy.com](https://www.godaddy.com)) 和 HostGator ([www.hostgator.com](https://www.hostgator.com))，提供功能齐全的托管服务，通常每月费用不到 5 美元。如果您认为您将从事超出创建基本主页的网页设计，您应该考虑使用商业网络托管。

当您与网络托管商签约后，通常需要几分钟到几小时的时间才能准备就绪。当您的托管服务准备就绪时，就是将您的文件上传到网上的时候了。

### B.3.2 上传您的文件

当您的 HTML 和 CSS 文件编码并验证无误，支持文件（如图片）就位，文件夹设置完成，您的网络托管商准备好向等待的世界提供服务时，剩下的就是将您的文件从您的计算机发送到网络托管商的服务器——这个过程被称为*上传*。您如何上传文件取决于您的网络托管商，但以下三种方法是迄今为止最常用的：

+   *FTP*—大多数托管商提供对 FTP 上传的支持。首先，您需要为自己获取一个*FTP 客户端*，这是一个软件程序，可以连接到您的网络托管商的 FTP 服务器，并提供基本文件操作的用户界面，例如导航和创建文件夹、上传文件以及删除和重命名文件。流行的 Windows 客户端有 CuteFTP ([www.globalscape.com/cuteftp](https://www.globalscape.com/cuteftp)) 和 Cyberduck ([`cyberduck.io`](https://cyberduck.io))。对于 Mac 用户，可以尝试 Transmit ([`panic.com/transmit`](https://panic.com/transmit)) 或 FileZilla ([`filezilla-project.org`](https://filezilla-project.org))。下载软件后，请查看您的网络托管商的支持页面，获取如何连接到托管商 FTP 服务器的信息。

+   *cPanel*—许多网络托管商提供一种名为 cPanel 的管理工具，它提供了一个简单的界面，用于处理诸如电子邮件和域名管理之类的托管任务。cPanel 还提供了一个文件管理器组件，您可以使用它上传文件并执行其他文件管理任务。

+   *专有*—一些网络托管商提供他们自己的上传和文件操作界面。请参阅您的托管商支持页面以获取说明。

无论可用什么方法，都要将所有网站文件和文件夹上传到你的主机根目录。然后，将你的网站加载到你喜欢的网页浏览器中，以确保一切正常工作。尝试在几个不同的浏览器和设备上测试你的网站，以确保它对广泛的用户都能正常工作，这不会有害。

# 附录 C. 学习一些 ChatGPT 最佳实践

网页开发者知道，创建网页是一门既包含艺术又包含技术的手艺，既包含设计又包含编码。我对这本书的主要假设是，你不想（或者没有时间或兴趣）成为一名网页开发者。因此，你在本书中学到的手艺是引导 ChatGPT 生成你想要上线网页所需的代码和文本的手艺。

将 ChatGPT 引导去做你的网页创建任务的一大关键部分是使用你的提示尽可能清晰地列出你想要的内容。这正是书中所有提示背后的目标。然而，提示 ChatGPT 是一种艺术，这意味着有无数微妙的方式来改进你的提示以获得更好的结果。你可能会发现（ fingers crossed!）这本书的提示为让 ChatGPT 帮助你构建网站提供了足够好的起点。如果这样，太好了！然而，如果不这样，也不要绝望。正如这个附录所示，有相当多的技巧、窍门和最佳实践可以帮助 ChatGPT 生成高质量的网页代码和文本。

## C.1 请求 ChatGPT 扮演一个角色

ChatGPT 的一个令人惊讶的特性是它可以在对话中采用指定的角色——例如，教师、顾问或数据分析师。告诉模型“它是谁”不仅为 ChatGPT 提供了一个生成输出的整体视角，而且将对话置于一个更具体的上下文中，这通常有助于模型制定更针对性的结果。

对于网页创建，你可以从以下示例角色提示开始你的对话：

+   *你是一名网页设计顾问*。

+   *扮演一个资深网页开发者*。

+   *提供前端网页工程师会编写的代码*。

+   *你是一名网站营销经理*。

小贴士：为了帮助你编写角色提示，请参阅 GitHub 仓库“Awesome ChatGPT Prompts”：[`github.com/f/awesome-chatgpt-prompts`](https://github.com/f/awesome-chatgpt-prompts)。

当然，你也可以要求 ChatGPT 扮演任何适合你需求的角色，这在请求帮助生成网页文本时特别有用。

## C.2 详细信息比简略信息更好

如果你没有在提示中包含重要信息，ChatGPT 会尝试猜测你想要的内容，这几乎肯定不会产生高质量的结果！不要害怕在你的提示中添加显著细节，以便 ChatGPT 的转换器部分有所依据。

例如，考虑以下提示（来自第一章）：

```py
Write web page code to display "Hello World" in a large font.
```

这里使用“大”这个词比较模糊，所以 ChatGPT 会猜测你想要的文本大小。例如，在第一章中，我展示了一些 ChatGPT 生成的代码，该代码以 48 像素的字体格式化文本。然而，如果你知道你想要文本以 72 像素的字体显示，请将其添加到你的提示中：

```py
Write web page code to display "Hello World" in a 72-pixel font.
```

以下是从这个提示生成的 ChatGPT 的一些示例代码：

```py
<!DOCTYPE html>
<html>
<head>
    <title>Hello World</title>
    <style>
        h1 {
            font-size: 72px;
        }
    </style>
</head>
<body>
    <h1>Hello World</h1>
</body>
</html>
```

警告：大型语言模型（LLM）如 ChatGPT 被训练产生不（或不是总是）无聊或平淡无奇的输出的一种方式是在过程中加入一些随机性。这种随机性首先意味着 ChatGPT 不一定从相同的提示中生成相同的结果，其次，有时 ChatGPT 似乎故意不理解你的提示。对于后者，几乎总是最好的策略是清除当前对话并重新开始。

在提示 ChatGPT 时，细节通常是你的朋友，但如果你发现模型超时、困惑或产生不完整的成果，过多的细节可能是罪魁祸首。在这种情况下，尝试将详细提示分解为两个或更多较不详细的提示。

## C.3 设置输出长度

当你与 ChatGPT 合作生成文本时，根据提示，ChatGPT 可能会输出一个长且/或详细的成果。这个冗长的结果可能正是你想要的，但网页组件通常在能容纳多少文本方面有所限制。例如，你可能希望产品描述只足够大，可以适应卡片组件；同样，你可能希望一些常见问题的答案简短明了。

因此，当提示 ChatGPT 生成网站文本时，你通常会希望文本有一个最大长度。这可能是一篇 200 字的短文、3 个段落、4 个句子，或者 5 个要点。无论长度如何，务必将其作为你提示的一部分。以下是一些示例：

+   `回答问题“为什么杰里·刘易斯在法国如此受欢迎？”。答案不超过 100 字`。

+   `用三个段落写一篇立方氧化锆珠宝的购买指南`。

+   `列出在印第安纳波利斯布罗德里普区可以做的十个有趣的事情`。

提示：ChatGPT 很可能会在其第一次响应中忽略你建议的输出长度！这对于用单词、段落和句子表示的长度尤其如此。一旦响应完成，运行后续提示，要求 ChatGPT 将答案缩减到你在原始提示中指定的长度。

设置输出长度是约束的一个例子，它指的是任何以某种方式限制 ChatGPT 响应的提示方面。以下是一些可以尝试的示例约束：

+   `以` *`X`* （其中 *`X`* 是作者或出版物）的风格撰写你的输出`。

+   `以` *`X`* （其中 *`X`* 是形容词或形容词短语，如 *学术的*、*随意的*或*适合 10 岁孩子的*）的方式撰写文本`。

+   `使文本` *`X`* （其中 *`X`* 是一个形容词，如 *vivid*，*lively* 或 *humorous*）。

限制你的请求是让 ChatGPT 写出更有趣文本的好方法。

## C.4 使用三重引号限定额外的文本输入

如果你为 ChatGPT 提供额外的文本输入，请用三重引号包围输入，并在你的提示中包含这一事实。例如，在一个之前的项目中，我要求 ChatGPT 写一篇关于诗人沃尔特·惠特曼的简短传记。我复制了这篇传记，然后将其粘贴到以下提示中：

```py
Create a limerick from the text surrounded by triple quotation marks.

"""Walt Whitman (1819-1892) was an American poet, essayist, and journalist, known as one of the most influential poets in the American canon. He was often called the "father of free verse" because of his unconventional use of form.

Whitman was born on May 31, 1819, in West Hills, New York. His family moved to Brooklyn when he was a child, where he attended public school before leaving at age eleven to work in a series of jobs such as office boy, printer's apprentice, and teacher.

In 1841, Whitman turned his interests to journalism and founded the "Long Islander," a weekly newspaper. He continued to write and edit for various periodicals throughout the 1840s and became known for his progressive views, championing issues like workers' rights and women's suffrage.

Whitman's groundbreaking poetry collection "Leaves of Grass," first published in 1855, was unlike any poetry that had been seen before in its free verse form and candid content. This volume, which he revised and expanded throughout his life, explored themes of democracy, sexuality, death, and the individual's place in the universe.

During the American Civil War, Whitman worked as a government clerk and volunteered as a nurse in an army hospital in Washington, D.C. His experiences with wounded soldiers and the realities of war deeply impacted him and influenced much of his later work, notably his poem "O Captain! My Captain!" mourning the death of President Lincoln.

Whitman continued to write and publish his work until his death on March 26, 1892, in Camden, New Jersey. His innovative style and uniquely American voice have made him a staple in the study of American literature."""
```

ChatGPT 以以下小曲接受了挑战：

```py
In New York, a poet named Whit,
Whose verse was a free-forming hit.
From "Leaves of Grass" sprang,
A new style Whitman sang,
In America's canon, he sits.
```

包含示例文本在你希望 ChatGPT 使用你自己的写作风格生成新文本时特别有用。例如，你可以这样说：

```py
Using the same style as the text surrounded by triple quotation marks, write a short essay on the nutritional benefits of eating rutabagas.
"""*Include a few paragraphs of your own writing here*"""
```

当在你的提示中包含示例文本时，请记住，大多数 ChatGPT 查询限制在大约 500 字（大约是早期谜语提示字数的两倍）。记住（正如我在第七章中解释的），你可以通过导航到包含 ChatGPT 需要参考的文本的页面，然后使用 Copilot 侧边栏来编写你的提示，来使用 Copilot 绕过这个限制。

## C.5 一个例子胜过千个提示

如果你要求 ChatGPT 输出不寻常或深奥的内容，模型可能无法理解你的需求。为了将 ChatGPT 引向正确的方向，请包含两到三个你期望的输出类型的示例。以下是一个示例：

```py
Create a dozen unique insults of the form "Not the Xest Y in the Z", replacing X, Y, and Z with related terms. For example: "Not the sharpest knife in the drawer", "Not the quickest bunny in the forest", "Not the brightest crayon in the box."
```

提示：这里显示的提示是一个*模板提示*的示例，你给 ChatGPT 一个包含一个或多个占位符（*`X`*，*`Y`* 和 *`Z`*）的整体模式（`"Not the *X*est *Y* in the *Z*"`），并告诉 ChatGPT 你希望它如何替换每个占位符。

然而，在花费时间想出例子之前，通常最好在没有例子的情况下单独尝试提示。ChatGPT 接受了大量文本的训练，它通常在第一次就能理解甚至晦涩的请求。

## C.6 翻转对话方向

大多数你的 ChatGPT 对话都是单向的，你要求模型执行某些任务，而模型（希望）成功完成请求。如果你没有得到高质量的结果，那可能是因为你没有给出足够好的提示，让 ChatGPT 能够理解你的需求。你知道谁可能能够找出正确的提示吗？ChatGPT！也就是说，与其不断打扰 ChatGPT 要求输出，不如反过来，让 ChatGPT 询问你需要的信息。

这里有一些示例提示：

+   `问我你需要我回答的任何问题，以便为我网站的“关于”页面创建一个页面`。

+   `我想创建一个产品的网页卡片。请问我需要哪些信息，直到你收集到足够的信息来生成卡片的 HTML 和 CSS 代码`。

+   `我想让你帮我写一个短篇故事。你需要从我这里得到哪些信息？请一次问一个问题`。

注意，在每种情况下，提示都包含一个特定的结果、目标或结果。这一点很重要，因为它使 ChatGPT 能够生成适当的问题。

## C.7 让 ChatGPT 改进你的提示

当你使用 ChatGPT 生成网页代码时，会遇到的一个问题是，由于你不是自己是一名网页开发者，你无法确定你的提示是否措辞正确，是否提出了正确的问题，或者是否寻求的是根本不可能实现的东西。本书的主要目标之一是给你足够的示例提示，让你熟悉从 ChatGPT 那里可以请求的广泛范围。然而，如果你发现自己处于新领域，请尽可能地向 ChatGPT 发出提示。如果结果不是你想要的，你可以要求 ChatGPT 为你改进提示：

+   你能建议一个比我之前提示更好的版本吗？

+   “我的上一个提示中有什么遗漏的东西可以帮助你生成更好的响应吗？”

+   在以下对话中，每次我让你生成一些代码时，建议一个比我请求更好的版本，并问我是否更喜欢使用这个版本而不是原始版本。

如果你能提供一些背景信息，也可能有所帮助。例如，如果你正在尝试创建更易于访问的网页，让 ChatGPT 知道，这样它的改进提示就可以考虑这个目标。

## C.8 让 ChatGPT 为你创建步骤

如果你想要学习如何执行某些复杂任务（例如，将你的网站部署到本书未涵盖的托管服务提供商），你可以要求 ChatGPT 为你提供完成该任务的步骤。对于这种提示，你通常需要给 ChatGPT 以下信息：

+   你试图完成的目标或任务

+   与该目标或任务相关的信息，你已经知道什么，或者你已经执行了哪些步骤

+   完成目标或任务需要哪些步骤

+   与你尚未拥有或尚未执行的信息相关的任何步骤

这里有一个示例提示，要求 ChatGPT 提供将网站发布到 Vercel 所需的步骤：

```py
I want to deploy my website to Vercel. I know I need a Vercel account. I have completed my website and all the files are in the my_app folder on my computer. What steps are required to deploy my website to Vercel? Please provide detailed information for each step I haven't yet completed.
```

类似的方法是要求 ChatGPT 告诉你如何使用它为你生成的网页代码。例如，如果 ChatGPT 给你一些代码，但你不确定代码应该在 HTML 文件中的哪个位置，你可以要求 ChatGPT 告诉你如何在文件中放置代码。

## C.9 让 ChatGPT 提供并评估替代方案

对于除了最简单的设计之外的所有设计，总会有多种方法来编写网页或页面组件。在 ChatGPT 提供其初始输出后，你总是可以点击“重新生成响应”来获取另一块代码，但你怎么知道哪个响应是你应该使用的呢？当然，你可以要求 ChatGPT 不仅提供实现目标的替代方法，还要对这些方法进行评级。以下是一些示例：

+   `我想在我的网页上添加一个响应式下拉菜单。如果有多种实现该目标的方法，请列出三种最佳方法`。

+   `列出我可以添加到我的网页中的导航栏的最多四种方法，并告诉我每种方法的优缺点`。

+   `告诉我将表单数据通过电子邮件发送给我的最流行的方法，并比较和对比每种方法`。

根据提示，你可能更喜欢使用 Copilot，它可以使用网络搜索来帮助它评估每个选项。

## C.10 在 Microsoft Copilot 中选择适当的对话风格

如果你正在使用 Copilot，请确保选择适合你任务的对话风格：

+   *更具创意*——当你希望 Copilot 展翅高飞，换句话说，生成更不传统、更具想象力或创新性的文本或想法时，这种风格最佳。这个版本的 Copilot 可以生成真正疯狂的文字，但容易声称其虚构的输出是事实，因此*消费者注意*。这种风格的输入限制为 4,000 个字符。

+   *更精确*——当你想要简洁、简单、直接的结果时，这种风格最佳。这种风格的输入限制为 4,000 个字符。

+   *更平衡*——这是默认风格，它将 Copilot 呈现为一个友好、信息丰富的助手，其结果介于创新和直接之间。这种风格的输入限制为 2,000 个字符。

在生成网页代码时，通常最好尝试更精确的风格，它生成的代码相对没有不必要的装饰。

## C.11 解决 ChatGPT 的错误

ChatGPT 是如何做到它的，并不是一个很大的秘密，当然也不是魔法，但正如你在本书中学到的，它确实非常令人印象深刻。然而，这种印象深刻并不意味着 ChatGPT 是完美的——远非如此。是的，幸运的是，大多数时候你从 ChatGPT 得到的响应是代码，不仅符合你的要求，而且还能正常工作（意味着当你将代码显示在网页浏览器中时，你会看到你要求的内容和样式）。然而，理解这一点至关重要，尽管很多人称 ChatGPT 为“AI”，但它甚至远非智能。它可以——不幸的是，经常这样做——生成不准确、错误或有时完全是胡说八道的代码。更糟糕的是，ChatGPT 会以与它展示“好”代码相同的愉快自信来展示这些“坏”代码。ChatGPT 根本不知道这两者之间的区别。

因此，你面临着一个大问题：既然你不知道（并且可能不想知道）如何编写网页代码，你如何“修复”ChatGPT 创建的任何代码问题？幸运的是，你并不孤立无援，因为你有一些方法可以让 ChatGPT 帮助修复它自己的问题：

+   请 ChatGPT 重新生成其响应。有时需要第二次甚至第三次尝试才能得到正确的结果。

+   修改您的提示。如果您的原始提示很简单，尝试添加更多细节；如果您的原始提示很复杂，尝试将其分解成多个简单且/或专注于单个任务的提示。

+   要求 ChatGPT 生成一个或多个它认为适合您所寻找输出的提示。

+   告诉 ChatGPT 生成的代码无法工作，并要求它修复问题。您会惊讶地发现这有多么频繁地有帮助！

我希望您不必经常切换到故障排除模式，因为 ChatGPT 确实擅长生成网页代码。

# 索引

符号

`<button>` 标签 20

`<em>` 标签 93

`<figcaption>` 标签 189

`<h1>` 标签 19, 20, 37

`<h2>` 标签 37

`<h3>` 标签 37

`<img>` 标签 170

`<label>` 标签 145

`<li>` 标签 153, 166

`<link>` 标签 92

`<ol>` 标签 153

`<p>` 标签 19, 145, 166

`<strong>` 标签 93

`<title>` 标签 20

`<head>` 标签 199

`<link>` 标签 39, 57, 74, 90, 116, 139, 162, 182, 183

`<nav>` 标签 86

`<p>` 标签 80, 189, 220

`<script>` 标签 183

A

折叠面板 66

`action` 属性 143

自适应布局 227

在文章中添加段落 220

扮演角色 281

美学 69

`alt` 属性 171, 189

替代方案，要求 ChatGPT 提供并评分 286

替代文本，标记 223

数组 20

箭头字符 152

文章元素 215 – 217, 229, 237, 247

文章页面 211, 213

添加内容 232

调整小屏幕布局 227

文章元素 215

定制 HTML 237

为其创建提示 229

CSS 网格 225

检查代码 234 – 236

CSS 235 – 236

HTML 234

HTML 页面布局元素 213

在侧边栏中包含 216

标记特殊单词和短语 221 – 223

替代文本 223

强调文本 223

重要文本 222

关键字 222

项目概述 212 – 213

文章

添加段落 220

添加章节 218

首字母下沉 224

aside 元素 215 – 218, 229, 232, 237

B

后端代码 6

background-color 属性 145, 166, 189, 258

带宽 271

b 元素 222 – 223

最佳实践

让 ChatGPT 为您创建步骤 285

让 ChatGPT 提供并评估替代方案 286

精炼提示 285

body 元素 166, 189

body 规则 121

粗体关键字 32

边框声明 209

边框属性 50

border-radius 属性 197

边框 48 – 52

用边框包围元素 50

border-top 属性 146

box-shadow 声明 208

box-shadow 属性 196

浏览器，测试网页 24

br 标签 60

项目符号列表 149

更改项目符号类型 152

处理较长的列表项 150

嵌套 150

项目符号 149

按钮元素 143

C

标题 175

卡片

添加阴影 196

构建 193

将图片扩展到边缘 195

制作响应式页面 198

圆角 197

ChatGPT

账户访问 262

最佳实践 280

采用角色扮演 281

请求 ChatGPT 为您创建步骤 285

详细信息 281

提示语示例 284

输出长度 282

构建表单 129 – 136

为每个控件添加标签 131

使用单选按钮选择多个选项 133

使用文本框收集文本 129

使用复选框获取是或否信息 132

使用文本区域处理更多文本 131

使用列表提供更多选择 134

指定表单端点 129

使用按钮提交表单 136

构建网页 46 – 57, 260

图片 52 – 53

填充、边框和边距 48 – 52

页脚 47

页眉 46

提示语 54 – 57

社交媒体链接 53

对话，翻转方向 284

复制网页代码 22

概述 2 – 5

将数据粘贴到 HTML 文件中 267

提示生成网页代码 16 – 21

检查单页网站提示语 20

检查结果 17 – 20

精炼提示 285

测试代码 263 – 267

从 ChatGPT 复制数据 263

将数据粘贴到在线编码沙盒 264

故障排除错误 287

创建网页的要求 260

使用创建网站 5

用写作 102 – 110

生成想法 102

为主题撰写生成想法 103

HTML 标签 110

研究主题 104

重写帖子文本 109

用自己的声音写作 106 – 109

ChatGPT Plus 订阅 262

复选框 132

复选标记字符 152

圆形字符 152

克拉克的三大定律 3

类属性 78

类值 60

Cloudflare Pages 270

更改站点域名 277

创建新应用 274

部署站点 276

设置账户 274

使用对话框上传文件 276

通过拖放上传文件 275

代码

复制 22

检查 58 – 61，75 – 78

用于主页 116 – 121

CSS 118

定制 120

HTML 117 – 118

进入文件 9

CodePen 266

颜色参数 51

颜色属性 145，146，167，189，258

颜色 27

颜色方案，生成 34

cols 属性 145

商业网络托管提供商 278

约束 283

内容

添加到文章页面 232

构建主页 111 – 116

英雄图片 111

提示 113 – 116

对话，翻转方向 284

对话风格，在 Microsoft Copilot 中选择 286

Copilot 图像创建器 68, 72

复制 13

角落，圆角 197

课程目录

自定义 258

检查代码 252

检查 HTML 252

获取并显示 JSON 数据 247

过滤数据 248 – 250

交互式

编码 239

结论 258

JavaScript 255

项目概述 240

提示 250

搜索、排序和过滤数据 248 – 250

课程目录项目

Excel 和 241 – 247

准备数据 241

JSON 数据格式 242 – 244

提示 ChatGPT 将 Excel 数据转换为 JSON 245

将 Excel 文件上传到 ChatGPT 244

CSS（层叠样式表）

自定义代码 62

检查代码 60, 77, 235 – 236

检查注册事件页面代码 144

网格 225

主页代码 118

在 HTML 文件中引用文件 268

草书字体 30

D

DALL-E 使用 67 – 72 生成图像

访问 68

提示 69

保存生成的图像 72

日期字段 143

部署，定义 13

部署 HTML 文件 10

部署网站 270

到 Netlify 271 – 273

更改子域名或域名 273

设置账户 271

使用对话框上传文件 272

通过拖放上传文件 271

详细信息元素 72

对话框，使用 272 上传文件

光盘 152

显示，flex 声明 87

div 元素 198

域名

更改 273

托管 278

拖放，通过拖放上传文件 271

首字母下沉 224

投影阴影 196

动态网页 6

E

强调元素 223

强调文本，标记 223

端点 129

错误，故障排除 287

事件处理器 178

事件注册页面

为 137 – 140 编写提示 137

自定义 145

检查代码 140 – 145

CSS 144

HTML 141 – 143

Excel，课程目录项目 241 – 247

准备数据 241

JSON 数据格式 242 – 244

指示 ChatGPT 将 Excel 数据转换为 JSON 245

将 Excel 文件上传到 ChatGPT 244

表达式，解释 228

F

幻想字体 30

获取方法 247

文件，网页。*见*网页，文件

一级标题 37

等宽字体 30

使用 Flexbox 布局照片库 178

浮点值 146, 167

Font Awesome 54

字体家族属性 30

字体 27

字体大小属性 19, 31

字体样式属性 32

字体粗细属性 32

页脚元素 100, 101, 189, 214

表单元素 143

表单 125

构建 129 – 136

为每个控件添加标签 131

使用单选按钮选择几个选项之一 133

使用文本框收集文本 129

使用复选框获取是或否信息 132

使用文本区域处理更多文本 131

使用列表提供更多选择 134

指定表单端点 129

使用按钮提交表单 136

免费网页托管提供商 278

Fritterware 7

前端代码 6

FTP 客户端 279

FTP (文件传输协议) 278, 279

G

生成式 AI 3

Getform 服务 127 – 128

GPT-4 (生成式预训练变换器 4)，使用 67 – 72 生成图像

grid-template-columns 值 237

H

h3 元素 233

标题元素 100, 101, 112, 167, 189, 213

标题 27

网页 36

心形字符 152

英雄图片 101, 111

主页

构建 111 – 116

英雄图片 111

提示 113 – 116

代码 116 – 121

HTML 117 – 118

CSS 118

定制 94, 120

检查代码 91 – 93

CSS 93

HTML 91 – 92

个人 28

蜜罐，定义 128

href 属性 85, 86

HTML (超文本标记语言)

文章元素 215

定制文章页面 237

定制代码 61

检查代码 58 – 60, 75 – 77, 234, 252

检查事件注册页面代码 141 – 143

主页代码 117 – 118

页面布局元素 213

将 ChatGPT 数据粘贴到文件中 267

在文件中引用 CSS 和 JavaScript 文件 268

将代码保存到 HTML 文件 22

HTML 标签 94, 120

使用 ChatGPT 写作 110

I

使用 ChatGPT 生成想法 102

关于主题写作 103

i（斜体）元素 223

插图 69

图片 52 – 53, 170 – 175

`<img>`标签 170, 189

标题 175

扩展到卡片边缘 195

全宽 100

使用 GPT-4 和 DALL-E 生成 67 – 72

占位符图片 171

缩略图 172 – 174

使用 macOS 预览应用创建 174

使用 Windows 照片应用创建 173

重要文本，标记 222

信息网站首页 84 – 91

为...编写提示 87 – 91

创建链接 84

创建导航栏 86

输入元素 143

斜体关键字 32

J

JavaScript

检查 255

在 HTML 文件中引用文件 268

JSON（JavaScript 对象表示法） 242

课程目录项目 242 – 244

提示 ChatGPT 将 Excel 数据转换为 JSON 245

获取并显示数据 247

K

关键词，标记 222

L

标签 131

弹出层 177

弹出层覆盖 176

行高声明 121

链接

创建 84

检查首页代码 91 – 93

CSS 93

HTML 91 – 92

导航和项目概述 82 – 83

列表项 149

列表 147

编号 152 – 158

更改列表的起始数字 154

更改编号样式 157

嵌套 156

反转列表顺序 154

...概述 148 – 149

菜单页面

检查代码 162 – 166

CSS 165

HTML 163 – 165

列表样式类型属性 166

li 标签 149

LLM (大型语言模型) 2, 262

小写字母关键字 166

M

macOS 预览应用 174

主元素 97, 100, 101, 120, 214, 217, 237

边距 48 – 52

与...一起工作 51

最大带宽 277

最大宽度值 121, 167

媒体查询 199, 228

meta charset 标签 59

微软 Copilot 4

选择对话风格 286

在 Bing 中 3

等宽字体 30

N

名称属性 143, 145

nav 元素 87, 213

导航栏，创建 86

导航元素 100, 101

Netlify 270 – 273

更改子域名或域名 273

设置账户 271

使用对话框上传文件 272

通过拖放上传文件 271

编号列表 152 – 158

更改列表的起始数字 154

更改编号样式 157

嵌套 156

反转列表顺序 154

O

ol 元素 166

在线期刊页面 *见* 页面帖子

OpenAI 应用 3

OpenAI DALL-E 应用 68, 72

输出长度 282

P

填充 48 – 52

添加 50

用边框包围元素 50

与边距一起工作 51

填充简写属性 50

页面页脚 47

页面页眉 46

页面帖子

构建在线期刊页面 66 – 75

手风琴 66

撰写提示 72 – 75

使用 GPT-4 和 DALL-E 生成图像 67 – 72

页面

文章，包括侧边栏 216

文章页面 213

向 232 添加内容

自定义 61

CSS 代码 62

HTML 代码 58 – 61

检查代码 58 – 61

CSS 60

使其响应式 198

页面副标题 101

页面标题 101

段落，添加到文章 220

p 元素 214

个人主页

构建 29 – 40

撰写提示 37 – 40

生成配色方案 34

从 ChatGPT 获取字体建议 32

设置字体大小 31

网站标题和副标题建议 29

设计字体样式 30

网页标题 36

与字体样式一起工作 32

自定义 42

检查代码 40 – 42

CSS 41

HTML 40

照片画廊 168

为 180, 184 撰写提示 180, 184

自定义 189

检查代码 184 – 188

CSS 186

HTML 184 – 186

JavaScript 188

图片 170 – 175

`<img>` 标签 170

标题 175

使用 macOS 预览应用创建 174

使用 Windows 图片应用创建 173

占位符图片 171

缩略图 172 – 174

实现弹出层覆盖 176

使用 Flexbox 布局 178

弹出层 177

项目概述 169

占位符属性 145

占位符图片 171

在游乐场中粘贴数据 264

站点页面 191 – 192

构建 193 – 199

添加阴影 196

卡片 193

将图片扩展到卡片边缘 195

制作响应式页面 198

圆化角落 197

为制作提示 199 – 204

定制 208

检查代码 204 – 208

CSS 206

HTML 205 – 206

项目概述 192 – 193

帖子

检查代码 75 – 78

CSS 77

HTML 75 – 77

页面帖子 65

预训练 2

最大化隐私 262

提示-复制-保存-部署周期，重复 11

提示 13, 54 – 57

为其他网站页面构建 122

为活动注册页面制作 137 – 140

工程学 8

为信息网站主页制作 87 – 91

为其他网站页面制作 97

提示 ChatGPT 8

精炼和修改 11

属性 19

p 标签 60

px 单位 121, 146, 167, 237

R

单选按钮 133

菜单页面

定制 166

为...制作提示 158 – 162

检查代码 162 – 166

CSS 165

HTML 163 – 165

相对测量 227

rem 单位 121, 146, 237

反转列表顺序 154

rgba() 函数 121, 189, 197

向右箭头字符 152

行属性 145

规则 20

S

无衬线字体 30

第二级标题 37

区分元素 94, 120, 214, 233, 247

部分，添加到文章中 218

区分标签 94

选择列表 134

语义 223

有衬线字体 30 – 31

添加阴影 196

侧边栏，包括在文章页面中 216

网站内容

为其他网站页面构建提示 122

创建 99

网站表单

定制事件注册页面 145

为事件注册页面制作提示 137 – 140

检查事件注册页面代码 140 – 145

CSS 144

HTML 141 – 143

生成 125

Getform 127

项目概述 126

网站标题和副标题建议 29

大小属性 145

笑脸字符 152

社交媒体链接 53

span 元素 224

特殊单词和短语，标记 221

替代文本 223

强调文本 223

重要文本 222

关键词 222

方形字符 152

src 属性 171

src 值 59

星号字符 152

静态网页 6

强调元素 222, 223, 224

样式值 51

摘要元素 72 – 73

T

标签。*另见*单个标签 19

模板提示 284

测试代码 263 – 267

从 ChatGPT 复制数据 263

将数据粘贴到在线编码沙盒中 264

测试，浏览器中的网页 24

文本对齐值 146

文本区域 131

文本框 129

三级标题 37

缩略图 172 – 174

使用 macOS 预览应用创建 174

使用 Windows 照片应用创建 173

标题 240

主题，使用 ChatGPT 进行研究 104

转换器 2

三重引号 283 – 284

类型属性 143, 145

字体

从 ChatGPT 获取建议 32

样式 30

类型大小，设置 31

字体样式，协同工作 32

U

UI 卡片（用户界面卡片） 193

无序列表标签 149

无序列表 149

URL（统一资源定位符） 85

V

值属性 143, 145

查看 ChatGPT 的结果 8

W

网页设计沙盒 264

WebDev 工作台 265

网络托管提供商 277 – 279

网页

构建 46 – 57

图片 52 – 53

填充、边框和边距 48 – 52

页面页脚 47

页面标题 46

提示词 54 – 57

社交媒体链接 53

与 ChatGPT 一起 260

复制代码 22

创建和部署 14, 24

流程 15

部署 24

文件 267 – 269

将 ChatGPT 数据粘贴到 HTML 文件 267

在 HTML 文件中引用 CSS 和 JavaScript 文件 268

保存工作 269

类型 267

引导 ChatGPT 生成代码 16 – 21

检查单页网站提示词 20

检查结果 17 – 20

创建要求 260

将代码保存到 HTML 文件 22

结构，概述 45

在浏览器中测试 24

网站创建

为项目 100 – 101

其他网站页面的提示词 97

页面类型 6

与 ChatGPT 一起，概述 2 – 5

网站页面

自定义 78

发布页面帖子 64 – 65

网站标语 100

网站标题 100

白钻石字符 152

宽度值 51

Windows 照片应用 173

与 ChatGPT 一起写作 102 – 110

生成想法 102

为写作话题生成想法 103

HTML 标签 110

研究话题 104

重写帖子文本 109

用自己的声音写作 106 – 109
