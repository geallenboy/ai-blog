https://medium.com/@jiamigou/deepseek-r1-%E6%9C%AC%E5%9C%B0%E5%AE%89%E8%A3%85%E9%83%A8%E7%BD%B2-%E4%BF%9D%E5%A7%86%E7%BA%A7%E6%95%99%E7%A8%8B-%E8%B6%85%E7%AE%80%E5%8D%95-fac9cee4e334
# DeepSeek R1 本地部署教程

## 1.为什么要本地运行

在本地运行 AI 模型具有以下优势：
🔸隐私：你的数据保留在你的机器上 — — 不存在共享敏感信息的风险；
🔸成本： DeepSeek R1 可免费使用，无需订阅费或使用费；
🔸控制：无需外部依赖即可进行微调和实验。

## 2.安装步骤

### 步骤1 

步骤1、安装Ollama
为了在本地运行 DeepSeek R1，我们将使用Ollama，这是一种专门为用户在自己的电脑上运行 AI 模型而设计的工具。
Ollama官网：https://ollama.com/download

### 骤二、拉取 DeepSeek R1 模型

Ollama 支持 DeepSeek R1 的多个版本。模型越大越智能，但所需的 GPU 也越大。

具体有以下版本：

🔹1.5B（最小）
🔹8B
🔹14B
🔹32B
🔹70B（最大、最智能）

运行 1.5B或者7B 模型

🔹首先，打开你的终端：
▪️MAC使用 command + space（空格），输入terminal 打开终端；
▪️WIN使用Win + R，在运行对话框中输入“cmd”；或者Win + X，选择“Windows PowerShell”或“命令提示符”来打开终端窗口。

运行以下指令：ollama run deepseek-r1:1.5b
如果报错，可以使用以下指令：ollama run deepseek-r1

使用以上任何指令后，系统会自动下载。

下载速度，看网速，我的网速不好，等了20分钟左右。

完成下载后，模型即可运行。

### 步骤 3、安装聊天框

上面不住完成，说明你已经在自己电脑部署好了DeepSeek，可以通过终端与 DeepSeek R1 进行交互，但如果想要一个更流畅的交互体验，可以使用 GUI。

一般使用Chatbox与本地模型集成，这是一个免费且注重隐私的桌面客户端。

下载 Chatbox，官网：https://chatboxai.app/en# （有中文版）


安装完成后，在选择配置API模型那里选择“Ollama API”；（图1）
🔸将 API 主机设置为：http://127.0.0.1:11434（图二）
🔸选择 DeepSeek R1 作为活动模型
🔸保存