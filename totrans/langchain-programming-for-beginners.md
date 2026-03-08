目录

前言

学习本书

需求

源代码

联系方式

第一章：生成式 AI 应用简介

什么是大型语言模型？

什么是 LangChain？

生成式 AI 应用程序的架构

开发环境设置

为什么有不同的 python 和 python3 命令？

摘要

第二章：您的第一个 LangChain 应用程序

获取 Google Gemini API 密钥

运行应用程序

资源耗尽错误

摘要

第三章：在 LangChain 中使用 OpenAI LLM

开始使用 OpenAI API

将 OpenAI 与 LangChain 集成

ChatGPT vs Gemini：使用哪一个？

摘要

第四章：在 LangChain 中使用开源 LLM

Ollama 简介

在 LangChain 中使用 Ollama

再次，使用哪一个？

摘要

第五章：使用 Streamlit 添加 Web GUI

Streamlit 简介

摘要

第六章：LangChain 提示模板

创建提示模板

具有多个输入的提示模板

限制 LLM 回答不想要的提示

摘要

第七章：LangChain 表达式语言（LCEL）

顺序链

简单的顺序链

在顺序链中使用多个 LLM

调试顺序链

摘要

第八章：常规顺序链

格式化输出变量

摘要

第九章：在 LangChain 中实现聊天历史

创建聊天提示模板

在 Streamlit Chat 历史中保存消息

显示聊天历史

使用 Streamlit Chat 输入克隆 ChatGPT

摘要

第十章：AI 代理和工具

创建 AI 代理

为代理添加 Streamlit UI

可用 AI 工具列表

AI 代理的类型

摘要

第十一章：在 LangChain 中与文档交互

获取文档

安装 ChromaDB

构建与文档的聊天应用程序

将 Streamlit 聊天 UI 添加到应用程序中

为上下文添加聊天记忆

流式传输答案

切换 LLM

摘要

第十二章：上传不同类型的文档

摘要

第十三章：与 YouTube 视频聊天

添加 YouTube 加载器

处理不存在转录错误

摘要

第十四章：使用多模态消息与图像交互

理解多模态消息

在 LangChain 中发送多模态消息

添加 UI 和聊天历史

Ollama 多模态消息

摘要

第十五章：将 AI 应用程序部署到生产环境

在 Streamlit 中创建侧边栏

在项目文件夹中添加 requirements.txt 文件

创建 GitHub 仓库

部署到 Streamlit

摘要

总结

关于作者

# LangChain 编程入门

使用 LangChain、Python、OpenAI/ChatGPT、Google/Gemini 和其他 LLM 开发 AI 应用程序的步骤指南

本书作者：Nathan Sebhastian

前言

本书的目标是提供一系列温和的、逐步的指导，帮助你从基础到高级逐步学习 LangChain。

你将看到为什么 LangChain 是构建 AI 应用程序的一个伟大工具，以及它是如何简化语言模型集成到你的项目中的。

我们将了解 LangChain 的关键功能，如提示模板、链、代理、文档加载器、输出解析器和模型类，是如何用于创建一个智能且灵活的生成式 AI 应用程序的。

完成本书后，你将知道如何使用 LangChain 和 Python 创建 AI 驱动的应用程序。

## 按照本书学习

本书分为 15 章简明扼要的内容，每章都专注于 LangChain 编程的一个特定主题。

我鼓励你编写这本书中看到的代码并运行它们，以便你有一个关于 LangChain 开发外观的感觉。当你与书中的示例一起编码时，你会学得最好。

使用本书的一个小贴士：在完成一个章节后至少休息 10 分钟，这样你可以恢复精力并集中注意力。

此外，如果某些概念难以理解，请不要气馁。学习任何新事物在第一次尝试时都很困难，尤其是像编程这样的技术性内容。最重要的是继续前进。

## 需求

为了充分利用本书，需要具备基本的 Python 知识。

如果你需要学习 Python 的一些帮助，你可以在[`g.codewithnathan.com/beginning-python`](https://g.codewithnathan.com/beginning-python)找到我的书。

## 源代码

你可以从以下链接在 GitHub 上下载源代码：

[`github.com/nathansebhastian/langchain-python`](https://github.com/nathansebhastian/langchain-python)

点击“代码”按钮，然后点击下面的“下载 ZIP”链接，如图所示：

![0 下载源代码](img/langchain-programming-for-beginners-image_rsrc1Y9.jpg)

图 1. 在 GitHub 上下载源代码

你需要解压存档以访问代码。通常，你只需双击存档即可提取内容。

文件夹名称中的数字表示本书中的章节编号。

## 联系方式

如果你需要帮助，你可以通过 nathan@codewithnathan.com 联系我。

你也可以在 LinkedIn 上连接或关注我，[`linkedin.com/in/nathansebhastian`](https://linkedin.com/in/nathansebhastian)

第一章：生成式 AI 应用简介

生成式 AI 应用是一种计算机应用程序，可以根据给定的输入（或提示）生成上下文相关的输出。

生成式 AI 应用在 2022 年引起了公众的关注，当时 OpenAI 发布了 ChatGPT，并在短短 5 天内迅速获得了 100 万用户：

![1 chatgpt stats](img/langchain-programming-for-beginners-image_rsrc1YA.jpg)

图 2. ChatGPT 在 5 天内达到 100 万用户

生成式 AI 应用的另一个例子是 chatpdf.com，它允许用户上传 PDF 并执行各种任务，例如从 PDF 中提取见解。

chatpdf.com 提供的答案包含对原始 PDF 文档中来源的引用，因此不再需要翻页查找来源。

在幕后，这些生成式 AI 应用利用大型语言模型的力量来生成答案。

## 什么是大型语言模型？

大型语言模型（LLM，简称）是一种机器学习模型，可以理解并生成人类可以理解的结果。

LLM 通常在互联网上可用的海量文本数据上进行训练，以便它们能够执行广泛的与语言相关的任务，例如翻译、摘要、问答和创意写作。

LLM 的例子包括 OpenAI 的 GPT-4、Google 的 Gemini、Meta 的 Llama 和 Mistral 的 Mistral。

一些 LLM 是闭源的，如 GPT 和 Gemini，而一些是开源的，如 Llama 和 Mistral。

## 什么是 LangChain？

LangChain 是一个开源框架，旨在简化开发 LLM 驱动应用程序的过程。

LangChain 允许你通过调用表示模型的类来简单地集成和调用 LLM，从而为生成式 AI 应用提供动力。

在幕后，LangChain 将执行与语言模型 API 交互所需的步骤，并管理输入和输出的处理，以便你可以通过最小的代码更改访问不同的 LLM。

更重要的是，您还可以使用 LangChain 与外部数据源（如 PDF、维基百科文章或搜索引擎结果）一起生成上下文相关的响应。

通过使用 LangChain，您可以开发针对特定用例优化的专用生成式 AI 应用程序，例如总结 YouTube 视频、从 PDF 中提取见解或撰写文章。

## 生成式 AI 应用的架构

传统应用程序通常使用以下客户端-服务器架构：

![1 client server arch](img/langchain-programming-for-beginners-image_rsrc1YB.jpg)

图 3. 客户端-服务器架构

客户端和服务器通过 HTTP 请求进行通信。当需要时，服务器可能会与数据库交互以完成客户端发送的请求。

另一方面，生成式 AI 应用程序利用 LLM 的力量来理解人类语言提示并生成相关的输出：

![1 ai client server arch](img/langchain-programming-for-beginners-image_rsrc1YC.jpg)

图 4. AI 驱动的应用架构

虽然架构与传统应用程序类似，但增加了一层来连接到 LLM。

这就是 LangChain 发挥作用的层次，因为它执行并管理与 LLM 相关的任务，例如将我们的输入处理成 LLM 可以理解的提示。它还将 LLM 的响应处理成传统应用程序接受的格式。

随着您在下一章中练习构建生成式 AI 应用程序，您将理解得更多。

现在，只需将 LangChain 视为您的应用程序服务器和 LLM 之间的管理层即可。

## 开发环境设置

要开始使用 LangChain 开发 AI 应用程序，您需要在您的计算机上准备三样东西：

1.  网络浏览器

1.  代码编辑器

1.  Python 编程语言

让我们在下一节中安装它们。

### 安装 Chrome 浏览器

任何网络浏览器都可以用来浏览互联网，但出于开发目的，您需要有一个具有足够开发工具的浏览器。

由谷歌开发的 Chrome 浏览器是一款非常适合网页开发的浏览器，如果您还没有安装此浏览器，可以在此处下载：

[`google.com/chrome`](https://google.com/chrome)

浏览器适用于所有主流操作系统。下载完成后，按照安装程序提供的步骤进行安装，即可在您的计算机上使用浏览器。

接下来，我们需要安装一个代码编辑器。互联网上有许多免费的代码编辑器可供选择，例如 Sublime Text、Visual Studio Code 和 Notepad++。

在这些编辑器中，我最喜欢的是 Visual Studio Code，因为它速度快且易于使用。

### 安装 Visual Studio Code

Visual Studio Code 或简称 VSCode 是一款专为编写代码而创建的代码编辑器应用程序。除了免费之外，VSCode 还速度快，可在所有主流操作系统上使用。

您可以在此处下载 Visual Studio Code：

[`code.visualstudio.com`](https://code.visualstudio.com)

当你打开上面的链接时，应该会显示一个按钮，显示与你的操作系统兼容的版本，如下所示：

![1 下载 vscode](img/langchain-programming-for-beginners-image_rsrc1YD.jpg)

图 5. 下载 VSCode

点击按钮下载 VSCode，并在你的电脑上安装它。

现在你已经安装了代码编辑器，下一步是安装 Node.js

### 安装 Python

以下部分将向您展示如何在 macOS、Windows 和 Linux 上安装 Python。请随意跳转到您使用的操作系统。

#### 在 macOS 上安装 Python

如果你使用的是最新版本的 macOS，那么 Python 应该已经包含在你的系统中了。

要检查你是否已安装 Python，打开终端应用程序并运行以下命令：

python3 --version

你应该看到以下输出：

![1 mac python version](img/langchain-programming-for-beginners-image_rsrc1YE.jpg)

图 6. 在 Mac 上检查 Python 版本

如果你看到“命令未找到：python3”的消息，这意味着你需要自己安装 Python。

打开你的浏览器并转到 [`www.python.org/downloads`](https://www.python.org/downloads) 下载适用于 Mac 的 Python 解释器。

网站应该会显示一个下载适用于你的 Mac 的 .dmg 或 .pkg 安装程序的链接。

下载后，只需按照屏幕上显示的安装步骤进行操作。

安装完成后，再次运行 python3 --version 命令。这次，你应该能在输出中看到 Python 版本。

#### 在 Windows 上安装 Python

要在 Windows 上安装 Python，你需要下载 [`www.python.org/downloads`](https://www.python.org/downloads) 上的 Python 安装程序。

网站应该检测到你使用的操作系统，并提供兼容的 Python 安装程序，如下所示：

![1 python windows](img/langchain-programming-for-beginners-image_rsrc1YF.jpg)

图 7. 在 Windows 上安装 Python

下载并运行 .exe 安装程序，以获取 Windows 上的最新稳定版 Python。

在设置向导中，你需要选择以下选项“将 Python.exe 添加到 PATH”：

![1 win add python topath](img/langchain-programming-for-beginners-image_rsrc1YG.jpg)

图 8. 在 Windows 上将 Python 添加到 PATH

这是为了让你以后可以从命令提示符访问 Python。接下来，选择“立即安装”选项以使用默认设置进行安装。

完成后，打开命令提示符并运行以下命令：

python --version

你应该在输出中看到 Python 版本号，如下所示：

![1 win python version](img/langchain-programming-for-beginners-image_rsrc1YH.jpg)

图 9. Windows Python 版本

如果不起作用，尝试运行 py --version，因为 Windows 系统通常将 py 别名为 Python 程序。

现在，你可以在 Windows 系统中运行 Python 代码了。

#### 在 Linux 上安装 Python

Linux 系统是为软件开发者设计的，因此许多 Linux 发行版默认已经包含了 Python。

如果你使用的是最新版本的 Ubuntu，尝试从终端运行 Python。输入 python3 --version 并运行命令。

你应该看到以下响应：

![1 ubuntu python version](img/langchain-programming-for-beginners-image_rsrc1YJ.jpg)

图 10. Ubuntu Python 版本

这意味着 Python 解释器已经安装在你的系统上了。

如果你看到 Linux 响应“命令 'python3' 未找到”，那么你可以使用以下方式使用 apt-get 安装它：

sudo apt-get install python3

现在，你可以在 Linux 系统上运行 Python 代码了。

## 为什么会有不同的 python 和 python3 命令？

在 macOS 和 Linux 系统中，Python 解释器通常包含在操作系统内，因为这两个系统中的许多应用程序都依赖于 Python。

操作系统捆绑的 Python 版本通常是 Python 2，你可以通过在 Mac 和 Linux 上运行 python --version 命令来验证这一点。

为了让你能够安装 Python 3 而不与捆绑版本冲突，Mac 和 Linux 的 Python 安装程序使用 python3 作为别名。

这就是为什么可以使用两个命令来运行 Python：python 和 python3。

因为 Windows 没有包含 Python 解释器，它通常只有 python 命令，而 macOS 和 Linux 可以提供 python 和 python3。

因此，根据你拥有的操作系统，你需要使用 python 或 python3 命令来运行 Python 3 解释器。

## 摘要

在本章中，你学习了生成式 AI 应用程序的架构，以及 LangChain 如何在服务器和 LLM API 端点之间扮演集成层的角色。

你也已经安装了在计算机上编写和运行 LangChain 应用程序所需的工具。

如果你遇到任何问题，你可以通过电子邮件 nathan@codewithnathan.com 联系我，我会尽我所能帮助你。

第二章：你的第一个 LangChain 应用程序

是时候创建我们的第一个 LangChain 应用程序了。

我们将创建一个简单的问答应用程序，我们可以向大型语言模型提出任何类型的问题。

首先，你需要使用 pip 安装 LangChain 模块。

pip 是一个用于安装和管理 Python 包的 Python 程序。当你安装 Python 到你的计算机上时，它已经包含在内了。

打开命令行，然后运行以下命令来检查 pip 版本：

pip --version

Python 包是你可以免费在你的项目中使用的 Python 库和框架。我们将使用 pip 来安装 LangChain 包。

如果你没有 pip，你需要按照上一章中的说明安装 Python。

在你的命令行中，运行以下命令：

pip install langchain==0.2.1 python-decouple==3.8 langchain-google-genai==1.0.5

pip install 命令用于安装你指定旁边的包。

为了避免破坏性更改，你可以指定要安装的包的确切版本，如上所示使用==version。

langchain 包包含了你需要开始使用 LangChain 的一切。python-decouple 包用于在你的项目中加载和使用环境变量。

langchain-google-genai 包包含了 LangChain 和 Google 生成 AI 模型之间的集成。

安装完成后，在您的计算机上创建一个文件夹，用于存储与此项目相关的所有文件。您可以将文件夹命名为 'beginning_langchain'。

然后，打开 Visual Studio Code，从菜单栏中选择文件 > 打开文件夹…。选择您之前创建的文件夹。

VSCode 将加载文件夹并在资源管理器侧边栏中显示内容，它应该是空的，因为我们还没有创建任何文件。

要创建文件，在 VSCode 窗口内的任何位置右键单击，然后从菜单中选择“新建文本文件”或“新建文件…”。

文件创建完成后，按 Control + S 或 Command + S 保存文件。将文件命名为 app.py。

下一步是编写问答应用的代码。

首先，按照以下方式导入应用程序所需的包：

from langchain_google_genai import ChatGoogleGenerativeAI

from decouple import config

要与 LangChain 中的 LLM 交互，您需要创建一个表示该 LLM API 的对象。

因为我们想与 Google 的 LLM 交互，所以我们需要从 ChatGoogleGenerativeAI 类创建一个对象，如下所示：

GOOGLE_GEMINI_KEY = config("GOOGLE_GEMINI_KEY")

llm = ChatGoogleGenerativeAI(model="gemini-pro", google_api_key=GOOGLE_GEMINI_KEY)

GOOGLE_GEMINI_KEY 包含您将在下一节中获取的 API 密钥。

目前，您只需了解 ChatGoogleGenerativeAI 对象代表 Google LLM。

当实例化 llm 对象时，您可以选择要交互的模型，然后通过 google_api_key 参数传递 API 密钥。

接下来，编写以下简单问答应用的代码：

print("Q & A With AI")

print("=============")

question = "What's the currency of Thailand?"

print("Question: " + question)

response = llm.invoke(question)

print("Answer: " + response.content)

在这里，我们简单地打印一些文本，显示我们想要向模型提出的问题。

llm.invoke() 方法会将输入问题发送给 LLM 并返回答案。

答案存储在 content 属性下，因此我们在上面的代码中打印 response.content。

虽然应用程序已经准备就绪，但我们仍然需要获取在此应用程序中使用的 Google Gemini API 密钥。

## 获取 Google Gemini API 密钥

要获取 API 密钥，您需要访问 Gemini API 页面 [`ai.google.dev/gemini-api`](https://ai.google.dev/gemini-api)。

在页面上，您需要点击如下所示的“在 Google AI Studio 获取 API 密钥”按钮：

![2 get gemini api key](img/langchain-programming-for-beginners-image_rsrc1YK.jpg)

图 11. 获取 Gemini API 密钥

从那里，您将被带到 Google AI Studio。

注意，当您点击按钮时，您可能会看到以下页面：

![2 google available regions](img/langchain-programming-for-beginners-image_rsrc1YM.jpg)

图 12. Google AI Studio 可用地区页面

当你位于一个由 Google AI Studio 不提供服务的地区时，这个页面通常会显示。

一种处理方法是通过使用 VPN 服务，但我建议您使用另一个 LLM，例如 OpenAI 或 Ollama，这些内容将在下一章中展示。

如果这是您第一次访问工作室，它会向您展示如下服务条款：

![2 个 Gemini 同意](img/langchain-programming-for-beginners-image_rsrc1YN.jpg)

图 13\. Google AI Studio 服务条款

只需勾选“我同意”选项，然后点击“继续”。

现在点击“创建 API 密钥”按钮以创建密钥：

![2 个 Gemini 创建密钥](img/langchain-programming-for-beginners-image_rsrc1YP.jpg)

图 14\. Gemini 创建 API 密钥

如果您被问及在哪里创建 API 密钥，请选择在新项目中创建：

![2 个 Gemini API 密钥新项目](img/langchain-programming-for-beginners-image_rsrc1YR.jpg)

图 15\. 在新项目中创建 API 密钥

Google 将为您创建一个云项目并生成密钥。

一段时间后，您应该会看到一个弹出框中显示的密钥，如下所示：

![2 个 Gemini 密钥显示](img/langchain-programming-for-beginners-image_rsrc1YS.jpg)

图 16\. 生成的 Gemini API 密钥

复制 API 密钥字符串，然后在您的应用程序文件夹中创建一个 .env 文件，内容如下：

GOOGLE_GEMINI_KEY='您的密钥'

将上面的“您的密钥”字符串替换为您的实际 API 密钥。

## 运行应用程序

设置了 API 密钥后，您就可以运行 LangChain 应用程序了。

在终端上，使用以下方式运行 .py 文件，使用 Python：

python app.py

您应该在终端中看到以下输出：

人工智能问答

=============

问题：泰国的货币是什么？

答案：泰铢

这意味着您已成功创建了您的第一个 LangChain 应用程序，并使用 API 密钥与 Google 的 Gemini LLM 进行了交互。

每个 LLM 模型都有其自身的特点。'gemini-pro'模型通常直接回答问题，不提供额外信息。

您可以尝试将模型更改为如下所示的 'gemini-1.5-flash-latest'：

llm = ChatGoogleGenerativeAI(model="gemini-1.5-flash-latest", google_api_key=GOOGLE_GEMINI_KEY)

现在再次使用 Python 运行 .py 文件，这次答案略有不同：

人工智能问答

=============

问题：泰国的货币是什么？

答案：泰国的货币是**泰铢**，缩写为**THB**或**฿**。

在这里，'gemini-1.5-flash' 首先重复了问题，然后提供了更多信息，例如货币缩写和符号。

THB 和 ฿ 周围的星号 **符号是为了使文本显示为粗体，但在终端中它以原样显示**。

现在尝试将问题变量替换为您想要询问 LLM 的任何问题。

## 资源耗尽错误

当使用 Google Gemini 时，运行应用程序时可能会看到如下错误：

资源耗尽错误：429 资源耗尽（例如检查配额）...

这个错误发生是因为免费层资源已耗尽。您需要稍后再试。

## 摘要

本章的代码可在 02_Simple_Q&A_Gemini 文件夹中找到。

在本章中，您已创建并运行了您的第一个 LangChain 应用程序。恭喜！

该应用程序可以连接到 Google 的 Gemini LLM 来提问并获得答案。

在下一章中，我们将学习如何在 LangChain 中使用 OpenAI 的 GPT 模型。

第三章：在 LangChain 中使用 OpenAI LLM

在上一章中，您已经看到了如何使用 LangChain 与 Google 的 Gemini 模型进行通信。

在本章中，我将向您展示如何将 OpenAI 作为替代方案在 LangChain 中使用。

但请记住，OpenAI API 没有免费层。它曾经提供价值 5 美元的 API 使用额度，但似乎已经悄悄停止。

因此，如果您想使用 OpenAI API，您需要购买最低信用额度，即 5 美元。

## 开始使用 OpenAI API

OpenAI 是一家致力于开发和推广有益于人类的人工智能软件的研究公司。著名的 ChatGPT 就是 OpenAI 开发的产品之一。

除了 ChatGPT 应用程序外，OpenAI 还提供 GPT 模型，这是 ChatGPT 的底层大型语言模型，以 HTTP API 端点形式提供。

要使用 OpenAI 的 API，您需要在他们的网站上注册账户 [`platform.openai.com`](https://platform.openai.com)。

在您注册后，您可以访问 [`platform.openai.com/api-keys`](https://platform.openai.com/api-keys) 创建一个新的密钥。

当您第一次尝试创建密钥时，您将被要求通过添加电话号码进行验证：

![3 openai phone verification](img/langchain-programming-for-beginners-image_rsrc1YT.jpg)

图 17\. OpenAI 电话验证

OpenAI 仅用于验证目的使用您的电话号码。您将通过短信收到验证码。

一旦您完成验证，您将被要求添加 API 使用信用额。如果没有，请访问 [`platform.openai.com/account/billing`](https://platform.openai.com/account/billing) 添加一些信用额。

![3 openai add credit](img/langchain-programming-for-beginners-image_rsrc1YU.jpg)

图 18\. OpenAI 添加信用额

OpenAI 通过信用卡收取费用，因此您需要拥有一张。您最低可以购买 5 美元，这足以运行本书中所有使用 OpenAI 的示例。

或者，如果您以某种方式获得了 5 美元的免费试用信用额，那么您不需要设置您的账单信息。

接下来，输入名称并选择密钥将属于的项目：

![3 openai create key](img/langchain-programming-for-beginners-image_rsrc1YV.jpg)

图 19\. OpenAI 创建 API 密钥

点击“创建密钥”按钮，OpenAI 将显示生成的密钥：

![3 openai copy key](img/langchain-programming-for-beginners-image_rsrc1YW.jpg)

图 20\. OpenAI 复制 API 密钥

您需要将此 API 密钥复制并粘贴到项目的 .env 文件中：

OPENAI_KEY='您的密钥位置'

现在您已经有了 OpenAI 密钥，是时候在 LangChain 应用程序中使用它了。

## 将 OpenAI 与 LangChain 集成

在 LangChain 中使用 OpenAI，您需要使用 pip 安装 langchain_openai 包：

pip install langchain-openai==0.1.7

一旦安装了包，创建一个名为 app_gpt.py 的新文件，并从包中导入 ChatOpenAI 类。

我们还需要使用 config() 添加 OPENAI_KEY，如下所示：

from decouple import config

from langchain_openai import ChatOpenAI

OPENAI_KEY = config("OPENAI_KEY")

llm = ChatOpenAI(model="gpt-4o", api_key=OPENAI_KEY)

你可以使用你想要使用的模型来更改模型参数。截至本文写作时，GPT-4o 是 OpenAI 发布的最新 LLM。

让我们向 GPT 提出与 Gemini 相同的问题：

print("Q & A With AI")

print("=============")

question = "What's the currency of Thailand?"

print("Question: " + question)

response = llm.invoke(question)

print("Answer: " + response.content)

保存更改，然后使用 Python 运行文件：

python app_gpt.py

你应该得到一个类似这样的响应：

Q & A With AI

=============

问题：泰国的货币是什么？

答案：泰国的货币是泰铢。其 ISO 代码是 THB。

这意味着 LangChain 应用程序成功与 OpenAI 的 GPT 聊天模型进行了通信。太棒了！

你可以通过更改问题变量的值尝试提出另一个问题。

## ChatGPT vs Gemini：使用哪一个？

ChatGPT 和 Gemini 都非常擅长执行这本书中我们希望它们完成的任务，所以这完全取决于你。

在过去，OpenAI 曾免费提供 5 美元的信用额度。但似乎不再是这样了，因为 OpenAI 论坛上的许多人表示，注册后他们没有收到。

另一方面，谷歌提供 Gemini 模型的免费层，以换取使用我们的数据来训练模型，所以对于学习和探索 LangChain 来说，使用它是可以的。

然而，谷歌有权随时停止免费层，所以让我再介绍一种在 LangChain 中使用 LLMs 的方法。

这次，我们将使用开源模型。

## 摘要

本章的代码可在书籍源代码的 03_Using_OpenAI 文件夹中找到。

在本章中，你学习了如何创建 OpenAI API 密钥并在 LangChain 应用程序中使用它。

在这里，我们开始看到使用 LangChain 的一个好处，那就是它易于与任何类型的 LLMs 集成。

LangChain 将 LLMs 表示为可以安装并导入到你的项目中的包。

你只需要创建模型类的实例并运行 invoke()方法来访问 LLM。

无论何时你需要使用另一个 LLM，你只需更改 llm 变量并传递所需的 API 密钥。

第四章：在 LangChain 中使用开源 LLMs

LangChain 库使你能够与任何类型的 LLMs 进行通信，从专有 LLMs 如谷歌的 Gemini 和 OpenAI 的 GPT 到开源 LLMs 如 Meta 的 Llama 和 Mistral。

本章将向你展示如何在 LangChain 中使用开源模型。让我们开始吧。

## Ollama 简介

Ollama 是一个用于在本地运行 LLMs 的工具。它负责下载、管理和打开你想要在电脑上使用的模型的 HTTP API 端点。

要开始，请访问[`ollama.com`](https://ollama.com)并点击“下载”按钮。

从那里，你可以选择适合你的操作系统的版本：

![4 download ollama](img/langchain-programming-for-beginners-image_rsrc1YX.jpg)

图 21. 下载 Ollama

下载完成后，打开包并按照说明操作，直到被要求按照以下方式安装命令行工具：

![4 ollama 终端](img/langchain-programming-for-beginners-image_rsrc1YY.jpg)

图 22. 安装 Ollama 终端命令

点击“安装”按钮继续。

安装完成后，Ollama 会向你展示如何运行模型：

![4 ollama 运行第一个模型](img/langchain-programming-for-beginners-image_rsrc1YZ.jpg)

图 23. Ollama 运行您的第一个模型

但由于 Llama 3 是一个 800 亿参数的模型，该模型相当大，有 4.7 GB。

我建议你运行 Gemma 模型，它有 20 亿参数：

ollama run gemma:2b

Gemma 模型是来自 Google 的一个轻量级模型，所以你可以将其视为 Google Gemini 的开源版本。

Gemma 2B 模型大小仅为 1.7 GB，所以在你想尝试 ollama 时非常有用。

下载完成后，你就可以立即从终端使用该模型。如下所示提问：

![4 运行 gemma](img/langchain-programming-for-beginners-image_rsrc1Z0.jpg)

图 24. 在 Ollama 中询问 Gemma 的示例

要退出正在运行的模型，请输入/bye 并按 Enter 键。

只要 Ollama 在你的电脑上运行，Ollama API 端点就可以在 localhost:11434 上访问，如下所示：

![4 ollama 本地](img/langchain-programming-for-beginners-image_rsrc1Z1.jpg)

图 25. Ollama 本地 API 端点

LangChain 将使用此 API 端点与 Ollama 模型通信，这是我们接下来要做的。

## 在 LangChain 中使用 Ollama

要使用 Ollama 下载的模型，你需要从 langchain_community.chat_models 模块导入 ChatOllama 类。

创建一个名为 app_ollama.py 的新文件，并按如下所示导入 Ollama 聊天模型：

from langchain_community.chat_models import ChatOllama

llm = ChatOllama(model="gemma:2b")

print("Q & A With AI")

print("=============")

question = "What's the currency of Thailand?"

print("Question: " + question)

print("Answer: " + response.content)

你还需要将 ChatOllama 对象分配给上面所示的 llm 变量。

由于 Ollama 是开源且本地的，使用时无需添加 API 密钥。

现在，你可以使用 Python 运行文件来与 LLM 进行通信。你应该得到以下类似的响应：

人工智能问答

=============

问题：泰国的货币是什么？

答案：泰国的货币是泰铢（THB），它被分为 100 分。泰铢用符号 THB 表示。

注意，由于 LLM 模型是在你的电脑上运行的，与 Gemini 和 GPT 模型相比，答案可能需要更长的时间。

这就是如何在 LangChain 中使用 Ollama。如果你想使用其他开源模型，你需要首先使用 Ollama 下载该模型：

ollama pull mistral

pull 命令下载模型，但不会在命令行上运行它。

之后，你可以在创建 ChatOllama 对象时切换模型参数：

# 切换模型

llm = ChatOllama(model="mistral")

记住，模型越大，运行所需的时间越长。

常规指南是，你应该至少有 8 GB 的 RAM 来运行 7B 模型，16 GB 来运行 13B 模型，以及 32 GB 来运行 33B 模型。

有许多开源模型可以使用 Ollama 运行，例如 Google 的 Gemma 和 Microsoft 的 Phi-3。

你可以探索 [`ollama.com/library`](https://ollama.com/library) 来查看所有可用的模型。

## 再次，选择哪一个？

到目前为止，你已经探索了如何使用 Google Gemini、OpenAI GPT 和 Ollama 开源模型。在你的应用程序中应该使用哪一个？

如果你负担得起，我建议你使用 OpenAI GPT，因为它的 API 没有速率限制，结果也非常出色。

如果你因为任何原因无法使用 OpenAI GPT，那么如果你的国家有提供，你可以使用 Google Gemini 的免费层。

如果没有，你可以根据你电脑的 RAM 容量使用 Ollama 下载 Gemma 2B 模型或 Llama 3。

除非特别说明，我将在这本书的所有示例代码中使用 OpenAI GPT。

但别担心，因为替换 LangChain 中的 LLM 部分非常简单。你只需更改本章节中显示的 llm 变量本身即可。

你可以在存储库中找到使用 Gemini 和 Ollama 的代码示例。

## 摘要

本章的代码可在书籍源代码的 04_Using_Ollama 文件夹中找到。

在本章中，你已经学习了如何使用 Ollama 和 LangChain 来使用开源 LLMs。

使用 Ollama，你可以下载并运行任何开源且免费使用的 Large Language Models。

如果你查看 Ollama 网站，你会找到许多非常强大的模型，甚至可以在性能上与专有模型如 Gemini 和 ChatGPT 相媲美。

如果你担心你的数据隐私，并想确保没有人用它来训练他们的 LLMs，那么使用像 Llama 3、Mistral 或 Gemma 这样的开源 LLMs 可以是一个很好的选择。

第五章：使用 Streamlit 添加 Web GUI

到目前为止，我们已经使用 Python 运行简单的问答应用程序。

我们不再使用终端与 LLMs 通信，而是创建一个简单的基于网络的用户界面来与 LLMs 交互。

要创建网络界面，我们将使用 Streamlit 模块。

## Streamlit 简介

Streamlit 是一个开源的 Python 框架，你可以用它用几行代码来构建以数据为导向的应用程序。

通过使用 Streamlit 和 LangChain，你可以为任何类型的 LLM 建立一个基于网络的交互界面。

要开始使用 Streamlit，你需要使用 pip 安装以下包：

pip install streamlit==1.35.0

接下来，导入 streamlit 模块以创建一个标题和文本框，如下所示：

import streamlit as st

# llm...

st.title("Q & A With AI")

question = st.text_input("Your Question")

if question:

response = llm.invoke(question)

st.write(response.content)

st.title() 创建一个 <h1> 元素，并渲染你传递给它的文本。

st.text_input() 创建一个文本输入。返回值是你在框中输入的任何值。

之后，使用 if 语句检查 question 变量是否包含问题。

当问题不为空时，我们运行 llm.invoke()方法并将返回的响应写入 Streamlit。

要运行 Streamlit 应用程序，你需要在命令行上使用 streamlit 而不是 python：

streamlit run app.py

Streamlit 将打开你的网络浏览器并导航到 localhost:8501，那里运行着 Streamlit 应用程序：

![5 streamlit running](img/langchain-programming-for-beginners-image_rsrc1Z2.jpg)

图 26. 在网络浏览器中打开 Streamlit

你可以在框中输入你的问题并按 Enter 键。

LLM 的响应将被写入问题框下方：

![5 streamlit qna](img/langchain-programming-for-beginners-image_rsrc1Z3.jpg)

图 27. Streamlit 输出示例

这样就是使用 Streamlit 为 LLM 驱动的应用程序创建简单界面的方法。

## 摘要

本章的代码可在书籍源代码的 05_Adding_Streamlit_GUI 文件夹中找到。

在本章中，你学习了如何使用 Streamlit 快速创建一个基于 Web 的界面，通过 LangChain 与大型语言模型进行交互。

随着我们构建更高级的 AI 应用程序，我们将进一步探索 Streamlit。

在下一章中，你将学习关于提示模板的内容。那里见！

第六章：LangChain 提示模板

LangChain 提示模板是一个 Python 类，用于创建发送给大型语言模型的特定提示（或指令）。

通过使用提示模板，我们可以在用户输入最少的情况下重复相同的指令。

为了给你一个例子，假设你正在创建一个简单的 AI 应用程序，该应用程序只提供特定国家的货币信息。

根据我们已知的，唯一的方法是重复问题，同时更改国家如下：

question = "What is the currency of Thailand?"

question = "What is the currency of Malaysia?"

question = "What is the currency of India?"

你可以创建一个模板来代替重复的问题，如下所示：

st.title("Currency Info")

country = st.text_input("Input Country")

if country:

question = "What is the currency of " + country + "?"

response = llm.invoke(question)

st.write(response.content)

现在你只需要在输入框中输入国家名称来运行提示。

你可以使用纯字符串或 f-string 来创建提示模板，但 LangChain 建议你使用提示模板类以实现有效重用。让我给你展示一下。

## 创建提示模板

要创建一个提示模板，你需要从 langchain.prompts 导入 PromptTemplate 类，如下所示：

from langchain.prompts import PromptTemplate

下一步是创建提示本身。

你可以创建一个名为 prompt 的变量，然后将调用 PromptTemplate()构造函数传递给该变量：

prompt = PromptTemplate()

当调用 PromptTemplate()构造函数时，你需要传递两个参数：

1.  input_variables - 模板中使用的变量名称列表

1.  template - 用于提示模板本身的字符串

以下是一个完整的 PromptTemplate() 调用的示例：

prompt = PromptTemplate(

input_variables=["country"],

template="{country}的货币是什么？请用一段简短的段落回答",

)

现在您可以在调用 llm.invoke() 方法时使用提示对象。

您需要调用 prompt.format() 方法，并按照 input_variables 参数中指定的变量传递，如下所示：

country = st.text_input("输入国家")

if country:

response = llm.invoke(prompt.format(country=country))

st.write(response.content)

现在运行 Streamlit 应用程序并请求特定国家的货币。

以下是一个请求西班牙货币的示例：

![6 提示结果](img/langchain-programming-for-beginners-image_rsrc1Z4.jpg)

图 28. LLM 响应

PromptTemplate 类提供了一个结构，您可以从该结构构建特定的提示。

## 带有多个输入的提示模板

提示模板可以接受您在模板字符串中需要的任何输入。

例如，假设您想控制段落的数量和答案的语言。您可以在提示模板中添加两个更多变量，如下所示：

prompt = PromptTemplate(

input_variables=["country", "paragraph", "language"],

template="{country}的货币是什么？请用 {paragraph} 段简短的段落在 {language} 中回答"，

)

现在在“国家”输入下方添加两个更多输入，如下所示：

country = st.text_input("输入国家")

paragraph = st.number_input("输入段落数量", min_value=1, max_value=5)

language = st.text_input("输入语言")

注意，段落输入限制在 1 到 5 之间，以避免生成过长的文章。

在 if 语句中添加两个更多变量，使用 and 运算符进行检查，然后在调用 prompt.format() 方法时传递变量：

if country and paragraph and language:

response = llm.invoke(prompt.format(country=country, paragraph=paragraph, language=language))

st.write(response.content)

就这样。现在您可以根据下面所示尝试运行网络应用程序：

![6 多输入提示](img/langchain-programming-for-beginners-image_rsrc1Z5.jpg)

图 29. 多输入结果

结合提示模板和 Streamlit 输入，您可以创建一个更复杂的货币信息应用程序，该应用程序可以生成恰好 N 段的答案，并使用您首选的语言。

## 限制 LLM 对不想要的提示进行响应

提示模板还可以防止您的模型对奇怪的问题给出答案。

例如，您可以询问纳尼亚的货币，纳尼亚是由英国作家 C.S. Lewis 创造的一个虚构国家：

![6 纳尼亚](img/langchain-programming-for-beginners-image_rsrc1Z6.jpg)

图 30. LLM 回答各种问题

虽然答案正确，但您可能不希望在应用程序中提供关于虚构或不存在国家的信息。

使用提示模板，您可以像下面这样在多行中指定提示字符串：

prompt = PromptTemplate(

input_variables=["country", "paragraph", "language"],

template='''

你是一位货币专家。你提供关于特定国家使用的特定货币的信息。

避免提供关于虚构地点的信息。

如果国家是虚构的或不存在的，回答：我不知道。

回答问题：{国家}的货币是什么？

用 {段落} 简短段落回答 {语言}

''',

)

上述提示指示 LLM 在被问及虚构地点时不回答。

现在如果你再次提问，LLM 将会这样回答：

![6 提示守卫](img/langchain-programming-for-beginners-image_rsrc1Z7.jpg)

图 31. LLM 不回答

如你所见，当被问及虚构国家的货币时，LLM 拒绝回答。

与反复使用 f-strings 相比，使用提示模板的代码更易于维护且更简洁。

## 摘要

本章的代码可在书籍源代码的 06_Prompt_Template 文件夹中找到。

提示模板的使用使你能够在仅需要用户最小输入的情况下为 LLM 制定复杂的指令。

你的指令越具体，响应就越准确。

你甚至可以指示 LLM 避免回答不想要的提示，如最后部分所示。

第七章：LangChain 表达式语言（LCEL）

在上一章中，我们在 llm.invoke() 方法内部调用了 prompt.format() 方法，如下所示：

response = llm.invoke(prompt.format(country=country, paragraph=paragraph, language=language))

虽然这种技术有效，但 LangChain 实际上提供了一种声明式的方法来顺序执行提示和 llm 对象。

这种声明式的方法被称为 LangChain 表达式语言（简称 LCEL）

使用 LCEL，你可以将提示和 llm 对象包装在链中，如下所示：

chain = prompt | llm

LCEL 以管道（|）运算符为标志，并且可以用来包装 LangChain 组件。LangChain 组件包括提示、LLM 以及链本身。

接下来，你可以从链对象中调用 invoke() 方法，并将提示所需输入作为字典传递，如下所示：

response = chain.invoke(

{"country": country, "paragraph": paragraph, "language": language}

)

st.write(response.content)

链对象将格式化提示，然后自动将其传递给 llm 对象。

响应对象与调用 llm.invoke() 方法时相同：它是一个包含在 content 属性下存储答案的消息对象。

## 顺序链

通过使用 LCEL，你可以在 LLM 对前一个提示做出响应后创建多个链并发送下一个提示。

在前一个提示被回答后发送下一个提示的方法被称为顺序链。

根据输入和输出结果，顺序链分为 2 类：

| ● | 简单顺序链 |
| --- | --- |
| ● | 正规顺序链 |

我们将在接下来的两个部分中看到这些顺序链的示例。

## 简单顺序链

简单的顺序链是链中的每一步只有一个输入/输出。一个步骤的输出将是下一个提示的输入：

![7 ssc](img/langchain-programming-for-beginners-image_rsrc1Z8.jpg)

图 32. 简单顺序链示意图

例如，假设你想创建一个可以写短文的应用程序。

你将提供主题，LLM 将首先决定标题，然后继续为该主题撰写文章。

要创建应用程序，你首先需要为标题创建一个提示：

title_prompt = PromptTemplate(

input_variables=["topic"],

template="""

你是一位专家记者。

你需要为以下主题想一个有趣的主题：{topic}

精确回答一个标题

""",

)

上面的 title_prompt 接收一个输入变量：它将生成的标题的主题。

接下来，你需要按照以下方式为短文创建一个提示：

essay_prompt = PromptTemplate(

input_variables=["title"],

template="""

你是一位专家非虚构作家。

你需要为以下标题写一篇 350 字的短文：

{title}

确保文章引人入胜，让读者感到兴奋。

""",

)

这个 essay_prompt 也接受单个输入：我们之前创建的 title_prompt 生成的标题。

现在你需要为每个提示创建两个链：

first_chain = title_prompt | llm | StrOutputParser()

second_chain = essay_prompt | llm

first_chain 使用 StrOutputParser()将 LLM 响应解析为字符串，因此你需要从 LangChain 导入解析器：

from langchain_core.output_parsers import StrOutputParser

我将在下面展示为什么需要解析器。

现在，你需要将上面的链组合成一个单一的总体链：

overall_chain = first_chain | second_chain

现在，你已经从 first_chain 和 second_chain 组件中创建了一个顺序链。

下一步是更新 Streamlit 界面和 if 语句：

st.title("作文作家")

topic = st.text_input("输入主题")

if topic:

response = overall_chain.invoke({"topic": topic})

st.write(response.content)

完成后。如果你运行应用程序并请求一个主题，你会得到一个类似以下的响应：

![7 sequential result](img/langchain-programming-for-beginners-image_rsrc1Z9.jpg)

图 33. 简单顺序链结果

上面的结果中删除了一些段落，但你已经可以看到，first_chain 提示生成了 second_chain 提示使用的标题变量。

使用简单的顺序链可以将复杂任务分解成一系列更小的任务，从而提高 LLM 结果的准确性。

## 在顺序链中使用多个 LLM

你也可以使用 LCEL 为创建的每个链分配不同的 LLM。

以下示例使用 Google Gemini 运行 first_chain，而 second_chain 使用 OpenAI GPT：

GOOGLE_GEMINI_KEY = config("GOOGLE_GEMINI_KEY")

OPENAI_KEY = config("OPENAI_KEY")

llm = ChatGoogleGenerativeAI(model="gemini-pro", google_api_key=GOOGLE_GEMINI_KEY)

llm2 = ChatOpenAI(model="gpt-4o", api_key=OPENAI_KEY)

# 为每个链使用不同的 LLM：

first_chain = title_prompt | llm | StrOutputParser()

second_chain = essay_prompt | llm2

因为 LCEL 是声明式的，所以你可以轻松地在链中交换组件。

## 调试顺序链

如果你想更详细地查看顺序链的过程，你可以从 LangChain 全局模块中启用调试模式：

from langchain.globals import set_debug

set_debug(True)

当你在 Streamlit 界面中重新运行提示时，你将在命令行上看到调试输出。

你可以通过搜索 [chain/start] 日志来查看 LangChain 发送的提示如下：

[chain/start] [chain:RunnableSequence] 正在运行链输入：

{

"topic": "人工智能对人类的影响"

}

如果你搜索第二个链的输入，你会看到如下定义的提示：

[chain/start] [chain:RunnableSequence > prompt:PromptTemplate] 正在运行输入提示：

{

"input": "**AI 的变革性拥抱：塑造人类未来**"

}

第二个提示的输入格式化为字符串，因为我们为第一个链使用了 StrOutputParser()。

如果你没有解析第一个链的输出，那么第二个链的提示将看起来像这样：

{

"prompts": [

"人类：\n    你是一位专家非虚构作家。\n\n    你需要为以下标题撰写一篇 350 字的短文：\n\n    content=\"**AI 的变革性拥抱：塑造人类未来**\" response_metadata={'prompt_feedback': {'block_reason': 0, 'safety_ratings': []}, 'finish_reason': 'STOP', 'safety_ratings': [{'category': 'HARM_CATEGORY_SEXUALLY_EXPLICIT', 'probability': 'NEGLIGIBLE', 'blocked': False}, {'category': 'HARM_CATEGORY_HATE_SPEECH', 'probability': 'NEGLIGIBLE', 'blocked': False}, {'category': 'HARM_CATEGORY_HARASSMENT', 'probability': 'NEGLIGIBLE', 'blocked': False}, {'category': 'HARM_CATEGORY_DANGEROUS_CONTENT', 'probability': 'NEGLIGIBLE', 'blocked': False}]} id='run-6e718aba-b2a6-4dfb-b9e0-8dc1e338308c-0'\n\n    确保文章引人入胜，让读者感到兴奋。"

]

}

在这里，包括了第一个链的整个响应对象，例如 response_metadata 和 id 属性。

虽然 LLM 足够智能，可以从响应对象中猜测标题，但让我们尽可能减少这种不完美的提示。

## 摘要

本章的代码可在书籍源代码的 07_LCEL 文件夹中找到。

在本章中，你了解了 LangChain 表达式语言，它可以用来以声明式的方式组合 LangChain 组件。

链只是一个这些 LangChain 组件的包装器：

1.  提示模板

1.  要使用的 LLM

1.  处理 LLM 输出的解析器

链的组件可以互换，这意味着你可以为第一个提示使用 GPT 模型，然后为第二个提示使用 Gemini 模型，如上所示。

通过使用 LCEL，你可以创建高级工作流程并与大型语言模型交互以解决复杂任务。

在下一章中，我将向你展示如何创建常规顺序链。

第八章：常规顺序链

常规顺序链是顺序链的更通用形式，允许多个输入和输出。

下一个链的输入通常是前一个链的输出和另一个来源（如本例所示）的混合：

![8 sc](img/langchain-programming-for-beginners-image_rsrc1ZA.jpg)

图 34.顺序链示意图

这个链比简单的顺序链要复杂一些，因为我们需要跟踪多个输入和输出。

例如，假设你将上一章的 essay_prompt 更改为具有两个 input_variables，如下所示：

essay_prompt = PromptTemplate(

input_variables=["title", "emotion"],

template="""

你是一位非虚构写作专家。

你需要为以下标题写一篇 350 字的短文：

{title}

确保文章引人入胜，让读者感受到{emotion}。

""",

)

文章提示所需的情感输入不来自第一个链，它只返回标题变量。

要注入情感输入，你需要在创建 overall_chain 时在 first_chain 和 second_chain 之间传递一个 lambda 函数，如下所示：

overall_chain = (

first_chain

| (lambda title: {"title": title, "emotion": emotion})

| second_chain

)

这样，标题输入来自 first_chain 的输出，而情感输入来自另一个来源。

你可以添加一个文本输入来获取情感输入：

st.title("文章撰写者")

topic = st.text_input("输入主题")

emotion = st.text_input("输入情感")

if topic and emotion:

response = overall_chain.invoke({"topic": topic})

st.write(response.content)

现在你有多个输入，其中一个输入来自第一个链的结果之外。

## 格式化输出变量

顺序链通常也会跟踪多个输出变量。

高级 LLM（如 GPT-4 和 Gemini）可以通过在提示模板中添加特定指令来帮助我们格式化输出为多个变量。

回到 essay_prompt，你可以指示 LLM 以 JSON 格式发送输出：

essay_prompt = PromptTemplate(

input_variables=["title", "emotion"],

template="""

你是一位非虚构写作专家。

你需要为以下标题写一篇 350 字的短文：

{title}

确保文章引人入胜，让读者感受到{emotion}。

将输出格式化为具有三个键的 JSON 对象：'title'、'emotion'、'essay'，并分别填充相应的值

""",

)

现在 LLM 被指示将输出格式化为 JSON 对象，你需要使用 JsonOutputParser 来解析输出。

如下所示将 JsonOutputParser 管道连接到 second_chain：

from langchain_core.output_parsers import StrOutputParser, JsonOutputParser

# ...

first_chain = title_prompt | llm | StrOutputParser()

second_chain = essay_prompt | llm | JsonOutputParser()

接下来，将 st.write() 方法更改为直接写入响应对象：

if topic and emotion:

response = overall_chain.invoke({"topic": topic})

st.write(response)

现在，你可以运行应用程序并看到输出确实是以 JSON 格式：

![8 json 输出](img/langchain-programming-for-beginners-image_rsrc1ZB.jpg)

图 35. 接收 JSON 输出

如果你想写入每个输出变量，你可以直接按如下方式访问它们：

if topic and emotion:

response = overall_chain.invoke({"topic": topic})

st.write(response.title)

st.write(response.emotion)

st.write(response.essay)

现在你有一个跟踪多个输入和输出的顺序链。做得好！

## 摘要

本章的代码可在书籍源代码的 08_Sequential_Chain 文件夹中找到。

当你创建一个顺序链时，你可以向下一个链添加额外的输入，这些输入不是来自上一个链。

使用 lambda 函数，你可以在运行链之前添加自定义逻辑，这样你就可以将上一个链的结果与额外的输入一起发送。

你还可以将输出格式化为 JSON 对象，以便使响应更有组织且更容易处理。

第九章：在 LangChain 中实现聊天历史

到目前为止，LLM 已经根据我们提出的问题从训练数据中检索到了答案。

回到第五章中的简单问答应用，你可以尝试向 LLM 提出一个问题，例如：

1.  世界杯最后一次是在什么时候举行的？

1.  将年份乘以 2

在撰写本文时，上一次 FIFA 世界杯是在 2022 年举行的。阅读上面的第二个提示，我们可以理解 'year' 指的是 '2022'。

然而，由于 LLM 没有意识到之前的交互，答案将不会相关。

使用 GPT，LLM 指的是当前年份而不是上一次 FIFA 世界杯年份：

![9 无历史](img/langchain-programming-for-beginners-image_rsrc1ZC.jpg)

图 36. LLM 无上下文示例

LLM 无法理解我们正在对上一个问题进行后续指令。

为了解决这个问题，你需要保存之前的消息并在发送新提示时使用它们。

为了跟随本章内容，你可以复制第五章的代码并将其用作起点。

## 创建聊天提示模板

首先，你需要创建一个聊天提示模板，其中包含注入的聊天历史。

聊天提示模板与通常的提示模板不同。它接受一个消息列表，并且每个消息都可以与一个特定的角色相关联。

这里是一个聊天提示模板的示例：

from langchain_core.prompts import ChatPromptTemplate

chat_template = ChatPromptTemplate.from_messages(

[

("system", "You are a helpful AI bot. Your name is {name}."),

("human", "Hello, how are you doing?"),

("ai", "I'm doing well, thanks!"),

("human", "{user_input}"),

]

)

在上面的示例中，消息与 'system'、'human' 和 'ai' 角色相关联。

你可以使用 ChatPromptTemplate 和 MessagesPlaceholder 类创建一个接受聊天历史的提示，如下所示：

from langchain_core.prompts import ChatPromptTemplate, MessagesPlaceholder

prompt = ChatPromptTemplate.from_messages(

[

(

"system",

"你是一个与人类进行对话的人工智能聊天机器人。使用以下上下文来理解人类的问题。不要在回答中包含表情符号。",

),

MessagesPlaceholder(variable_name="chat_history"),

("human", "{input}"),

]

)

MessagesPlaceholder 类充当一个开放参数，你可以从中注入聊天历史，这就是我们接下来要做的。

## 在 Streamlit 聊天历史中保存消息

Streamlit 会话状态用于在 Streamlit 应用程序运行期间存储变量。

要在 Streamlit 中保存聊天历史，你需要导入 StreamlitChatMessageHistory 类，并从这个类中实例化一个对象：

from langchain_community.chat_message_histories import StreamlitChatMessageHistory

# 其他代码 ...

chain = prompt | llm

history = StreamlitChatMessageHistory()

接下来，你需要将存储在 Streamlit 中的历史记录注入到链中。

这可以通过使用 RunnableWithMessageHistory 类来完成，它是一个包装了注入聊天历史的链的包装器：

from langchain_core.runnables.history import RunnableWithMessageHistory

# 其他代码...

chain = prompt | llm

history = StreamlitChatMessageHistory()

chain_with_history = RunnableWithMessageHistory(

chain,

lambda session_id: history,

input_messages_key="input",

history_messages_key="chat_history",

)

在创建 RunnableWithMessageHistory 对象时，你需要传递你想要注入历史的链和一个返回聊天历史的函数。

The input_messages_key 是提示中存在的输入键，而 history_messages_key 是接受历史记录的变量（它应该与之前传递给 MessagesPlaceholder 的 variable_name 相同）

现在 chain_with_history 对象已经完成，你可以修改 Streamlit 界面和 if 语句如下：

st.title("与 AI 的问答")

question = st.text_input("你的问题")

if question:

response = chain_with_history.invoke(

{"input": question}, config={"configurable": {"session_id": "any"}}

)

st.write(response.content)

当调用 chain_with_history 对象时，你需要将 session_id 键传递到 config 参数中，如上所示。

session_id 可以是任何字符串值。

现在你可以通过提出一个后续问题来测试应用程序：

Q: 上一个 FIFA 世界杯是在什么时候举办的？

A: 上一个 FIFA 世界杯是在 2022 年举办的。

Q: 将年份乘以 2

A: 2022 乘以 2 等于 4044。

因为聊天历史被注入到提示中，LLM 可以将第二个问题放在第一个问题的上下文中。

如果你通过 set_debug(True)激活调试模式，你将看到如下提示：

"prompts": [

"系统：你是一个与人类进行对话的人工智能聊天机器人。使用以下上下文来理解人类的问题。在回答中不要包含表情符号。\n 人类：上一次 FIFA 世界杯是在哪一年举行的？\nAI：上一次 FIFA 世界杯是在 2022 年。\n\n 人类：将年份乘以 2"

]

如你所见，RunnableWithMessageHistory 在提示中放置 MessagesPlaceholder()的地方注入了历史记录。

## 显示聊天历史

要显示聊天历史，你需要在 st.write()方法下方添加一个 for 循环：

st.write(response.content)

for message in st.session_state["langchain_messages"]:

if message.type == "human":

st.write("问题: " + message.content)

else:

st.write("答案: " + message.content)

上面的 for 循环遍历 st.session_state["langchain_messages"]列表。

我们还检查了消息的类型，在消息内容之前添加了'问题'和'答案'字符串。

现在你应该看到以下聊天历史：

![9 chat history](img/langchain-programming-for-beginners-image_rsrc1ZD.jpg)

图 37. 显示的聊天历史

到目前为止做得很好！

## 使用 Streamlit Chat Input 克隆 ChatGPT

现在我们已经将聊天历史添加到我们的应用程序中，我们可以借助 Streamlit 创建一个看起来像 ChatGPT 的界面。

在文本框中不使用 text_input，你需要使用 chat_input 如下所示：

question = st.chat_input("你的问题")

接下来，使用 with st.chat_message()方法并将角色'user'传递给写入问题：

question = st.chat_input("你的问题")

如果有疑问：

with st.chat_message("user"):

st.markdown(question)

然后将 invoke()调用替换为如下所示的 stream()：

if question:

with st.chat_message("user"):

st.markdown(question)

response = chain_with_history.stream(

{"input": question}, config={"configurable": {"session_id": "any"}}

)

在编写响应时，你需要使用 with st.chat_message()并将'assistant'角色传递给方法：

response = chain_with_history.stream(

{"input": question}, config={"configurable": {"session_id": "any"}}

)

with st.chat_message("assistant"):

st.write_stream(response)

最后，你需要在页面标题下方显示聊天历史，如下所示：

st.title("与 AI 的问答")

for message in st.session_state["langchain_messages"]:

role = "user" if message.type == "human" else "assistant"

with st.chat_message(role):

st.markdown(message.content)

你可以通过检查 message.type 的值来确定消息的角色。

再次运行应用程序，你将看到以下输出：

![9 chatgpt clone](img/langchain-programming-for-beginners-image_rsrc1ZE.jpg)

图 38. 一个更简单的 ChatGPT 克隆

现在你有一个看起来就像 ChatGPT 的合适的人工智能聊天应用程序。太棒了！

## 摘要

本章的代码可在书籍源代码的 09_Chat_History 文件夹中找到。

在本章中，你学习了如何使用 LangChain 的 RunnableWithMessageHistory 类将聊天历史注入提示。

添加聊天历史使 AI 能够根据之前的消息来上下文化你的问题。

结合聊天历史和 Streamlit 用户界面，您可以轻松创建类似于 ChatGPT 的应用程序。

第十章：人工智能代理和工具

人工智能代理是一种能够通过一系列动作解决任务的思考软件。它使用 LLM 作为推理引擎来规划和执行动作。

您需要做的只是给代理一个特定的任务。代理将处理任务，确定解决它所需的动作，然后执行这些动作。

代理还可以使用工具在现实世界中采取行动，例如在互联网上搜索特定信息。

这里有一个插图来帮助您理解代理的概念：

![10 llm agents](img/langchain-programming-for-beginners-image_rsrc1ZF.jpg)

图 39. LLM 代理插图

并非所有 LLM 都能创建代理，因此需要像 GPT-4、Gemini 1.5 Pro 或 Mistral 这样的高级模型。

让我向您展示如何使用 LangChain 创建一个代理。

## 创建人工智能代理

创建一个名为 react_agent.py 的新 Python 文件，并导入以下模块：

from decouple import config

from langchain import hub

from langchain.agents import create_react_agent, AgentExecutor

from langchain_community.agent_toolkits.load_tools import load_tools

from langchain_google_genai import ChatGoogleGenerativeAI

config 和 ChatGoogleGenerativeAI 已经使用过，但其余的都是用于创建人工智能代理的新模块。

中心模块用于从 LangChain 社区中心检索提示。您可以通过[`smith.langchain.com/hub`](https://smith.langchain.com/hub)访问中心。

LangChain 社区中心是一个免费的提示库，您可以在项目中免费使用。

create_react_agent 模块创建一个使用 ReAct 提示的代理，而 AgentExecutor 管理代理的执行，例如处理输入、生成响应和更新代理的状态。

load_tools 模块用于加载 LangChain 中可用的工具。

接下来，初始化 llm 并从中心获取提示，如下所示：

OPENAI_KEY = config("OPENAI_KEY")

llm = ChatOpenAI(model="gpt-4o", api_key=OPENAI_KEY)

prompt = hub.pull("hwchase17/react")

hub.pull()方法从 LangChain 中心库中的存储库检索提示。在这里，我们使用用户"hwchase17"创建的"react"提示。

如果您想查看提示，可以访问[`smith.langchain.com/hub/hwchase17/react`](https://smith.langchain.com/hub/hwchase17/react)

接下来，加载我们想要提供给 LLM 的工具，然后创建代理执行器对象，如下所示：

tools = load_tools(["wikipedia", "ddg-search", "llm-math"], llm)

agent = create_react_agent(llm, tools, prompt)

agent_executor = AgentExecutor(agent=agent, tools=tools, verbose=True)

我们为代理提供了三个工具：

1.  wikipedia 用于访问和总结维基百科文章

1.  ddg-search 用于使用 DuckDuckGo 搜索引擎在互联网上搜索

1.  llm-math 用于计算数学方程

要正确运行这些工具，你需要使用 pip 安装以下包：

pip install wikipedia==1.4.0 duckduckgo-search==6.1.2 numexpr==2.10.0

llm-math 在后台使用 numexpr 包。

安装完成后，通过添加输入提示并调用 invoke()方法来完成代理：

question = input("给我一个任务：")

agent_executor.invoke({"input": question})

并且 AI 代理现在已完成。

你可以使用以下 Python 命令运行代理：

python react_agent.py

现在给代理一个任务来完成，例如 '谁是美国的第一个总统？'

因为在 AgentExecutor 中设置了 verbose 参数为 True，所以你会看到 LLM 的推理过程：

![10 个代理运行](img/langchain-programming-for-beginners-image_rsrc1ZG.jpg)

图 40. LLM 代理推理和采取行动

代理在得到最终答案之前将执行几个动作：

![10 个代理完成](img/langchain-programming-for-beginners-image_rsrc1ZH.jpg)

图 41. LLM 代理完成

现在这些输出被显示出来，因为我们使用了 verbose 参数。

你可以通过调用 stream()方法而不是 invoke()来显示代理采取的步骤，然后检查返回的响应中的特定键：

# 关闭 verbose 以避免污染命令行

agent_executor = AgentExecutor(agent=agent, tools=tools)

question = input("给我一个任务：")

# 用 stream()代替 invoke()

response = agent_executor.stream({"input": question})

# 代理动作

if "actions" in response:

for action in response["actions"]:

打印(f"调用工具: `{action.tool}`，输入 `{action.tool_input}`")

# 观察

elif "steps" in response:

for step in response["steps"]:

print(f"工具结果: `{step.observation}`")

# 最终结果

elif "output" in response:

print(f'最终输出: {response["output"]}')

else:

raise ValueError()

print("---")

现在如果你再次运行代理，你将只会看到动作、步骤和最终输出。以下为了简洁省略了摘要：

给我一项任务：谁是美国的第一个总统？

调用工具: `wikipedia`，输入 `first president of the United States`

---

工具结果：`Page: George Washington

摘要：...

页面：美国总统

摘要：...

---

调用工具: `wikipedia`，输入 `first president of the United States`

---

工具结果：`Page: George Washington

摘要：...

页面：美国总统

摘要：...

---

最终输出：乔治·华盛顿是美国的第一任总统。

---

如果你使用另一个模型如 GPT-4o，你可能会直接得到最终输出：

给我一项任务：谁是美国的第一个总统？

最终输出：美国的第一个总统是乔治·华盛顿。

---

这是因为 LLM 在其训练数据中已经有了答案，所以它决定直接回答。

## 为代理添加 Streamlit UI

现在代理正在运行，你可以添加 Streamlit UI 来提高用户体验。

你只需要添加一个 chat_input 来接受任务，然后按照以下方式编写问题和答案：

导入 streamlit 库作为 st

# ...其他代码

agent_executor = AgentExecutor(agent=agent, tools=tools, verbose=True)

st.title("AI Agent")

question = st.chat_input("给我一个任务：")

if question:

with st.chat_message("user"):

st.markdown(question)

with st.chat_message("assistant"):

for response in agent_executor.stream({"input": question}):

# 代理动作

if "actions" in response:

for action in response["actions"]:

st.write(f"调用工具: `{action.tool}`，输入 `{action.tool_input}`")

# 观察结果

elif "steps" in response:

for step in response["steps"]:

st.write(f"工具结果: `{step.observation}`")

# 最终结果

elif "output" in response:

st.write(f'最终输出: {response["output"]}')

else:

raise ValueError()

st.write("---")

因为输出是在 Streamlit UI 上写的，所以在开发时可以打开 AgentExecutor 的 verbose 参数。

使用 Streamlit 运行应用程序：

streamlit run app.py

你现在可以提出不同类型的问题，看看 LLM 是否可以使用可用的工具。

如果你问 '今天伦敦的天气怎么样？'，LLM 应该使用 DuckDuckGo 搜索来获取伦敦的最新天气信息：

![10 代理搜索](img/langchain-programming-for-beginners-image_rsrc1ZJ.jpg)

图 42. LLM 代理进行搜索

如果你问一个数学问题，例如 '将 5 的平方乘以 6 和 3 的和'，代理应该使用 llm-math 工具：

![10 代理数学](img/langchain-programming-for-beginners-image_rsrc1ZK.jpg)

图 43. LLM 代理进行数学计算

此外，AI 代理还可以使用许多工具来完成任务。

如果你问 '哈利·波特首次出版是在哪一年？加 2 到年份'，那么代理将执行以下步骤：

给我一个任务：哈利·波特首次出版是在哪一年？加 2 到年份

调用工具: `wikipedia`，输入 `哈利·波特出版日期`

---

工具结果：`页面: 哈利·波特与凤凰社`

摘要: ...

页面: 哈利·波特与魔法石

摘要: ...

页面: 哈利·波特与混血王子

摘要: ...

---

调用工具: `Calculator`，输入 `1997 + 2`

---

工具结果：`答案：1999`

---

最终输出: 1999.

这里，代理使用维基百科和 LLM-math 工具来完成工作。非常好！

## 可用 AI 工具列表

AI 代理只能使用你在创建代理时添加的工具。

LangChain 中可用的工具列表可以在 load_tools 模块中找到。

在导入 load_tools 行时，将光标放在 load_tools 内部并按 F12。

你也可以通过右键单击 load_tools 名称并从上下文菜单中选择 '转到定义' 来使用鼠标。

在 load_tools.py 文件中，搜索下面的 get_all_tool_names() 函数：

def get_all_tool_names() -> List[str]:

"""获取所有可能的工具名称。”

return (

list(_BASE_TOOLS)

+ list(_EXTRA_OPTIONAL_TOOLS)

+ list(_EXTRA_LLM_TOOLS)

+ list(_LLM_TOOLS)

+ list(DANGEROUS_TOOLS)

)

上面的 *_TOOLS 常量包含你可以使用的工具名称。

例如，DuckDuckGo 搜索可以在下面的 _EXTRA_OPTIONAL_TOOLS 中找到：

![10 可用工具](img/langchain-programming-for-beginners-image_rsrc1ZM.jpg)

图 44. LLM 代理可用工具

您还可以看到其他工具，如 Google 搜索和 Bing 搜索，但使用这些工具需要 API 密钥。

## AI 代理类型

目前已经识别出几种类型的 AI 代理，我们创建的代理被称为 ReAct（推理+行动）代理。

ReAct 代理是一种通用代理，还有更多专门的代理，如 XML 代理和 JSON 代理。

您可以在[`python.langchain.com/v0.1/docs/modules/agents/agent_types/`](https://python.langchain.com/v0.1/docs/modules/agents/agent_types/)了解更多关于不同代理类型的信息。

随着 LLM 和 LangChain 的改进，可能会创建新的代理类型，因此上述定义不一定总是相关。

## 摘要

本章的代码可在书籍源代码的 10_Agents_and_Tools 文件夹中找到。

尽管我们今天的世界中还没有自主的机器人助手（尚无），但我们已经可以看到 AI 代理的发展有一天可能会被用作 AI 机器人的大脑。

AI 代理是一项惊人的创新，展示了机器如何提出一系列动作以实现目标。

当您创建代理时，LLM 用作推理引擎，需要提出逻辑步骤以完成任务。

代理还可以使用各种工具来执行操作，例如浏览网页或解决数学方程式。

这些代理还可以执行使用多个工具的更复杂任务。

有时，经过良好训练的 LLM 可以直接从训练数据中回答，无需使用工具。

第十一章：在 LangChain 中与文档交互

最有趣的 AI 用例之一是“与文档聊天”功能，它使用户能够通过会话查询与文档进行交互。

通过简单地提问，用户可以快速找到相关信息，总结内容，并获得见解，而无需阅读和整理大量文本。

下面是创建“与文档聊天”应用程序所需过程的说明：

![11 chatdoc 过程](img/langchain-programming-for-beginners-image_rsrc1ZN.jpg)

图 45. 与文档应用程序的聊天过程

您首先需要将单个文档分割成块，以便有效地处理和索引文档。然后，这些块被转换为向量嵌入。

向量嵌入是表示各种类型信息的数字数组，包括文本、图像、音频等，通过以数值格式捕获其特征。

当您提出问题时，LangChain 会将查询转换为向量，然后在文档向量中搜索最相关的匹配项。

LangChain 随后将用户查询和相关的文本片段发送给 LLM，以便 LLM 可以根据给定的输入生成响应。

寻找相关文本信息并将其发送到 LLM 的过程也被称为检索增强生成，简称 RAG。

使用 LangChain 和 Streamlit，你可以创建一个应用程序，允许你上传一个文档并对其内容提出相关问题。

让我们开始吧。

## 获取文档

你将上传一个文档到应用程序并对其提问。你可以从 11_Chat_With_Document 文件夹中获取名为 ai-discussion.txt 的文本文件。

该文本文件包含一个关于人工智能对人类影响的故事。

因为它是虚构的，你可以确信 LLM 从文档中获取答案，而不是从其训练数据中获取。

## 安装 ChromaDB

要创建一个带有文档的聊天应用程序，你需要安装一个名为 ChromaDB 的包：

pip install chromadb == 0.4.18

ChromaDB 是我们将用于存储和查询向量数据的向量数据库。

## 构建带有文档的聊天应用程序

创建一个名为 rag_prompt.py 的新 Python 文件，然后按照以下方式导入用于带有文档的聊天应用程序所需的包：

从 decouple 导入 config

从 langchain_openai 导入 ChatOpenAI，OpenAIEmbeddings

从 langchain_core.prompts 导入 ChatPromptTemplate

# 新的包：

从 langchain_community.document_loaders 导入 TextLoader

从 langchain.text_splitter 导入 RecursiveCharacterTextSplitter

从 langchain_community.vectorstores 导入 Chroma

从 langchain.chains.combine_documents 导入 create_stuff_documents_chain

从 langchain.chains 导入 create_retrieval_chain

OpenAIEmbeddings 类用于访问 OpenAI 嵌入模型。

TextLoader 类用于加载文本文件，而 RecursiveCharacterTextSplitter 用于将文本分割成小块，以便更有效地由 LLM 处理。

Chroma 类用于创建向量数据库。create_retrieval_chain 方法检索文档并将其传递给 create_stuff_documents_chain，该链将文档传递给 LLM。

在导入包后，你可以像下面那样定义 llm：

OPENAI_KEY = config("OPENAI_KEY")

llm = ChatOpenAI(model="gpt-4o", api_key=OPENAI_KEY)

在 llm 之后，使用 TextLoader 加载文本，并按照以下方式传递文档的路径到 TextLoader：

loader = TextLoader("./ai-discussion.txt")

documents = loader.load()

在加载文档列表后，你需要创建文本分割器并将文档分割成块：

text_splitter = RecursiveCharacterTextSplitter(chunk_size=1000, chunk_overlap=200)

chunks = text_splitter.split_documents(documents)

要将文档块转换为向量，你需要使用一个嵌入模型。

OpenAI 提供了一个 API 端点，可以将文档转换为向量，LangChain 提供了 OpenAIEmbeddings 类，以便你可以轻松使用此嵌入。

在 chunks 变量下方添加以下代码：

embeddings = OpenAIEmbeddings(openai_api_key=OPENAI_KEY)

vector_store = Chroma.from_documents(chunks, embeddings)

retriever = vector_store.as_retriever()

Chroma.from_documents() 方法将块和嵌入数据发送到 Chroma 数据库。

然后，你需要调用 as_retriever()方法来创建一个检索器对象，该对象接受用户输入并返回文档的相关部分。

接下来，你需要创建要发送到 LLM 的提示：

system_prompt = (

"您是问答任务的助手。"

"使用以下检索到的上下文来回答"

"这个问题。如果你不知道答案，就说你"

"不知道。最多用三句话，并保持简洁。"

"回答要简洁。"

"\n\n"

"{context}"

)

prompt = ChatPromptTemplate.from_messages(

[

("system", system_prompt),

("human", "{input}"),

]

]

通过创建提示，你需要通过调用 create_stuff_documents_chain()函数来创建一个链，并像这样传递 llm 和 prompt：

question_answer_chain = create_stuff_documents_chain(llm, prompt)

这个 question_answer_chain 将处理填充提示模板并将提示发送到 LLM。

接下来，将 question_answer_chain 传递给 create_retrieval_chain()函数：

rag_chain = create_retrieval_chain(retriever, question_answer_chain)

上述 rag_chain 将输入传递给检索器，检索器返回链的相关文档部分。

链接的相关部分和输入随后传递给 question_answer_chain 以获取结果。

现在，你可以请求用户输入，然后使用该输入运行 invoke()方法：

question = input("Ask Your Question: ")

if question:

response = rag_chain.invoke({"input": question})

print(response["answer"])

当 LLM 返回答案时，你将答案打印到命令行。

现在应用程序已完成。您可以从命令行使用 Python 运行它：

python rag_prompt.py

然后提出与文档上下文相关的问题。以下是一个示例：

python3 rag_prompt.py

询问您的问题：汤普森先生在哪里工作？

汤普森先生在 VegaTech Inc.担任首席人工智能科学家。

如我们所见，LLM 可以通过分析 LangChain 和我们的输入创建的提示来回答问题。

## 将 Streamlit Chat UI 添加到应用程序中

当应用程序的核心功能完成时，我们可以添加 Web UI 和聊天记忆来改进应用程序。

首先添加 Web UI。将 Streamlit 导入到应用程序中，然后在 rag_chain 变量下方添加 Streamlit UI：

import streamlit as st

# ... 其他代码

rag_chain = create_retrieval_chain(retriever, question_answer_chain)

st.title("与文档聊天")

question = st.chat_input("Your Question: ")

if question:

with st.chat_message("user"):

st.markdown(question)

response = rag_chain.invoke({"input": question})

with st.chat_message("assistant"):

st.write(response["answer"])

现在你可以使用 streamlit run 命令运行应用程序。

下一步是将记忆部分添加到应用程序中。

## 添加上下文聊天记忆

当向 RAG 链添加聊天记忆时，你还需要通过创建一个历史感知检索器来升级检索器对象。

这个具有历史感知的检索器随后用于通过分析聊天历史来上下文化你最新的问题。

你需要导入 create_history_aware_retriever 链，然后按照以下方式创建一个 history_aware_retriever 对象：

from langchain.chains import create_history_aware_retriever

# ... 其他代码

retriever = vector_store.as_retriever()

contextualize_system_prompt = """Given a chat history and the latest user question \

这可能引用聊天历史中的上下文，形成一个独立的问题

这可以在没有聊天历史的情况下理解。**不要回答问题**，

如果需要，重新表述它，否则按原样返回。”

contextualize_prompt = ChatPromptTemplate.from_messages(

[

("system", contextualize_system_prompt),

MessagesPlaceholder("chat_history"),

("human", "{input}"),

]

)

history_aware_retriever = create_history_aware_retriever(

llm, retriever, contextualize_prompt

)

在创建 history_aware_retriever 对象后，你需要更新 rag_chain 以使用检索器，如下所示：

rag_chain = create_retrieval_chain(history_aware_retriever, question_answer_chain)

现在你已经更新了 RAG 链，像第九章中那样将链传递给 RunnableWithMessageHistory() 类：

# 添加导入

from langchain_community.chat_message_histories import StreamlitChatMessageHistory

from langchain_core.runnables.history import RunnableWithMessageHistory

# ... 其他代码

rag_chain = create_retrieval_chain(history_aware_retriever, question_answer_chain)

history = StreamlitChatMessageHistory()

conversational_rag_chain = RunnableWithMessageHistory(

rag_chain,

lambda session_id: history,

input_messages_key="input",

history_messages_key="chat_history",

output_messages_key="answer",

)

要向用户显示聊天历史，像以前一样在 st.session_state 中查找消息对象：

st.title("与文档聊天")

for message in st.session_state["langchain_messages"]:

role = "user" if message.type == "human" else "assistant"

with st.chat_message(role):

st.markdown(message.content)

作为最后一步，更改应用程序接收到问题时调用的链，并添加 "session_id" 的配置参数：

if question:

with st.chat_message("user"):

st.markdown(question)

response = conversational_rag_chain.stream(

{"input": question}, config={"configurable": {"session_id": "any"}}

)

with st.chat_message("assistant"):

st.write(response["answer"])

好的。现在我们有一个很好的界面来与文档进行交互，AI 也知道聊天历史。

## 流式传输答案

到目前为止，我们仍然使用 invoke() 方法来运行链。让我们尝试流式传输 AI 答案：

with st.chat_message("user"):

st.markdown(question)

response = conversational_rag_chain.stream(

{"input": question}, config={"configurable": {"session_id": "any"}}

)

with st.chat_message("assistant"):

st.write_stream(response)

如果你运行应用程序并将问题传递给 LLM，你会注意到响应是一个包含四个键的字典："input"，"chat_history"，"context" 和 "answer"。

![11 流响应](img/langchain-programming-for-beginners-image_rsrc1ZP.jpg)

图 46. RAG 链的流响应

如果你决定只写入 "answer" 键，你将得到一个来自 Python 的 'generator' 对象不可索引的 TypeError：

st.write_stream(response["answer"]) # TypeError

如果你只想将答案流式传输给用户，你需要调用 pick() 方法并传递 "answer" 键，如下所示：

answer_chain = conversational_rag_chain.pick("answer")

response = answer_chain.stream(

{"input": question}, config={"configurable": {"session_id": "any"}}

)

The pick() 方法过滤返回的输出，并且只返回你传递为其参数的键的内容。

这样，响应对象现在是一个只返回答案的流：

![11 聊天输出](img/langchain-programming-for-beginners-image_rsrc1ZR.jpg)

图 47. 使用 pick() 控制 RAG 链响应

## 切换 LLM

如果你想要更改此应用程序使用的 LLM，你还需要更改用于向量生成的嵌入模型。

对于 Google Gemini，你可以按照以下方式导入 GoogleGenerativeAIEmbeddings 模型：

from langchain_google_genai import ChatGoogleGenerativeAI, GoogleGenerativeAIEmbeddings

# llm GOOGLE_GEMINI_KEY = config("GOOGLE_GEMINI_KEY")

llm = ChatGoogleGenerativeAI(

model="gemini-1.5-pro-latest", google_api_key=GOOGLE_GEMINI_KEY

)

# embeddings embeddings = GoogleGenerativeAIEmbeddings(

google_api_key=GOOGLE_GEMINI_KEY, model="models/embedding-001"

)

对于 Ollama，你可以像这样使用社区开发的 OllamaEmbeddings 类：

from langchain_community.chat_models import ChatOllama

from langchain_community.embeddings import OllamaEmbeddings

# llm

llm = ChatOllama(model="mistral")

# embeddings

embeddings = OllamaEmbeddings(model="mistral")

确保在实例化 ChatOllama 和 OllamaEmbeddings 类时使用相同的模型。

## 摘要

本章的代码可在书籍源代码的 11_Chat_With_Document 文件夹中找到。

在本章中，你学习了如何使用 LangChain 创建一个与文档聊天的应用程序。

使用 RAG 技术，LangChain 可以从文档中检索信息，然后将信息传递给 LLM。

首先你需要做的是处理文档并将其转换为块，然后可以使用嵌入模型将这些块转换为向量。

这些向量存储在 ChromaDB 中，当用户发送查询或输入时，使用从数据库创建的检索器。

一旦核心功能完成，你可以轻松地使用 Streamlit 添加一个网络界面和聊天记忆到应用程序中。

接下来，让我们看看如何加载不同格式的文档，例如 .docx 和 .pdf。

第十二章：上传不同类型的文档

现在我们可以在 LangChain 中加载和交互 .txt 文档，让我们改进应用程序，以便我们还可以加载其他文档类型或格式，如 .docx 和 .pdf。

要加载不同类型的文档，您需要在 Streamlit 中创建一个文件上传界面。

在 Streamlit 标题下方，添加以下新代码：

st.title("询问文档")

uploaded_file = st.file_uploader("上传您的文档：", type=["pdf", "docx", "txt"])

add_file = st.button("提交文件", on_click=clear_history)

if uploaded_file and add_file:

process_file(uploaded_file)

st.file_uploader() 方法创建了一个文件上传输入，然后我们添加了一个按钮来提交文件。

当点击提交按钮时，将执行 clear_history() 方法，因此您需要定义该方法：

def clear_history():

if "langchain_messages" in st.session_state:

del st.session_state["langchain_messages"]

在 clear_history() 函数上方，创建一个名为 process_file() 的新函数来处理上传的文件。

此函数需要检查文档的扩展名以使用正确的加载器：

def process_file(file):

with st.spinner("文件正在处理中..."):

data = file.read()

file_name = os.path.join("./", file.name)

with open(file_name, "wb") as f:

f.write(data)

name, extension = os.path.splitext(file_name)

if extension == ".pdf":

from langchain_community.document_loaders import PyPDFLoader

loader = PyPDFLoader(file_name)

elif extension == ".docx":

from langchain_community.document_loaders import Docx2txtLoader

loader = Docx2txtLoader(file_name)

elif extension == ".txt":

from langchain_community.document_loaders import TextLoader

loader = TextLoader(file_name)

else:

st.error("此格式不受支持！")

LangChain 加载器简单地使用 Python 包加载相应的文档。

您需要安装加载器使用的 PyPDF 和 Docx2txt 包：

pip install pypdf == 4.2.0 docx2txt == 0.8

一旦创建加载器，您就可以加载并将文档分割成块，将块转换为向量，并像以前一样创建链：

docs = loader.load()

text_splitter = RecursiveCharacterTextSplitter(

chunk_size=1000, chunk_overlap=200

)

chunks = text_splitter.split_documents(docs)

embeddings = OpenAIEmbeddings(openai_api_key=OPENAI_KEY)

vector_store = Chroma.from_documents(chunks, embeddings)

retriever = vector_store.as_retriever()

history_aware_retriever = create_history_aware_retriever(

llm, retriever, contextualize_prompt

)

rag_chain = create_retrieval_chain(

history_aware_retriever, question_answer_chain

)

conversational_rag_chain = RunnableWithMessageHistory(

rag_chain,

lambda session_id: history,

input_messages_key="input",

history_messages_key="chat_history",

output_messages_key="answer",

)

要使 conversational_rag_chain 可在外部函数中使用，我们需要通过将其保存在 Streamlit 会话状态中来实现持久化。

我们还显示一条消息，说明文件已成功上传并嵌入：

st.session_state.crc = conversational_rag_chain

st.success("文件上传并嵌入成功")

当用户提出问题，你可以检查 crc 是否在 st.session_state 中，并使用它。

同时，别忘了调用 crc 链的 pick()方法来流式传输答案：

if question:

with st.chat_message("user"):

st.markdown(question)

if "crc" in st.session_state:

crc = st.session_state["crc"]

answer_chain = crc.pick("answer")

response = answer_chain.stream(

{"input": question}, config={"configurable": {"session_id": "any"}}

)

with st.chat_message("assistant"):

st.write_stream(response)

else:

st.error("未上传文档。请先上传文档")

在这里，我们还添加了一个 else 语句，以通知用户尚未上传文档。

就这样。现在你可以上传一个.txt、.docx 或.pdf 文档，并就文档内容提出相关问题。

如果你上传其他类型的文档，Python 将显示“不支持的文档格式”错误。做得好！

## 摘要

本章的代码可在书籍源代码的 12_Uploading_Different_Document_Types 文件夹中找到。

在本章中，你通过创建一个上传文件的界面进一步改进了 Chat With Document 应用程序，然后根据文档类型使用不同的加载器加载文档。

在下一章中，我将向你展示如何与 YouTube 视频聊天。那里见！

第十三章：与 YouTube 视频聊天

现在你已经学会了如何让 AI 与文档交互，让我们继续创建一个 Chat with YouTube 应用程序。

要创建此应用程序，你可以从第十二章复制完成的程序，并根据本章所示进行更改。

让我们开始吧！

## 添加 YouTube 加载器

Chat With YouTube 应用程序使用 RAG 技术通过视频的文本数据增强 LLM。

要获取 YouTube 视频的文本，你需要使用 pip 安装 youtube-transcript-api 包，如下所示：

pip install youtube-transcript-api==0.6.2

此 API 由 LangChain 的 YouTube 加载器用于获取视频的文本。

在文件顶部，从 LangChain 导入 YoutubeLoader 类，如下所示：

from langchain_community.document_loaders import YoutubeLoader

在 Streamlit 标题下方，创建一个 Streamlit 文本输入来替换文件上传器，如下所示：

youtube_url = st.text_input("输入 YouTube URL")

if youtube_url:

process_youtube_url(youtube_url)

接下来，创建 process_youtube_url()函数，该函数替换 process_file()函数。

而不是导入不同的加载器来加载文档，你可以使用 YoutubeLoader 从 YouTube URL 创建文档，如下所示：

def process_youtube_url(url):

with st.spinner("处理 YouTube 视频..."):

loader = YoutubeLoader.from_youtube_url(url)

docs = loader.load()

text_splitter = RecursiveCharacterTextSplitter(

chunk_size=1000, chunk_overlap=200

)

#... 函数其余部分

#...

st.success("视频处理完成。提出您的问题")

YoutubeLoader.from_youtube_url()方法将获取 YouTube 视频的文本记录作为文档，然后您可以使用 text_splitter 对象将其拆分为块。

函数的其余代码与之前相同，只是在创建 rag_chain 时，我们显示了'视频处理'成功消息。

现在运行应用程序，使用 streamlit run，传递 URL，并询问与 YouTube 视频内容相关的相关问题。

例如，我传递了视频的 URL 到[`youtu.be/Sr4KeW078P4`](https://youtu.be/Sr4KeW078P4)，该 URL 解释了 JavaScript Promise 语法：

![13 询问 YouTube 结果](img/langchain-programming-for-beginners-image_rsrc1ZS.jpg)

图 48. 询问 YouTube 应用程序结果

您可以传递 YouTube 短链接或完整链接。它将按上述方式工作。

## 处理不存在文本记录错误

由于 YouTube 音乐视频没有文本记录，当您将其提供给应用程序时，您会得到一个错误：

ValueError: 预期 ID 列表非空，但得到 []

这个错误发生是因为 YoutubeLoader 加载了一个空的文档列表，因此这个空列表被传递到 Chroma.from_documents()方法中。

为了防止此错误，在运行进一步处理之前，您需要检查 docs 变量是否不为空：

if docs:

text_splitter = RecursiveCharacterTextSplitter(

chunk_size=1000, chunk_overlap=200

)

chunks = text_splitter.split_documents(docs)

# ...

st.session_state.crc = conversational_rag_chain

st.success("视频处理完成。提出您的问题")

else:

st.error("视频没有文本记录。请尝试另一个视频")

这样，当视频没有文本记录时，会显示错误消息，而 ChromaDB 不会抛出错误：

![13 无文本记录](img/langchain-programming-for-beginners-image_rsrc1ZT.jpg)

图 49. 未检测到文本记录

没有文本记录，我们无法生成向量数据。

## 摘要

本章的代码可在书籍源代码的 13_Chat_With_Youtube 文件夹中找到。

在本章中，你学习了如何创建一个使用 URL 获取 YouTube 视频文本记录的 Chat With YouTube 应用程序，然后将文本记录转换为向量，这些向量可以用来增强 LLM 的知识。

通过使用 AI，您可以在不观看视频的情况下请求长视频的关键点或摘要。

第十四章：使用多模态消息与图像交互

现在我们能够加载不同类型的文档，让我们继续制作让 AI 理解图像。

## 理解多模态消息

多模态消息是使用多种通信模式进行交流的消息。

人类已知的信息交流模式有：

|  | 文本 |
| --- | --- |
|  | 视频 |
|  | 音频 |
|  | 图像 |

高级模型如 GPT-4 和 Gemini Pro 已经具备视觉能力，这意味着模型可以“看到”图像并回答有关它们的问题。

通过发送多模态消息，我们可以使用 AI 与图像交互，例如询问图像中有多少人或图像中的主导颜色是什么。

让我们学习如何使用 LangChain 创建这样的应用程序。

## 在 LangChain 中发送多模态消息

要在 LangChain 中发送多模态消息，您只需调整提示模板，并将人类消息传递为一个列表而不是一个字符串。

首先，创建一个名为 handle_image.py 的新文件，导入所需的包，并定义要使用的 LLM，如下所示：

from decouple import config

from langchain_openai import ChatOpenAI

from langchain_core.prompts import ChatPromptTemplate

import base64

OPENAI_KEY = config("OPENAI_KEY")

llm = ChatOpenAI(model="gpt-4o", api_key=OPENAI_KEY)

将使用 base64 模块以 base 64 格式编码图片。

在 llm 变量下方编写编码图片的函数：

def encode_image(image_path):

with open(image_path, "rb") as image_file:

return base64.b64encode(image_file.read()).decode("utf-8")

image = encode_image("./image-1.jpg")

您可以将您电脑上的任何图片传递给 encode_image() 函数。只需确保图片中不包含任何敏感数据。

编码后的图片可以按如下方式传递到聊天提示模板中：

prompt = ChatPromptTemplate.from_messages(

[

("system", "您是一个能够详细描述图片的有用助手。"),

(

"human",

[

{"type": "text", "text": "{input}"},

{

"type": "image_url",

"image_url": {

"url": f"data:image/jpeg;base64,{image}",

"detail": "low",

},

},

],

),

]

)

在上面的模板中，您可以看到有两个消息作为人类消息传递：问题的 "text" 和图片的 "image_url"。

我们可以传递一个公开的图片 URL，例如 'https://'，但在这里我们使用 data:image URI，因为我们是从电脑上传图片。

在幕后，LangChain 自动将消息转换为多模态消息。

从提示和 llm 创建链，并请求用户输入：

chain = prompt | llm

response = chain.invoke({"input": "在这张图片上您看到了什么？"})

print(response.content)

LLM 将处理图片，然后给出适当的答案。

## 添加 UI 和聊天历史

现在您可以使用语言模型对图片提出问题，让我们通过添加网页界面和聊天历史来改进应用程序。

如往常一样，首先导入添加网页界面和历史的所需包：

from decouple import config

from langchain_openai import ChatOpenAI

import streamlit as st

# 添加来自 langchain_core.prompts 的历史记录

from langchain_community.chat_message_histories import StreamlitChatMessageHistory

from langchain_core.runnables.history import RunnableWithMessageHistory

import os, base64

接下来，您需要实例化 Streamlit 聊天历史并升级链以包括聊天历史，类似于第九章。

您还需要创建一个 process_image() 函数，该函数将编码图片并将其存储在会话状态中：

history = StreamlitChatMessageHistory()

chain = prompt | llm

chain_with_history = RunnableWithMessageHistory(

chain,

lambda session_id: history,

input_messages_key="input",

history_messages_key="chat_history",

)

def process_image(file):

with st.spinner("处理图像..."):

data = file.read()

file_name = os.path.join("./", file.name)

with open(file_name, "wb") as f:

f.write(data)

image = encode_image(file_name)

st.session_state.encoded_image = image

st.success("图像已编码。提出你的问题")

下一步是创建一个清除聊天历史的函数，然后使用 Streamlit 创建一个文件上传器。

当上传图像时，使用 process_image()函数处理该图像：

def clear_history():

if "langchain_messages" in st.session_state:

del st.session_state["langchain_messages"]

st.title("与图像聊天")

uploaded_file = st.file_uploader("上传你的图像: ", type=["jpg", "png"])

add_file = st.button("提交图像", on_click=clear_history)

if uploaded_file and add_file:

process_image(uploaded_file)

在将图像编码并保存在会话状态后，你只需要显示聊天历史，创建聊天输入，并运行 chain_with_history.stream()方法以流式传输答案。

这部分与之前的应用类似：

for message in st.session_state["langchain_messages"]:

role = "user" if message.type == "human" else "assistant"

with st.chat_message(role):

st.markdown(message.content)

question = st.chat_input("你的问题")

if question:

with st.chat_message("user"):

st.markdown(question)

if "encoded_image" in st.session_state:

image = st.session_state["encoded_image"]

response = chain_with_history.stream(

{"input": question, "image": image},

config={"configurable": {"session_id": "any"}},

)

with st.chat_message("assistant"):

st.write_stream(response)

else:

st.error("未上传图像。请先上传图像。")

当没有图像时，显示错误消息“未上传图像。请先上传图像。”

现在运行应用程序，使用 streamlit run 命令，你可以询问关于你上传的图像的问题。

我在下面的示例中使用了一个来自[`g.codewithnathan.com/lc-image`](https://g.codewithnathan.com/lc-image)的图像：

![14 聊天图像](img/langchain-programming-for-beginners-image_rsrc1ZU.jpg)

图 50. 与图像聊天结果

尝试询问一些特定细节，例如图像中可以看到多少人，或者图像中哪种颜色占主导地位。

## Ollama 多模态消息

如果你想向 Ollama 发送多模态消息，你需要下载一个支持该消息格式的模型，例如 bakllava 和 llava。

你可以运行命令 ollama pull bakllava 将模型下载到你的机器上。请注意，这两个模型都需要 8GB 的 RAM 才能正常运行，没有任何问题。

要向 Ollama 发送多模态消息，你需要确保 image_url 键包含以下字符串值：

{

"type": "image_url",

"image_url": f"data:image/jpeg;base64,""{image}",

},

但再次强调，LangChain 端存在一个错误，将 image_url 键转换为字典，并在该字典中添加一个 url 键。

我已经将此问题报告给了 LangChain 维护者，[`github.com/langchain-ai/langchain/issues/22460`](https://github.com/langchain-ai/langchain/issues/22460)

您需要打开 ollama.py 源代码，并将第 123 行的代码修改如下：

if isinstance(content_part.get("image_url")["url"], str):

image_url_components = content_part["image_url"]["url"].split(",")

一旦问题得到解决，我将更新本节。

## 摘要

本章的代码可在书籍源代码的 14_Handling_Images 文件夹中找到。

在本章中，您已经学习了如何使用 LangChain 向语言模型发送多模态消息。

注意，并非所有模型都能理解多模态消息。如果您使用 Ollama，则需要使用 bakllava 这样的模型，而不是 mistral 或 gemma。

如果 LLM 不理解，它通常会告诉您它无法理解您发送的消息。

第十五章：将 AI 应用程序部署到生产环境

现在您已经创建了各种 AI 驱动的应用程序，是时候学习如何将其部署到互联网上，以便其他人可以使用它。

在本章中，我们将学习如何部署使用 Google Gemini 和 OpenAI GPT 的应用程序。

注意，我们不会探讨如何部署由 Ollama 驱动的应用程序，因为我们需要自行托管 Ollama 以正确运行应用程序。

由于我们使用 Streamlit 创建了应用程序，部署应用程序的一种方法是在 Streamlit Cloud Community 上启动它。

请记住，由于 Streamlit Cloud Community 是免费的，当您的应用程序处于非活动状态时，可能会被暂停以节省服务器资源。

## 在 Streamlit 中创建侧边栏

在部署应用程序之前，我们需要对其进行一些小的修改。

注意，您创建的应用程序都使用您自己的 API 密钥来访问 LLM 提供商的 API。

这不建议用于生产，因为每次用户使用您的应用程序时，您都会被收费。

而不是提供您的 API 密钥供使用，您需要启用用户添加他们自己的 API 密钥。

在 Streamlit 中，这很简单，因为您只需要在侧边栏中创建一个用于 API 密钥的文本输入。

在我们的应用程序中，在实例化 llm 对象之前创建一个侧边栏，如下所示：

st.title("Ask YouTube Video")

with st.sidebar:

st.title("Add Your API Key First")

openai_key = st.text_input("OpenAI API Key", type="password")

if not openai_key:

st.info("Enter your OpenAI API Key to continue")

st.stop()

llm = ChatOpenAI(model="gpt-4o", api_key=openai_key)

在上面的代码中，我们使用 with st.sidebar 语法创建了一个侧边栏，然后向侧边栏添加了标题和文本输入元素。

当 openai_key 变量为空时，我们运行 st.info() 方法向用户显示指令，然后调用 st.stop() 方法，这样 Streamlit 就会停止执行您的 Python 代码。

这样，在添加 API 密钥之前，界面的其余部分都不会显示：

![15 默认界面](img/langchain-programming-for-beginners-image_rsrc1ZV.jpg)

图 51. Streamlit 请求 API 密钥

添加了 API 密钥后，其余的界面将显示出来：

![15 api key added](img/langchain-programming-for-beginners-image_rsrc1ZW.jpg)

图 52\. 添加 API 密钥时显示的 Streamlit UI

好的，现在你可以删除 from decouple import config 这一行，因为它不再需要了。

## 在项目文件夹中添加 requirements.txt 文件

下一步是将 requirements.txt 文件包含在项目文件夹中。

此文件将由 Streamlit 用于安装运行应用程序所需的依赖项。

这是 requirements.txt 文件的内容：

langchain == 0.2.1

langchain_community==0.2.1

langchain_core==0.2.3

langchain-openai==0.1.7

streamlit==1.35.0

chromadb==0.4.18

youtube-transcript-api==0.6.2

注意，langchain_community 和 langchain_core 包也包含在上面的 .txt 文件中。

Streamlit Cloud 使用 uv 而不是 pip 来安装包，uv 在你安装 langchain 时不会自动安装额外的包，因此你需要指定它们。

## 创建 GitHub 仓库

部署 Streamlit 应用程序需要你将代码上传到 GitHub。GitHub 是一个你可以用来托管和分享你的软件项目的平台。

前往 [`github.com`](https://github.com) 并登录或注册一个新账户（如果你还没有的话）。

从仪表板，通过点击左侧侧边栏的“+ 新建”或导航栏右侧的“+”号来创建一个新的仓库：

![15 github new repository](img/langchain-programming-for-beginners-image_rsrc1ZX.jpg)

图 53\. 在 GitHub 中创建仓库的两种方式

仓库（或 repo）是一个用于存储软件项目文件的存储空间。

在“创建仓库”页面，填写你项目的详细信息。唯一必需的详细信息是仓库名称：

![15 lc yt repo](img/langchain-programming-for-beginners-image_rsrc1ZY.jpg)

图 54\. 创建 GitHub 仓库

如果你希望这个项目成为你作品集的一部分，你可以将其设为公开，或者你可以将其设为私有。

一旦创建了一个新的仓库，你将收到如何将文件推送到仓库中的说明。

你需要遵循推送现有仓库的说明：

![15 git push instructions](img/langchain-programming-for-beginners-image_rsrc1ZZ.jpg)

图 55\. Git 推送说明

现在，你需要为你的项目创建一个仓库。在项目文件夹中打开命令行，然后运行 git init 命令：

git init

这将使你的项目成为一个本地仓库。通过运行 git add . 命令将所有项目文件添加到这个本地仓库中：

git add .

添加到仓库中的更改在你运行 git commit 命令之前不会是永久的。按照以下方式提交更改：

git commit -m 'Ready for Deployment'

-m 选项用于为提交添加消息。通常，你将提交到仓库中的更改总结为消息。

现在，你需要将这个现有仓库推送到 GitHub。你可以通过遵循 GitHub 指示来完成此操作：

git remote add origin <URL>

git branch -M main

git push -u origin main

当运行 git push 命令时，你可能需要输入你的 GitHub 用户名和密码。

推送完成后，在浏览器中刷新 GitHub 仓库页面，您应该在那里看到您的项目文件和文件夹。

这意味着我们的应用程序已经推送到 GitHub 上托管的远程仓库。

我们将要部署应用程序的远程服务器可以从这个仓库获取代码。

您可以在我的 GitHub 仓库[`github.com/nathansebhastian/langchain-ask-youtube`](https://github.com/nathansebhastian/langchain-ask-youtube)查看。

## 部署到 Streamlit

应用程序现在已准备好部署。有两种方法可以将应用程序部署到 Streamlit：

1.  从 Streamlit 网站[`share.streamlit.io`](https://share.streamlit.io)

1.  使用 streamlit run 命令从本地主机

我将向您展示第一种方法，然后继续介绍第二种方法。

您需要访问 Streamlit 的社区云[`share.streamlit.io`](https://share.streamlit.io)并注册一个账户：

![15 streamlit share page](img/langchain-programming-for-beginners-image_rsrc200.jpg)

图 56. Streamlit 分享主页

创建账户后，您将被引导到一个工作空间。点击右上角的“创建应用程序”链接：

![15 st create app](img/langchain-programming-for-beginners-image_rsrc201.jpg)

图 57. Streamlit “创建应用程序”链接

Streamlit 将要求连接到 GitHub。点击下面的“连接到 GitHub”按钮：

![15 st connect gh](img/langchain-programming-for-beginners-image_rsrc202.jpg)

图 58. Streamlit 连接到 GitHub

然后，授权 Streamlit 访问您的 GitHub 仓库。

在下一屏幕上，选择“我有应用程序”如下所示：

![15 st gh](img/langchain-programming-for-beginners-image_rsrc203.jpg)

图 59. Streamlit 部署现有应用程序

接下来，您需要在部署页面填写您应用程序的详细信息。

添加您在上一节中创建的代码仓库，然后设置分支、主文件路径和应用程序 URL。

您可以自定义应用程序 URL 以使其更短。以下是我的输入作为参考：

![15 st deploy page](img/langchain-programming-for-beginners-image_rsrc204.jpg)

图 60. Streamlit 部署页面

完成后，点击“部署”，以便 Streamlit 从 GitHub 获取代码并将其部署到他们的社区云服务器。

完成后，您可以通过生成的 streamlit.app URL 访问应用程序。

您可以在[`nsebhastian-lc-ask-youtube.streamlit.app`](https://nsebhastian-lc-ask-youtube.streamlit.app)查看我的部署。

您可以通过运行 streamlit run 命令在本地主机上运行应用程序，然后点击右上角的“部署”链接来将应用程序部署到 Streamlit 云：

![15 streamlit run deploy](img/langchain-programming-for-beginners-image_rsrc205.jpg)

图 61. Streamlit 从本地主机部署

从那里，选择 Streamlit Cloud Community 以免费部署：

![15 streamlit cc](img/langchain-programming-for-beginners-image_rsrc206.jpg)

图 62. Streamlit Select Cloud Community

如果您已将项目上传到 GitHub 仓库，您将被带到相同的部署页面。完成后，点击“部署”按钮。

## 摘要

本章中的代码更改可以在之前链接的[`github.com/nathansebhastian/langchain-ask-youtube`](https://github.com/nathansebhastian/langchain-ask-youtube)找到。

你已经成功将 Streamlit 应用程序部署到互联网上。现在你可以与大家分享你的辛勤工作了。做得好！

正如你所见，部署一个 AI 应用程序与部署一个常规网络应用程序并没有太大的区别。

由于 AI 模型可以通过 HTTP 协议访问，你只需要确保将访问模型的 API 密钥添加到应用程序中。

而不是提供自己的密钥并承担运行模型产生的费用，你可以要求用户为自己提供密钥以供个人使用。

总结

恭喜你完成这本书！我们一起探讨了众多概念和主题，帮助你学习如何使用 LangChain、Streamlit、GPT、Gemini 和 Ollama 开发 AI 应用程序。

你也已经学会了如何将应用程序部署到 Streamlit Cloud Community，以便可以从互联网上访问。

我希望你喜欢用这本书学习并探索 LangChain，就像我喜欢写这本书一样。

我想请你帮个小忙。

如果你喜欢这本书，请在亚马逊上留下一个诚实的评价（我会阅读所有向我而来的评价）

每一条评价都很重要，你的支持意义重大。

再次感谢您的慷慨支持！

待到下次再会，

Nathan

关于作者

Nathan Sebhastian 是一位拥有 8 年以上经验的资深软件开发者，专注于开发和构建网络和移动应用程序。

他热衷于让每个人都能获得技术教育，并且自 2018 年以来一直在网上授课。

LangChain 编程入门

使用 LangChain、Python、OpenAI/ChatGPT、Google/Gemini 和其他 LLMs 开发 AI 应用程序的逐步指南

By Nathan Sebhastian

[`codewithnathan.com`](https://codewithnathan.com)

版权所有 © 2024 Nathan Sebhastian

所有权利保留。

本书任何部分不得以任何形式或任何手段（包括但不限于电子、机械、影印、录音或其他方式）进行复制、存储或传输，除非获得作者明确的书面许可。
