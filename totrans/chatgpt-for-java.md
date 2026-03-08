![封面图片](img/chatgpt-for-java-979-8-8688-0116-7_CoverFigure.jpg)《ChatGPT for Java》的封面

# ChatGPT for Java

## ChatGPT 和 Open AI API 的实战开发者指南

前言由 Private AI 的联合创始人兼首席执行官 Patricia Thaine 撰写![封面图片](img/chatgpt-for-java-607613_1_En_BookFrontmatter_Figa_HTML.png)

Apress 标志。

布鲁斯·霍普金斯

本 Apress 出版社由注册公司 APress Media, LLC 出版，该公司是 Springer Nature 的一部分。

注册公司地址为：1 New York Plaza, New York, NY 10004, U.S.A.

前言

在过去几年中，我有幸认识布鲁斯，亲眼目睹了他将尖端概念和问题转化为来自不同背景和能力的程序员能够理解的能力。布鲁斯的经验特别适合将许多最新的 AI 技术，如 ChatGPT，分解成开发者可以在日常问题解决中使用的核心组件。他是《Bluetooth for Java》的合著者，这本书在蓝牙进入市场后仅四年就出版了，他还是为需要其最新发明被开发者采用的各大科技公司撰写的大量技术指南的作者。

作为一家由微软支持的 AI 公司 Private AI 的联合创始人和 CEO，我有幸与世界各地的开发者、经理和 C 级高管交谈，不仅关于数据的负责任使用实施，还关于他们对生成式 AI 的疑问，要解决哪些问题，以及从哪里开始。像 ChatGPT 这样的技术如此新颖，使其能够表现得如此出色的底层模型架构——即 Transformer 架构——仅在 2017 年的一篇名为“Attention Is All You Need”的研究论文中首次出现。因此，管理者们所面临的大量关键问题也是开发者们热衷于深入探讨的问题，包括“我能用这项技术做什么？”，“我应该在何处以及如何实施它？”，“我应该从哪里开始？”，“有哪些陷阱？”，以及当大量关注点集中在新的发明上时，始终存在的疑问：“这只是一场炒作吗？”

幸运的是，本书中具体地解决了许多这些问题，这是深入理解新技术实际用途的关键步骤。就像学习编程语言教会你以一种与使用自然语言完全不同的方式思考一样，学习如何充分利用 AI 会使你以一种与编程完全不同的方式思考。在自然语言中，关键是学习词汇、语法、句法和语义。在编程语言中，是逻辑、数学、句法和规模，以及更多关于世界第一原理的理解。在人工智能中，一切都关于数据和它们与手头任务的关系。你可以拥有世界上最强大的用于生成文本、导航道路、生成艺术等任务的模型，但如果你将它们应用于它们本不应完成的任务，准备失望吧。然而，如果你从根本上理解它们被构建来做什么，并相应地使用它们，准备惊讶吧。

本书中的简洁、实用的示例不仅可以帮助你快速开始使用 ChatGPT 构建项目，还可以开始磨练你对如何思考这项技术的直觉。确实，虽然重点是使用 Java 进行工作，但任何编程语言的使用者都能从深入研究这项技术中受益。

> Patricia Thaine
> 
> 联合创始人兼 CEO，Private AI
> 
> [www.private-ai.com](http://www.private-ai.com)

目录第一章：为 Java 开发者介绍 ChatGPT1 本书面向谁？1 章节概述 2 立即下载代码！2 那么，ChatGPT 究竟是什么，为什么我需要使用 OpenAI API？2 正则表达式与 ChatGPT：战斗！5 分析问题#1：谁没有吃到冰淇淋，为什么？7 分析问题#2：哪个孩子可能感到很伤心？9 为了更好地了解 ChatGPT API，让我们忘掉一些词汇 10 模型。模型？模型！！！10 当我们谈论标记时，想想 StringTokenizer 而不是访问令牌 15 温度全在于创造力 16 从 OpenAI 游乐场开始 171. 系统 192. 用户 203. 助手（可选）204. 添加消息（可选）215. 查看代码（可选）216. 模型（可选）217. 温度（可选）228. 最大长度（可选）22 现在试试！通过“系统”角色进行实验 22 结论 23 第二章：将 ChatGPT 作为您的 Java 配对程序员使用 25 创建您的第一个 Java ChatGPT 应用程序：ListModels.java26 模型列表端点 26 创建请求 26 处理 JSON 响应 27 模型（JSON）27 聊天端点 32 创建请求 32 聊天（JSON）33 处理响应 42 聊天完成（JSON）43 等等，我的提示中有多少个标记？46ChatGPT 标记计数器 46 创建下一个 Java 应用程序：ChatGPTClient.java48 结论 56 第三章：在企业中使用 AI！为 Slack 消息创建文本摘要器 57 那么，提示工程是什么？58 使用建造者模式更新 ChatGPTClient.java（和相关类）58ChatGPT 来了，要夺走每个人的工作（其实不是）64 考察一个现实世界的问题：软件公司的客户支持 64 提示工程 101：文本摘要 68 提示#1：“tl;dr”69 提示#2：“用不超过 3 句话解释”71 提示#3：“我是一名经理。向我解释发生了什么”72 提示#4：“给我提供下一步的建议”74 让我们谈谈真正的提示工程 77 注册 Slack 机器人应用程序 77 通过设置范围来指定您的机器人可以（和不能）做什么 80 确认您的设置 82 查看 OAuth 和权限页面 82 将您的 Slack 机器人应用程序安装到工作区 83 获取您的 Slack 机器人（访问）令牌 85 邀请您的机器人到您的频道 86 找到您的频道 ID87 使用您的 Slack 机器人应用程序自动从频道获取消息 87 设置您的依赖项 87 使用 ChannelReaderSla​ckBot.java 从 Slack 以编程方式读取消息 91 留给读者的练习 96 结论 97 第四章：多模态 AI：使用 Whisper 和 DALL·E 3 创建播客可视化器 99 介绍 OpenAI 的 Whisper 模型 102Whisper 模型的特性和局限性 105 转录端点 108 创建请求 108 请求体（multipart 表单数据）109 创建一个分割音频文件的实用应用程序：AudioSplitter.java111 创建音频转录器：WhisperClient.java116 用播客玩玩，试试看 122 元问题：提示工程 GPT-4 为 DALL·E 编写提示 126 创建图像端点 128 创建请求 128 创建图像（JSON）129 处理响应 131 图像（JSON）132 创建图像生成器：DALLEClient.java132DALL·E 提示工程和最佳实践 136DALL·E 黄金法则#1：熟悉 DALL·E 可以生成的图像类型 137DALL·E 黄金法则#2：在前景和背景中描述您想要的内容 138 结论 139 留给读者的练习 140 第五章：使用 Discord 和 Java 创建自动化的社区管理员机器人 141 选择 Discord 作为您的社区平台 142 创建比我们的 Slack 机器人更高级的机器人 143 创建比任何典型 Discord 机器人更高级的机器人 143 了解机器人的角色 144 我们的示例银行：Crook 的银行 144 首先：创建您自己的 Discord 服务器 145 创建问答频道 147 在 Discord 上注册新的机器人应用程序 148 指定机器人的通用信息 150 指定机器人的 OAuth2 参数 151 邀请您的机器人到您的服务器 153 获取您的机器人的 Discord ID 令牌并设置网关意图 155 在 Java 中创建一个问答机器人应用程序来回答频道的提问 158 设置您的依赖项 159 创建第一个 Discord 机器人：TechSupportBotDu​mb.java160 喜欢 Lambda 表达式简化代码 164 处理发送到 Discord 服务器的消息 165 成功！运行您的第一个 Discord 机器人：TechSupportBotDu​mb.java166 简化注册下一个 Discord 机器人应用程序的过程 167 在 Discord 上注册新的机器人应用程序 167 指定机器人的通用信息 168 指定机器人的 OAuth2 参数 168 邀请您的机器人到您的服务器 169 获取您的机器人的 Discord ID 令牌并设置网关意图 169 创建下一个 Discord 机器人：ContentModerator​BotDumb.java169 处理发送到 Discord 服务器的消息 173 再次成功！运行您的第二个 Discord 机器人：ContentModerator​BotDumb.java174 结论 174 留给读者的练习 175 第六章：为我们的 Discord 机器人添加智能，第一部分：使用聊天端点进行问答 177 使 TechSupportBot.java 更智能 178 注意从之前版本的客户支持机器人中做出的重要更改 185 对 onMessageReceive​d()方法的更新 186 分析 ChatGPTClientFor​QAandModeration.java186 使用 JSONPath 在 JSON 文件中快速提取内容 192 运行我们的智能问答机器人：TechSupportBot.java192 我们取得了巨大的成就……但有一个小瑕疵 195 更新系统消息到 ChatGPT 并再次尝试 196 结论 198 第七章：为我们的 Discord 机器人添加智能，第二部分：使用聊天和审核端点进行审核 199 审核端点 201 创建请求 202 创建审核（JSON）203 处理 JSON 响应 203 审核（JSON）204 为审核端点创建我们的客户端：ModerationClient​.java208 使 ContentModerator​Bot.java 更智能 213 注意从之前版本的内容审核机器人中做出的重要更改 219 对 onMessageReceive​d( )方法的更新 220 运行我们的智能内容审核机器人：ContentModerator​Bot.java221 结论 223 留给读者的练习 223 附录 1：OpenAI 模型列表 225 索引 229 关于作者 Bruce Hopkins![图片](img/chatgpt-for-java-607613_1_En_BookFrontmatter_Figb_HTML.jpg)

布鲁斯·霍普金斯的照片。

是一位技术作家和世界知名专家。他既是 Oracle Java 冠军，也是 Intel 软件创新者。布鲁斯还是 Apress 书籍《Bluetooth for Java》的作者。关于技术审稿人万·万·阿斯达尔![../images/607613_1_En_BookFrontmatter_Figc_HTML.png]

万的照片。

是一位拥有 30 多年软件行业经验的技术领导者。他拥有马萨诸塞大学洛厄尔分校计算机信息系统学士学位和密苏里州立大学信息系统硕士学位。他曾担任软件工程师、架构师、经理和教师。万目前在一家顶级金融服务公司领导一个团队，并在密苏里州立大学担任兼职讲师。© 作者（们），独家许可给 APress 媒体公司，Springer Nature 的一部分，2024B. 希金斯 ChatGPT for Java[`doi.org/10.1007/979-8-8688-0116-7_1`](https://doi.org/10.1007/979-8-8688-0116-7_1)

# 1. 为 Java 开发者介绍 ChatGPT

布鲁斯·霍普金斯^(1  )(1)美国俄勒冈州比佛顿

## 这本书适合谁？

首先，这本书是为那些在人工智能、自然语言处理、机器学习或深度学习方面没有任何培训或经验的 Java 开发者而写的。你可能听说过“语言模型”这个术语，但我会假设这不是你每天都会使用的术语。

其次，你可能熟悉（或尝试过）ChatGPT，但你并不完全理解“内部”是如何运作的，你也不确定如何开始，以便将 Java 和 ChatGPT 程序化地结合起来，以“AI 赋能”你自己的应用程序和服务。

注意

虽然 ChatGPT 是一个家喻户晓的名字，但背后的公司 OpenAI 却缺乏广泛的认可。因此，尽管这本书是关于如何在 Java 应用程序中程序化地使用 ChatGPT，但我们将要使用的 API 是官方的 OpenAI REST API。因此，我们将使用“ChatGPT API”和“OpenAI API”同义。

## 章节概述

在本章中，我们将直接深入解释一些你可能不熟悉的术语，然后直接进入 ChatGPT 游乐场。游乐场本质上是一个基于 ChatGPT REST API 构建的开发者网页界面。因此，一旦你熟悉了游乐场，ChatGPT API 的调用和响应将对你来说就像第二本能一样自然。

## 立即下载代码！

![](img/chatgpt-for-java-607613_1_En_1_Figa_HTML.png)

一个下载代码的图标。它类似于一本打开的书，下面有一个向下箭头。

这本书充满了大量的示例和示例代码，那么为什么还要自己输入所有内容呢？下面是 GitHub 仓库的 URL，可以访问源代码。

[**https://github.com/Apress/ChatGPT-for-Java**](https://github.com/Apress/ChatGPT-for-Java)

## 那么，ChatGPT 究竟是什么，为什么我需要使用 OpenAI API？

简而言之，ChatGPT 是由 OpenAI 开发的一组 **语言模型**（这些模型是深度学习算法训练的结果），能够根据给定的 **提示**生成类似人类的文本回复。那么什么是提示呢？提示就是您提供给 ChatGPT 的输入文本。那么让我们先通过给 ChatGPT 提供一个提示来询问它对 Java 设计模式的熟悉程度（见列表 1-1）。描述 3 种 Java 开发者常用的设计模式及其为什么这些模式很重要

PROMPT. 关于 Java 设计模式的简单提示与 ChatGPT

如果你曾经有机会在一家使用 Java 作为专业语言的公司工作，那么你可能在面试中遇到过与上面提示非常相似的问题。列出 1-2 是 ChatGPT 的回答。![聊天 GPT 标志](img/chatgpt-for-java-607613_1_En_1_Figb_HTML.gif)当然！设计模式是针对在软件设计中出现的常见问题的可重用解决方案。它们是经验丰富的开发者经过时间发现和完善的最佳实践。Java 开发者经常利用设计模式，因为这种语言具有面向对象的特点。以下是 Java 中常用的三种设计模式：1. 单例模式：   - 目的：此模式确保一个类只有一个实例，并提供一个全局访问该实例的点。当需要控制对共享资源（如配置管理器或连接池）的访问时，特别有用。   - 重要性：单例模式很重要，因为它提供了一个受控的机制来防止创建类的多个实例，这可以节省内存并同步对资源的访问。此外，它确保使用单例的操作使用的是相同的实例和数据，这在需要一致状态或协调动作的场景中至关重要。2. 观察者模式：   - 目的：此模式定义了对象之间的一对多依赖关系。当一个对象（称为主题或可观察对象）改变其状态时，所有依赖的对象（观察者）都会被通知并自动更新。这是模型-视图-控制器（MVC）架构背后的基本原理，其中模型是主题，视图是观察者。   - 重要性：观察者模式对于构建模块化和解耦的系统至关重要。系统某一部分的更改不会直接影响到其他部分，这使得维护和扩展更容易。此模式还使得在不修改现有代码的情况下添加新的观察者变得更容易，增强了系统的可扩展性。3. 工厂模式：   - 目的：工厂模式提供了一个创建类实例的接口，但具体实现方法和确定要实例化的类由派生子类来完成。它通过消除将应用程序特定的类绑定到代码中的需求来促进松散耦合。代码仅与结果接口或抽象类交互，因此系统可以在不更改调用代码的情况下进化。   - 重要性：使用工厂模式，系统可以更加灵活和可扩展。如果需要引入新产品或修改现有产品，可以做到而不影响现有代码。它封装了对象创建过程，并将其与程序的主要逻辑分离，促进了单一职责原则。这确保了一个类只负责一个原因而改变。所有这些模式，以及许多其他模式，为开发者提供了一种词汇，使得沟通复杂的软件设计和概念更容易。它们体现了对重复问题的解决方案，可以显著加快开发过程，减少错误，并提高代码质量。列出 1-2

**回应**. ChatGPT 对列表 1-1 中提示的回应

不坏，对吧？ChatGPT 不仅能够提供 Java 开发者常用的设计模式列表，还能用自然语言解释为什么它们很重要。

所以，最终，这对 Java 开发者意味着什么呢？实际上，这是一个很大的事情。这是因为开发者现在能够创建能够对自然语言文本进行某种“理解”的应用程序。在 ChatGPT 等 AI 工具出现之前，开发者通常必须创建正则表达式（也称为“regex”），以便在文本中进行基本的字符和字符串模式匹配。然而，模式匹配和自然语言理解是两件完全不同的事情。

## 正则表达式与 ChatGPT：对决！

**注意**

如果你已经知道正则表达式无法执行自然语言理解或情感分析，那么你可以自由地跳过这一部分。

我坚信，每个程序员在其一生中都会遇到某个擅长编写正则表达式的“家伙”。正则表达式很棒，因为它们能够解析大量文本，以编程方式在文本中查找模式。

然而，正则表达式的一个最大的缺点是，一旦编写完成，它们就极其难以阅读（在我看来，即使是最初编写它们的开发者也很难读懂）。

那么，让我们看看正则表达式与具有自然语言处理（NLP）和自然语言理解（NLU）能力的 ChatGPT 相比表现如何。

列表 1-3 讲述了一个不切实际的悲伤情况。然而，它强调了尽管正则表达式可以用来在文本中查找单词和短语，但它不能用来提供任何类型的自然语言理解（NLU）。在美国 Buttersville 市的 Milkmaid 街上，有三名朋友：Marion Yogurt、Janelle de Queso 和 Steve Cheeseworth III。在一个炎热的夏日，他们听到了冰淇淋车的音乐，决定买些东西吃。Marion 喜欢草莓，Janelle 喜欢巧克力，而 Steve 对乳糖不耐受。那天，只有两个孩子吃了冰淇淋，其中一个孩子买了一瓶室温的水。冰淇淋车装满了典型的冰淇淋口味。列表 1-3

Sadstory.txt - 一个关于一个没吃冰淇淋的孩子的悲伤故事

### 分析问题 #1：谁没有吃到冰淇淋，原因是什么？

现在我们来分析一下这个问题，并互相提出一些问题。首先，谁没有吃到冰淇淋，原因是什么？显然的答案是史蒂夫因为乳糖不耐症而没有吃到冰淇淋。然而，由于故事中没有直接说明史蒂夫没有买冰淇淋，所以正则表达式无法匹配故事中的文本模式。

正则表达式可以查找诸如“didn’t have”、“no ice cream”或孩子的名字等关键词。然而，它只能根据这些模式的存在提供响应。例如，如果正则表达式与“didn’t have”或“no ice cream”与 Steve 的名字匹配，它可以显示文本模式的结果。然而，它肯定无法解释**为什么**Steve 没有得到冰淇淋，或提供任何特定于上下文的推理。

现在，让我们将同样的故事提供给 ChatGPT 并提问，“谁没有得到冰淇淋？”列表 1-4 将我们的问题和前面的故事结合起来作为一个提示。使用以下故事中的信息，谁没有得到冰淇淋以及为什么？###在美国的 Buttersville 市牛奶女仆街上，有三个朋友：Marion 酸奶、Janelle de Queso 和 Steve Cheeseworth III。在一个炎热的夏日，他们听到了冰淇淋车的音乐，决定买些东西吃。Marion 喜欢草莓，Janelle 喜欢巧克力，而 Steve 对乳糖不耐受。那天，只有两个孩子吃了冰淇淋，其中一个买了一瓶室温的水。冰淇淋车装满了典型的冰淇淋口味。列表 1-4

提示。将悲伤的故事放入提示中

注意，在创建包含指令和数据（如上述示例）的提示时，提供某种类型的分隔是一种最佳实践，在这种情况下是“###”。稍后，当我们开始使用游乐场或 Java 以编程方式调用 ChatGPT API 时，你会看到有更好的方法来提供这种分隔。

因此，在发送提示后，ChatGPT 将提供如列表 1-5 所示的答案。![](img/chatgpt-for-java-607613_1_En_1_Figc_HTML.gif)Chat G P T 标志。根据给定信息，Steve 对乳糖不耐受，因此不能吃冰淇淋。因此，Steve 是那个没有得到冰淇淋的人。列表 1-5

回复。ChatGPT 对分析问题 #1 的回答

正如你所见，ChatGPT 可以利用 NLP 和 NLU，因此它能够*理解*（即通过人工智能）场景的上下文。它能够解释孩子们之间的关系、他们的喜好以及史蒂夫的乳糖不耐症。它能够理解孩子们的姓氏、街道名称和城市名称是乳制品的名称，但显然与当前的问题无关。

### 分析问题 #2：哪个孩子可能感到难过？

现在，为了进一步证明正则表达式无法提供任何类型的 NLP 或 NLU，让我们使用一个新术语，称为**情感分析**。因此，在冰淇淋车开走之后，哪个孩子感到难过？

由于故事中没有提及任何孩子的感受或情绪，没有文本模式能让任何正则表达式返回匹配结果。

然而，如果你向 ChatGPT 提出相同的问题，它将返回如列表 1-6 中所示的反应。![图 d](img/chatgpt-for-java-607613_1_En_1_Figd_HTML.gif)Chat G P T 标志。由于 Steve 对乳糖不耐受，不能吃冰淇淋，所以他将是那个因为不能像 Marion 和 Janelle 一样享受冰淇淋而感到悲伤的孩子。列表 1-6

反应。ChatGPT 对分析问题#2 的回答

因此，ChatGPT 能够理解场景，推理信息，并针对该答案提供*解释*。

## 让我们忘掉一些词汇，以便更好地了解 ChatGPT API。

首先，在你开始使用 ChatGPT 和 OpenAI API 之前，有一些单词和术语你应该先熟悉；否则，事情可能不会完全明了。所以让我们确保我们所有人都清楚在使用 ChatGPT 编程时对模型、提示、标记和温度的定义。

### 模型。模型？模型！！！

作为一名 Java 开发者，当你听到“模型”这个词时，你可能立刻会想到面向对象编程以及你在 Java 类中代表现实世界实体的方式，对吧？例如，想想“对象模型”这个术语。另外，如果你之前曾与任何类型的数据库合作过，那么“模型”这个术语也可能让你联想到数据及其在数据库中的关系。例如，想想“数据模型”这个术语。

然而，当使用 ChatGPT API（以及一般的人工智能）时，你需要忘记这两个定义，因为它们不适用。在人工智能领域，“模型”是一个预训练的**神经网络**。

记住，正如我之前提到的，你不需要机器学习博士学位就能阅读这本书。那么神经网络是什么呢？简单来说，神经网络是人工智能系统的一个基本组成部分，因为它们通过使用相互连接的人工神经元层来模拟人脑的工作方式，以处理和分析数据。这些网络可以在大量数据上训练，以学习模式、关系并做出预测。![图 1-1](img/chatgpt-for-java-607613_1_En_1_Fig1_HTML.png)

一幅图展示了各种数据源如何连接到 Chat G P T 模型。

图 1-1

人工智能模型是在大量数据上训练的。

在人工智能的背景下，“预训练模型”指的是在提供给开发者使用之前，已经在特定任务或数据集上训练过的神经网络。这个过程涉及将模型暴露于大量标记和分类（也称为“注释”）的数据中，并调整其内部参数以优化其在给定任务上的性能。

让我们来看看 OpenAI 为开发者提供的部分模型，以便他们可以使用这些模型将应用程序 AI 化。

| GPT-4 | GPT-4 是 OpenAI GPT 模型系列的最新一代。GPT 代表生成预训练转换器，这些模型经过训练，可以理解自然语言以及多种编程语言。GPT-4 模型接受文本和图像作为提示输入，并以文本作为输出。一些可用的 GPT-4 模型有：• gpt-4• gpt-4-32k• gpt-4-vision |
| --- | --- |
| GPT-3.5 | GPT-3.x 是 OpenAI GPT 模型系列的上一代。2022 年 11 月向公众发布的原始 ChatGPT 使用了 GPT 3。一些可用的 GPT-3 模型有：• gpt-3.5-turbo• gpt-3.5-turbo-16k |
| DALL·E | DALL·E 模型可以根据自然语言提示生成和编辑图像。在这本书的第四章中，我们将使用 DALL·E 模型来可视化您最喜欢的播客节目中正在讨论的内容的对话。一些可用的 DALL·E 模型有：• dall-e-3• dall-e-2 |
| TTS | TTS 模型将文本转换为音频，效果出奇地好。在大多数情况下，音频几乎与人类声音无法区分。一些可用的 TTS 模型有：• tts-1• tts-1-hd |
| Whisper | 简单来说，Whisper 模型将音频转换为文本。在这本书中，我们将使用 Whisper 模型在播客节目中搜索文本。 |
| 嵌入模型 | 嵌入模型可以将大量文本转换为文本中字符串之间关系的数值表示。那么这有什么用呢？嵌入模型允许开发者使用自定义数据集执行特定任务。是的，这意味着您可以在与您的应用程序相关的特定数据上训练嵌入模型。这使您能够执行以下操作：• 在您自己的文本体中进行搜索• 将数据聚类，以便文本字符串根据其相似性分组• 获取推荐（推荐具有相关文本字符串的项目）• 检测异常（识别出关系较少的异常值）• 测量多样性（分析相似性分布）• 对数据进行分类（根据最相似的标签对文本字符串进行分类） |
| 审查 | 审查模型是经过微调的模型，可以检测文本是否可能敏感或不安全。这些模型可以分析文本内容，并根据以下类别进行分类：• 恶意• 恶意/威胁• 嘲讽• 嘲讽/威胁• 自伤• 自伤/意图• 自伤/指令• 性相关• 性相关/未成年人• 暴力• 暴力/血腥审查模型包括：• Text-moderation-latest• Text-moderation-stable |
| 过时和弃用 | 自 ChatGPT 推出以来，OpenAI 一直支持他们的旧 AI 模型，但它们已被标记为“过时”或“弃用”模型。这些模型仍然存在；然而，他们发布了其他更准确、更快、更便宜的模型。 |

注意

这绝不是 OpenAI 为开发者提供的所有模型的详尽列表！随着新模型的发布，旧模型将被标记为过时或弃用。因此，通过检查 OpenAI 文档中可用的模型列表来保持最新是很重要的：[`platform.openai.com/docs/models`](https://platform.openai.com/docs/models)

### 当我们谈论标记时，要想到 StringTokenizer 而不是访问令牌

当使用第三方 API 时，你可能会将标记视为与访问令牌相同的概念，通常是一个 UUID，允许你识别自己并与服务保持会话。好吧，现在就忘记这个定义吧。

现在，作为一名 Java 开发者，你可能已经有机会使用`java.util.StringTokenizer`类，将一个字符串分割成更小的字符串数组，以便你可以遍历它以实现所需的目的。例如，如果你有一段文本，你可以让分隔符为“.”，以便获取段落中的句子数组。

好消息是，OpenAI API 中的**标记**概念与 Java 中的概念非常相似，因为它是一个文本片段。对于 OpenAI API，一个标记是文本的一个片段，大约有 4 个字符长。仅此而已——没有其他特别之处。

所以如果标记大约是一个 4 个字符的文本块，那么我们为什么关心它呢？

当与 OpenAI 文本模型一起工作时，开发者需要意识到标记限制，因为它们会影响 API 调用的成本和性能。例如，gpt-3.5-turbo 模型的标记限制为 4096 个标记，而 gpt-4-vision 模型的限制为 128,000 个标记（大约相当于一本 300 页小说的大小）。模型的标记限制被称为**上下文窗口**。

因此，开发者需要考虑提示的长度作为模型输入和输出的因素，确保它们在模型的标记约束范围内。

表 1-1 提供了当前一些最常用模型的标记限制及其定价。表 1-1

模型及其标记限制和每标记成本的列表

| 模型 | 最大令牌数 | 令牌输入成本 | 令牌输出成本 |
| --- | --- | --- | --- |
| gpt-4 | 8,192 | $0.03 / 1K tokens | $0.06 / 1K tokens |
| gpt-4-32k | 32,768 | $0.06 / 1K tokens | $0.12 / 1K tokens |
| gpt-4-vision | 128,000 | $0.01 / 1K tokens | $0.03 / 1K tokens |
| gpt-3.5-turbo-instruct | 4,096 | $0.0015 / 1K tokens | $0.002 / 1K tokens |
| gpt-3.5-turbo-16k | 16,384 | $0.0010 / 1K tokens | $0.002 / 1K tokens |
| text-embedding-ada-002 | 8192 | $0.0001 / 1K tokens |

### 温度关乎创造力

当然，ChatGPT 并不具有意识，因此它无法像我们人类一样思考。然而，通过调整 ChatGPT API 中提示的 **温度** 设置，你可以使响应更加富有创意。但如果你想要充分利用其潜力，理解它所理解的内容是至关重要的！![图 2](img/chatgpt-for-java-607613_1_En_1_Fig2_HTML.png)

一个温度计的图形测量了一个发光灯泡的温度，从缺乏创意且非常可预测到非常富有创意且非常随机。

图 1-2

调整温度以获得更多（或更少）富有创造性的响应

## 开始使用 OpenAI 操场

现在是时候将我们迄今为止学到的概念付诸实践了！然而，我们需要先做最重要的事情，因此，你需要有一个 OpenAI 的开发者账户并创建一个 API 密钥。

访问以下 URL 创建您的开发者账户和 API 密钥：

[`platform.openai.com/account/api-keys`](https://platform.openai.com/account/api-keys)

如图 1-3 所示，你可以将你的 API 密钥命名为任何你想要的内容！![图 1-3](img/chatgpt-for-java-607613_1_En_1_Fig3_HTML.png)

Chapt G P T 页面的截图被创建新的密钥弹出窗口覆盖。它显示了创建密钥按钮被选中的名称。该名称作为 Java 应用程序的开发者密钥给出。

图 1-3

在您能够访问操场或进行 API 调用之前，您需要有一个 API 密钥

你应该知道，作为创建 API 密钥的要求，你需要向 OpenAI 提供一张信用卡，以便你可以为其模型的使用付费。

现在你已经获得了你的 API 密钥，让我们直接前往以下 URL 的 Chat 操场：

[`platform.openai.com/playground`](https://platform.openai.com/playground)

进入操场后，点击顶部的组合框并选择聊天选项以结束 Chat 操场，如图 1-4 所示。![图 1-4](img/chatgpt-for-java-607613_1_En_1_Fig4_HTML.jpg)

Chapt G P T 页面的截图显示了操场选项卡下的详细信息。列出了一个下拉菜单，其中选定了助手选项。

图 1-4

进入操场后，选择聊天选项

图 1-5 描述了 Chat 操场，某些部分已编号以便于识别。![图 1-5](img/chatgpt-for-java-607613_1_En_1_Fig5_HTML.png)

Chat G P T 页面的截图显示了开始界面。系统从游乐场中选择，列出了用户、助手和添加消息。选择“查看代码”按钮，显示模型为 g p t 4，温度详情和最大长度。

图 1-5

Chat 游乐场一开始可能会让人感到有些令人畏惧

### 1. **系统**

如您所见，Chat 游乐场的用户界面比其他人使用的 ChatGPT 网站要复杂得多。那么，让我们来谈谈**系统**字段（见图 1-5，项目 1）。

在我看来，ChatGPT 可以被描述为“一种非常强大的形式的人工智能……但患有健忘症。” 因此，当您以编程方式使用 ChatGPT 时，您需要通知系统它在对话中的身份！

如下所示的图 1-6，展示了 ChatGPT 在对话中可以扮演的数千种不同角色！![图 1-6](img/chatgpt-for-java-607613_1_En_1_Fig6_HTML.png)

一页显示了一条消息，内容为“系统，您是一位...”，后面跟着以下图形。一个带有图表和美元符号的经济学家，一个带有信息云的博主，一个带有墨水瓶的十五世纪诗人，和一个戴着厨师帽的厨师。

图 1-6

Chat 游乐场中的**系统**字段允许您设置 ChatGPT 在对话中将扮演的角色

### 2. **用户**

ChatGPT 游乐场中的**用户**字段（图 1-5，项目 2）是您输入提示到 ChatGPT 的地方，可以是您想要的任何内容，例如，“描述远程医疗将如何影响医疗行业。”

### 3. **助手**（可选）

当您首次加载 Chat 游乐场时，助手字段（图 1-5，项目 3）是不可见的。为了使其出现，您需要点击“**+**”符号旁边的“添加消息”。现在，您可能会问自己，“为什么这个字段是必需的？” 好问题。如果您想让 ChatGPT 记住它在之前的对话中已经告诉您的事情，那么您需要在**助手**字段中输入任何您认为相关的信息，以便继续对话。记住，它是一个非常强大的 AI，但它有健忘症！

### 4. **添加消息**（可选）

**添加消息** “**+**” 符号（图 1-5，项目 4）是您点击以添加**助手**消息到对话中，或添加另一个**用户**消息的地方。现在，您可能会问，“当我可以在上面的原始**用户**字段中输入我想说的话时，为什么还要在对话中添加另一个**用户**消息？” 这是一个好问题。

如果您想将您的命令与您的数据分开，那么您将使用一个单独的**用户**消息来做到这一点。

你还记得在本章前面的列表 1-4 中，我们不得不使用“###”来将 ChatGPT 的命令与我们想要它分析的数据分开吗？嗯，现在不再需要了，因为命令将是第一个 **用户** 消息，数据将是第二个 **用户** 消息。

### 5. 查看代码（可选）

在你使用游乐场提交提示后，你可以点击 **查看代码** 按钮（图 1-5，项目 5），以查看发送相同提示所需的代码，使用他们支持的语言中的任何一种。

你可能会注意到 Java 不是一个官方支持的语言，但我们在第二章节中会解决这个问题，当我们使用 ChatGPT 作为配对程序员并将他们的 REST 接口移植到 Java 时。

### 6. 模型（可选）

在本章前面，我们讨论了可供开发者使用的各种模型。点击模型字段，以查看可用的模型列表。

你还可能注意到，一些模型的名字与月份和日期相关联，这只是一个该模型的快照。通过编程选择快照，开发者可以使从 ChatGPT 收到的响应具有某种可预测性，因为当前模型总是更新的。

### 7. 温度（可选）

如本章前面所述，温度选择器介于 0 和 2 之间，允许你选择响应的“随机性”。

### 8. 最大长度（可选）

你还记得本章前面关于标记的讨论吗？通过选择此项目的任何范围，你可以调整响应中的标记数量（这直接影响单词数量）。

## 现在就试试！尝试“系统”角色

现在我们已经熟悉了 Chat Playground 的几个功能，让我们使用上面讨论的设置发送我们的第一个提示。列表 1-7 和 1-8 使用相同的提示要求 ChatGPT 提供关于远程医疗的几段内容，但系统角色的作用与彼此大不相同。**系统**：你是一位严格事实的研究员**用户**：列出远程医疗的利弊（列表 1-7）

PROMPT. 作为研究人员，远程医疗的利弊

**系统**：你是一位有强烈观点的健康博主，总是有第一手经验的故事**用户**：列出远程医疗的利弊（列表 1-8）

PROMPT. 作为有观点的健康博主，远程医疗的利弊

鼓励你自己尝试这两个提示，看看会得到什么响应。调整温度和标记长度的设置，以便熟悉这些参数如何影响结果。

## 结论

你刚刚学习了更多关于开发者如何使用 ChatGPT 的信息。我们介绍了一些 Chat Playground 的基础知识，这是一个开发者与 ChatGPT API 交互的网页界面。

我们讨论了如何在 Chat Playground 中设置系统、用户和助手角色，以及如何调整温度和输出最大长度等设置。

您已经了解了使用 Chat Playground 所需的一些参数和术语，例如模型、温度和令牌。熟悉 Chat Playground 的参数对于了解如何使用 REST API 至关重要，因为 Playground 是 REST API 提供的能力子集。

在下一章中，我们将看到如何使用 ChatGPT 作为您的“配对程序员”，并将官方支持的 ChatGPT REST 接口移植到 Java。

© 作者（们），独家授权给 APress Media, LLC，Springer Nature 的一部分，2024B. HopkinsChatGPT for Java[`doi.org/10.1007/979-8-8688-0116-7_2`](https://doi.org/10.1007/979-8-8688-0116-7_2)

# 2. 使用 ChatGPT 作为您的 Java 配对程序员

布鲁斯·霍普金斯^(1  )(1)美国俄勒冈州比佛顿

我非常欣赏 XP（极限编程）的一些实践，尤其是配对编程。无论您更喜欢哪种配对编程风格，它都涉及两名工程师坐在同一屏幕前共同解决问题。您获得的最大好处之一是问题的新视角，当然，现在您有两个工程师“接触”了代码库，而不是一个。有时可以有一个工程师编写代码，另一个编写测试和注释。无论如何划分，这都是好事。

现在，ChatGPT 和 OpenAI 的其他模型的 OpenAI REST API 已正式支持 Python、Typescript，当然还有 cURL（这是 REST API 的事实标准）。

存在一些由第三方开发者创建的 Java API，但在我看来，最大的问题是这个领域正在迅速变化。OpenAI 不断更新他们的模型和 HTTP 接口，因此他们经常添加或弃用功能和功能。如果您选择在项目中使用第三方 Java API，您可能会遇到使用过时或与 OpenAI REST API 不同步的 API 的问题。

因此，在本章中，我们将使用 ChatGPT 作为我们的配对程序员，并将官方 OpenAI REST API 直接移植到 Java。每当 OpenAI 对其官方支持的语言和接口进行任何更改时，我们都能立即更新我们自己的库所需的一切。让我们这么做吧！

## 创建您的第一个 Java ChatGPT 应用程序：ListModels.java

我们实际上将同时完成两个任务。我们将使用 OpenAI API 创建一个基本的 Java 应用程序，并在过程中验证我们已经正确地获取了 API 密钥。因此，不用说，如果你还没有这样做，请按照第一章的说明创建你的 OpenAI 开发者账户并获取你的 API 密钥。从现在开始，本书中的所有代码示例都需要一个有效的 API 密钥。

## List Models 端点

我们可以调用的最基本（但也是最重要的）服务之一是 **List Models** 端点。为什么你会问这个问题？List Models 端点允许你通过 REST API 获取所有当前可供开发者使用的 AI 模型列表。

### 创建请求

表 2-1 列出了调用 List Models 端点所需的全部 HTTP 参数。表 2-1

调用 List Models 端点所需的 HTTP 参数

| HTTP 参数 | 描述 |
| --- | --- |
| 端点 URL | [`api.openai.com/v1/models`](https://api.openai.com/v1/models) |
| 方法 | GET |
| 标题 | 授权: Bearer **$OPENAI_API_KEY** |

### 处理 JSON 响应

在成功调用 List Models 端点后，服务将提供一个包含所示结构的 JSON 响应，如表 2-2 所示。

### 模型 (JSON)

表 2-2

模型 JSON 对象的结构

| 字段 | 类型 | 描述 |
| --- | --- | --- |
| object | 字符串 | 总是返回字面量，"list" |
| data | 数组 | OpenAI 提供的 AI 模型列表 |
|   ↳ id | 字符串 | AI 模型的唯一 ID，实际上是模型的完整名称 |
|   ↳ object | 字符串 | 总是返回字面量，"model" |
|   ↳ created | 整数 | 模型的创建日期 |
|   ↳ owned_by | 字符串 | 拥有该模型的组织的名称 |
| 权限 | 数组 | 这是模型权限的元数据数组 |
| root | 字符串 | 这通常是 data.id 字段的副本，即模型名称 |
| parent | 字符串 | 目前这是一个未使用的字段 |

备注

由于 JSON 对象可以包含数组（在表格中难以表示），我们使用“ ↳ ”符号来表示数组的元素。如前表所示，“id”、“object”、“created”和“owned_by”都是 JSON 响应中“data”数组的元素。

现在我们已经了解了 HTTP 请求和响应的详细信息，我们可以使用如清单 2-1 所示的提示来创建 ListModel.java 应用程序。**系统**: 你是一位 Java 开发者**用户**: 将以下 cURL 命令转换为 Java。文件名为 "ListModels.java"**用户**: curl https://api.openai.com/v1/models \  -H "Authorization: Bearer $OPENAI_API_KEY"清单 2-1

PROMPT. 使用 ChatGPT 创建 ListModels.java 应用程序

因此，在发送提示后，ChatGPT 将提供如列表 2-2 所示的答案。![open A I 的标志](img/chatgpt-for-java-607613_1_En_2_Figa_HTML.gif)open A I 的标志导入 java.io.BufferedReader;导入 java.io.InputStreamReader;导入 java.net.HttpURLConnection;导入 java.net.URL;public class ListModels {        public static void main(String[] args) {        try {            // 为 API 端点创建 URL 对象            URL url = new URL("https://api.openai.com/v1/models");            // 创建 HttpURLConnection 对象            HttpURLConnection conn = (HttpURLConnection) url.openConnection();            // 设置请求方法            conn.setRequestMethod("GET");            // 设置 Authorization 头            conn.setRequestProperty("Authorization", "Bearer $OPENAI_API_KEY");            // 获取响应代码            int responseCode = conn.getResponseCode();            // 如果请求成功（状态码 200）            if (responseCode == HttpURLConnection.HTTP_OK) {                // 从 API 读取响应                BufferedReader in = new BufferedReader(new InputStreamReader(conn.getInputStream()));                String inputLine;                StringBuilder response = new StringBuilder();                while ((inputLine = in.readLine()) != null) {                response.append(inputLine);                }                in.close();                // 打印响应                System.out.println(response.toString());            } else {                System.out.println("请求失败。响应代码: " + responseCode);            }            // 关闭连接            conn.disconnect();        } catch (Exception e) {            e.printStackTrace();        }        }}列表 2-2

RESPONSE. ListModels.java

太棒了！现在你只需要将“$OPENAI_API_KEY”替换为你的实际 API 密钥的值。

运行这个类后，你会得到一个包含 OpenAI API 提供的所有模型的 JSON 文件，如列表 2-3 所示。![](img/chatgpt-for-java-607613_1_En_2_Figb_HTML.gif)Open A I 的标志。{  "object": "list",  "data":     {      "id": "text-search-babbage-doc-001",      "object": "model",      "created": 1651172509,      "owned_by": "openai-dev"    },    {      "id": "gpt-4",      "object": "model",      "created": 1687882411,      "owned_by": "openai"    },    {      "id": "gpt-3.5-turbo-16k",      "object": "model",      "created": 1683758102,      "owned_by": "openai-internal"    },    {      "id": "curie-search-query",      "object": "model",      "created": 1651172509,      "owned_by": "openai-dev"    },    {      "id": "text-davinci-003",      "object": "model",      "created": 1669599635,      "owned_by": "openai-internal"    },    {      "id": "text-search-babbage-query-001",      "object": "model",      "created": 1651172509,      "owned_by": "openai-dev"    },    {      "id": "babbage",      "object": "model",      "created": 1649358449,      "owned_by": "openai"    },...列表 2-3

响应。运行 ListModels.java 后的 JSON 部分响应

列表 [2-3 是由于可供开发者使用的模型数量庞大而提供的部分列表！然而，好消息是完整的响应作为表格提供在附录中。

现在我们可以通过编程方式获取可用的模型列表，是时候使用 Java 向 ChatGPT 发送提示了。这是通过使用 Chat 端点来实现的。

## Chat 端点

Chat 端点（以前称为“Chat Completion”）是一个 REST 服务，基本上是你可以在 Chat Playground 中执行操作的 1-to-1 表示；因此，这项服务应该对你来说就像第二本能一样。

### 创建请求

表 2-3 列出了调用 Chat 端点所需的全部 HTTP 参数。表 2-3

Chat 端点的 HTTP 参数

| HTTP 参数 | 描述 |
| --- | --- |
| 端点 URL | https://api.openai.com/v1/chat/completions |
| 方法 | POST |
| 头部 | Authorization: Bearer **$OPENAI_API_KEY** |
| Content-Type | application/json |

表 2-4 描述了用于 Chat 端点请求体的必要 JSON 对象格式。快速浏览后，你可以看到为了成功调用服务，实际上只需要几个字段。

### Chat (JSON)

表 2-4

Chat JSON 对象的结构

| 字段 | 类型 | 必需？ | 描述 |
| --- | --- | --- |
| model | String | Required | 你想要用于 Chat Completion 的模型的 ID。兼容的模型包括• gpt-4• gpt-4-0613• gpt-4-32k• gpt-4-32k-0613• gpt-3.5-turbo• gpt-3.5-turbo-0613• gpt-3.5-turbo-16k• gpt-3.5-turbo-16k-0613 |
| messages | Array | Required | 作为持续对话一部分的消息数组。数组中的每个消息有两个属性：“role”和“content。” |
|   ↳ role | 字符串 | 必需 | 指定消息的角色，可以是以下任何一种：• "system"• "user"• "assistant"• "tool" |
|   ↳ content | 字符串 | 必需 | 包含指定角色的消息文本。 |
| tools | 数组 | 可选 | 这允许您指定模型可以调用的工具列表。目前，唯一支持的工具类型是函数。此参数使您能够定义模型可以生成 JSON 输入的函数集。 |
|   ↳ type | 字符串 | 必需 | 这是工具的类型，可以是以下任何一种：• "function" |
|   ↳ function | 数组 | 可选 | 模型在聊天完成中可能使用的函数数组。 |
|   ↳↳ name | 字符串 | 必需 | 要调用的函数的名称。有效的名称必须是 a-z、A-Z、0-9，或包含下划线和破折号。最大长度为 64 个字符。 |
|   ↳↳ description | 字符串 | 可选 | 函数的功能描述。这有助于模型决定是否在聊天完成中调用函数。 |
|   ↳↳ 参数 | JSON 对象 | 必需 | 函数接受的参数格式为 JSON Schema 对象。 |
| tool_choice | 字符串或 JSON 对象默认值："none" 当请求中不包含函数时 "auto" 当请求中包含函数时 | 可选 | 这允许您确定模型应该调用哪个函数（如果有的话）。当设置为"none"时，模型将避免调用任何函数，仅生成消息响应。当设置为"auto"时，模型可以根据其内部决策过程灵活选择生成消息响应或调用函数。 |
| temperature | 数字或 null 默认值：1 | 可选 | 有效值介于 0 和 2 之间。控制模型输出的随机性。最佳实践是调整 top_p 或温度，但不要同时调整两者。 |
| top_p | 数字或 null 默认值：1 | 可选 | 有效值介于 0 和 1 之间。表示是否考虑少数可能性（0）或所有可能性（1）。最佳实践是调整 top_p 或温度，但不要同时调整两者。 |
| n | 整数或 null 默认值：1 | 可选 | 指定模型为每个输入消息应生成的聊天完成选项数量。 |
| stream | 布尔或 null 默认值：false | 可选 | 如果"stream"设置为"true"，则将发送部分消息更新作为服务器发送事件。这意味着标记将在可用时作为仅数据事件发送，并且流将以"data: [DONE]"消息结束 |
| stop | 字符串 / 数组 / null 默认值：null | 可选 | 您可以提供最多 4 个序列，API 将在其中停止生成进一步的标记。这可以用于控制响应的长度或内容。 |
| max_tokens | 整数或 null 默认值：inf | 可选 | 此参数设置生成的聊天完成的最大标记数。 |
| response_format | JSON 对象 | 可选 | 您有两个选项：{ "type": "json_object" } 用于 JSON 对象响应或 { "type": "text" } 用于文本响应 |
| seed | 整数或 null | 可选 | 通过指定一个种子，系统将尝试生成可重复的结果。理论上，这意味着如果您使用相同的种子和参数进行重复请求，您应该期望收到相同的结果。为了将种子值放入后续请求中，请复制您上次响应中的 system_fingerprint。 |
| presence_penalty | 数字或 null 默认值：0 | 可选 | 一个介于-2.0 和 2.0 之间的数字。正值根据新标记是否出现在对话历史中对其进行惩罚，鼓励模型讨论新主题。 |
| frequency_penalty | 数字或 null 默认值：0 | 可选 | 一个介于-2.0 和 2.0 之间的数字。正值根据它们在对话历史中的现有频率对标记进行惩罚，降低重复相同行文字的概率。 |
| logit_bias | JSON 映射默认值：null | 可选 | 允许您修改特定标记在完成中的出现概率。您提供一个将标记（由分词器中的标记 ID 指定）映射到关联偏置值的 JSON 对象，范围从-100 到 100。此偏置在采样之前添加到模型的 logits 中。 |
| user | 字符串 | 可选 | 这是一个可选生成的唯一 ID，可以代表您的最终用户。这将帮助 OpenAI 监控和检测滥用。 |

注意

在这本书中，我们将使用默认设置为 false 的“stream”参数。这意味着我们将一次性作为单个 HTTP 响应接收来自 ChatGPT 的结果。

然而，有些情况下您可能希望将此设置设置为 true。比如说，您正在构建一个交互式语音启用的聊天机器人。再比如说，您对将 ChatGPT 的文本转换为音频感兴趣，以便您的用户可以听到可听到的响应。在这种情况下，您肯定希望将“stream”参数设置为 true。为什么是这样呢？当响应以流的形式返回到您的 Java 应用程序时，您有机会在那个时刻将文本片段转换为音频。这将使您能够在接收更多文本的同时并行地将文本片段转换为音频。这将使响应对最终用户来说看起来更自然，并帮助对话感觉像**真实的**对话。

列表 2-4 是正确调用聊天端点时 JSON 对象的一个示例。{  "model": "gpt-3.5-turbo",  "messages": [    {      "role": "system",      "content": "You are a product marketer"    },    {      "role": "user",      "content": "Explain why Java is so widely used in the enterprise "    }  ],  "temperature": 1,  "max_tokens": 256,  "top_p": 1,  "frequency_penalty": 0,  "presence_penalty": 0}列表 2-4

Chat JSON 对象示例

### 处理响应

在成功调用 Chat 端点后，API 将响应一个 Chat Completion 对象，如果启用了流式传输，则返回一系列完成块。以下是 Chat Completion 对象的分解。

### Chat Completion (JSON)

表 2-5

Chat Competion JSON 对象的结构

| 字段 | 类型 | 描述 |
| --- | --- | --- |
| id | 字符串 | Chat Completion 的唯一标识符。 |
| object | 字符串 | 这始终返回字面量，“chat.completion。” |
| system_fingerprint | 字符串 | 如果您想要在后续请求中重现之前对话的结果，请将此参数用作“种子”。 |
| created | 整数 | Chat Completion 的时间戳。 |
| model | 字符串 | 用于 Chat Completion 的模型。 |
| choices | 数组 | 可用的 Chat Completion 选择列表。如果您在 Chat JSON 请求中指定了所需的响应数量，则可以获取多个消息选择。"n" 参数用于指定。请参阅表 2-4。 |
|   ↳ index | 整数 | 列表中选择的索引。 |
|   ↳ message | 数组 | 模型生成的聊天完成消息。 |
|   ↳ finish_reason | 字符串 | 每个响应都将包含一个 finish_reason。finish_reason 的可能值有：stop：API 返回了完整的消息，或由 stop 参数提供的终止序列之一终止的消息.length：由于请求中的 max_tokens 参数或模型本身的标记限制，模型输出不完整.tool_call：模型调用了工具，例如函数.content_filter：由于违反内容过滤器，响应被终止.null：API 响应仍在进行中或未完成。 |
| usage | 数组 | 完成请求的使用统计信息，包括提示、完成和总请求中的标记数量。 |
|   ↳ prompt_tokens | 整数 | 提示中使用的标记数量。 |
|   ↳ completion_tokens | 整数 | 响应中使用的标记数量。 |
|   ↳ total_tokens | 整数 | 请求和响应中所有标记的总和。 |

列表 2-5 是调用 Chat 端点后的 JSON 响应示例。![open A I.的标志](img/chatgpt-for-java-607613_1_En_2_Figc_HTML.gif)A logo of open A I.{  "id": "chatcmpl-7wUOFQ3S34scDLmrLdWTTqvHmXztQ",  "object": "chat.completion",  "created": 1694174199,  "model": "gpt-3.5-turbo-0613",  "choices": [    {      "index": 0,      "message": {        "role": "assistant",        "content": "Java is widely used in the enterprise because it is platform-independent, allowing applications to run on any system. Additionally, Java has a large and mature ecosystem with a vast array of libraries, frameworks, and tools, making it easier for developers to build robust and scalable enterprise applications."      },      "finish_reason": "stop"    }  ],  "usage": {    "prompt_tokens": 32,    "completion_tokens": 55,    "total_tokens": 87  }}列表 2-5

Chat Completion JSON 对象

## 等等，我的提示中有多少个 token？

在某个时刻，你将开始思考计划发送给 ChatGPT 的提示，并对你想要使用的模型的 token 限制（以及成本）给予相当多的思考。如果你忘记了，请务必参考表 1-1 以获取模型列表和 token 价格。此外，OpenAI 创建了一个简单易用的网站，允许你查看你的提示中有多少个 token，如图 2-1 所示。

### ChatGPT Token 计数器

[`platform.openai.com/tokenizer`](https://platform.openai.com/tokenizer)![](img/chatgpt-for-java-607613_1_En_2_Fig1_HTML.jpg)

一个名为“Tokenizer”的页面有几段介绍语言模型分词的内容。一个文本框写着，“这一行文本中有多少个 token？”答案在底部给出，为 10 个 token 和 41 个字符。

图 2-1

ChatGPT 分词器可以快速计算你的提示中的 token 数量

## 创建下一个 Java 应用程序：ChatGPTClient.java

现在是时候构建我们自己的 ChatGPTClient 了。让我们直接深入，并通过 ChatGPT Playground 提供 ChatGPT 所需的信息。**系统**：你是一名 Java 开发者**用户**：将以下 cURL 命令转换为 Java。确保 API 的 URL 和 API 密钥是变量。我想使用 Jackson 库在请求中创建 JSON 对象。将主类命名为 ChatGPTClient，并在必要时创建辅助类。**用户**：curl https://api.openai.com/v1/chat/completions \  -H "Content-Type: application/json" \  -H "Authorization: Bearer $OPENAI_API_KEY" \  -d '{  "model": "gpt-3.5-turbo",  "messages": [    {      "role": "system",      "content": "You are a product marketer"    },    {      "role": "user",      "content": "Explain why Java is so widely used in the enterprise "    }  ],  "temperature": 1,  "max_tokens": 256,  "top_p": 1,  "frequency_penalty": 0,  "presence_penalty": 0}'列表 2-6

创建 ChatGPTClient.java 的初始对话

ChatGPT 的响应是一个良好的开端，但并没有完全符合我想要的内容。现在，由于我没有明确指定 HTTP 调用应该如何进行，ChatGPT 决定使用 Apache HTTPClient 库。因此，我添加了以下用户消息（列表 2-7）。**用户**：我有一个 Java 11 环境，所以请使用 Java 11 HTTP 类进行 API 调用。我更愿意使用纯 Java 而不是 Apache HttpClient

PROMPT. 向对话中添加额外信息以创建 ChatGPTClient.java

这里的目标是进行一场对话。期望 ChatGPT 在单个提示中就完全符合你的要求是不切实际的。即使是开发者也不会这样做！因此，请随意与 ChatGPT 进行对话，并向其澄清它可能猜测或假设错误的事情。

列表 2-8 展示了 ChatGPTClient.java 的最终结果。![开放 AI 的标志](img/chatgpt-for-java-607613_1_En_2_Figd_HTML.gif)导入 com.fasterxml.jackson.core.JsonProcessingException;导入 com.fasterxml.jackson.databind.ObjectMapper;导入 com.fasterxml.jackson.annotation.JsonProperty;导入 java.io.BufferedReader;导入 java.io.IOException;导入 java.io.InputStreamReader;导入 java.io.OutputStream;导入 java.net.HttpURLConnection;导入 java.net.URL;导入 java.util.ArrayList;导入 java.util.List;public class ChatGPTClient {        public static void main(String[] args) {        String openAIKey = "在此处插入您的 API 密钥";        String endpoint = "https://api.openai.com/v1/chat/completions";        String model = "gpt-3.5-turbo";        float temperature = 1.0f;        int max_tokens = 256;        float top_p = 1.0f;        int frequency_penalty = 0;        int presence_penalty = 0;        List<Message> messages = new ArrayList<>();        messages.add(new Message("system", "您是一位产品营销人员。"));        messages.add(new Message("user", "解释为什么 Java 在企业中如此广泛使用"));        String jsonInput = null;        try {            ObjectMapper mapper = new ObjectMapper();            Chat chat = new Chat(model, messages, temperature, max_tokens, top_p, frequency_penalty, presence_penalty);            jsonInput = mapper.writeValueAsString(chat);        } catch (JsonProcessingException e) {            e.printStackTrace();        }        try {            URL url = new URL(endpoint);            HttpURLConnection connection = (HttpURLConnection) url.openConnection();            connection.setRequestMethod("POST");            connection.setRequestProperty("Content-Type", "application/json");            connection.setRequestProperty("Authorization", "Bearer " + openAIKey);            connection.setDoOutput(true);            OutputStream outputStream = connection.getOutputStream();            outputStream.write(jsonInput.getBytes());            outputStream.flush();            outputStream.close();            int responseCode = connection.getResponseCode();            if (responseCode == HttpURLConnection.HTTP_OK) {                BufferedReader reader = new BufferedReader(new InputStreamReader(connection.getInputStream()));                StringBuilder response = new StringBuilder();                String line;                while ((line = reader.readLine()) != null) {                    response.append(line);                }                reader.close();                // 打印响应                System.out.println(response.toString());            } else {                System.out.println("错误: " + responseCode);            }            connection.disconnect();        } catch (IOException e) {            e.printStackTrace();        }    }    // 表示 Chat 对象的辅助类    static class Chat {        @JsonProperty("model")        private String model;        @JsonProperty("messages")        private List<Message> messages;        @JsonProperty("temperature")        private float temperature;        @JsonProperty("max_tokens")        private int max_tokens;        @JsonProperty("top_p")        private float top_p;        @JsonProperty("frequency_penalty")        private int frequency_penalty;        @JsonProperty("presence_penalty")        private int presence_penalty;        public Chat(String model, List<Message> messages, float temperature, int max_tokens, float top_p, int frequency_penalty, int presence_penalty) {            this.model = model;            this.messages = messages;            this.temperature = temperature;            this.max_tokens = max_tokens;            this.top_p = top_p;            this.frequency_penalty = frequency_penalty;            this.presence_penalty = presence_penalty;        }        // 获取器和设置器（可选，但如果有必要在以后修改对象，则可能有用）        }    // 表示 Chat 消息的辅助类    static class Message {        @JsonProperty("role")        private String role;        @JsonProperty("content")        private String content;        public Message(String role, String content) {            this.role = role;            this.content = content;        }    }}列表 2-8

响应。ChatGPTClient.java

当你检查前面的代码列表时，你会发现 HTTP 调用是使用纯 Java API 完成的，而不是使用任何外部库——正如我在提示中请求的那样。然而，请注意，在纯 Java 中创建和解析 JSON 对象可能会很痛苦，所以我个人指定了应该使用 Jackson API，这在导入语句和代码本身中都有体现。

产生的代码包含两个内部类，Chat 和 Message，这些类可以轻松地分离成单独的 Java 文件。我可以手动进行操作，或者向 ChatGPT 添加一个新的“用户”消息，请求将内部类分离成独立的 Java 文件。

执行 ChatGPTClient.java 后，列表 2-9 包含了响应。![开放 AI 的标志](img/chatgpt-for-java-607613_1_En_2_Fige_HTML.gif)A logo of open A I.{  "id": "chatcmpl-7xIRvjByGobmWH9Vo7OObHCSSwzgI",  "object": "chat.completion",  "created": 1694366627,  "model": "gpt-3.5-turbo-0613",  "choices": [    {      "index": 0,      "message": {        "role": "assistant",        "content": "Java is widely used in the enterprise primarily due to its numerous benefits and features that make it a popular choice among large organizations. Here are some key reasons why Java is so widely adopted in the enterprise:\n\n1\. Platform Independence: One of the biggest advantages of Java is its platform independence. Java programs can run on any operating system, making it highly adaptable across a wide range of devices and platforms. This makes it easier for enterprises to develop applications that can be deployed on different systems without any major modifications.\n\n2\. Robustness and Stability: Java is known for its strong emphasis on reliability, stability, and error handling. It has a built-in memory management system that prevents memory leaks and ensures robust performance. This stability is highly valued in enterprise environments where systems need to run consistently without disruptions.\n\n3\. Scalability: Java offers excellent scalability, making it suitable for large-scale enterprise applications. It provides robust support for multi-threading, allowing applications to handle a large number of concurrent users smoothly. Java's ability to handle high traffic loads and distribute processing across multiple servers makes it ideal for enterprise-level systems.\n\n4\. Rich Standard Library and Frameworks: Java comes with a comprehensive standard library, offering a wide range of pre-built functions and classes that simplify development. Additionally, Java has a"      },      "finish_reason": "length"    }  ],  "usage": {    "prompt_tokens": 28,    "completion_tokens": 256,    "total_tokens": 284  }}列表 2-9

响应。调用 ChatGPTClient.java 的结果

你注意到在前面的列表中，我对提示的回答被截断了吗？“此外，Java 有一个”不是一个完整的句子，但由于我要求响应中不超过 256 个标记，它没有超过这个限制。

## 结论

与流行观点相反，ChatGPT 不是读心者！它没有能力取代开发者和架构师，因为它（惊讶！）是人工智能。它非常有用，可以提出一个问题并立即得到直接回答。它确实可以用来将自然语言提示（或请求）转换为代码，但你绝对需要一个开发者来判断生成的代码是否应该被使用、改进或完全忽略。

© 作者（们），独家授权给 APress Media, LLC，Springer Nature 的一部分，2024B. HopkinsChatGPT for Java[`doi.org/10.1007/979-8-8688-0116-7_3`](https://doi.org/10.1007/979-8-8688-0116-7_3)

# 3. 在企业中使用 AI！为 Slack 消息创建文本摘要器

布鲁斯·霍普金斯^(1  )(1)美国俄勒冈州比佛顿

在当今的职场中，公司拥有一个 Slack（或 Microsoft Teams）的实例来组织自己，并将其作为公司内部沟通的中心场所是非常常见的。现在，如果你之前使用过 Slack，我想你知道一个频道如何因为公司或世界上某个地方发生了**某些**重要的事情而迅速被大量消息淹没。

当然，你在公司中的责任越大（例如，经理、团队领导、架构师等），你被期望参与的频道就越多。在我看来，Slack 是一把双刃剑。你需要用它来完成你的工作，但作为一个开发者，你绝对不能参加每日站立会议并说，“昨天，嗯，我整天都在阅读 Slack。没有遇到任何障碍。”

此外，如果你为拥有在不同时区有客户的公司工作（这在当今相当普遍），早上打开 Slack 并看到你离开键盘时发布的许多消息是非常令人沮丧的。

因此，在本章中，我们将应用 AI 到企业中，使 Slack 更加有用。我们将利用上一章中的代码，并创建一个 Java 编写的 Slack 机器人，它将总结 Slack 频道中的重要对话。我们将利用 ChatGPT 的文本摘要能力，并稍微更多地关注**提示工程**。

## 那么，什么是提示工程？

简而言之，提示工程是一个精心设计和完善提示和输入参数的过程，以指导 ChatGPT 和其他 AI 模型的行为。它基本上是行业内为了得到你想要的结果而创建正确输入的术语。

然而，在我们继续之前，让我们先做一些整理工作，并改进上一章中的 ChatGPTClient.java。

## 使用 Builder 模式更新 ChatGPTClient.java（和相关类）

因此，在上一章中，我们创建了 ChatGPTClient.java 作为发送我们的提示到 Chat 端点的基本应用程序。这是一个好的开始，但肯定还有改进的空间。

首先让我们看看 Chat 对象的构造函数，它模拟了发送到 Chat 端点的 JSON Chat 对象，如列表 3-1 所示。        public Chat(String model, List<Message> messages, float temperature,                    int max_tokens, float top_p, int frequency_penalty,                    int presence_penalty) {            this.model = model;            this.messages = messages;            this.temperature = temperature;            this.max_tokens = max_tokens;            this.top_p = top_p;            this.frequency_penalty = frequency_penalty;            this.presence_penalty = presence_penalty;        }列表 3-1

Chat 对象的构造函数

因此，如果你参考第二章中的表 2-4，你会看到只有模型和消息参数是成功调用 Chat 端点所必需的。所有其他参数都是可选的，如果你不指定任何内容，其中一些参数有自己的内置默认值。这就是为什么我们不需要“模型化”整个 Chat JSON 对象的原因。

因此，这个构造函数基本上是在恳求使用 Builder 模式进行重构。Builder 模式允许我们获取我们想要的实例，同时只指定我们关心的参数。

此外，Chat 和 Message 对象不再是内部类，而是存在于它们自己的 .java 文件中。列表 3-2 展示了我们可以如何获取使用 Builder 模式修改过的 Chat 对象的实例。    Chat chat = Chat.builder()        .model(model)        .messages(messages)        .temperature(temperature)        .maxTokens(max_tokens)        .topP(top_p)        .frequencyPenalty(frequency_penalty)        .presencePenalty(presence_penalty)        .build();列表 3-2

获取 Chat 对象的实例

由于对 Chat 端点的请求必须指定 Chat JSON 对象中的模型和消息，因此已在 Chat.java 类中添加了一些默认值，以便使其更安全地使用（在减少用户错误倾向的意义上更安全）。列表 3-3 是新的 Chat.java 文件。导入 java.util.List;导入 java.util.ArrayList;导入 com.fasterxml.jackson.annotation.JsonProperty;public class Chat {    @JsonProperty("model")    private String model;    @JsonProperty("messages")    private List<Message> messages;    @JsonProperty("temperature")    private float temperature;    @JsonProperty("max_tokens")    private int max_tokens;    @JsonProperty("top_p")    private float top_p;    @JsonProperty("frequency_penalty")    private int frequency_penalty;    @JsonProperty("presence_penalty")    private int presence_penalty;    private Chat(ChatBuilder builder) {        this.model = builder.model;        this.messages = builder.messages;        this.temperature = builder.temperature;        this.max_tokens = builder.max_tokens;        this.top_p = builder.top_p;        this.frequency_penalty = builder.frequency_penalty;        this.presence_penalty = builder.presence_penalty;    }    public static ChatBuilder builder() {        // 我们在这里需要一个默认消息以避免 API 返回 400 错误        List<Message> messages = new ArrayList<>();        messages.add(new Message("system", "您是一个有用的助手"));        messages.add(new Message("user", "你好"));        return new ChatBuilder().messages(messages);    }    public static class ChatBuilder {        private String model = "gpt-3.5-turbo";        private List<Message> messages = null;        private float temperature = 1.0f;        private int max_tokens = 2048;        private float top_p = 0f;        private int frequency_penalty = 0;        private int presence_penalty = 0;        private ChatBuilder() {        }        public ChatBuilder model(String model) {            this.model = model;            return this;        }        public ChatBuilder messages(List<Message> messages) {            this.messages = messages;            return this;        }        public ChatBuilder temperature(float temperature) {            this.temperature = temperature;            return this;        }        public ChatBuilder maxTokens(int max_tokens) {            this.max_tokens = max_tokens;            return this;        }        public ChatBuilder topP(float top_p) {            this.top_p = top_p;            return this;        }        public ChatBuilder frequencyPenalty(int frequency_penalty) {            this.frequency_penalty = frequency_penalty;            return this;        }        public ChatBuilder presencePenalty(int presence_penalty) {            this.presence_penalty = presence_penalty;            return this;        }        public Chat build() {            return new Chat(this);        }    }}列表 3-3

Chat.java 现在使用构建器模式

这个类（使用这种设计模式）足够灵活，您可以添加或删除调用 Chat 端点所需的自定义参数。如果 OpenAI 在任何时候向 Chat 端点添加新的参数和功能，您可以修改这个类以支持新的要求。

为了完整性，列表 3-4 展示了 Message.java 类。import com.fasterxml.jackson.annotation.JsonProperty;public class Message {    @JsonProperty("role")    private String role;    @JsonProperty("content")    private String content;    public Message(String role, String content) {        this.role = role;        this.content = content;    }}列表 3-4

Message.java

## ChatGPT 来了，要夺走每个人的工作（其实不是）

我谦卑地认为，世界上每家公司都坐在一座未被开采的金矿上。如果您使用任何记录员工之间交流的系统、客户支持请求的数据库或任何大型文本存储库（是的，这包括您的电子邮件、Microsoft Exchange 和公司 Gmail），那么您就有了一个大量未结构化文本的存储库，等待被利用。

因此，ChatGPT 的最佳用途不是消除任何人的工作。它应该被用来增强和扩展您公司团队成员已经做的事情。正如我们在上一章中看到的，作为一个程序员，ChatGPT 可以作为一个非常有效的配对程序员。它也非常擅长高效快速地完成某些困难的任务。所以，让我们看看一个实际例子，看看如何使大量未结构化文本变得有用。

## 检查现实世界问题：软件公司的客户支持

软件开发中最艰巨的任务之一是提供技术支持。想象一下整天处理来自可能感到沮丧、困惑或只是需要解决方案的人的电话和信息是多么的快乐。以下是客户支持为什么是一个难题的一些原因：

+   您的最终用户和您的客户在解释您软件中的问题时，名声不佳。

+   一级技术人员，通常是第一道防线，通常处理最基本的问题或用户错误。但当问题变得更加复杂时，用户会被提升到二级。

+   中间层是一个棘手的地方，因为他们比一级技术支持人员拥有更多的知识和经验；然而，他们没有机会直接从最终用户那里获得答案。

+   真正糟糕的问题会被提升到三级；然而，这些是最昂贵的客服人员，因为他们拥有最多的知识和经验。他们不仅对代码有实际经验，还对服务器和基础设施有实际经验。

让我们用一个典型的 Slack 技术支持渠道中的典型对话的真实世界例子来工作。以下是一个虚构公司中团队成员及其角色的列表：

+   法蒂玛（客户服务代表）

+   约翰（软件工程师）

+   戴夫（项目经理）

+   基思（首席技术官）

列表 3-5 展示了一个软件初创公司团队成员之间的对话示例。客户服务代表法蒂玛（Fatima）通知团队，他们的应用程序在启动后立即崩溃（这不是一个好问题）。首席技术官基思（Keith）立即介入以升级问题。法蒂玛 [16:00 | 02/08/2019]: 嘿，大家好，我有一个紧急问题要讨论。我刚和一个遇到应用程序崩溃的客户通完电话，他们在加载应用程序后立即遇到了这个问题。他们真的很沮丧。我们能尽快解决这个问题吗？ ![哭泣表情](img/chatgpt-for-java-607613_1_En_3_Figa_HTML.gif) 一个闭眼张嘴哭泣的表情符号。基思 [16:01 | 02/08/2019]: 感谢你把这个问题带到我们注意，法蒂玛。让我们立即着手解决这个问题。@约翰，由于我们的架构师今天因病缺席，你能负责调查这个问题吗？约翰 [16:02 | 02/08/2019]: 当然可以，基思。我会深入代码库，看看是否能找到导致崩溃的潜在原因。约翰 [16:02 | 02/08/2019]: 法蒂玛，你能从客户那里收集一些额外的信息吗？询问他们具体的设备、操作系统以及他们可能安装的任何最近更新。法蒂玛 [16:03 | 02/08/2019]: 当然可以，约翰。我会立即联系客户并收集这些详细信息。一旦有了这些信息，我会立即通知大家。戴夫 [16:04 | 02/08/2019]: 我理解这里的紧迫性。让我们确保让客户了解我们的进展 ![哭泣表情](img/chatgpt-for-java-607613_1_En_3_Figb_HTML.gif) 一个闭眼张嘴哭泣的表情符号。法蒂玛。我们不想在故障排除过程中让他们感到被忽视。法蒂玛 [16:04 | 02/08/2019]: 当然，戴夫 ![点赞表情](img/chatgpt-for-java-607613_1_En_3_Figc_HTML.gif) 一个点赞的手势图标。我会定期更新客户，提供我们发现的任何相关信息。约翰 [16:20 | 02/08/2019]: 我已经检查了代码库，到目前为止，我没有发现任何明显的问题。应用程序在加载时崩溃很奇怪。这可能是与内存相关的问题吗？基思，我们最近是否有关于内存泄漏或高内存使用的报告？基思 [16:22 | 02/08/2019]: 约翰，我会调出监控日志，检查最近发布中是否有任何与内存相关的异常。我会尽快告诉你。法蒂玛 [17:01 | 02/08/2019]: 快速更新，大家。客户正在使用运行 iOS 15.1 的 iPhone X。他们提到，问题是在几天前更新应用程序后开始的 ![思考表情](img/chatgpt-for-java-607613_1_En_3_Figd_HTML.gif) 一个思考的表情符号。基思 [17:05 | 02/08/2019]: 感谢你的更新，法蒂玛。这是有帮助的信息。约翰，让我们专注于在 iOS 15.1 的 iPhone X 模拟器上测试最新的应用程序更新，看看我们是否能重现这个问题。约翰 [17:06 | 02/08/2019]: 好主意，基思。我会立即设置模拟器并运行一些测试。基思 [17:30 | 02/08/2019]: 约翰，你在模拟器上重现问题的进展如何？约翰 [17:32 | 02/08/2019]: 是的，基思。我设法在模拟器上重现了崩溃。这似乎与 iOS 15.1 的兼容性问题有关 ![爆炸头表情](img/chatgpt-for-java-607613_1_En_3_Fige_HTML.gif) 一个爆炸头表情符号。我怀疑是由于一个已弃用的方法调用。我会修复它并运行更多测试以确认。约翰 [18:03 | 02/08/2019]: 修复了已弃用的方法问题，应用程序在加载时不再崩溃。看起来我们已经识别并解决了这个问题。我将准备一个补丁并发送给您，基思，以便您审查和部署。基思 [18:04 | 02/08/2019]: ![鼓掌表情](img/chatgpt-for-java-607613_1_En_3_Figf_HTML.gif) 三个鼓掌的手势表情符号。谢谢你，请尽快提供补丁。一旦我审查完毕，我们将部署修复程序到应用商店。戴夫 [18:06 | 02/08/2019]: 干得好，团队 ![三角形脸和卷发表情](img/chatgpt-for-java-607613_1_En_3_Figg_HTML.gif) 一个三角形脸和卷发的表情符号。约翰，请继续通知客户进展情况，并让他们知道我们将在下一个应用程序更新中为他们提供修复方案。有人能确保发布说明反映了这一点吗？约翰 [18:07 | 02/08/2019]: 我会做到的，戴夫。我会更新客户并确保他们知道即将到来的修复方案。基思 [18:27 | 02/08/2019]: 补丁已审查并批准，约翰。请继续更新商店中的应用程序。让我们争取在下一个小时内完成。约翰 [18:26 | 02/08/2019]: 我明白了，基思。我现在正在上传中。法蒂玛 [18:38 | 02/08/2019]: 我刚刚通知了客户关于修复方案的消息。他们感到如释重负，并对我们的快速响应表示感谢。谢谢大家，感谢你们的协作和迅速行动。与这样一支有能力的团队合作是一种乐趣。戴夫 [18:40 | 02/08/2019]: 干得好，团队！你们的努力非常值得赞赏。我们设法在创纪录的时间内解决了这个紧急问题。让我们继续保持良好的工作状态 ![点赞表情](img/chatgpt-for-java-607613_1_En_3_Figh_HTML.gif) 一个点赞的手势表情符号。列表 3-5

在 Slack 频道中试图分析客户问题的团队成员

## 提示工程 101：文本摘要

因此，不用说，没有人愿意整天在 Slack 频道中不断滚动阅读关于正在燃烧的问题和问题的文章。我们将利用 ChatGPT 的文本摘要功能。为了保持简单，让我们尝试几个提示，将整个聊天消息列表发送给 ChatGPT，以便它给我们一个所有发生事件的可用摘要。

### 提示 #1：“tl;dr”

这个提示非常简洁、明了。如果你不熟悉它，这是一个在网上经常用来简要总结长篇文章的术语。它字面意思是“太长了；没读”，这正是我在工作繁忙时对 Slack 上许多对话的感受。方便的是，ChatGPT 可以理解这个简单的术语（我并不一定称之为单词）作为提示，结果相当令人印象深刻。**系统**：您是一个有用的助手**用户**：Fatima [16:00 | 02/08/2019]：大家好，我有一个紧急的...**用户**：tl;dr**模型**：gpt-4**温度**：1**最大长度**：360**Top P**：1**频率惩罚**：0**存在惩罚**：0 列表 3-6

提示。请求对较长的对话进行总结

注意

现在您有两种方法可以将前面的提示发送到 ChatGPT。第一种方法是使用 ChatGPTClient.java 应用程序及其支持类。第二种方法是使用 Chat Playground。在两种情况下，请确保第一个用户消息包含列表 3-5 中的所有文本。它在列表 3-6 中被截断，以便更易于阅读。

注意，令牌数量保持很小，为 360，这最终将帮助 ChatGPT 创建简短的响应。同时看到温度保持在 1（默认值），但 Top P 提高到最大值（即 1）。因此，重要的是要尝试调整温度和其他设置，以控制 ChatGPT 响应的语气和多样性。

列表 3-7 显示了 ChatGPT 对列表 3-5 中对话的摘要。![](img/chatgpt-for-java-607613_1_En_3_Figi_HTML.gif)Chat G P T 标志。团队迅速响应客户的崩溃问题。John 调查代码库，Fatima 从客户那里收集信息。他们发现与 iOS 15.1 不兼容的问题。John 修复了它。补丁经过审查并获得批准，应用程序在商店中更新。客户被告知并感谢快速解决。团队因他们的协作和迅速行动而受到赞扬。列表 3-7

响应。获取非常长对话的总结

太棒了！它将那个极其冗长的对话简化成了一个只有 68 个单词的简单摘要。如您所见，ChatGPT 在这里并没有取代任何工作；然而，它肯定会让人更加高效。现在，让我们尝试几个更多的提示，怎么样？

### Prompt #2: “用 3 句话或更少的解释”

因此，如果“tl;dr”没有提供足够简明的解释，那么我们可以告诉 ChatGPT 使事情更加简单。ChatGPT 在参数方面做得很好，所以让我们指定解释不应超过 3 句话，如列表 3-8 所示。**系统**: 你是一个有用的助手**用户**: 法蒂玛 [16:00 | 02/08/2019]: 嘿，大家好，我有一个紧急的...**用户**: 请用 3 句话或更少的解释。**模型**: gpt-4**温度**: 1**最大长度**: 250**Top P**: 0**频率惩罚**: 0**存在惩罚**: 0 列表 3-8

PROMPT. 请求一个更长对话的简短版本

如您所注意到的，在这个例子中，温度设置为 0.82。我们真的希望 ChatGPT 在这里给我们一个简洁的回答，所以“越干”越好！![Chat G P T 标志](img/chatgpt-for-java-607613_1_En_3_Figj_HTML.gif)一位客户向团队报告了一个紧急的应用程序崩溃问题。约翰调查了这个问题，并要求法蒂玛从客户那里收集更多信息。他们发现问题是与 iOS 15.1 的兼容性问题有关。约翰修复了这个问题，基思批准将修复部署到客户的生成环境中。列表 3-9

RESPONSE. 获取 3 句话的摘要

### Prompt #3: “我是一个经理。向我解释发生了什么”

当你不想听起来像是那个不理解的人时，ChatGPT 有重新表述所说内容并将其分解到非常简单的程度的能力（列表 3-10）。**系统**: 你是一个有用的助手**用户**: 法蒂玛 [16:00 | 02/08/2019]: 嘿，大家好，我有一个紧急的...**用户**: 总结这次对话，并像我对一个技术经验很少的经理一样解释给我听。**模型**: gpt-3.5-turbo**温度**: 0.82**最大长度**: 750**Top P**: 1**频率惩罚**: 0**存在惩罚**: 0 列表 3-10

PROMPT. 请求一个更复杂对话的简化版本

再次强调，温度被设置为低于 1.0，这样 ChatGPT 可以保持答案简短且易于理解。我们增加了标记长度，以便 ChatGPT 有足够的时间解释一些可能的技术概念。![Chat G P T 标志](img/chatgpt-for-java-607613_1_En_3_Figk_HTML.gif)在这个对话中，法蒂玛提到了一个紧急问题，客户在加载应用程序后立即遇到应用程序崩溃。基思指派约翰调查这个问题，因为他们的架构师因病缺席。约翰要求法蒂玛从客户那里收集有关他们的设备、操作系统和最近更新的额外信息。戴夫强调了在整个故障排除过程中保持客户知情的重要性。约翰检查了代码库，但没有发现任何明显的问题，所以他怀疑可能是与内存相关的问题。基思同意检查最近发布中的内存相关异常。法蒂玛提供更新称，客户使用的是运行 iOS 15.1 的 iPhone X，并提到问题是在更新应用程序后开始的。基思建议在 iOS 15.1 的 iPhone X 模拟器上测试最新的应用程序更新以重现问题。约翰在模拟器上成功重现了崩溃，并确定了一个与 iOS 15.1 的兼容性问题，可能是由于过时的方法调用。他修复了这个问题，并为审查和部署准备了一个补丁。基思批准了补丁，并要求约翰更新商店中的应用程序。戴夫要求保持客户知情，并且发布说明反映了即将进行的修复。约翰上传了补丁，并通知客户关于修复的信息。基思审查并批准了补丁，约翰继续在商店中更新应用程序。法蒂玛通知客户关于修复的信息，他们表示对快速响应感到欣慰和感激。戴夫称赞团队的合作和快速行动，强调了保持良好工作的重要性。总之，团队迅速解决了一个紧急问题，即客户的加载应用程序时崩溃的问题。他们调查了问题，确定了与 iOS 15.1 的兼容性问题，修复了它，并为部署准备了补丁。在整个过程中，客户都得到了通知，修复成功实施，客户感到欣慰和感激。列表 3-11

响应：获取更复杂对话的简化版本

### 提示 #4：“给我下一步的建议”

除了制作更容易理解的摘要外，ChatGPT 还可以用不同的风格和“语气”进行解释。我们将把 Top P 提高到 0.75，因为我们希望 ChatGPT 考虑比默认更多的可能性。我们还将增加存在惩罚到 0.5，因为我们希望鼓励多样化的回答。**系统**：您是一个有用的助手**用户**：Fatima [16:00 | 02/08/2019]：嘿，大家好，我有一个紧急的...**用户**：我是公司的 QA 工程师。给我一些建议的下一步行动。**模型**：gpt-4**温度**：1**最大长度**：1200**Top P**：0.75**频率惩罚**：0**存在惩罚**：0.5 列表 3-12

PROMPT. 向 ChatGPT 请求关于最佳下一步行动的建议

![](img/chatgpt-for-java-607613_1_En_3_Figl_HTML.gif)Chat G P T 标志。作为一名 QA 工程师，以下是一些建议的下一步行动：1. 测试补丁：一旦补丁部署到应用商店，请在各种设备和操作系统上彻底测试，以确保问题已解决，没有引入新的错误或回归。2. 进行回归测试：除了测试特定问题外，还要进行全面的回归测试，以确保修复不会对应用的其他功能产生意外的副作用。3. 将修复方案告知客户：保持客户对进度的更新，并让他们知道修复已在最新应用更新中可用。提供明确的指导，说明如何更新他们的应用，并鼓励他们在自己的端上测试。4. 监控用户反馈：修复部署后，密切关注用户反馈。鼓励用户报告他们遇到的问题，并积极及时地解决这些问题。5. 记录问题和解决方案：创建详细报告，记录问题、重现和解决步骤以及任何其他相关信息。这将作为未来故障排除的参考，并有助于改进开发过程。6. 进行事后分析：问题解决并部署修复后，安排一次团队的事后会议，讨论根本原因、经验教训以及可以实施以防止未来类似问题的流程改进。7. 持续改进：利用这次事件作为机会，识别开发和测试过程中的改进领域。评估是否可以做出任何改变以防止未来发生类似问题。记住，开放沟通、协作和持续学习是确保应用最高质量和维护与客户良好关系的关键。列表 3-13

RESPONSE. ChatGPT 关于可能下一步行动的建议

现在，当然，ChatGPT（就像地球上其他所有形式的人工智能一样）并不完全完美。例如，第三项建议是一个有效的操作项，但事实上，这通常不是 QA 人员的责任，以便直接与客户或客户沟通。这种沟通可以通过技术支持完成，或者与拥有这些沟通渠道的产品经理（特别是如果他们是重要客户）进行沟通。因此，建议是好的，但并不适合在公司中担任该角色的人。

### 让我们谈谈真正的提示工程

如果你搜索“提示工程”这个术语，你会找到大量的例子、博客，甚至有订阅计划的完整网站，它们会试图说服你，完美的提示可以通过仅使用文本来创建。正如你从上面的例子中看到的，提示工程不能仅仅通过仅仅构建文本输入来完成。

实际上，这个过程与烹饪一道复杂的菜肴非常相似。想象一下，例如，只用盐作为调味料来尝试烹饪波尔多牛肉，而忽略了所有其他成分和香料！说实话，结果与实际菜肴相比将相形见绌。

类似地，尝试组装一个完整的管弦乐队，但只使用一种乐器和一个音乐家。那将是一个尴尬的“单打独斗”。因此，仅仅调整文本以符合提示并不足以真正进行提示工程。模型温度等参数，它控制随机性；top-p，影响标记概率；使用的特定模型；标记数量；以及发送到端点的其他参数，都在获得良好响应中扮演着至关重要的角色。

这本书不是关于提示工程的，因为（正如你从上面的解释中可以看到）它真正涉及几个与 Java 无关的因素。然而，你被强烈鼓励尝试所有由 OpenAI 提供的模型和端点的参数，以找到最适合你用例的方案。

## 注册 Slack 机器人应用

现在我们知道了 ChatGPT 为我们总结大量文本的各种方法，让我们看看为了创建一个简单的 Java 机器人，该机器人可以程序化地从 Slack 实例中的某个频道获取所有消息，需要哪些条件。

注意

为了完成这些步骤，你需要对 Slack 工作空间有管理权限。大多数开发者**不会**有这些级别的权限；因此，为了完全实验，我建议你创建自己的个人 Slack 工作空间进行测试。这样，你将拥有安装你的 Slack 机器人的所有权利和特权。

但一步一个脚印。首先，我们将创建我们的 Slack 机器人应用，所以前往 Slack API 网站（图 3-1）。

[`api.slack.com/`](https://api.slack.com/)![](img/chatgpt-for-java-607613_1_En_3_Fig1_HTML.png)

Slack API 界面的截图。它显示了主屏幕，在顶部“您的应用”标签下有一个下拉菜单。

图 3-1

为了创建一个 Slack Bot，请访问 Slack API 网站

当然，您需要一个 Slack 账户才能使这生效，所以如果您还没有，那么您需要先创建一个。

登录后，前往页面右上角，导航到“**您的应用 ➤ 创建您的第一个应用**”，如图 3-1 所示。在 Slack 术语中，“bot”就是“应用”，并且除非它们已在 Slack 上注册，否则 bot 不允许在 Slack 实例上运行。![图片](img/chatgpt-for-java-607613_1_En_3_Fig2_HTML.png)

Slack API 界面的截图被创建应用弹出框覆盖。它列出了创建应用从头开始和应用程序清单的选项。

图 3-2

为 Slack 创建新的 Bot 应用

如图 3-2 所示，您将被带到**您的应用**页面，在那里您可以管理您的 Slack 应用。立即，您会在屏幕中间看到一个弹出创建**应用**按钮。

选择创建应用**从头开始**的选项。这是因为我们希望能够自己操作应用的所有细节，而不需要用一大堆默认设置来复杂化事情。

之后，您将被提示为您的 bot 指定一个名称，并选择您希望 bot 可以访问的工作空间，如图 3-3 所示。

点击**创建应用**按钮继续。![图片](img/chatgpt-for-java-607613_1_En_3_Fig3_HTML.png)

Slack API 界面的截图被 Name App 和选择工作空间弹出框覆盖。它列出了输入名称和工作空间的字段，以及取消和创建应用的按钮。

图 3-3

为 Slack 创建新的 Bot 应用

### 通过设置作用域来指定您的 Bot 可以（和不可以）做什么

现在，您将看到一个屏幕，它为 Slack 工作空间中的 bot 提供了大量选项。然而，您首先需要从左侧的侧边栏中点击**OAuth & Permissions**。

我们的 bot 将会非常简单；它只需要从频道中读取消息，以便为我们提供所说的内容的摘要。除了读取消息外，我们还需要知道 Slack 工作空间中人的名字；否则，我们将得到一个表示人的 UUID，这对我们来说是没有意义的。

因此，向下滚动并确保将以下 OAuth 作用域添加到您的 Slack Bot 中，如图 3-4 所示。

+   channels:history

+   channels:read

+   users:read

![图片](img/chatgpt-for-java-607613_1_En_3_Fig4_HTML.png)

Slack API 界面的截图。它显示了作用域下的应用。在 Bot 令牌作用域下列出了 OAuth 作用域和描述。

图 3-4

为 Slack Bot 应用添加作用域

### 确认您的设置

在为你的机器人添加了适当的作用域后，向上滚动并从左侧栏点击**基本信息**。

在接下来的页面上，你会看到现在“添加功能”旁边有一个绿色的勾选标记，这确认你已经正确添加了作用域，如图 3-5 所示。![图 3-5](img/chatgpt-for-java-607613_1_En_3_Fig5_HTML.png)

Slack API 界面的截图。在显示基本信息的设置下选中了块信息。它显示了以下选项：添加功能，安装应用，管理分发。

图 3-5

确认你的设置

### 查看 OAuth 和权限页面

如图 3-6 所示，导航到**OAuth & Permissions**页面并点击“安装到工作区”按钮。![图 3-6](img/chatgpt-for-java-607613_1_En_3_Fig6_HTML.png)

Slack API 界面的截图。在显示高级功能选项下选中了 OAuth 和权限，通过令牌轮换和为工作区设置提供 OAuth 令牌的高级令牌安全。

图 3-6

OAuth & Permission 屏幕

### 将你的 Slack 机器人应用到工作区

现在所有权限都已请求，是时候将你的机器人安装到工作区了。在安装过程中，你应该会看到一个如图 3-7 所示的屏幕。![图 3-7](img/chatgpt-for-java-607613_1_En_3_Fig7_HTML.png)

Slack 窗口的截图。它显示了以下消息。Tester Bot 请求访问 Apress Book Testing Slack 工作区的权限，并且已选中允许按钮。

图 3-7

“安装”新的 Slack 机器人应用

点击**允许**按钮以授权机器人并允许你在上一步分配的权限。

注意

在这里理解“安装”的含义很重要。在传统的 Java 意义上，安装一个应用意味着将 JAR、WAR 或 EAR 文件加载到另一台机器上并执行它。这里的情况并非如此。

在这里，当你“安装”一个机器人应用时，你是在使你的 Slack 工作区允许应用加入工作区——仅此而已。你的机器人代码将在你的机器上运行，而不是在 Slack 的服务器上。

### 获取你的 Slack 机器人（访问）令牌

这次，“令牌”实际上是指访问令牌！为了连接到 Slack API 并以编程方式访问消息和用户信息，你需要为你的 Slack 机器人生成一个特定的 OAuth 令牌！![图 3-8](img/chatgpt-for-java-607613_1_En_3_Fig8_HTML.png)

Slack API 界面的截图。在显示高级功能选项下选中了 OAuth 和权限，通过令牌轮换和为工作区提供带有机器人用户 OAuth 令牌的 OAuth 令牌的高级令牌安全。

图 3-8

复制你的 Slack 机器人应用的 OAuth 令牌

返回到**OAuth & Permissions**页面，确保从页面此处复制机器人令牌（通常以“xoxb-”开头），如图 3-8 所示。

### 邀请您的机器人到频道

接下来，您将前往您想要测试机器人的频道，并在该频道本身输入以下命令./invite

选择“**将应用程序添加到此频道**”选项，然后选择您在将机器人与 Slack 注册时指定的 Slack 机器人的名称。

![图片](img/chatgpt-for-java-607613_1_En_3_Fig9_HTML.jpg)

一张截图显示了一个下拉列表，列出了以下选项：邀请某人加入此频道、邀请新成员加入此工作空间和将应用程序添加到此频道。已选择“将应用程序添加到此频道”选项。

图 3-9

将您的 Slack 机器人添加到频道

恭喜！您现在已成功在 Slack 上注册了 Slack 机器人应用程序，并使其能够读取您工作空间中的消息，并将 Slack 机器人添加到了频道。在我们能够编写 Java 代码来访问我们工作空间中的频道之前，我们需要知道 Slack 为我们频道使用的内部 ID。

## 查找您频道的频道 ID

好的，这是一个简单的步骤。在 Slack 中，右键单击您频道的名称，选择“**查看** **频道详情**”选项。弹出窗口的底部是您频道的 ID。复制该数字并保存以备后用。您的 Java 应用程序需要这个 ID 才能加入 Slack 工作空间中的正确频道。

## 使用您的 Slack 机器人应用程序自动从频道抓取消息

好的，现在我们已经完成了所有先决条件，并且知道了我们频道的 ID，让我们来看看 Java 代码，该代码可以访问特定 Slack 频道中的所有消息。

### 设置您的依赖项

Slack API 库为 Java 提供了方便的方法来与 Slack 平台交互。我们需要的几乎所有内容都来自 com.slack.api.methods.*或 com.slack.api.model.*包，这些包存在于 slack-api-client-<VERSION>和 slack-api-model-<VERSION> jar 文件中。

Slack Java API 有其自己的依赖项，包括

+   GSON

    +   gson-<VERSION>.jar

+   Kotlin

    +   kotlin-stdlib-<VERSION>.jar

    +   kotlin-stdlib-jdk8-<VERSION>.jar

+   OK HTTP 和 OK IO

    +   okhttp-<VERSION>.jar

    +   okio-<VERSION>.jar

    +   okio-jvm-<VERSION>.jar

+   SL4J

    +   slf4j-api-<VERSION>.jar

因此，列表 3-14 和 3-15 是 Maven pom.xml 和 Gradle build.gradle 文件中必要的片段（使用我测试的版本），以便构建一切。    <dependencies>        <!-- Gson 库 -->        <dependency>            <groupId>com.google.code.gson</groupId>            <artifactId>gson</artifactId>            <version>2.10.1</version>        </dependency>        <!-- Kotlin 标准库 -->        <dependency>            <groupId>org.jetbrains.kotlin</groupId>            <artifactId>kotlin-stdlib</artifactId>            <version>1.6.20</version>        </dependency>        <dependency>            <groupId>org.jetbrains.kotlin</groupId>            <artifactId>kotlin-stdlib-jdk8</artifactId>            <version>1.6.20</version>        </dependency>        <!-- OkHttp 库 -->        <dependency>            <groupId>com.squareup.okhttp3</groupId>            <artifactId>okhttp</artifactId>            <version>4.11.0</version>        </dependency>        <!-- Okio 库 -->        <dependency>            <groupId>com.squareup.okio</groupId>            <artifactId>okio</artifactId>            <version>3.2.0</version>        </dependency>        <dependency>            <groupId>com.squareup.okio</groupId>            <artifactId>okio-jvm</artifactId>            <version>3.2.0</version>        </dependency>        <!-- Slack SDK 库 -->        <dependency>            <groupId>com.slack.api</groupId>            <artifactId>slack-api-client</artifactId>            <version>1.30.0</version>        </dependency>        <dependency>            <groupId>com.slack.api</groupId>            <artifactId>slack-api-model</artifactId>            <version>1.30.0</version>        </dependency>        <!-- SLF4J 日志门面 -->        <dependency>            <groupId>org.slf4j</groupId>            <artifactId>slf4j-api</artifactId>            <version>2.0.7</version>        </dependency>    </dependencies>列表 3-14

Maven pom.xml

dependencies {    // Gson 库    implementation 'com.google.code.gson:gson:2.10.1'    // Kotlin 标准库    implementation 'org.jetbrains.kotlin:kotlin-stdlib:1.6.20'    implementation 'org.jetbrains.kotlin:kotlin-stdlib-jdk8:1.6.20'    // OkHttp 库    implementation 'com.squareup.okhttp3:okhttp:4.11.0'    // Okio 库    implementation 'com.squareup.okio:okio:3.2.0'    implementation 'com.squareup.okio:okio-jvm:3.2.0'    // Slack SDK 库    implementation 'com.slack.api:slack-api-client:1.30.0'    implementation 'com.slack.api:slack-api-model:1.30.0'    // SLF4J 日志门面    implementation 'org.slf4j:slf4j-api:2.0.7'}compileKotlin {    kotlinOptions {        jvmTarget = "1.8"    }}compileTestKotlin {    kotlinOptions {        jvmTarget = "1.8"    }}列表 3-15

Gradle build.gradle

现在我们已经拥有了访问令牌以及所有必要的依赖项，接下来让我们看看访问频道并获取指定时间范围内的所有聊天记录所需的代码。出于明显的原因，我们想要获取频道中每条帖子的用户名、时间戳和消息内容。

### 使用 ChannelReaderSlackBot.java 从 Slack 读取消息

列表 3-16 是一个简单的 Java Slack Bot，它能够获取指定时间段内频道中每条帖子的用户名、时间戳和消息内容.import com.slack.api.Slack;import com.slack.api.methods.MethodsClient;import com.slack.api.methods.request.conversations.ConversationsHistoryRequest;import com.slack.api.methods.response.conversations.ConversationsHistoryResponse;import com.slack.api.methods.request.users.UsersInfoRequest;import com.slack.api.methods.response.users.UsersInfoResponse;import com.slack.api.model.Message;import com.slack.api.model.User;import com.slack.api.model.block.LayoutBlock;import java.time.*;import java.util.Collections;import java.util.List;public class ChannelReaderSlackBot {        private static final String SLACK_BOT_TOKEN = "YOUR_SLACK_API_TOKEN";        public static void main(String[] args) {        Slack slack = Slack.getInstance();        MethodsClient methods = slack.methods(SLACK_BOT_TOKEN);        String channelId = "YOUR_CHANNEL_ID";        LocalDateTime startTimeUTC = LocalDateTime.of(2023, Month.AUGUST, 3, 10, 0);        LocalDateTime endTimeUTC = LocalDateTime.of(2023, Month.AUGUST, 12, 15, 0);        long startTime = startTimeUTC.atZone(ZoneOffset.UTC).toEpochSecond();        long endTime = endTimeUTC.atZone(ZoneOffset.UTC).toEpochSecond();        ConversationsHistoryRequest request = ConversationsHistoryRequest.builder()            .channel(channelId)            .oldest(String.valueOf(startTime))            .latest(String.valueOf(endTime))            .build();        try {            ConversationsHistoryResponse response = methods.conversationsHistory(request);            if (response != null && response.isOk()) {                List<Message> messages = response.getMessages();                Collections.reverse(messages);                for (Message message : messages) {                    String userId = message.getUser();                    String timestamp = formatTimestamp(message.getTs());                    UsersInfoRequest userInfoRequest = UsersInfoRequest.builder()                        .user(userId)                        .build();                    UsersInfoResponse userInfoResponse = methods.usersInfo(userInfoRequest);                    if (userInfoResponse != null && userInfoResponse.isOk()) {                        User user = userInfoResponse.getUser();                        System.out.println("用户: " + user.getName());                        System.out.println("时间戳: " + timestamp);                        System.out.println("消息: " + message.getText());                        System.out.println();                    }                }            } else {                System.out.println("获取消息失败: " + response.getError());            }        } catch (Exception e) {            e.printStackTrace();        }    }    private static String formatTimestamp(String ts) {        double timestamp = Double.parseDouble(ts);        Instant instant = Instant.ofEpochSecond((long) timestamp);        LocalDateTime dateTime = LocalDateTime.ofInstant(instant, ZoneOffset.UTC);        return dateTime.toString();    }}列表 3-16

ChannelReaderSlackBot.java

当然，你应该将“YOUR_SLACK_API_TOKEN”替换为你的实际 Slack API 令牌，将“YOUR_CHANNEL_ID”替换为你想要读取消息的 Slack 通道的 ID。

如果你想做一些非常基础的事情，实际上 Slack Java API 的使用相当简单。在执行任何操作之前，你需要使用静态调用“Slack.getInstance()”方法来获取“Slack”类的实例。这连接到底层的 Slack API 基础设施，允许你与公开的方法交互并检索我们想要的信息。

接下来，我们需要通过调用“slack.methods()”方法来获取“MethodsClient”类的实例，我们提供我们的访问令牌。

为了检索聊天历史，我们使用 ConversationsHistoryRequest 类，这是 Slack API 提供的另一个类。在这里，你需要做的就是指定所需的通道 ID、最早的时间戳和最新的时间戳，以定义聊天历史的日期范围。在这个例子中，我们检索了从 2023 年 8 月 3 日 10:00 到 2023 年 8 月 12 日 15:00 的消息。简单易行。

列表 3-17 展示了执行 ChannelReaderSlackBot.java 后的输出，这里进行了截断，因为您已经在本章前面的列表 3-5 中看到了完整的文本。Fatima [2023-08-11T09:04:20]：大家好，我有一个紧急问题要讨论。我刚和一个客户通完电话，他们一加载应用就会崩溃。他们真的很沮丧。我们能尽快解决这个问题吗？:tired_face:Keith [2023-08-11T09:04:35]：谢谢你把这个问题带到我们的注意下，Fatima。让我们立即着手解决这个问题。John，由于我们的架构师今天因病缺席，你能负责调查这个问题吗？John [2023-08-11T09:04:52]：当然可以，Keith。我会深入代码库，看看是否能找到导致崩溃的潜在原因。John [2023-08-11T09:05:30]：Fatima，你能从客户那里收集一些额外的信息吗？请他们说明具体的设备、操作系统以及他们可能安装的任何更新……列表 3-17

执行 ChannelReaderSlackBot.java 的输出

## 留给读者的练习

因此，显然我们还可以做几件额外的事情，这些步骤将留给您（读者）来完成，例如：

+   使 ChatGPTClient.java（相关类）对新手用户更加安全。例如，对于 ChatGPT，top P 参数的有效值仅在 0 到 1 之间。如果用户指定的任何内容超出了任何有效值的范围，Chat.java 类的构造函数应该抛出异常。

+   将 ChannelReaderSlackBot.java 中读取 Slack 消息的代码与 ChatGPTClient.java 连接起来，以便抓取消息并获取摘要成为一个单一的过程。

+   向 Slack 机器人本身添加更多功能，例如添加命令，以便频道中的任何人都可以请求摘要。在当前状态下，机器人不会在频道中发布任何内容。然而，机器人的“用户界面”就是频道本身；因此，应该有人能够通过输入命令（例如请求摘要）与 Slack 机器人进行交互。

+   确保机器人不会使糟糕的情况变得更糟。每当机器人提供摘要时，它都不应该在频道本身发布，因为这可能会给已经嘈杂的情况增加很多噪音。最佳实践是让机器人向请求摘要的人（或你创建的任何新命令）发送私密消息。

## 结论

在本章中，我们讨论了人工智能在当今企业中可以应用的多种实用方式之一。我们展示了如何通过利用构建者模式来改进我们的 ChatGPTClient.java 应用程序，从而使你的类构建比上一章更加灵活。

然而，最值得注意的是，我们讨论了真正的“提示工程”是什么，通过讨论提示工程不能仅仅通过向 ChatGPT 单独输入文本来完成。为了正确和有效地进行提示工程，你绝对需要理解 ChatGPT API 所有输入参数的后果。

利用我们关于提示工程的知识，我们能够成功地获取任何提供给我们的大量文本的摘要。最后，我们看到了运行一个自动机器人从任何 Slack 频道程序化地抓取消息所需的代码，如果我们指定一个有效的日期范围的话。

在本章（以及上一章）中，我们一直在使用 OpenAI API 的 Chat Completions 端点。在下一章，我们将通过实验 Whisper 和 DALL·E 端点来拓展可能性的边界。

© 作者（们），独家授权给 APress 媒体公司，Springer Nature 部分版权所有 2024B. HopkinsChatGPT for Java[`doi.org/10.1007/979-8-8688-0116-7_4`](https://doi.org/10.1007/979-8-8688-0116-7_4)

# 4. 多模态 AI：使用 Whisper 和 DALL·E 3 创建播客可视化器

布鲁斯·霍普金斯^(1  )(1)美国俄勒冈州比佛顿 Now let’s introduce a new term: **multimodal AI**. In the most simplest of terms, generative AI models can create content in 1 of 4 formats:

+   文本

+   音频

+   图片

+   视频

这些格式中的每一个都是一个**模式**。多模态 AI 是使用多个 AI 模型一起生成（或理解）内容的过程，其中输入是一种模式，输出是另一种模式。

以 OpenAI 的 Whisper 模型为例。如果你提供音频，它能够将所说的所有内容转录成文本。同样，这也适用于 DALL⋅E。如果你提供文本提示，它就能够生成你所描述的图像。

在本章中，我们将把多模态人工智能提升到新的水平！作为一名热衷的播客听众，我常常想知道在收听音频格式的非常沉浸式故事时，场景、意象、人物、主题或背景看起来是什么样子。

因此，我们将使用 OpenAI 的多个模型创建一个播客可视化器。涉及几个步骤，但最终结果令人惊叹。在收听关于一个用豆腐烹饪一些令人惊叹的事情的播客（不要尝试之前就贬低它）时，播客可视化器产生了图 4-1 中的图像。![图 4-1](img/chatgpt-for-java-607613_1_En_4_Fig1_HTML.png)

一张戴着眼镜、手持一碗豆腐的男人的特写照片。

图 4-1

使用 GPT-4、Whisper 和 DALL⋅E 模型可视化关于豆腐的播客的 AI 生成结果

为了使播客可视化器的代码易于理解，我们将在以下三个步骤中分别进行操作：

+   Step-1: 选择一个播客节目并使用 Whisper 模型获取转录本。

+   Step-2: 将生成的转录本用于 GTP-4 模型以描述播客节目中讨论内容的视觉方面。

+   Step-3: 将生成的描述用于 DALL⋅E 模型以生成图像。

本章中展示的代码具有许多实际用途，例如：

+   如果您只是对播客节目中事物可能看起来什么样感到好奇（对我来说总是这样），您可以得到一个简单的代表性视觉图像来关联您正在收听的内容。

+   对于听力受损的人，您可以轻松地将播客或广播节目转换成图像幻灯片。这大大提高了内容的可访问性。

+   对于播客制作者来说，现在您可以简单地将视觉/英雄图像添加到每个播客节目中。这很有用，因为播客播放器，如 Apple Podcasts 和 Spotify，允许播客制作者显示单个图像以关联到单个节目。这有助于提高听众的参与度。

## 介绍 OpenAI 的 Whisper 模型

现在让我们介绍另一个新术语：**自动语音识别** (ASR)。由于该技术集成到移动电话（例如，iPhone 的 Siri）和智能扬声器（例如，任何 Alexa 设备）中，普通消费者对此技术非常熟悉。在其核心，ASR 技术将语音转换为文本。

Whisper 是 OpenAI 的语音识别模型，其准确率令人惊讶。列表 4-1 是 DuoLingo 西班牙语播客一集的转录，该播客通过将英语和西班牙语结合在一个编织的故事中，使西班牙语对英语听众来说更容易理解。转录是使用 Whisper 模型生成的。……我是 Martina Castro。每一集我们都会带来引人入胜的真实故事，帮助你提高西班牙语听力并从世界中获得新的视角。讲述者将使用中级西班牙语，而我将用英语提供背景信息。如果你错过了什么，你可以随时回放并再次收听。我们还在 podcast.duolingo.com 提供完整的转录。Linda 在成长过程中对她的祖母 Erlinda 非常着迷。Erlinda 是一位治疗师或 curandera，她为精神、情感、身体或精神疾病提供治疗方法。在危地马拉，这种做法是通过家族内部代代相传的口头传统。许多危地马拉人认为，人类有能力将负面能量传递给他人，因此他们把婴儿带到 Linda 的祖母那里，当他们怀疑有能量失衡时。她的母亲会带他去我们家治疗……列表 4-1

Whisper 模型执行语音识别，将音频转换为文本 如果你之前曾经使用过语音识别系统（即使是像 Siri 和 Alexa 这样的复杂技术），你就会知道它存在问题，例如：

+   **语音识别在处理标点符号时存在问题**

    +   你有没有注意到没有人说话时使用标点符号？对于英语来说，我们使用音调或音量的变化来提问或感叹。我们还会使用短停顿和长停顿来表示逗号和句号。

+   **语音识别在处理外来词和口音时存在问题**

    +   根据你问的人，英语中至少有 170k 个单词。然而，在英语口语中，我们总是使用外语，例如

        +   海啸（日语起源）：由地震引起的大海浪

        +   Hors d’oeuvre（法语起源）：开胃菜

        +   Lingerie（法语起源）：女性的内衣或睡衣

        +   Aficionado（西班牙语起源）：对某个特定活动或主题非常热情的人

        +   Piñata（西班牙语起源）：一个色彩鲜艳的糖果盒，孩子们可以不停地敲打

+   **语音识别在处理人名时存在问题**

    +   有些人名、公司名和网站名往往拼写困难，难以理解

+   **语音识别在处理同音异义词时存在问题**

    +   你还记得那些发音相同但拼写和意义不同的单词吗？这本书的神奇编辑者知道所有这些！

        +   Would / Wood

        +   Flour / Flower

        +   Two / Too / To

        +   They’re / There / Their

        +   Pair / Pare / Pear

        +   Break / Brake

        +   Allowed / Aloud

如你所见，从列表 4-1 中可以看出，Whisper 能够理解音频中的所有标点符号，识别所有外语（其中有很多），并且理解 URL 中的名字以及公司名称（“duolingo”）！当然，如果你注意到了，它也能理解“wood”和“would”之间的区别。

## Whisper 模型的功能和限制

Whisper 模型能够将以下语言的口语音频转换为文本：

+   阿非利堪斯语

+   阿拉伯语

+   亚美尼亚语

+   阿塞拜疆语

+   白俄罗斯语

+   波斯尼亚语

+   保加利亚语

+   加泰罗尼亚语

+   中文

+   克罗地亚语

+   捷克语

+   丹麦语

+   荷兰语

+   **英语**（当然！）

+   爱沙尼亚语

+   芬兰语

+   法语

+   加利西亚语

+   德语

+   希腊语

+   希伯来语

+   印地语

+   匈牙利语

+   冰岛语

+   印度尼西亚语

+   意大利语

+   日语

+   卡纳达语

+   哈萨克语

+   韩语

+   拉脱维亚语

+   立陶宛语

+   马其顿语

+   马来语

+   马拉地语

+   毛利语

+   尼泊尔语

+   挪威语

+   波斯语

+   波兰语

+   葡萄牙语

+   罗马尼亚语

+   俄语

+   塞尔维亚语

+   斯洛伐克语

+   斯洛文尼亚语

+   西班牙语

+   斯瓦希里语

+   瑞典语

+   菲律宾语

+   泰米尔语

+   泰语

+   土耳其语

+   乌克兰语

+   乌尔都语

+   越南语

+   威尔士语

所以，最终，它将能够理解你自己说的音频，以及可能你朋友和同事说的任何语言。

开发者被限制每分钟向端点发送不超过 50 个请求，因此如果你想要转录大量音频，需要考虑这个限制。

Whisper 支持以下格式的音频：flac、mp3、mp4、mpeg、mpga、m4a、ogg、wav 或 webm。无论你使用哪种格式，发送到端点的最大文件大小为 25MB。

现在，如果你没有大量处理音频文件，请注意，某些格式会创建非常大的文件（例如，wav 格式），而其他格式会创建非常小的文件（例如，m4a 格式）。因此，将你的文件转换为不同的格式可以帮助你克服 25MB 的限制。然而，在本章的后面，我们将看到如何使用一个工具将单个大音频文件分割成多个较小的文件。

## 转写端点

转写端点是一个 REST 服务，它将音频转换为文本，并且仅与 Whisper 模型兼容。

### 创建请求

表 4-1 列出了调用转写端点所需的全部 HTTP 参数。表 4-1

转写端点的 HTTP 参数

| HTTP 参数 | 描述 |
| --- | --- |
| 端点 URL | [`api.openai.com/v1/audio/transcriptions`](https://api.openai.com/v1/audio/transcriptions) |
| 方法 | POST |
| 头部 | 授权：Bearer **$OPENAI_API_KEY** |
| 内容类型 | multipart/form-data |

备注

请密切注意前面表格中的内容类型！与发送所有 HTTP 请求参数作为 JSON 对象的 Chat 端点不同，转写端点仅接受作为 **表单数据元素** 的参数。如果你尝试发送格式良好的（甚至格式糟糕的）JSON 对象，转写端点将返回一个非常模糊的错误。

### 请求体（多部分表单数据）

表 4-2

Whisper 请求体

| 字段 | 类型 | 是否必需 | 描述 |
| --- | --- | --- | --- |
| 文件 | 文件 | 必需 | 您想要转录的整个音频文件。接受的格式是• flac• mp3• mp4• mpeg• mpga• m4a• ogg• wav• webm |
| 模型 | 字符串 | 必需 | 您想要用于转录的模型的 ID。兼容的模型包括• whisper-1 |
| 提示 | 字符串 | 可选 | 这可以是提供给模型以改变转录风格或从之前的音频片段提供更多上下文的任何文本。请确保提示与音频语言相同，以获得最佳结果。此外，此字段可用于更改 Whisper 不熟悉的任何单词的拼写或大小写。 |
| 响应格式 | 字符串 默认值：json | 可选 | 这是转录输出的格式。接受的格式是• json• text• srt• verbose_json• vtt |
| 温度 | 数字 默认值：0 | 可选 | 这是采样温度，范围从 0 到 1。更高的值会增加输出的随机性，而较低的值确保输出更加确定。 |
| 语言 | 字符串 | 可选 | 这是输入音频的语言。这是可选的，但提供此值可以提高转录的准确性和延迟。 |

## 创建分割音频文件的实用应用程序：AudioSplitter.java

因此，我们几乎到了能够使用转录端点程序调用 Whisper 模型的地步。然而，Whisper 模型对每个文件的限制是 25MB。

现在，如果您正在收听，例如，德克萨斯大学奥斯汀分校的 StarDate 播客，这不会成为问题。这个播客在约 2 分钟的音频中为您提供了关于夜空中要寻找什么的绝佳视角。然而，对于其他音频节目，它们通常持续长达一小时（甚至更长）。在这种情况下，您肯定会超过 25MB 的文件限制。

因此，让我们与 ChatGPT 进行配对编程，并利用我们的人类智慧来创建我们自己的实用程序，该实用程序将单个音频文件分割成多个更小的文件。

注意

在本节中，我将展示如何将大型音频文件分割成更小片段的多种可能性之一。例如，您可以使用流行的音频编辑应用程序（如开源工具 Audacity 或授权工具 Adobe Audition）手动将大文件切割成更小的文件。

列表 4-2 是我发送给 ChatGPT 以获取分割音频文件的基本应用程序的提示。**系统**：您是一位 Java 开发者**用户**：编写一个应用程序，它接受单个 MP3 文件作为输入，并将文件分割成不超过 10 分钟的连续片段。文件名为"AudioSplitter.java"列表 4-2

PROMPT. 使用 ChatGPT 创建 AudioSplitter.java 应用程序

经过一番尝试，我能够创建（如列表 4-3 所示）包含我对 ChatGPT 生成的代码编辑的 AudioSplitter.Java 应用程序！![开放 AI 的标志](img/chatgpt-for-java-607613_1_En_4_Figa_HTML.gif)导入 org.bytedeco.javacv.FFmpegFrameGrabber;导入 org.bytedeco.javacv.FFmpegFrameRecorder;导入 java.io.IOException;public class AudioSplitter {        public static void main(String[] args) {        String inputFilePath = "path/to/file/sample.mp3";        String outputDirectory = "path/to/folder/";        int segmentDurationInSeconds = 600; // 10 minutes in seconds        try (FFmpegFrameGrabber grabber = new FFmpegFrameGrabber(inputFilePath)) {            grabber.start();            long totalDurationInSeconds = (long) grabber.getLengthInTime() / 1000000; // Convert microseconds to seconds            double frameRate = grabber.getFrameRate();            long segmentStartTime = 0;            long segmentEndTime;            int segmentNumber = 1;            while (segmentStartTime < totalDurationInSeconds) {                String outputFilePath = outputDirectory + "segment_" + segmentNumber + ".mp3";                try (FFmpegFrameRecorder recorder = new FFmpegFrameRecorder(outputFilePath, 0)) {                    recorder.setAudioChannels(2);                    recorder.setAudioCodecName("libmp3lame"); // Set the audio codec to MP3                    recorder.setAudioBitrate(192000); // Adjust bitrate as needed                    recorder.setSampleRate(44100); // Adjust sample rate as needed                    recorder.setFrameRate(frameRate);                    recorder.setFormat("mp3"); // Set the output format to MP3                    recorder.start();                    segmentEndTime = Math.min(segmentStartTime + segmentDurationInSeconds, totalDurationInSeconds);                    grabber.setTimestamp(segmentStartTime * 1000000); // Set the grabber's timestamp to the start time in microseconds                    while (grabber.getTimestamp() / 1000000 < segmentEndTime) {                        recorder.record(grabber.grabSamples());                    }                }                segmentStartTime = segmentEndTime;                segmentNumber++;            }        } catch (IOException e) {            e.printStackTrace();        }        }}列表 4-3

RESPONSE. AudioSplitter.java

由于标准的 Java 库对各种媒体格式的支持不够广泛，我们正在使用 FFmpeg 库和 JavaCV（两者都是免费和开源的）的组合。

目标很简单：使用 Java 语言将 MP3 文件分割成连续的段，每段不超过 10 分钟。在这个简单的应用程序中，我们执行以下步骤：

+   首先，我们指定输入文件路径、输出目录和所需的段持续时间（以秒为单位，10 分钟）。

+   接下来，我们使用 FFmpegFrameGrabber 打开输入 MP3 文件，并收集有关它的信息，例如帧率、音频编解码器、采样率等。

+   之后，我们遍历输入 MP3 文件，将其分割成指定持续时间（10 分钟或更短）的小部分。对于每个部分，我们创建一个新的 FFmpegFrameRecorder，设置其参数，并在段持续时间内记录帧。

+   最后，我们增加每个段的起始时间和段号，直到我们处理完整个输入 MP3 文件。

为了使这可行，你需要正确安装和配置 JavaCV 和 FFmpeg 库在你的项目中。

注意

FFmpeg 是一个开源的二进制文件，你需要在你的机器上安装它，并将其放置在 PATH 中或在你的项目中使其可访问。JavaCV 通过 JNI（Java 本地接口）使用 FFmpeg。

FFmpeg 是一个非常通用的媒体转换器，它不仅处理 MP3 音频文件，还处理各种其他音频文件格式（包括 M4A、OGG 和 WAV）。它还能够转换视频格式以及静态图像，如 PNG、JPEG 和 GIF。

在对 MP3 文件运行 AudioSplitter.java 实用程序后，你将有一个包含分割音频文件的文件夹，这些文件长度为 10 分钟或更短。使用 AudioSplitter.java 实用程序，你可以在单个 Java 文件中修改最适合你的设置。就我们的目的而言，这里的目的是拥有小于 25MB 的音频文件，所以如果你以 WAV 格式转录 8 小时的法庭程序，例如，你可能需要调整持续时间，使其更短，比如 6 分钟长度。

当使用 AudioSplitter 时，最佳实践是将输出文件夹与输入文件夹分开，你将在我们开始使用 Whisper 模型调用 Transcriptions Endpoint 时看到原因。

## 创建音频转录器：WhisperClient.java

现在，让我们构建我们的下一个 Java 应用程序，WhisperClient.java。同样，我们将与 ChatGPT 进行结对编程，以获得工作的基础。这次，我们将要求使用 OK HTTP 库来构建此应用程序，原因有两个：

+   我们已经在第三章中使用了这个库来构建 Slack Bot 应用程序。

+   当使用 HTTP 多部分表单时，OK HTTP 库使得操作变得稍微容易一些。列表 4-4 是放入 Chat Playground 以开始操作的提示。请注意，我要求 60 秒的 HTTP 请求超时，因为 Whisper 可能需要一点时间来生成转录本。**系统**：您是一位 Java 开发者。**用户**：将以下代码从 cURL 转换为 Java，使用 OkHttp 发送请求。确保我的请求有 60 秒的超时。遍历我的本地计算机上的单个文件夹，并将文件夹中的所有文件发送到 webservice。文件名为 WhisperClient.java。**用户**：curl https://api.openai.com/v1/audio/transcriptions \  -H "Authorization: Bearer $OPENAI_API_KEY" \  -H "Content-Type: multipart/form-data" \  -F file="@/path/to/file/audio.mp3" \  -F model="whisper-1"**模型**：gpt-4**温度**：1**最大长度**：1150 列表 4-4

PROMPT: 请 ChatGPT 将 cURL 转换为 Java 并发送到 Whisper 的 API

经过一番讨论，这是 ChatGPT 给出的有效响应，如列表 4-5 所示。![开放 AI 的标志](img/chatgpt-for-java-607613_1_En_4_Figb_HTML.gif)A logo of open A I.import java.io.*;import java.nio.file.*;import okhttp3.*;import java.util.*;import java.util.concurrent.TimeUnit;import java.util.stream.Collectors;import java.util.stream.Stream;/*** 客户端类，用于使用 OpenAI Whisper 模型转录 MP3 文件。*/public class WhisperClient {    public static void main(String[] args) throws IOException {        // OpenAI 的 API 密钥（这应该替换为你的实际 API 密钥）        String openAIKey = "";        // OpenAI 转录端点        String endpoint = "https://api.openai.com/v1/audio/transcriptions";        // 用于转录的模型        String model = "whisper-1";        // MP3 文件的媒体类型        MediaType MEDIA_TYPE_MP3 = MediaType.parse("audio/mpeg");        // 包含要转录的 MP3 文件的文件夹        String mp3FolderPath = "/Users/me/audio/segments";        // 转录响应期望的格式        String responseFormat = "text";        // 使用指定的超时配置 HTTP 客户端        OkHttpClient client = new OkHttpClient.Builder()            .connectTimeout(60, TimeUnit.SECONDS)            .writeTimeout(60, TimeUnit.SECONDS)            .readTimeout(60, TimeUnit.SECONDS)            .build();        // 存储目录中所有 mp3 文件的列表        List<File> mp3Files = new ArrayList<>();        // 尝试收集目录中的所有 mp3 文件并将它们存储在列表中        try (Stream<Path> paths = Files.walk(Paths.get(mp3FolderPath))) {            mp3Files = paths                .filter(Files::isRegularFile)                .filter(p -> p.toString().endsWith(".mp3"))                .map(Path::toFile)                .sorted(Comparator.comparing(File::getName)) // 按字母顺序排序文件                .collect(Collectors.toList());        } catch (IOException e) {            System.out.println("文件读取错误: " + e.getMessage());            return; // 如果读取文件出错，则退出        }        // 遍历每个 MP3 文件，转录它并打印响应        for (File mp3File : mp3Files) {            // 构建转录请求体            RequestBody requestBody = new MultipartBody.Builder()                .setType(MultipartBody.FORM)                .addFormDataPart(                    "file",                    mp3File.getName(),                    RequestBody.create(mp3File, MEDIA_TYPE_MP3))                .addFormDataPart("model", model)                .addFormDataPart("response_format", responseFormat)                .build();            // 构建 HTTP 请求            Request request = new Request.Builder()                .url(endpoint)                .header("Authorization", "Bearer " + openAIKey)                .post(requestBody)                .build();            // 发送请求并处理响应            try (Response response = client.newCall(request).execute()) {                if (!response.isSuccessful()) throw new IOException("Unexpected code " + response);                System.out.println(response.body().string());            } catch (IOException e) {                System.out.println("文件：" + mp3File.getName() + " 的请求错误 - " + e.getMessage());            }        }    }}列表 4-5

响应：WhisperClient.java

如你所见，OkHttpClient 类允许我们使用 Builder 模式创建一个具有我们指定的超时设置的类实例。

现在，这里就是为什么在使用 AudioSplitter.java 工具时，将输出文件夹与输入文件夹分开是一个好主意的原因。我们正在创建一个包含目录内所有 MP3 文件的集合。更具体地说，它是一个名为“mp3Files”的“List<File>”，用于保存我们想要转录的所有文件。因此，如果我们想要分割成更小段落的文件与这些段落在同一个文件夹中，那么我们将把大于 25MB 的大文件（即那个大于 25MB 的文件）以及较小的文件一起发送到转录端点，这违背了使用 AudioSplitter.java 应用程序的目的。

因此，“Files.walk()”方法允许我们递归遍历“mp3FolderPath”目录，收集所有 MP3 文件，并过滤掉不以“ .mp3”扩展名结尾的文件（出于安全考虑，并防止与 Web 服务发生任何错误）。然后，我们将每个“Path”映射到其对应的“File”对象，并根据文件名对文件进行字母排序。最后，我们使用“Collectors.toList()”方法将所有排序后的文件收集到“mp3Files”列表中。

手持一组 MP3 文件，现在是时候将它们发送到转录端点了。在我们构建 RequestBody 的过程中，你应该注意的最重要的一行是：.addFormDataPart("model", model) 和 .addFormDataPart("response_format", responseFormat)

这是因为如果你想在 HTTP 请求中添加任何可选参数（请参阅表 4-2 中所有参数），例如提示或温度，那么你需要以我们指定模型和响应格式相同的方式在这里添加它们。

注意

让我重申——调用转录端点与调用聊天端点完全不同。你可能已经注意到了 ChatGPTClient.java 和 WhisperClient.java 之间的一大主要区别是导入语句。ChatGPTClient.java（在第 2 和 3 章）的导入语句中包含了 Jackson 库，因为我们需要以 JSON 对象的形式发送请求。然而，WhisperClient.java 中的导入语句没有提及 Jackson，因为我们是以表单数据的形式发送所有内容的。

## 用播客尝试一些有趣的事情并尝试新事物

好的，那么让我们使用到目前为止所展示的代码运行一个测试。“This American Life”是一档由 Ira Glass 主持的每周公共广播节目（也是一个播客），由 WBEZ 芝加哥合作制作。

![图片](img/chatgpt-for-java-607613_1_En_4_Fig2_HTML.jpg)

一个播客标志，上面写着：This American Life from W B E Z。

图 4-2

如果你正在寻找一个有吸引力的故事播客，我推荐你听“This American Life”。图片来源：WBEZ 芝加哥

每一集都会围绕一个特定的主题或话题编织一系列故事。有些故事是调查性新闻，而其他故事则是采访有吸引力的故事的普通人。第 811 集的标题是“我无法去的地方”，文件大小为 56MB，MP3 格式。由于我们已经知道 56MB 太大，无法发送给 Whisper 进行转录，列表 4-6 显示了 AudioSplitter.java 在 MP3 文件上的输出。[mp3 @ 0x139e9c6a0] 从比特率估计持续时间，这可能是错误的输入#0，mp3，来自'/Users/me/thislife/ep811.mp3'：  元数据：    编码器         : Lavf58.78.100    注释         : preroll_1;postroll_1  持续时间：00:58:58.34，开始：0.000000，比特率：128 kb/s  流#0:0：音频：mp3，44100 Hz，立体声，fltp，128 kb/s 输出#0，mp3，到'/Users/me/thislife/segments/segment_1.mp3'：  元数据：    TSSE            : Lavf60.3.100  流#0:0：音频：mp3，44100 Hz，立体声，fltp，192 kb/s[libmp3lame @ 0x139ea92e0] 关闭队列时留下 2 帧 Output #0，mp3，到'/Users/me/thislife/segments/segment_2.mp3'：  元数据：    TSSE            : Lavf60.3.100  流#0:0：音频：mp3，44100 Hz，立体声，fltp，192 kb/s[libmp3lame @ 0x13b167720] 关闭队列时留下 2 帧 Output #0，mp3，到'/Users/me/thislife/segments/segment_3.mp3'：  元数据：    TSSE            : Lavf60.3.100  流#0:0：音频：mp3，44100 Hz，立体声，fltp，192 kb/s[libmp3lame @ 0x13b166df0] 关闭队列时留下 2 帧 Output #0，mp3，到'/Users/me/thislife/segments/segment_4.mp3'：  元数据：    TSSE            : Lavf60.3.100  流#0:0：音频：mp3，44100 Hz，立体声，fltp，192 kb/s[libmp3lame @ 0x13b166df0] 关闭队列时留下 2 帧 Output #0，mp3，到'/Users/me/thislife/segments/segment_5.mp3'：  元数据：    TSSE            : Lavf60.3.100  流#0:0：音频：mp3，44100 Hz，立体声，fltp，192 kb/s[libmp3lame @ 0x139ea35f0] 关闭队列时留下 2 帧 Output #0，mp3，到'/Users/me/thislife/segments/segment_6.mp3'：  元数据：    TSSE            : Lavf60.3.100  流#0:0：音频：mp3，44100 Hz，立体声，fltp，192 kb/s[libmp3lame @ 0x139ea3540] 关闭队列时留下 2 帧

在《美国生活》第 811 集上运行 AudioSplitter.java 的结果

由于 AudioSplitter.java 实用程序使用 JNI 包装器与 FFmpeg 接口，你会在音频分割过程中看到很多诊断信息，如列表 4-6 所示。除非你关心编解码器、频率和比特率，否则展示的大部分信息对你来说将毫无意义。然而，好消息是，我们现在有一个包含 6 个 MP3 文件的文件夹，这些文件已经准备好进行转录！

当然，正如你从列表 4-5 中的代码中可以看到，WhisperClient.java 遍历文件夹中的所有文件，并将它们发送到转录端点以使用 Whisper 模型。

列表 4-7 是该期节目全文转录本的摘录。“...我的表妹卡米勒并不是一个真正喜欢狗的人，但她有一只她非常喜爱的狗。它的名字叫福克斯，因为它看起来就像一只狐狸，只是它是黑色的。它是邻居的狗，但似乎她和卡米勒之间有一种真正的亲情，也许是因为她们都不离地面太远。当时卡米勒大约四到五岁，她有点口吃，所以福克斯听起来像是 Fozzie。我觉得这是我听过的最可爱的事情之一。卡米勒对福克斯的记忆几乎就像一部电影。她的记忆感觉像是无尽的夏日，模糊而完美，就像是在胶片上拍摄的场景。我刚刚想起了那种兴奋地去见福克斯的感觉。我脑海中有一个画面，就像来到房子里，我可以看到福克斯在外面。我可以看到福克斯通过通往花园的门。关于卡米勒和福克斯有一个故事，我经常在想。我已经和我的姐姐谈论了多年，但从未和卡米勒说过。那就是。有一次，当他们玩耍时...”列表 4-7

This American Life 第 811 期节目的部分转录本

为了简洁，我们只展示转录本的摘录。由于该期节目长度近 1 小时，全文转录本本身超过 8000 字。

## 走向元界：提示工程 GPT-4 为 DALL·E 编写提示

由于我们想要可视化的播客节目全文转录本有数千字，我们将使用 GPT-4 自动创建 DALL⋅E 模型所需的提示。DALL⋅E 能够根据提示中的文本描述创建图像，但最好将提示尽可能保持简短。列表 4-8 是 GPT-4 生成 DALL⋅E 提示的示例。**系统**：您是一个帮助可视化播客的服务。**用户**：阅读以下播客转录本。为视障人士描述代表该期节目整体主题的背景和主题。以下短语均可作为开头：“一张照片”、“一幅画”、“一张 35mm 的宏观照片”、“数字艺术”**用户**：支持 This American Life 来自 Squarespace...**模型**：gpt-4-32k**温度**：1.47**最大长度**：150**Top P**：0**频率惩罚**：0.33**存在惩罚**：0 列表 4-8

GPT-4 创建 DALL⋅E 提示的提示

如提示所示，我们使用的是 GPT-4 的 32k 令牌版本，以便我们处理非常长的文本转录本。DALL⋅E 需要知道要生成的图像类型，因此我们需要指定图像应该是照片、绘画、数字艺术等。我们需要确保 GPT-4 生成的文本尽可能短，因此我们希望最大长度为 150 个令牌。此外，为了防止 GPT-4 多次重复某些短语，我们引入了 0.33 的频率惩罚。

列表 4-9 展示了 GPT-4 在阅读 This American Life 第 811 集的转录后的结果。![图片](img/chatgpt-for-java-607613_1_En_4_Figc_HTML.gif)一个开放的 A I 标志。一位年轻女孩坐在花园里，旁边是一只看起来像狐狸的黑狗。女孩在微笑，狗摇着尾巴。图像有一种朦胧、梦幻般的感觉，带有粗糙的电影效果，以唤起怀旧之情。列表 4-9

GPT-4 创建的 DALL⋅E 提示

## Create Image 端点

为了使用 DALL⋅E 模型根据文本提示动态创建图像，您需要调用 **Create Image** 端点。

### 创建请求

表 4-3 列出了调用 Create Image 端点所需的全部 HTTP 参数。表 4-3

调用 Create Image 端点所需的 HTTP 参数

| HTTP 参数 | 描述 |
| --- | --- |
| 端点 URL | [`api.openai.com/v1/images/generations`](https://api.openai.com/v1/images/generations) |
| 方法 | POST |
| 标头 | Authorization: Bearer **$OPENAI_API_KEY** |
| Content-Type | application/json |

表 4-4 描述了用于 Create Image 端点请求体的 JSON 对象的格式。显然，提示是成功调用服务所需的唯一必需参数。

### Create Image (JSON)

表 4-4

Create Image 端点的请求体

| 字段 | 类型 | 必需？ | 描述 |
| --- | --- | --- | --- |
| 提示 | 字符串 | 必需 | 这里描述您想要创建的图像。dall-e-2 的最大长度为 1000 个字符，dall-e-3 的最大长度为 4000 个字符。 |
| model | 字符串 | 可选 | 生成图像的模型名称。兼容的模型包括：• "dall-e-2"• "dall-e-3" |
| n | 整数或 null 默认值: 1 | 可选 | 这是您想要创建的图像数量。必须在 1 到 10 之间。注意：由于 dall-e-3 所需的复杂性，OpenAI 可能会限制您的请求为单个图像。 |
| quality | 字符串默认值: "standard" | 可选 | 这允许您指定生成的图像质量。此参数仅对 dall-e-3 有效。接受的值有：• "standard"• "hd" |
| size | 字符串或 null 默认值: "1024x1024" | 可选 | 生成图像的大小。dall-e-2 可用的图像大小有：• "256x256"• "512x512"• "1024x1024"。dall-e-3 可用的图像大小有：• "1024x1024"• "1792x1024"（横向）• "1024x1792"（纵向） |
| style | 字符串默认值: "vivid" | 可选 | 这允许您指定生成的图像应该有多自然。此参数仅对 dall-e-3 有效。接受的值有：• "natural"（适合照片）• "vivid"（适合艺术外观） |
| response_format | 字符串或 null 默认值: "url" | 可选 | 这是生成图像的格式。接受的值有：• "url"• "b64_json" |
| user | 字符串 | 可选 | 这是一个代表您的最终用户的唯一标识符，可以帮助 OpenAI 监控和检测滥用。 |

### 处理响应

在成功调用创建图像端点后，API 将响应一个图像 JSON 对象。以下是图像对象的分解，它只有一个参数（表 4-5）。

### 图像 (JSON)

表 4-5

图像 JSON 对象的结构

| 字段 | 类型 | 描述 |
| --- | --- | --- |
| url（或）b64_json | 字符串 | 如果请求中的 response_format 是 "url"，则这是一个指向您生成的图像的 URL。（或）如果请求中的 response_format 是 "b64_json"，则这是一个 base64 编码的 JSON 图像。 |

## 创建图像生成器：DALLEClient.java

如您从表 4-4 和 4-5 中可以看到，创建图像端点与聊天端点行为相当相似：您需要指定给 DALL⋈E 模型的全部内容都封装在一个 JSON 对象中。因此，我们代码中的列表 4-10 也将使用 Jackson 库，因为我们还将再次处理 JSON 对象.import java.io.IOException;import com.fasterxml.jackson.annotation.JsonProperty;import com.fasterxml.jackson.databind.ObjectMapper;import okhttp3.*;public class DALLEClient {    public static void main(String[] args) {        String openAIKey = "";        String endpoint = "https://api.openai.com/v1/images/generations";        String contentType = "application/json";        String prompt = "a 35mm macro photo of 3 cute rottweiler puppies with no collars laying down in a field";        int numberOfImages = 2;        String size = "1024x1024";        OkHttpClient client = new OkHttpClient();        MediaType mediaType = MediaType.get(contentType);        // 创建创建图像的 JSON 对象        CreateImage createImage = new CreateImage(prompt, numberOfImages, size);        // 使用 Jackson ObjectMapper 将对象转换为 JSON 字符串        String json = "";        try {            ObjectMapper mapper = new ObjectMapper();            json = mapper.writeValueAsString(createImage);        } catch (Exception e) {            e.printStackTrace();            return;        }        RequestBody body = RequestBody.Companion.create(json, mediaType);        Request request = new Request.Builder()                .url(endpoint)                .method("POST", body)                .addHeader("Content-Type", contentType)                .addHeader("Authorization", "Bearer " + openAIKey)                .build();        try {            Response response = client.newCall(request).execute();            if (!response.isSuccessful()) throw new IOException("Unexpected code " + response);                System.out.println(response.body().string());        } catch (Exception e) {            e.printStackTrace();        }    }    // 创建图像 JSON 对象的内部类    public static class CreateImage {        @JsonProperty("prompt")        private String prompt;        @JsonProperty("n")        private int n;        @JsonProperty("size")        private String size;        public CreateImage(String prompt, int n, String size) {            this.prompt = prompt;            this.n = n;            this.size = size;        }    }}列表 4-10

在 DALLEClient.java 中使用 DALL⋈E API

现在，由于我们已经在使用 OkHttp 库通过 Whisper 模型的转录端点进行 HTTP 请求，我们将继续使用它为 DALL⋈E 模型的创建图像端点。

在这里需要理解的最重要的事情是 CreateImage 内部类。它具有@JsonProperty 注解，并封装了创建图像所需的重要参数：

+   描述图像细节的文本提示

+   你想要生成的图像数量

+   你想要生成的图像大小

图 4-3 和 4-4 显示了从列表 4-9 中的文本提示生成的图像。

![图片](img/chatgpt-for-java-607613_1_En_4_Fig3_HTML.png)

一张由人工智能生成的微笑小女孩和她的狗的照片。在背景中，有植物和花朵。

图 4-3

来自“美国生活”播客第 811 集的 DALL·E 生成的女孩和她的狗的图像

![图片](img/chatgpt-for-java-607613_1_En_4_Fig4_HTML.png)

一张由人工智能生成的微笑女孩的照片，她的左手放在她的狗身上。在背景中，有树木。

图 4-4

来自“美国生活”播客第 811 集的 DALL·E 生成的女孩和她的狗的图像

## DALL·E 提示工程和最佳实践

现在，使用 DALL⋅E 创建图像需要提示工程，以获得一致、理想的结果，尝试不同的提示以获得一些练习，看看哪些对你和你的用例有效。也许你更喜欢画作而不是看起来像 3D 的图像？也许你需要照片而不是数字艺术？也许你想要图像是特写而不是肖像？有很多可能性需要考虑。

无论你的用例如何，以下两条金规则可以帮助你最大限度地发挥 DALL⋅E 提示的作用。

### DALL·E 金规则 #1：熟悉 DALL·E 可以生成的图像类型

首先也是最重要的，DALL⋅E 需要理解的是需要生成的图像类型。以下是一些 DALL⋅E 能够创建的最常见的图像类型列表：

+   3D 渲染

+   画作

+   抽象画

+   表达性的油画

+   油画（任何已故艺术家的风格）

+   油蜡笔

+   数字艺术

+   照片

+   写实照片

+   超现实主义

+   荧光照片

+   35 毫米微距照片

+   高质量照片

+   轮廓

+   虚拟产品

+   卡通

+   毛绒玩具

+   大理石雕塑

+   手绘草图

+   海报

+   铅笔和水彩

+   合成波

+   漫画风格

+   手绘

### DALL·E 金规则 #2：详细描述前景和背景中的内容

我无法强调得更多，你需要用 DALL⋅E 描述图像，以便获得一致、理想的结果。这可能听起来很奇怪，但向 DALL⋅E 描述图像的最佳方式就像向另一个人描述一个梦一样。

所以，作为你和我之间的一次心理练习，试着描述你的最后一个梦。当你描述梦中的人物、地点和事物时，你心中记得最重要的东西，以及你感受到的经历。当你向另一个人描述事物时，一些细节开始浮现，比如

+   有多少人（如果有）在场？

+   人们或动物处于什么位置？站立、坐着还是躺着？

+   场景和背景中有哪些东西？

+   有哪些物品引起了你的注意？声音？气味？颜色？

+   你感觉如何？快乐、诡异、兴奋？

+   你感觉一天中的什么时间？早上、中午还是晚上？

如果你能够向另一个人描述一个梦，那么你应该没有问题描述你想要 DALL⋅E 的内容。

## 结论

在这一章中，我们取得了很大的成就！通过几个类，我们创建了一个播客可视化器。

+   我们创建并使用了 AudioSplitter.java 类，它作为我们的实用工具。如果你有一个大于 Whisper 模型限制的音频文件，这个类将为你提供一个包含较小音频文件的文件夹，以便发送给 Whisper。

+   我们创建并使用了 WhisperClient.java 类来获取一个音频文件夹的转录。该文件夹可以包含单个音频文件或多个文件。你唯一的限制是你可以发送到转录端点和 Whisper 模型的请求数量。

+   我们用 GPT-4 做了一些提示工程，以便根据播客的文本获取对图像的描述性提示。

+   最后，我们创建并使用了 DALLEClient.java 类，从调用 GPT-4 模型获取提示并得到一个代表播客集的视觉图像。

## 留给读者的练习

因此，显然我们在这里还可以做几件额外的事情，这些步骤将留给你们（读者）去完成，例如：

+   AudioSplitter.java 应用是 FFmpeg 的 Java 接口。FFmpeg 不仅可以分割音频文件，还可以对媒体文件做更多的事情，例如格式转换和重新编码。尝试看看 Whisper 支持的哪些媒体格式生成的音频文件最小。提示：绝对不是 WAV 格式。

+   如果你计划创建一个基于你终端用户文本提示自动生成图像的应用或服务，那么你肯定希望更新 DALLEClient.java 类，以确保你在 HTTP 请求中跟踪并提供用户参数。这是因为你的终端用户有可能通过你的 API 密钥生成有害的图像。记住，你有一个 Open AI 的 API 账户，而他们没有！因此，你需要意识到，如果你需要通过你的服务终止与违反 Open AI 内容规则的用户的商业关系。

© 作者（们），独家授权给 APress 媒体公司，Springer Nature 部分版权所有 2024B. HopkinsChatGPT for Java[`doi.org/10.1007/979-8-8688-0116-7_5`](https://doi.org/10.1007/979-8-8688-0116-7_5)

# 5. 使用 Discord 和 Java 创建自动化的社区管理机器人

布鲁斯·霍普金斯^(1  )(1)美国俄勒冈州比佛顿 When you’re launching an app or a service, it’s important to build and maintain your own community. Below are the telltale signs of a healthy user community:

+   会员参与有意义的讨论，分享见解、反馈和支持。

+   会有分歧或辩论发生，但它们是以建设性的方式进行的，不会诉诸人身攻击或侮辱性语言。

+   存在一个尊重的氛围，成员们互相倾听并承认不同的观点。

+   老成员和新成员的混合积极参与，确保社区保持活力，不会停滞不前。

+   用户贡献了多样化的内容，从回答问题到分享资源，这丰富了社区的知识库。

+   在给予和索取之间有一个平衡；寻求帮助或信息的人也会向他人提供帮助。

+   新成员经常加入，通常由现有成员推荐，这表明社区受到积极评价，值得推荐。

+   用户经常成为社区或平台的倡导者，在直接社区空间之外推广它，例如在社交媒体或其他论坛上。

+   社区通过提供新功能和新功能性的想法来帮助塑造应用程序或服务。

无论我创建什么类型的应用程序或服务，我都希望我的用户社区能够体现上述各项内容！

## 选择 Discord 作为您的社区平台

在过去的几年里，Discord 因其作为社区管理的有用工具而迅速流行起来，这对于热衷于自己社区的人来说是一个很好的选择。这部分的功劳要归功于其跨平台兼容性，允许成员无论在桌面、移动设备还是网页浏览器上都能保持连接。然而，它最突出的功能是基于邀请的社区系统，这有助于社区管理者控制增长并防止垃圾邮件。这种模式不仅确保了为成员提供定制体验，还增强了安全性，因为社区管理者有权决定是否授予或拒绝访问。

Discord 不仅支持文本消息，还支持语音聊天和流式视频。与 Slack 非常相似，Discord 允许社区管理者将内容分离到频道中，以组织讨论、简化信息流，并帮助用户看到他们感兴趣的内容。

## 创建比我们的 Slack 机器人更高级的机器人

现在，如果您成功完成了第三章中的步骤，其中我们与 Slack 机器人合作，那么本章的步骤对您来说将感到熟悉。在第三章中，我们创建了一个 Slack 机器人，在一段时间内读取单个频道并总结讨论的内容。这个 Slack 机器人不是一个社区管理者，而更像是一个有用的助手。

在本书的剩余部分，我们将执行所有必要的步骤来创建强大的 Discord 机器人，这些机器人将使用 AI 来帮助实际管理社区。

## 创建比任何典型 Discord 机器人更高级的机器人

如果您曾经使用过 Discord 机器人，那么您可能知道与它们交互的最常见方式是使用所谓的“/命令”。这使典型的机器人（即非智能机器人）仅在接收到非常具体的操作或命令时才能工作。如果没有提供“/命令”，则机器人将保持沉默，不会做任何事情。本质上，它体现了“言多必失”的谚语。

然而，我们正在创建一个具有人工智能的 Discord 机器人，因此它将比任何典型的 Discord 机器人都要先进得多。我们将创建能够阅读和查看 Discord 服务器中所有消息的机器人，并且足够智能，能够正确地做出回应。

### 理解机器人的角色

让我们探索一个场景，以便使事情变得具体。我们正在创建一个公共 Discord 服务器，以与移动银行应用程序的用户互动。我们的最终目标是拥有用 Java 编写的机器人来处理以下场景：

+   Q&A：监控特定频道并自动回答用户关于如何使用银行应用程序的问题。为了实现这一点，机器人需要接受关于应用程序如何工作的训练

+   无推销：对于任何商业社区来说，重要的是社区参与者不会受到不诚实个人的针对。例如，如果您正在创建银行应用程序，您希望您的客户被任何用户名为“B4nk Admin”的人联系吗？

+   无有害内容：对于任何社区来说，保护成员免受有害内容（如仇恨言论）的影响都是非常重要的。

## 我们的示例银行：Crook’s Bank

在本例中，我选择了一个虚构的银行名称，其与真实银行名称重合的可能性极低。因此，在本例中，“Crook’s Bank”将为他们的银行客户推出一款新的移动应用程序。他们希望有一个由机器人监控的渠道来回答应用程序用户的提问，并且他们还希望确保没有人向他们的应用程序用户进行推销，或在他们的 Discord 服务器上发布伤害性或有害的内容。

![图片](img/chatgpt-for-java-607613_1_En_5_Fig1_HTML.png)

一张移动界面的截图显示了假银行应用程序。它写着“欢迎来到 Crooks Bank”，并附有一个抢劫者的插图。

图 5-1

这个来自虚构银行的假应用程序存在真实问题

## 首要任务：创建您的 Discord 服务器

在我们能够创建一个 AI Discord 机器人之前，显然我们需要一个机器人可以与之交互的 Discord 服务器。使用 Discord 应用程序或访问 Discord 网站（当然，首先需要登录），然后开始添加/创建一个新的服务器的过程。

在开始此过程后，选择如图 5-2 所示的标记为“**创建我的**”的选项！[](../images/607613_1_En_5_Chapter/607613_1_En_5_Fig2_HTML.png)

页面截图被创建您的第一个发现服务器弹出框覆盖。它显示了以下选项。创建我的，游戏，学校俱乐部和学习小组。

图 5-2

创建您的 Discord 服务器

接下来，您将被提示提供有关您服务器的其他信息。继续进行创建过程，直到您被提示提供服务器名称和图标，如图 5-3 所示。![图 5-3](img/chatgpt-for-java-607613_1_En_5_Fig3_HTML.png)

页面截图被自定义您的服务器弹出框覆盖。它包含创建服务器名称的字段，创建按钮已被选中。

图 5-3

为您自己的 Discord 服务器提供名称

指定您服务器的名称并提供可选的服务器图标（如果您有的话）。

## 创建问答频道

默认情况下，每个 Discord 服务器都有一个“通用”频道，但我们要创建一个专门用于问答的频道。根据您创建服务器的方式，您将看到如图 5-4 和 5-5 所示的选项来创建您的新频道。![图 5-4](img/chatgpt-for-java-607613_1_En_5_Fig4_HTML.png)

页面截图被 Crooks 银行、开始对话弹出框覆盖。它包含创建主题的字段和完成按钮。

图 5-4

使用 Web 界面创建频道

![图 5-5](img/chatgpt-for-java-607613_1_En_5_Fig5_HTML.png)

创建频道的弹出框截图。在频道类型下选中了文本单选按钮，底部有创建频道按钮。

图 5-5

使用 Discord 应用程序创建频道

## 使用 Discord 注册新的 Discord 机器人应用程序

现在我们已经创建了具有适当频道的 Discord 服务器，是时候注册机器人本身了——或者更确切地说，在我们的情况下，是注册机器人。为了保持代码的整洁和管理，我们实际上将为我们的 Discord 服务器拥有多个机器人。第一个机器人将专门用于“问答”频道中的问答。第二个机器人将监控所有频道，以防止不希望的内容，如有害内容或请求。

为了创建我们的机器人，请访问 Discord 开发者网站：

[**https://discord.com/developers**](https://discord.com/developers)

在页面右上角，单击如图 5-6 所示的“**新建应用程序**”按钮。![图 5-6](img/chatgpt-for-java-607613_1_En_5_Fig6_HTML.png)

开发者门户页面的截图。它显示了应用程序下的详细信息，以及右上角的新应用程序按钮。

图 5-6

要创建 Discord 机器人，请访问 Discord 开发者网站

在 Discord 和 Slack 术语中，一个“机器人”是一个“应用程序”，并且除非它们已在 Discord 上注册，否则机器人不允许在 Discord 服务器上运行。

指定机器人的名称，并单击如图 5-7 所示的“**创建**”按钮。![图 5-7](img/chatgpt-for-java-607613_1_En_5_Fig7_HTML.png)

应用程序页面的截图上叠加了创建和应用弹出框。它显示了创建名称的字段，并选择了创建按钮。

图 5-7

为 Discord 创建/注册机器人

## 指定机器人的通用信息

之后，你将被带到可以指定关于你的机器人的通用信息的页面，如图 5-8 所示。

一定要熟悉页面左侧的导航菜单。如你所见，我们有几个类别设置要为我们的机器人配置。默认情况下，我们已经 landed 在“**通用信息**”页面，在那里我们指定了关于我们机器人的基本信息。如果你为你的机器人准备好了图标，你可以在这里上传它！![图片](img/chatgpt-for-java-607613_1_En_5_Fig8_HTML.png)

开发者页面的截图显示了设置。在显示添加应用图标、名称、描述框、标签和应用 ID 的字段以及保存更改按钮的设置下选择了通用信息。

图 5-8

我决定给我的机器人一个可爱的小机器人图标

## 指定机器人的 OAuth2 参数

现在是时候指定我们机器人的作用域和权限了。如果你遵循了第三章创建 Slack 机器人的步骤，那么（如前所述）这个过程对你来说应该很熟悉。机器人**不能**也不应该拥有做任何事情的权限——它们应该只被允许执行它们被设计来执行的操作列表。

在左侧的设置导航菜单中，导航到“**OAuth2 ➤ URL 生成器**”以继续。

下面是我们想要的作用域：

+   作用域

    +   机器人

这在图 5-9 中体现。![图片](img/chatgpt-for-java-607613_1_En_5_Fig9_HTML.png)

开发者页面的截图显示了设置。在显示 OAuth2 URL 生成器详细信息的设置下选择了 OAuth 2。在作用域下选择了机器人。

图 5-9

选择作用域

在我们选择机器人的作用域后，我们可以看到所有仅适用于机器人的权限。机器人权限分为三类：**通用**、**文本**和**语音**。

如果你对此类别感兴趣，通用权限允许机器人在正常人类管理员的身份下行动，例如管理服务器、角色和频道。具有这些权限的机器人还可以踢出和禁止成员。

文本权限允许机器人在文本频道中发送和接收消息，而语音权限允许机器人在语音频道中参与。很简单，对吧？

选择以下权限供机器人使用：

+   机器人权限

    +   文本权限

        +   发送消息

        +   读取消息历史

适当的权限在图 5-10 中体现。![图片](img/chatgpt-for-java-607613_1_En_5_Fig10_HTML.png)

开发者页面的截图显示了设置。在显示机器人权限的设置下选择了 OAuth 2。在文本权限下选择了发送消息和读取消息历史选项。

图 5-10

选择文本权限

尽管你还没有编写任何 Java 代码，但现在是你邀请你的机器人到你的服务器的时候了。

## 邀请你的机器人到你的服务器

如图 5-10 所示，在你选择了适当的权限后，Discord 将为你提供一个动态生成的 URL，这将使你能够邀请你的机器人到你的服务器。

复制 URL 并将其粘贴到你已经认证到 Discord 的网页浏览器中。结果如图 5-11 所示。![图 5-11](img/chatgpt-for-java-607613_1_En_5_Fig11_HTML.png)

Discord 页面的截图显示了与 Q 和 A Bot 的界面。Discord 显示了“买你一顿美味的海鲜晚餐”的消息，以及添加机器人到服务器和创建命令的消息。

图 5-11

如果你仔细阅读屏幕上的内容，你会看到 Discord 有一种幽默感。

点击“**继续**”按钮，将机器人添加到你的服务器。

接下来，你将看到一个看起来与上一个页面非常相似的页面，但主要区别是它将为你提供机器人的所有权限和功能的摘要。通常，如果你要将机器人添加到你没有创建的服务器，这非常有用。然而，由于我们自己是创建了这个机器人，这只是为了确认我们之前已经指定的设置。

![图 5-12](img/chatgpt-for-java-607613_1_En_5_Fig12_HTML.png)

Discord 页面的截图显示了与 Q 和 A Bot 的界面。在功能下选中了发送消息和读取消息历史复选框。

图 5-12

验证机器人的功能

点击“**授权**”按钮，以授予机器人在你服务器上运行权限。

如果一切顺利，那么你应该在你的服务器的通用频道中看到一个自动消息，表明过程已成功。

## 获取你的机器人的 Discord ID 令牌并设置网关意图

现在是时候获取你的机器人的 Discord ID 令牌了，你将在代码中使用它来程序化地验证你的机器人。

注意

由于显而易见的原因，在这里使用“令牌”这个词让我感到紧张，因为这个词在这个书中由于上下文有两个不同的含义，但这里是一个关于这些含义的快速回顾：

+   当使用 Discord 和 Slack API 时，“令牌”是一个认证令牌。

+   当使用 OpenAI API 时，“令牌”是单词的一部分。

返回 Discord 开发者网站，并点击设置导航菜单中的“**机器人**”类别以继续。

尽管你还没有看到你的令牌，但你需要点击如图 5-13 所示的“重置令牌”按钮。![图 5-13](img/chatgpt-for-java-607613_1_En_5_Fig13_HTML.png)

开发者页面的截图显示了设置。在设置中，机器人被选中，读取 Bot、Build-A-Bot 和授权流程。

图 5-13

点击“重置令牌”按钮以查看您的 ID 令牌

一定要将 ID 令牌复制并保存在安全的地方。你将在本章后面展示的 Java 代码中需要这个令牌。

滚动到页面上的“**特权网关意图**”部分，并启用名为“**消息内容意图**”的选项。

注意

让我们放慢节奏，谈谈意图。究竟什么是“意图”，为什么需要它？对于 Discord API 来说，你需要明确指定你想要通过 Discord 程序通知的每种类型的信息。否则，Discord 会不断地向你发送与你或你的机器人无关的事件。例如，就我们的目的而言，我们不在乎人们何时加入或离开服务器。然而，如果你想要向第一次加入你服务器的任何人发送服务器规则列表，那么你肯定希望启用“**服务器成员意图**”。当我们深入代码时，你会看到更多关于意图的信息。

一定要点击绿色的“**保存更改**”按钮来保存你的更改。结果如图 5-14 所示。![](img/chatgpt-for-java-607613_1_En_5_Fig14_HTML.png)

开发者页面的截图显示了设置。在设置中，机器人被选中，读取存在意图的服务器成员意图，以及在特权网关意图下的消息内容意图。

图 5-14

启用名为“MESSAGE CONTENT INTENT”的选项

## 使用 Java 创建一个问答机器人应用程序以回答频道的提问

当然，现在我们已经完成了所有必要的先决条件，并且知道了我们想要监控以获取用户问题的频道的名称，让我们来看看 Java 代码，该代码将加入我们的服务器并访问特定 Discord 频道的所有消息。

### 设置您的依赖项

Java Discord API（JDA）库为 Java 开发者提供了一个创建与 Discord 服务器协同工作的自动化应用程序的非常直接的方法。我们需要的几乎所有东西都来自 net.dv8tion.jda.api 包，该包存在于 net.dv8tion-<VERSION> jar 文件中。

JDA 库有其自己的依赖项，它们是

+   Java 注解 API（这添加了对基本注解的支持）

    +   javax.annotation-api-<VERSION>.jar

+   Opus Java（一个用于实时音频通信的 Java 库）

    +   opus-java-<VERSION>.jar

+   Neovisionaries WebSocket 客户端（一个用于通过 WebSocket 进行通信的 Java 库）

    +   nv-websocket-client-<VERSION>.jar

+   OK HTTP（我们已经熟悉这个用于 HTTP 通信的库）

    +   okhttp-<VERSION>.jar

+   Apache Commons（Java 开发者非常常用的库）

    +   commons-collections4-<VERSION>.jar

+   SLF4J（我们已经熟悉这个用于日志记录的库）

    +   slf4j-api-<VERSION>.jar

## 创建第一个 Discord 机器人：TechSupportBotDumb.java

这是本章中我们创建的两个 Discord 机器人中的第一个。这个机器人，TechSupportBotDumb.java，将负责监视我们 Discord 服务器中“问答”频道的信息。

在本章的后面部分，我们将创建另一个机器人，该机器人将负责在 Discord 服务器中管理所有内容，包括“问答”频道中的不受欢迎的内容。这里的目的是遵循“关注点分离”的架构模式。而不是创建一个庞大的 Java Discord 机器人，该机器人执行 Discord 服务器所有管理需求，我们将功能分为两个不同的应用程序。

我们也将逐步进行，并将本章的重点放在克服 Java 中 Discord 功能的学习曲线。在本书的最后一章，我们将增强机器人和使用 Open AI API 使其具有人工智能。

列表 5-1 是我们创建一个基本的 Discord 机器人所需的代码，该机器人会监视单个频道中发布的所有消息并提供答案.import java.io.IOException;import java.util.EnumSet;import net.dv8tion.jda.api.JDA;import net.dv8tion.jda.api.JDABuilder;import net.dv8tion.jda.api.entities.Activity;import net.dv8tion.jda.api.entities.User;import net.dv8tion.jda.api.entities.channel.ChannelType;import net.dv8tion.jda.api.events.message.MessageReceivedEvent;import net.dv8tion.jda.api.hooks.ListenerAdapter;import net.dv8tion.jda.api.requests.GatewayIntent;// 这个类扩展了 ListenerAdapter 以处理 Discord 上的消息事件.public class TechSupportBotDumb extends ListenerAdapter {    // 机器人的 Discord 认证令牌。    static String discordToken = "YOUR_DISCORD_BOT_TOKEN";    // 机器人应监视和交互的频道名称。    static String channelToWatch = "q-and-a";    public static void main(String[] args) throws IOException {        // 声明意图集合，指定机器人打算监听哪些类型的事件。        EnumSet<GatewayIntent> intents = EnumSet.of(                GatewayIntent.GUILD_MESSAGES, // 用于公会中的消息。                GatewayIntent.DIRECT_MESSAGES, // 用于私人直接消息。                GatewayIntent.MESSAGE_CONTENT // 允许访问消息内容。        );        // 使用最小配置和指定的意图初始化机器人。        try {            JDA jda = JDABuilder.createLight(discordToken, intents)                    .addEventListeners(new TechSupportBotDumb()) // 将当前类添加为事件监听器。                    .setActivity(Activity.customStatus("Ready to answer questions")) // 设置机器人的自定义状态。                    .build();            // 从 Discord API 异步获取 REST ping 并打印。             jda.getRestPing().queue(ping ->   System.out.println("Logged in with ping: " + ping) );            // 阻塞主线程，直到 JDA 完全加载。            jda.awaitReady();            // 打印机器人连接到的公会数量。            System.out.println("Guilds: " + jda.getGuildCache().size());        } catch (InterruptedException e) {            // 处理在 awaitReady 过程中线程被中断时的异常。            e.printStackTrace();        }    }    // 此方法处理传入的消息。    @Override    public void onMessageReceived(MessageReceivedEvent messageEvent) {        // 发送者的 ID。        User senderDiscordID = messageEvent.getAuthor();        // 忽略机器人发送的消息，以防止自我响应。        if (senderDiscordID.equals(messageEvent.getJDA().getSelfUser())) {            return;        } else if (messageEvent.getChannelType() == ChannelType.TEXT) {            // 忽略不在指定 "q-and-a" 频道中的消息。            if (!messageEvent.getChannel().getName().equalsIgnoreCase(channelToWatch)) {                return;            }        }        // 向发送消息的用户发送问候回复。        String reply = "hi <@" + senderDiscordID.getId() + ">, I can help you with that!";        messageEvent.getChannel().sendMessage(reply).queue();    }}列表 5-1

TechSupportBotDumb.java

在我们的类中，我们需要扩展 JDA API 中的 ListenerAdapter 类，以便使一切正常工作。现在，当你分析 TechSupportBotDumb.java 时，你应该看到我们保持了简单性，因此我们只需要关注两个方法：main() 和 onMessageReceived()()。

在类开始时，你应该也会注意到我们使用“channelToWatch”变量指定了我们感兴趣要监控的频道。

注意

由于某种原因，Discord 自己的术语有时将 Discord 服务器称为“公会”。因此，JDA 库在提到 Discord 服务器时也会使用这个词，然而，从我们的角度来看，公会只是一个 Discord 服务器。

在 main() 方法中，我们有一个集合（具体来说，它是一个 EnumSet，但最终它仍然是一个集合）的 GatewayIntents。你可能记得，你使用 Intents 来明确指定你感兴趣的信息类型。在我们的情况下，我们感兴趣的是

+   发送到服务器的消息（公会消息）

+   用户直接向机器人发送的消息（直接消息）

+   发送消息的内容（消息内容）

之后，我们再次使用 Builder 模式与 JDABuilder 类以及我们的 discordToken 和我们感兴趣的意图，通过以下调用：JDA jda = JDABuilder.createLight(discordToken, intents)

### 爱上 Lambda 表达式以简化代码

在 main() 方法中，我们使用 Lambda 表达式异步地通过 JDA 库向 Discord 服务器发送 ping 请求。像所有网络请求一样，如果不异步执行，则我们的主线程将被阻塞，直到收到响应，这是不好的。因此，在收到 ping 响应后，我们执行 println() 语句以显示 ping 请求到达服务器所需的时间。使用 Java Lambda 表达式，这是通过以下方式实现的：jda.getRestPing().queue(ping -> System.out.println("Logged in with ping: " + ping)); 所以，如果我们没有使用 Lambda 表达式来获取 Discord 服务器的 ping 时间，代码将看起来更像是这样：// 实例化一个新的 PingConsumerjda.getRestPing().queue(new PingConsumer());...// 定义 PingConsumer 为一个内部类 class PingConsumer implements Consumer<Long> {    @Override    public void accept(Long ping) {        System.out.println("Logged in with ping: " + ping);    }}

没有 Lambda，我们需要创建一个实现 Consumer 接口的内部类（老实说，我们并不真正关心这个）。通过实现接口，我们需要实现 accept() 方法，该方法将在响应返回时异步调用。然后，我们会在 jda.getRestPing().queue() 方法调用中创建一个新的 PingConsumer 实例。

### 处理发送到 Discord 服务器的消息

在我们结束这个第一个 Java Discord 机器人的讨论时，我们需要谈谈 onMessageReceived() 方法。这个方法在 Discord 服务器中的每一条消息以及用户直接向机器人发送的私信中都会异步调用。

注意

您知道吗，当机器人在 Discord 服务器中向某人的问题发送答案时，Discord 会调用机器人的 onMessageReceived() 方法，将机器人刚刚发送的消息传递给机器人。这听起来像是一个无限循环的配方，不是吗？因此，我们已经在机器人中设置了逻辑，使其忽略来自自身的消息。

在 onMessageReceived() 方法的最后几行，我们确保通过在回复中“@ 标记”原始信息发送者，向他们提供一个友好的回复。正如我们之前提到的，这个问答机器人的第一个版本是愚蠢的。当您在 Discord 服务器中发布问题时，它会响应，但实际上的回复并不会回答您的问题。

### 成功！运行您的第一个 Discord 机器人：TechSupportBotDumb.java

![图片](img/chatgpt-for-java-607613_1_En_5_Fig15_HTML.png)

开发者页面的截图显示了 Crooks 银行界面。它运行了 Discord 中的问答机器人。

图 5-15

在 Discord 中成功运行问答机器人

现在让我们运行我们的 Java Discord 机器人。在执行应用后，请确保返回到您的 Discord 服务器，并在您为问答设置的频道中尝试输入一个问题。图 5-15 展示了我提出的问题“这个机器人会回答我关于应用的提问吗？”的响应。

当您仔细检查图 5-15 时，您会看到一些关键特性，例如

+   在右侧，您会看到一个绿色的状态指示器，表明机器人正在线。

+   机器人还有一个自定义状态，让您知道它在频道中将做什么。

+   在频道中提出问题后，机器人会直接标记您。

## 使用 Discord 简化我们下一个 Discord 机器人应用的注册过程

现在我们已经成功完成了所有步骤，以获得一个功能齐全的 Discord 机器人，创建第二个机器人将易如反掌！所以，让我们简要回顾一下上述步骤，以便创建我们的第二个 Discord 机器人。我会确保指出需要更改或增强的项目，因为第二个机器人将作为一个审核员工作，而不是为我们的 Discord 服务器用户提供答案。

### 使用 Discord 注册新的 Discord 机器人应用

执行与上述相同的步骤；然而，给机器人起一个不同的名字会是个明智的选择。对我来说，这个第二个机器人将被命名为“内容审核机器人”。

### 为机器人指定通用信息

对于我来说，内容审核机器人有一个不同的图标，所以我在这里指定了它（图 5-16）。![图片](img/chatgpt-for-java-607613_1_En_5_Fig16_HTML.png)

开发者页面截图显示了设置。在设置中选择了“读取字段以添加应用图标、名称、描述和标签”的一般信息，并选择了“保存更改”按钮。

图 5-16

为第二个机器人提供名称和图标

### 为机器人指定 OAuth2 参数

这个第二个机器人需要更多的权限才能执行更多任务。以下是我们想要的范围：

+   Scopes

    +   Bot

为机器人选择以下权限：

+   Bot Permissions

    +   一般权限

        +   踢出成员

        +   禁言成员

    +   文本权限

        +   发送消息

        +   管理消息

        +   读取消息历史

### 邀请您的机器人到您的服务器

为第一个机器人重复上述相同步骤。

### 获取您的机器人的 Discord ID 令牌并设置网关意图

再次，按照上述步骤获取 Discord ID 令牌。然后滚动到页面底部名为“**特权网关意图**”的部分，并启用名为“**SERVER MEMBERS INTENT**”和“**MESSAGE CONTENT INTENT**”的选项。

## 创建下一个 Discord 机器人：ContentModeratorBotDumb.java

内容审核员的角色是确保不希望的内容不会发布在 Discord 服务器上。就像我们在本章前面创建的之前的机器人一样，这个机器人目前（还）不是人工智能。在其当前状态下，机器人将无差别地删除服务器上任何地方发布的包含单词“puppies”的消息。

这并不是因为小狗天生就是邪恶的。然而，当它们被单独留下时，它们确实有破坏你最喜欢的鞋子的倾向。坦白说，我们只是需要一些东西来在我们运行机器人时在 Discord 上测试我们的代码。

列表 5-2 是 `ContentModeratorBotDumb.java` 的代码。`import java.io.IOException; import java.util.EnumSet; import net.dv8tion.jda.api.JDA; import net.dv8tion.jda.api.JDABuilder; import net.dv8tion.jda.api.entities.Activity; import net.dv8tion.jda.api.entities.Message; import net.dv8tion.jda.api.entities.User; import net.dv8tion.jda.api.entities.channel.unions.MessageChannelUnion; import net.dv8tion.jda.api.events.message.MessageReceivedEvent; import net.dv8tion.jda.api.hooks.ListenerAdapter; import net.dv8tion.jda.api.requests.GatewayIntent; // This class extends a ListenerAdapter to handle message events on Discord. public class ContentModeratorBotDumb extends ListenerAdapter { // The bot's Discord token for authentication. static String discordToken = "YOUR_DISCORD_BOT_TOKEN"; static String bannedWord = "puppies"; public static void main(String[] args) throws IOException { // Set of intents declaring which types of events the bot intends to listen to. EnumSet<GatewayIntent> intents = EnumSet.of( GatewayIntent.GUILD_MEMBERS, // to get access to the members of the Discord server GatewayIntent.GUILD_MODERATION, // to ban and unban members GatewayIntent.GUILD_MESSAGES, // For messages in guilds GatewayIntent.MESSAGE_CONTENT // To allow access to message content ); // Initialize the bot with minimal configuration and the specified intents. try { JDA jda = JDABuilder.createLight(discordToken, intents) .addEventListeners(new ContentModeratorBotDumb()) // Adding the current class as an event listener. .setActivity(Activity.customStatus("Helping to keep a friendly Discord server")) // Set the bot's custom status. .build(); // Asynchronously get REST ping from Discord API and print it. jda.getRestPing().queue(ping -> System.out.println("Logged in with ping: " + ping)); // Block the main thread until JDA is fully loaded. jda.awaitReady(); // Print the number of guilds the bot is connected to. System.out.println("Guilds: " + jda.getGuildCache().size()); // Print the Discord userID of the bot System.out.println("Bot's ID: " + jda.getSelfUser()); } catch (InterruptedException e) { // Handle exceptions if the thread is interrupted during the awaitReady process. e.printStackTrace(); } } @Override public void onMessageReceived(MessageReceivedEvent messageEvent){ User senderDiscordID = messageEvent.getAuthor(); MessageChannelUnion channel = messageEvent.getChannel(); Message message = messageEvent.getMessage(); // Check whether the message was sent in a guild / server if (messageEvent.isFromGuild()){ String content = message.getContentDisplay(); // Check if the message contains the banned word if (content.contains(bannedWord)){ // Delete the message message.delete().queue(); // Mention the user who sent the inappropriate message String authorMention = senderDiscordID.getAsMention(); // Send a message mentioning the user and explaining why it was inappropriate channel.sendMessage(authorMention + " This comment was deemed inappropriate for this channel. " + "If you believe this to be in error, please contact one of the human server moderators.").queue(); } } } Listing 5-2

ContentModeratorBotDumb.java

### 处理发送到 Discord 服务器的消息

再次，让我们将注意力集中在 onMessageReceived() 方法上，因为它在每次向 Discord 服务器发布消息时都会异步调用。如您所见，如果发布到服务器的消息包含被禁止的单词，则我们删除该消息，并在发布违规消息的同一条频道中通过 @mention 消息警告发送者。

### 再次成功！运行您的第二个 Discord 机器人：ContentModeratorBotDumb.java

现在让我们运行我们的第二个 Java Discord 机器人。在执行应用程序后，务必返回到您的 Discord 服务器，并在任何包含违规单词的频道中输入一条消息。图 5-17 展示了机器人在行动中的样子！![图 5-17](img/chatgpt-for-java-607613_1_En_5_Fig17_HTML.png)

开发者页面的截图显示了 Crooks 银行界面。在显示欢迎页面的“事件”选项卡下选择了常规选项卡，其中包含来自内容审核机器人到 Java Chat GPT 的聊天。

图 5-17

这个机器人对讨论“小狗”有严格的规则；然而，讨论“小猫”则是完全可行的

## 结论

我们刚刚完成了创建两个功能齐全的 Java Discord 机器人所需的所有步骤。对于那些不熟悉创建 Discord 服务器过程的人来说，我们展示了如何设置服务器以管理我们的社区。

如您所见，我们采取了与第三章中我们创建的 Slack 机器人截然不同的方法！我们创建的 Slack 机器人主要关注工作场所内的用户生产力。而这两个 Discord 机器人则真正专注于社区管理。我们已经为这些机器人配备了所有必要的功能，以便在 OpenAI 的 API 帮助下实现人工智能。所有这些都在最后两个章节中完成。

## 留给读者的练习

在下一章中，我们将使我们的“笨拙”机器人变得智能，但至少我们现在可以做一些事情。与其使用命令行来报告状态消息，不如让机器人拥有自己的专用频道，专门用于状态报告。这样，当机器人启动、关闭或需要通知管理员任何重要信息时，所有记录都会集中记录。

© 作者（们），独家授权给 APress 媒体公司，Springer Nature 部分版权所有 2024B. HopkinsChatGPT for Java[`doi.org/10.1007/979-8-8688-0116-7_6`](https://doi.org/10.1007/979-8-8688-0116-7_6)

# 6. 为我们的 Discord 机器人添加智能，第一部分：使用聊天端点进行问答

布鲁斯·霍普金斯^(1  )(1)比佛顿，俄勒冈州，美国 在这一点上，我们已经拥有了所有必要的结构，使得我们在上一章中创建的两个 Discord 机器人能够完全功能化和具有人工智能。在本书的最后两章中，我们将遵循所有必要的步骤，以便使这两个机器人变得具有人工智能。在本章中，我们将开始构建我们的技术支持机器人，它被称为 TechSupportBotDumb.java。以下是我们要进行的两个主要更改：

+   修改我们的 ChatGPTClient.java 类，以便 Discord 机器人类可以就我们提供给它的特定信息提出问题。更新后的类将被称为 ChatGPTClientForQAandModeration.java。它将在本章用于问答目的，但也会在本书的最后一章中使用。

+   修改我们的 TechSupportBot.java 类（之前命名为 TechSupportBotDumb.java），使其能够加载包含常见问题和答案的外部文本文件。TechSupportBot.java 将随后将文本文件的内容提供给 ChatGPTClientForQAandModeration.java 类，该类负责创建提示并当然调用聊天端点。

## 使 TechSupportBot.java 更智能

列表 6-1 包含了虚构的客户支持团队根据新推出的移动银行应用程序用户的支持票据所创建的常见问题解答的完整内容。1. 什么是对手银行移动应用程序？对手银行移动应用程序是一款前沿的移动银行应用程序，允许您从您的移动设备方便地管理您的财务、进行交易和访问广泛的银行服务。2. 我如何下载对手银行移动应用程序？您可以从苹果设备的 App Store 和安卓设备的 Google Play 下载对手银行移动应用程序。只需搜索“对手银行移动应用程序”并点击“安装”按钮。3. 对手银行移动应用程序安全吗？是的，对手银行移动应用程序优先考虑您的安全。我们使用最先进的加密和安全协议来保护您的数据和交易。您的信息在我们这里是安全的。4. 对手银行移动应用程序提供哪些功能？对手银行移动应用程序提供各种功能，包括：•    账户管理：查看账户余额、交易历史等。•    转账：轻松在您的账户之间或向其他银行账户转账。•    账单支付：支付账单和管理定期支付。•    支票存款：拍摄支票进行远程存款。•    ATM 定位器：查找附近的 ATM 和分行。•    通知：接收账户活动和重要更新的警报。5. 我可以将外部账户链接到对手银行移动应用程序吗？是的，对手银行移动应用程序支持从其他金融机构链接外部账户。您可以在一个地方监控和管理不同银行的账户。6. 如果我忘记密码怎么办？如果您忘记密码，只需在登录屏幕上点击“忘记密码”选项。您将收到有关如何重置密码的说明。7. 与对手银行移动应用程序相关的费用有哪些？对手银行移动应用程序旨在对其费用保持透明。您可以在应用程序内的“费用”部分或我们的网站上找到有关账户费用、交易费用和其他费用的信息。8. 我可以通过对手银行移动应用程序获得客户支持吗？当然可以！我们通过应用程序内的消息功能提供客户支持。您也可以在我们的网站上找到我们的客户服务联系方式。9. 对手银行移动应用程序适用于企业账户吗？对手银行移动应用程序主要针对个人银行需求。然而，我们计划在未来推出企业银行服务。10. 我如何为对手银行移动应用程序提供反馈或建议？我们欢迎您的反馈！您可以通过应用程序内的“联系我们”部分或我们的网站提交建议和反馈。列表 6-1

FAQ.txt

如您在列表 6-1 中的常见问题解答文本文件中所见，这里没有涉及任何魔法。它仅仅是一个问题和答案的列表。现在，让我们看看新修改的 TechSupportBot.java 类。这可以在列表 6-2 中找到。import java.io.BufferedReader;import java.io.FileReader;import java.io.IOException;import java.util.EnumSet;import net.dv8tion.jda.api.JDA;import net.dv8tion.jda.api.JDABuilder;import net.dv8tion.jda.api.entities.Activity;import net.dv8tion.jda.api.entities.User;import net.dv8tion.jda.api.entities.channel.ChannelType;import net.dv8tion.jda.api.entities.channel.unions.MessageChannelUnion;import net.dv8tion.jda.api.events.message.MessageReceivedEvent;import net.dv8tion.jda.api.hooks.ListenerAdapter;import net.dv8tion.jda.api.requests.GatewayIntent;// 这个类扩展了 ListenerAdapter 以处理 Discord 上的消息事件.public class TechSupportBot extends ListenerAdapter {    // 机器人的 Discord 认证令牌。    static String discordToken = "";    // 机器人应该监控和与之交互的频道名称。    static String channelToWatch = "q-and-a";    // 用于存储常见问题解答内容的变量    static String contentsFromFAQ = "";    static String pathToFAQFile = "/Users/Desktop/FAQ.txt";    // 系统消息    static String systemMessage = "您是一个为 Crooks Bank 银行应用程序提供支持的虚拟助手。 "。”;    // 我们用于问答和管理的 ChatGPT 客户端    static ChatGPTClientForQAandModeration chatGPTClient = null;    public static void main(String[] args) throws IOException {        // 声明意图集合，指定机器人打算监听哪些类型的事件。        EnumSet<GatewayIntent> intents = EnumSet.of(                GatewayIntent.GUILD_MESSAGES, // 用于公会中的消息。                GatewayIntent.DIRECT_MESSAGES, // 用于私人直接消息。                GatewayIntent.MESSAGE_CONTENT // 允许访问消息内容。        );        // 将外部文本文件的内容读取到 FAQContents 变量中        contentsFromFAQ = readFileContents(pathToFAQFile);        // 创建一个新的 ChatGPTClientForQAandModeration 实例        chatGPTClient = new ChatGPTClientForQAandModeration(contentsFromFAQ, systemMessage);        // 使用最小配置和指定的意图初始化机器人。        try {            JDA jda = JDABuilder.createLight(discordToken, intents)                    .addEventListeners(new TechSupportBot()) // 将当前类添加为事件监听器。                    .setActivity(Activity.customStatus("Ready to answer questions")) // 设置机器人的自定义状态。                    .build();            // 从 Discord API 异步获取 REST ping 并打印。            jda.getRestPing().queue(ping -> System.out.println("Logged in with ping: " + ping));            // 阻塞主线程，直到 JDA 完全加载。            jda.awaitReady();            // 打印机器人连接到的公会数量。            System.out.println("Guilds: " + jda.getGuildCache().size());            System.out.println("Self user: " + jda.getSelfUser());        } catch (InterruptedException e) {            // 处理在 awaitReady 过程中线程被中断时的异常。            e.printStackTrace();        }    }    // 此方法处理传入的消息。    @Override    public void onMessageReceived(MessageReceivedEvent messageEvent) {        // 发送者的 ID        User senderDiscordID = messageEvent.getAuthor();        // 消息被发布的 Discord 频道        MessageChannelUnion channel = messageEvent.getChannel();        net.dv8tion.jda.api.entities.Message message = messageEvent.getMessage();        String reply = null;        // 忽略机器人发送的消息，以防止自我响应。        if (senderDiscordID.equals(messageEvent.getJDA().getSelfUser())) {            return;        } else if (messageEvent.getChannelType() == ChannelType.TEXT) {            // 忽略不在指定 "q-and-a" 频道中的消息。            if (!channel.getName().equalsIgnoreCase(channelToWatch)) {                return;            }        }        // 在机器人工作时显示 "输入中" 状态        channel.sendTyping().queue();        // 这一行从 Discord 用户那里获取问题并询问 ChatGPT        reply = chatGPTClient.sendMessageFromDiscordUser(message.getContentDisplay());        channel.sendMessage(reply).queue();    }    // 新方法读取文件内容    private static String readFileContents(String filePath) {        try (BufferedReader reader = new BufferedReader(new FileReader(filePath))) {            StringBuilder content = new StringBuilder();            String line;            while ((line = reader.readLine()) != null) {                content.append(line).append("\n");            }            return content.toString();        } catch (IOException e) {            e.printStackTrace();            return "Failed to read FAQ contents.";        }    }}Listing 6-2

TechSupportBot.java

## 需要注意的从技术支持机器人前一个版本的重要变更

让我们简要分析 TechSupportBot.java 并讨论所做的变更。以下代码片段包含类定义部分的一部分。    `static String contentsFromFAQ = "";`    `static String pathToFAQFile = "/Users/Desktop/FAQ.txt";`    `static String systemMessage = "您是一个为 Crooks Bank 银行应用程序提供支持的虚拟助手。";`    `static ChatGPTClientForQAandModeration chatGPTClient = null;`

如您所见，我们定义了一些 String，它们提供了对存储常见问题文件路径位置的引用。我们还有一个 String，将用于包含文件本身的内 容。

现在，正如我们从本书的前几章中学到的，你可以通过在提示中向系统本身提供特定的消息来极大地设定对话的基调。因此，这里也有一个包含系统消息的 String。最后，我们有一个对 Class 的引用，即 ChatGPTClientForQAandModeration，它将非常类似于我们在本书中之前使用的其他 ChatGPTClient 类。

### onMessageReceived()方法的更新

现在，当收到一条消息时，务必注意以下行：`net.dv8tion.jda.api.entities.Message message = messageEvent.getMessage();`

在这里，我们需要给出 JDA 库中使用的 Message 类的完整包名和类名，因为我们已经在发送 HTTP 请求到 Chat Endpoint 时创建并使用了 Message 类来封装和表示 JSON 对象。

现在，让我们进一步检查以下三行代码：        `channel.sendTyping().queue();`        `reply = chatGPTClient.sendMessageFromDiscordUser(message.getContentDisplay());`        `channel.sendMessage(reply).queue();`

在这里，我们提供了一个良好的用户体验，向用户展示机器人正在“打字”，同时用户的提问被发送到 ChatGPT。当响应返回时，我们向用户提供回复。

## 分析 ChatGPTClientForQAandModeration.java

在列表 6-2 中，TechSupportBot.java 实例化了 ChatGPTClientForQAandModeration.java，该类（正如我们之前所述）与我们之前使用的 ChatGPTClient 类非常相似。ChatGPTClientForQAandModeration.java 的完整源代码显示在列表 6-3 中。import com.fasterxml.jackson.core.JsonProcessingException;import com.fasterxml.jackson.databind.JsonNode;import com.fasterxml.jackson.databind.ObjectMapper;import java.io.BufferedReader;import java.io.IOException;import java.io.InputStreamReader;import java.io.OutputStream;import java.net.HttpURLConnection;import java.net.URL;import java.util.ArrayList;import java.util.List;public class ChatGPTClientForQAandModeration {    //    //  OpenAI 参数，我们已知如何使用    //    String openAIKey = "";    String endpoint = "https://api.openai.com/v1/chat/completions";    String model = "gpt-4";    float temperature = 1.0f;    int max_tokens = 256;    float top_p = 1.0f;    int frequency_penalty = 0;    int presence_penalty = 0;    String systemMessage = null;    String initialInstructionsToChatGPT = null;    //    // 构造函数需要传递来自 FAQ.txt 文件的内容以及系统消息    //    public ChatGPTClientForQAandModeration(String systemMessage, String initialInstructionsToChatGPT) {        this.systemMessage = systemMessage;        this.initialInstructionsToChatGPT = initialInstructionsToChatGPT;    }    public String sendMessageFromDiscordUser(String discordMessageText) {        String answerFromChatGPT = "";        List<Message> messages = new ArrayList<>();        messages.add(new Message("system", systemMessage));        messages.add(new Message("user", initialInstructionsToChatGPT));        messages.add(new Message("user", discordMessageText));        String jsonInput = null;        try {            ObjectMapper mapper = new ObjectMapper();            Chat chat = Chat.builder()                .model(model)                .messages(messages)                .temperature(temperature)                .maxTokens(max_tokens)                .topP(top_p)                .frequencyPenalty(frequency_penalty)                .presencePenalty(presence_penalty)                .build();            jsonInput = mapper.writeValueAsString(chat);            System.out.println(jsonInput);        } catch (JsonProcessingException e) {            e.printStackTrace();        }        try {            URL url = new URL(endpoint);            HttpURLConnection connection = (HttpURLConnection) url.openConnection();            connection.setRequestMethod("POST");            connection.setRequestProperty("Content-Type", "application/json");            connection.setRequestProperty("Authorization", "Bearer " + openAIKey);            connection.setDoOutput(true);            OutputStream outputStream = connection.getOutputStream();            outputStream.write(jsonInput.getBytes());            outputStream.flush();            outputStream.close();            int responseCode = connection.getResponseCode();            if (responseCode == HttpURLConnection.HTTP_OK) {                BufferedReader reader = new BufferedReader(new InputStreamReader(connection.getInputStream()));                StringBuilder response = new StringBuilder();                String line;                while ((line = reader.readLine()) != null) {                    response.append(line);                }                reader.close();                // 打印响应                answerFromChatGPT = extractAnswerFromJSON(response.toString());                System.out.println(answerFromChatGPT);            } else {                System.out.println("Error: " + responseCode);            }            connection.disconnect();        } catch (IOException e) {            e.printStackTrace();        }        return answerFromChatGPT;    }    //    // 我们只对 JSON 响应中的 "message.content" 感兴趣    // 所以这里有一个简单的方法来提取它    //    public String extractAnswerFromJSON(String jsonResponse) {        String chatGPTAnswer = "";         try {            // 创建 ObjectMapper 实例            ObjectMapper objectMapper = new ObjectMapper();            // 解析 JSON 字符串            JsonNode rootNode = objectMapper.readTree(jsonResponse);            // 提取 "content" 参数            JsonNode contentNode = rootNode.at("/choices/0/message/content");            chatGPTAnswer = contentNode.asText();            System.out.println("Content: " + chatGPTAnswer);        } catch (Exception e) {            e.printStackTrace();        }        return chatGPTAnswer;    }}Listing 6-3

ChatGPTClientForQAandModeration.java 需要注意的一个重要事项是，在构造函数中，我们发送了常见问题内容的完整字符串以及我们将提供给系统的消息本身.public ChatGPTClientForQAandModeration(String knowledgeBaseFileContents, String systemMessage) {        this.knowledgeBaseFileContents = knowledgeBaseFileContents;        this.systemMessage = systemMessage;    }

这样，在我们构建了 ChatGPTClientForQAandModeration.java 类之后，我们可以重用已经构建的对象来回答用户的单个问题。

每当在我们的 Discord 频道中发布一个问题，TechSupportBot.java 将会从 ChatGPTClientForQAandModeration.java 调用 sendMessageFromDiscordUser() 方法。在这个方法中，我们将执行所有必要的常规操作，以调用 Chat 端点。

### 使用 JSONPath 快速从 JSON 文件中提取内容

有时，为了从 JSON 文件中提取单个节点，编写必要的代码可能会有些混乱。因此，我编写了一个简单的方法，使用 JSONPath 来提取由 Chat 端点返回的 JSON 文件中的“message.content”节点。所有操作都通过这一行代码完成：JsonNode contentNode = rootNode.at("/choices/0/message/content");

在我看来，JSONPath 在从 JSON 文件中提取单个节点或节点组方面非常高效，但表达式本身以及必要的语法可能和正则表达式一样难以阅读。所以，如果你之前从未使用过 JSONPath，或者需要帮助编写表达式，那么和 ChatGPT 进行结对编程吧！

### 运行我们的智能问答机器人：TechSupportBot.java

现在，让我们运行我们新改进的问答 Java Discord 机器人，TechSupportBot.java。在执行应用程序后，请确保返回到您的 Discord 服务器，并开始提问。图 6-1 展示了机器人的运行情况.![](img/chatgpt-for-java-607613_1_En_6_Fig1_HTML.png)

一张 Discord 页面截图，其中问答频道已打开。Java Chat G P T 和问答机器人的消息在对话中给出。

图 6-1

与我们的智能 DISCORD 问答机器人 TechSupportBot.java 列表 6-4 展示了我们与 Discord 机器人的对话。**我**：嗨，我是这个频道的新人。我能问些什么问题？**问答机器人**：你好！欢迎来到我们的支持频道。在这里，你可以问我们任何与 Crooks 银行移动应用相关的问题，例如：1. 如何安装和设置应用。2. 如何在应用中浏览不同的功能，如进行交易、账单支付、支票存款等。3. 与应用的安全性和安全性相关的问题。4. 如果你在使用我们的应用时遇到任何问题，我们可以提供帮助。5. 与应用相关的任何费用问题。不要犹豫，问我们任何与我们的服务相关的问题！我们在这里帮助你。**我**：我有一部旧的黑莓手机，这个应用支持我的设备吗？**问答机器人**：很抱歉给您带来不便，但目前 Crooks 银行移动应用仅适用于 iOS 和 Android 设备。它不支持黑莓或其他操作系统。您可以通过手机浏览器访问我们的网站来管理您的银行账户。**我**：那么，如果我使用 iPhone，我该如何设置这个应用？**问答机器人**：当然，以下是您如何在 iPhone 上设置 Crooks 银行移动应用的步骤：1. 打开 iPhone 上的 App Store。2. 在顶部的搜索栏中，输入“Crooks 银行移动应用”并点击“搜索”。3. 一旦您在搜索结果中看到应用，只需点击“获取”按钮下载即可。4. 应用下载完成后，点击“打开”。5. 在首次启动时，您需要同意我们的条款和条件。6. 如果您是 Crooks 银行的现有成员，可以使用您的在线银行用户 ID 和密码登录。如果您是新成员，则需要注册一个账户。7. 登录后，您可以为将来更快、更安全地登录设置 Touch ID 或 Face ID。8. 现在，您可以使用 Crooks 银行移动应用来管理您的财务、支付账单、进行交易等！请确保您定期更新应用以访问新功能和改进。如果在设置过程中遇到任何挑战，请通过应用的支持功能联系我们或拨打我们的客户服务电话。列表 6-4

我们与智能问答 Discord 机器人的第一次对话

## 我们取得的巨大成就……但有一点小瑕疵

好的，如果你退后一步审视我们迄今为止所取得的成就，你应该意识到我们所面对的简直是一项无与伦比的成就。我们有以下这些：

+   由几个类组成的系统，允许用户输入问题，并获取有关如何使用我们移动应用的问题和答案。

+   使用一个简单的文本文件，我们可以教会我们的机器人如何回答用户的问题。这可以由公司中的任何人编辑，并可以用作知识库，以帮助机器人每天提高智能。这是了不起的事情。

+   系统允许客户使用自然语言输入问题，机器人会为他们提供智能回答。猜猜看？客户不喜欢阅读常见问题解答——尤其是特别长的那些。然而，使用这个系统，他们不需要这么做！他们只需提出与他们相关的问题即可。

所以，尽管我们已经取得了所有这些成就，但我们不能忽视一个巨大的缺陷。在列表 6-4 中，机器人对用户说：“一旦您登录，您可以为未来的快速、安全登录设置 Touch ID 或 Face ID。”不，不，不！坏机器人！如果您没有完全阅读常见问题解答文件，请允许我解释这里出了什么问题：

1.  1.

    列表 6-1 中的 FAQ.txt 文件明确指出 Crooks Bank 移动应用是一个移动应用。目前，Touch ID 只能在苹果的桌面和笔记本电脑上使用。所以这甚至都不合理。

1.  2.

    FAQ.txt 文件完全没有提到移动应用的身份验证中使用的 Face ID。

所以，不幸的是，ChatGPT 在编造一些根本不真实的事情，并假设某些功能存在，而实际上并不存在。因此，为了真正的技术支持，这是绝对不可接受的。

那么，我们该如何解决这个问题？在阅读下一节之前，先思考一下你如何解决这个问题。

## 更新系统消息到 ChatGPT 并再次尝试

你已经想出解决方案了吗？解决这个问题的方法之一是更新系统消息。参考以下列表 6-2 中的这一行：`static String systemMessage = "You are a virtual assistant that provides support for the Crooks Bank banking app. ";` 记住，系统消息会向 ChatGPT 指示其在聊天对话中的角色。目前它被指示成为一个有用的助手，因此它已经自行推测某些功能存在于移动应用程序中。现在，让我们确保 ChatGPT 不会做出任何假设。将系统消息更新如下：`static String systemMessage = "You are a virtual assistant that provides support for the Crooks Bank banking app. You will be provided Information about the application, and users will ask you questions about the application. Your role is to answer questions explicitly from the training information. If you were not given an answer to a question, then provide an apologetic message to the user explaining that you do not know the answer.";` 这样就完成了。`FAQ.txt` 文件保持与之前完全相同，我们所需做的只是更新系统消息，让 ChatGPT 知道它在对话中的角色。列表 6-5 展示了我们与 Discord 机器人的新对话。**我**：你今天怎么样？**问答机器人**：作为一个虚拟助手，我没有感情或情绪，但我在这里，准备好帮助你。今天我能如何帮助你在 Crooks Bank 移动应用程序上？**我**：我有一部旧的黑莓手机，这个应用程序在我的设备上支持吗？**问答机器人**：很抱歉，但根据提供的信息，Crooks Bank 移动应用程序只能从 App Store 下载用于 iOS 设备，从 Google Play 下载用于 Android 设备。没有提到黑莓设备，因此我无法确认它是否兼容。**我**：那么，如果我使用 iPhone，我该如何设置应用程序？**问答机器人**：要在你的 iPhone 上设置 Crooks Bank 移动应用程序，你可以从 App Store 下载。只需搜索“Crooks Bank 移动应用程序”并点击“安装”按钮。安装完成后，打开应用程序，按照提示设置您的账户。如果您已经有了账户，请使用您的登录信息通过应用程序访问您的账户。列表 6-5

我们与智能问答 Discord 机器人的第二次更深入的对话

现在好多了！我们的技术支持机器人“坚持脚本”并且不允许编造或假设任何内容。

## 结论

在本章中，我们取得了很大的成就！我们有一个完全功能齐全的 Discord 机器人，任何人都可以通过一个简单的文本文件来训练，而不需要任何 AI、NLP 或机器学习的经验。我们了解到，“有用的助手”有时可能会变得过于有用，并假设一些不真实的事实。然而，我们也重申了系统消息的概念和价值，它是提示工程的重要组成部分。

既然我们已经使我们的问答 Discord 机器人变得智能，那么现在让我们来看看如何使内容审查机器人也变得智能！

© 作者保留，独家授权给 APress 媒体公司，Springer Nature 集团，2024B. HopkinsChatGPT for Java[`doi.org/10.1007/979-8-8688-0116-7_7`](https://doi.org/10.1007/979-8-8688-0116-7_7)

# 7. 为我们的 Discord 机器人添加智能，第二部分：使用 Chat 和 Moderation 端点进行审查

布鲁斯·霍普金斯^(1  )(1)美国俄勒冈州比佛顿 In this chapter, we’re going to take the steps necessary in order to make our Content Moderator Discord bot artificially intelligent. Let’s overview the changes that we’re going to make:

+   创建一个新的类，ModerationClient.java，用于调用 Moderations 端点。Moderations 端点使我们能够知道任何文本内容是否属于以下任何一类：

    +   厌恶

    +   厌恶/威胁

    +   市扰

    +   市扰/威胁

    +   自伤

    +   自伤/意图

    +   自伤/指导

    +   性相关

    +   性相关/未成年人

    +   暴力

    +   暴力/血腥

+   从上一章复用 ChatGPTClientForQAandModeration.java。在第六章，它被用来从我们的用户那里调用 Chat 端点以进行问答。在这一章中，它将被用来再次调用 Chat 端点，但这次是为了进行审查。这就是为什么这个类名字恰当的原因。“ChatGPTClientForQAandModeration”，因为它在第六章用于问答，但在这个章节也用于审查。

+   修改我们的 ContentModeratorBot.java 类（之前命名为 ContentModeratorBotDumb.java），使其能够调用 ModerationClient.java 和 ChatGPTClientForQAandModeration.java。如果任一类指示 Discord 通道中输入的内容令人反感，则从该 Discord 通道中删除该消息。记住，这个机器人监视 Discord 服务器中所有通道的所有内容！

注意

现在，在这个时候，你可能自己会问，如果 Moderations 端点已经知道如何标记任何有害内容，那么为什么我们还需要使用 Chat 端点呢？这是个好问题。

是的，Moderations 端点将使我们了解有害内容，但它 **不会** 通知我们关于我们场景中其他类型不受欢迎的内容，例如当不诚实的人试图诱骗我们的用户参与诈骗时。记住，这是一个银行应用的 Discord 服务器，因此骗子肯定会喜欢针对这个 Discord 服务器中的所有成员，因为这个服务器是一个充满银行用户的中心位置！

因此，我们将使用 ModerationClient.java 调用 Moderations 端点，以了解 Discord 服务器中的任何内容是否有害，并且我们将复用上一章中的 ChatGPTClientForQAandModeration.java，以便调用 Chat 端点，以便了解 Discord 服务器中发布的任何其他不受欢迎的内容，例如诈骗尝试。

## Moderations 端点

调解端点允许开发者提交一段文本，并随后了解该文本是否具有暴力、仇恨、威胁或包含任何形式的骚扰。

### 创建请求

表 7-1 列出了调用调解端点所需的全部 HTTP 参数。表 7-1

调解端点的 HTTP 参数

| HTTP Param | 描述 |
| --- | --- |
| 端点 URL | [`api.openai.com/v1/moderations`](https://api.openai.com/v1/moderations) |
| 方法 | POST |
| Header | Authorization: Bearer **$OPENAI_API_KEY** |
| Content-Type | application/json |

表 7-2 描述了用于调解端点请求体的 JSON 对象的格式。服务非常简单易用，因为只需要一个参数就可以正确调用服务。

### 创建调解（JSON）

表 7-2

调解端点的请求体

| 字段 | 类型 | 必需？ | 描述 |
| --- | --- | --- | --- |
| Input | String or Array | 必需 | 需要分类的文本。 |
| Model | Stringdefault: “text-moderation-latest” | 可选 | 实际上，有两种内容调解模型可供使用：“text-moderation-stable”和“text-moderation-latest”。默认设置为“text-moderation-latest”。它将随着时间的推移自动升级，这确保您始终使用最准确的模式。如果您使用“text-moderation-stable”，在模型更新之前您将收到提前通知。“text-moderation-stable”的准确性通常略低于“text-moderation-latest”。 |

### 处理 JSON 响应

在成功调用调解端点后，服务将提供一个具有如表 7-3 所示结构的 JSON 响应。

### 调解（JSON）

表 7-3

调解 JSON 对象的结构

| 字段 | 类型 | 描述 |
| --- | --- | --- |
| Id | String | 调解请求的唯一标识符。 |
| Model | String | 执行调解请求所使用的模型。 |
| Results | Array | 调解对象的列表。 |
| ↳ flagged | Boolean | 标记内容是否违反了 OpenAI 的使用政策。 |
| ↳ categories | Array | 一组分类及其是否被标记的状态。 |
| ↳↳ hate | Boolean | 这表示给定的文本是否表达、煽动或推广基于种族、性别、宗教、民族、国籍、残疾状态、性取向或种姓的仇恨。 |
| ↳↳ hate/threatening | Boolean | 这表示给定的文本是否包含基于上述偏见表达的有害内容，并威胁对目标群体造成暴力或严重伤害。 |
| ↳↳ harassment | Boolean | 这表示给定的文本是否包含表达、煽动或推广针对任何目标的骚扰性语言的内容。 |
| ↳↳ 嫌疑/威胁 | 布尔值 | 这表示给定的文本是否包含包含骚扰内容且威胁对任何目标实施暴力或严重伤害的内容。 |
| ↳↳ 自伤 | 布尔值 | 这表示给定的文本是否包含提倡、鼓励或描绘自伤行为的内容，例如自杀、割伤和饮食失调。 |
| ↳↳ 自伤/意图 | 布尔值 | 这表示给定的文本是否包含说话者表达他们正在或打算进行自伤行为的内容，例如自杀、割伤和饮食失调。 |
| ↳↳ 自伤/指示 | 布尔值 | 这表示给定的文本是否包含鼓励执行自伤行为的内容，例如自杀、割伤和饮食失调。这包括提供如何执行此类行为的指示或建议的内容。 |
| ↳↳ 性 | 布尔值 | 这表示给定的文本是否包含旨在唤起性兴奋的内容，例如性活动的描述。这包括推广性服务的内容；然而，这***不包括***性教育和健康等话题。 |
| ↳↳ 性/未成年人 | 布尔值 | 这表示给定的文本是否包含包含 18 岁以下个人的内容。 |
| ↳↳ 暴力 | 布尔值 | 这表示给定的文本是否包含描绘死亡、暴力或身体伤害的内容。 |
| ↳↳ 暴力/图形 | 布尔值 | 这表示给定的文本是否包含详细描绘死亡、暴力或身体伤害的内容。 |
| ↳ category_scores | 数组 | 模型给出的类别及其得分的列表。 |
| ↳↳ 仇恨 | 数量 | “仇恨”类别的得分。 |
| ↳↳ 仇恨/威胁 | 数量 | “仇恨/威胁”类别的得分。 |
| ↳↳ 嫌疑 | 数量 | “嫌疑”类别的得分。 |
| ↳↳ 嫌疑/威胁 | 数量 | “嫌疑/威胁”类别的得分。 |
| ↳↳ 自伤 | 数量 | “自伤”类别的得分。 |
| ↳↳ 自伤/意图 | 数量 | “自伤/意图”类别的得分。 |
| ↳↳ 自伤/指示 | 数量 | “自伤/指示”类别的得分。 |
| ↳↳ 性 | 数量 | “性”类别的得分。 |
| ↳↳ 暴力 | 数量 | “暴力”类别的得分。 |
| ↳↳ 暴力/图形 | 数量 | “暴力/图形”类别的得分。 |

列表 7-1 是调用审查端点后的 JSON 响应示例。表 7-3 看起来有些复杂，但正如你所见，如果任何类别被标记为“true”，则**results.flagged**节点也被标记为“true”。

请查看列表 7-1 以了解 Moderation JSON 对象的实际示例！![开放人工智能的标志](img/chatgpt-for-java-607613_1_En_7_Figa_HTML.gif)A logo of open A I.{  "id": "modr-XXXXX",  "model": "text-moderation-005",  "results": [        {        "flagged": true,        "categories": {        "sexual": false,        "hate": false,        "harassment": false,        "self-harm": false,        "sexual/minors": false,        "hate/threatening": false,        "violence/graphic": false,        "self-harm/intent": false,        "self-harm/instructions": false,        "harassment/threatening": true,        "violence": true,        },        "category_scores": {        "sexual": 1.2282071e-06,        "hate": 0.010696256,        "harassment": 0.29842457,        "self-harm": 1.5236925e-08,        "sexual/minors": 5.7246268e-08,        "hate/threatening": 0.0060676364,        "violence/graphic": 4.435014e-06,        "self-harm/intent": 8.098441e-10,        "self-harm/instructions": 2.8498655e-11,        "harassment/threatening": 0.63055265,        "violence": 0.99011886,        }        }  ]}列表 7-1

Moderation JSON 对象

## 为 Moderations 端点创建我们的客户端：ModerationClient.java

列表 7-2 是我们客户端调用 Moderations 端点的方法。请查看它，然后我们将在之后讨论其重要部分。

ModerationClient.java

由于在这本书的前几章中，我们为 OpenAI API 的其他端点创建了客户端，上面的类应该看起来相当熟悉。然而，在类的末尾，我们有一个名为 `ModerationResponse` 的内部类。    `class ModerationResponse {        boolean isFlagged = false;        ArrayList<String> offendingCategories = new ArrayList<>();

这个类封装了从 Moderations 端点返回的 Moderation JSON 对象中的宝贵信息。具体来说，如果我们想要评估的原始 Discord 消息违反了内容规则，我们有一个布尔值 `isFlagged` 来通知我们。如果 `isFlagged` 为真，则 `offendingCategories` 将填充内容被标记为违规的类别。

因此，`getModerationResponsefromJSON()` 方法确实如其名称所描述的那样工作。我们传递由 Moderations 端点返回的 Moderation JSON 对象，然后我们得到一个完全实例化的 ModerationResponse 对象。

## 使 `ContentModeratorBot.java` 更智能

既然我们现在有了 `ModerationClient.java` 来调用 Moderations 端点，让我们看看更新后的 `ContentModeratorBot.java`（之前命名为 `ContentModeratorBotDumb.java`），它将使用 `ModerationClient.java` 来检查有害内容，以及 `ChatGPTClientForQAandModeration.java`（与上一章未修改）来检查潜在的诈骗。

列表 7-3 是我们智能 Discord 管理员机器人 ContentModeratorBot.java 的完整源代码。import java.io.IOException;import java.util.EnumSet;import net.dv8tion.jda.api.JDA;import net.dv8tion.jda.api.JDABuilder;import net.dv8tion.jda.api.entities.Activity;import net.dv8tion.jda.api.entities.User;import net.dv8tion.jda.api.entities.channel.unions.MessageChannelUnion;import net.dv8tion.jda.api.events.message.MessageReceivedEvent;import net.dv8tion.jda.api.hooks.ListenerAdapter;import net.dv8tion.jda.api.requests.GatewayIntent;// 这个类扩展了 ListenerAdapter 以处理 Discord 上的消息事件.public class ContentModeratorBot extends ListenerAdapter {    // 机器人的 Discord 认证令牌。    static String discordToken = "";    // 系统消息    // 这是一个 Java 13+ 多行字符串注释。最终，它仍然是一个字符串    static String systemMessage = """        您是 Discord 服务器自动化的管理员助手。        请审查以下消息是否存在以下违规规则：        1. 敏感信息        2. 侮辱        3. 不恰当的评论        4. 邮件垃圾，例如；全大写的消息，重复相同的短语或单词，超过 3 个感叹号或问号。        5. 广告        6. 外部链接        7. 政治信息或辩论        8. 宗教信息或辩论        如果检测到任何这些违规行为，请回复 "FLAG"（不带引号的大写）。如果消息符合规则，请回复 "SAFE"（不带引号的大写）。        """;    static String instructionsToChatGPT = "分析以下消息是否存在违规规则：";    // 这是我们的 Chat Endpoint 客户端    static ChatGPTClientForQAandModeration chatGPTClient = null;    // 这是我们的 Moderations Endpoint 客户端    static ModerationClient moderationClient = null;    public static void main(String[] args) throws IOException {        // 声明意图集合，指定机器人希望监听哪些类型的事件。        EnumSet<GatewayIntent> intents = EnumSet.of(                GatewayIntent.GUILD_MEMBERS,   // 获取 Discord 服务器成员的访问权限                GatewayIntent.GUILD_MODERATION, // 禁止和解除成员的权限                GatewayIntent.GUILD_MESSAGES, // 服务器中的消息                GatewayIntent.MESSAGE_CONTENT // 允许访问消息内容        );        // 创建一个新的 ChatGPTClientForQAandModeration        chatGPTClient = new ChatGPTClientForQAandModeration(systemMessage, instructionsToChatGPT);        // 创建一个新的 ModerationClient        moderationClient = new ModerationClient();        // 使用最小配置和指定的意图初始化机器人。        try {            JDA jda = JDABuilder.createLight(discordToken, intents)                    .addEventListeners(new ContentModeratorBot()) // 将当前类添加为事件监听器。                    .setActivity(Activity.customStatus("帮助保持友好的 Discord 服务器")) // 设置机器人的自定义状态。                    .build();            // 从 Discord API 异步获取 REST ping 并打印。            jda.getRestPing().queue(ping -> System.out.println("已登录，ping: " + ping));            // 阻塞主线程，直到 JDA 完全加载。            jda.awaitReady();            // 打印机器人连接到的服务器数量。            System.out.println("服务器数量: " + jda.getGuildCache().size());            // 打印机器人的 Discord 用户 ID            System.out.println("机器人的 ID: " + jda.getSelfUser());        } catch (InterruptedException e) {            // 处理在 awaitReady 过程中线程被中断的异常。            e.printStackTrace();        }    }    @Override    public void onMessageReceived(MessageReceivedEvent messageEvent){        String chatGPTResponse = "";        ModerationClient.ModerationResponse moderationResponse = null;        User senderDiscordID = messageEvent.getAuthor();        // 消息被发布的 Discord 频道        MessageChannelUnion channel = messageEvent.getChannel();        net.dv8tion.jda.api.entities.Message message = messageEvent.getMessage();        // 忽略机器人发送的消息，以防止自我响应。        if (senderDiscordID.equals(messageEvent.getJDA().getSelfUser())) {            return;        }        // 这行代码从 Discord 用户那里获取消息并调用 Moderation Endpoint        moderationResponse = moderationClient.checkForObjectionableContent(message.getContentDisplay());        // 这行代码从 Discord 用户那里获取消息并调用 Chat Endpoint        chatGPTResponse = chatGPTClient.sendMessageFromDiscordUser(message.getContentDisplay());        // 检查消息是否在公会/服务器中发送        if (messageEvent.isFromGuild()){            // 检查 Chat Endpoint 和 Moderations Endpoint 是否标记了消息        if (chatGPTResponse.equals("FLAG") || moderationResponse.isFlagged ){                // 删除消息                message.delete().queue();                // 提及发送不适当消息的用户                String authorMention = senderDiscordID.getAsMention();                // 发送提及用户的消息并解释为什么它不适当                channel.sendMessage(authorMention + " 这条评论被认为不适合此频道。 " +                        "如果您认为这是错误的，请联系服务器的人类管理员。").queue();            }        }    }}Listing 7-3

ContentModeratorBot.java

## 需要注意的 Content Moderator Bot 前一个版本的重要更改

让我们简要地看一下 Listing 7-3 中的 ContentModeratorBot.java，并讨论所做的更改。以下代码片段包含类定义部分的一部分.static String systemMessage = """        You are the automated moderator assistant for a Discord server.        Review each message for the following rule violations:        1\. Sensitive information        2\. Abuse        3\. Inappropriate comments        4\. Spam, for example; a message in all capital letters, the same phrase or word being repeated over and over, more than 3 exclamation marks or question marks.        5\. Advertisement        6\. External links        7\. Political messages or debate        8\. Religious messages or debate        If any of these violations are detected, respond with "FLAG" (in uppercase without quotation marks). If the message adheres to the rules, respond with "SAFE" (in uppercase without quotation marks).        """;    static String instructionsToChatGPT = "Analyze the following message for rule violations:";    // 这是我们的聊天端点客户端    static ChatGPTClientForQAandModeration chatGPTClient = null;    // 这是我们的审核端点客户端    static ModerationClient moderationClient = null;

如果你使用的是 Java 13+，则可以使用“三引号”记法定义整个文本块。这是我们定义将被 ChatGPTClientForQAandModeration 类使用的系统消息的方式。

### onMessageReceived()方法的更新

在 Discord 服务器的任何通道接收到消息后，会调用 onMessageReceived()方法。以下是需要特别注意的重要更改：        moderationResponse = moderationClient.checkForObjectionalContent(message.getContentDisplay());        chatGPTResponse = chatGPTClient.sendMessageFromDiscordUser(message.getContentDisplay());        // 检查消息是否在公会/服务器中发送        if (messageEvent.isFromGuild()){            // 检查聊天端点和审核端点以查看消息是否被标记            if (chatGPTResponse.equals("FLAG") || moderationResponse.isFlagged ){                // 删除消息                message.delete().queue();                // 提及发送不适当消息的用户                String authorMention = senderDiscordID.getAsMention();                // 发送提及用户并解释为什么该消息不适当                channel.sendMessage(authorMention + " This comment was deemed inappropriate for this channel. " +                        "If you believe this to be in error, please contact one of the human server moderators.").queue();            }

在这里，我们检查 Discord 服务器中发布的每条消息，并与审核端点和聊天端点进行核对。如果任一端点返回通知我们消息被标记，那么我们将删除该通道中的消息，并通知用户他们的消息违反了规则。

现在既然我们的内容审核员 Discord 机器人变得智能了，让我们试试看吧！

## 运行我们的智能内容审核员机器人：ContentModeratorBot.java

现在让我们运行我们新的改进版内容审核员 Java Discord 机器人，ContentModeratorBot.java。在执行应用程序后，请确保返回到您的 Discord 服务器，并开始提问。图 7-1 显示了机器人的运行情况！![图 7-1](img/chatgpt-for-java-607613_1_En_7_Fig1_HTML.png)

Crooks Bank 页面的截图。来自 JavaChatGPT 的文本消息显示：嗨，大家好，我喜欢 Crooks Bank 应用！这个应用太棒了，有一个爱心表情符号。

图 7-1

与我们的智能 DISCORD 内容审核员机器人进行讨论：ContentModeratorBot.java

列表 7-4 显示了我们与 Discord 机器人之间的对话，以测试它能做什么。**我**：嗨，大家好，我喜欢 Crooks Bank 应用！**我**：这个应用太棒了！![表情符号](img/chatgpt-for-java-607613_1_En_7_Figb_HTML.gif)一个爱心表情符号。**我**：来我的网站！http://www.google.com**内容审核机器人**：@JavaChatGPT 这个评论被认为不适合这个频道。如果您认为这是错误的，请联系服务器的人类审核员。**我**：对不起，我违反了规则。我现在是另一个人了**我**：但我有一些坏消息要告诉你**我**：我想![表情符号](img/chatgpt-for-java-607613_1_En_7_Figc_HTML.gif)一个危险的表情符号。它包括一个骷髅和交叉骨。大家**内容审核机器人**：@JavaChatGPT 这个评论被认为不适合这个频道。如果您认为这是错误的，请联系服务器的人类审核员。列表 7-4

我们与智能内容审核员 Discord 机器人的攻击性对话

在这两种情况下，当任何 Discord 服务器的通道中发布不适当的内容时，不仅会指出违规用户，还会删除不良信息。好机器人！

你注意到审核和聊天端点也能读取表情符号了吗？

## 结论

在本章中，我们为整个 Discord 服务器创建了一个完全功能化的内容审核员！我们利用了 OpenAI 的审核和聊天端点来创建一个自定义的内容审核员，它不仅能够标记不安全的内容，如仇恨和威胁性信息，还能防止 Discord 服务器的用户受到不想要的请求。

## 读者剩余的练习

尽管我们在本章（以及本书中）取得了很大的成就，但我们还可以做一件事来改进代码。例如：

+   我们创建的独立 Discord 机器人知道不要回复它们自己发送的消息。然而，这些机器人还没有意识到它们不应该回复其他机器人发送的消息。换句话说，如果你同时运行两个机器人，有人在“问答”频道发布不良内容，内容审核员当然会删除这条消息并通知所有人该消息已被删除。然而，由于技术支持机器人不知道它不应该回复其他机器人，它会尝试创建一个回复。当然，机器人之间不应该互相交流。

IndexA, B 应用程序编程接口 (APIs)SeeOpenAIAI (人工智能)ChatGPT 客户端 ForQAandModeration.javaFAQ.txt 文件 moderations 端点 monumental achievementonMessageReceived() 方法 TechSupportBot.java 类 See also 多模态 AIAudioSplitter.java 自动语音识别 (ASR)C 聊天生成预训练转换器 (ChatGPT)分析信息数据模型工厂模式 Java 设计模式语言模型神经网络观察者模式 OpenAISeeOpenAI 预训练模型正则表达式响应单例模式字符串分词温度令牌计数器 ChatGPTSee 聊天生成预训练转换器 (ChatGPT)ChatGPT 客户端 ForQAandModeration.javaJSONPath 源代码 TechSupportBot.javaChatGPT 客户端.Javabuilder 模式 Chat 对象初始对话 Message.java 类生成的代码源代码社区管理 app/serviceDiscordSeeDiscord 机器人 Slack 机器人内容审核机器人 Dumb.javaContentModeratorBot.javaclass 定义 onMessageReceived() 方法源代码 DDALL⋅E 模型创建图像端点 HTTP 参数 JSON 对象请求体响应处理 DALLEClient.java 类 GPT-4 提示工程常见类型描述性文本提示 Discord 机器人授权按钮功能频道创建“/command”社区平台内容审核机器人 Dumb.javaContentModeratorBot.java 继续按钮创建/注册应用程序 Crook’s Bank 依赖项开发者网站一般信息一般信息页面 ID 令牌智能 See 人工智能 (AI)JDA 库消息内容意图 OAuth2 参数 onMessageReceived() 方法特权网关意图注册机器人应用程序场景系统消息 TechSupportBotDumb.javaTechSupportBot.java 类文本权限 Web 界面 E, F 嵌入模型 Xtreme Programming (XP)G, H 生成预训练转换器 (GPT)I 智能 See 人工智能 (AI)J, KJava Discord API (JDA)Java 编程，列表模型 JavaScript 对象表示法 (JSON)聊天完成对象聊天结构 DALL E 模型图像端点列表模型端点 moderations 端点 LLegacy/deprecated models 列表模型端点 OpenAI 模型 MM 移动银行应用程序审核模型审核端点类别内容审核机器人 Dumb.javaContentModeratorBot.javaHTTP 参数智能 discordJSON 对象 ModerationClient.java 冒犯性对话请求体结构多模态 AIAudioSplitter.java 内容创建 DALL⋅ESeeDALL⋅E 模型 JavaCV/FFmpeg 库分割音频文件步骤转录端点 WhisperClient.javawhisper 模型 NN 自然语言处理 (NLP)自然语言理解 (NLU)OOpenAIAPI 概念关键模型沙盒 API 密钥助手字段聊天选项识别最大长度模型系统字段系统角色温度用户字段查看代码按钮 REST APIsWhisper 模型 P, Q 配对编程播客可视化提示工程 DALL⋅E 模型 GPT-4 文本 See 文本摘要 RREST APIsSSlack 消息机器人应用程序账户创建 API 网站 APP 按钮创建频道信息安装过程 OAuth/权限页面 cope 设置 token 频道详情 ChatGPTClient.javaSeeChatGPTClient.java 社区管理虚构公司抓取消息 ChannelReaderSlackBot.java 方便的方法依赖项 MethodsClient 类提示工程现实世界问题软件开发语音识别系统 T, U, VTechSupportBotDumb.javaTechSupportBot.java 类文本摘要复杂对话长对话真实提示工程建议信息过长；没读 (tl;dr)文本到语音 (TTS) 模型转录端点 HTTP 参数请求体 W, X, Y, ZWhisperClient.javaWhisper 模型 AudioSplitter.java 功能/限制含义语音识别转录端点
