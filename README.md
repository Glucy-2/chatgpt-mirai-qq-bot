![cover](https://user-images.githubusercontent.com/117586514/230783378-34ddb86a-c8d3-47a6-baa5-86e39200b258.png)

------------------------------------
<p align="center">
  <h2 align="center">ChatGPT for Bot</h2>
  <p align="center">
    一款支持各种主流语言模型的聊天的机器人！
    <br/>
    <br/>
    <a href="https://chatgpt-qq.lss233.com/"><strong>» 查看使用教程 »</strong></a>
    <br/>
  </p>
</p>

<p align="center">
  <a href="https://github.com/lss233/chatgpt-mirai-qq-bot/stargazers"><img src="https://img.shields.io/github/stars/lss233/chatgpt-mirai-qq-bot?color=pink&amp;logo=github&amp;style=for-the-badge" alt="Github stars"></a>
  <a href="https://github.com/lss233/chatgpt-mirai-qq-bot/actions/workflows/docker-latest.yml"><img src="https://img.shields.io/github/actions/workflow/status/lss233/chatgpt-mirai-qq-bot/docker-latest.yml?color=green&amp;logo=docker&amp;logoColor=white&amp;style=for-the-badge" alt="Docker build latest"></a>
  <a href="https://hub.docker.com/r/lss233/chatgpt-mirai-qq-bot/"><img src="https://img.shields.io/docker/pulls/lss233/chatgpt-mirai-qq-bot?color=gold&amp;logo=docker&amp;logoColor=white&amp;style=for-the-badge" alt="Docker Pulls"></a>
  <a href="./LICENSE"><img src="https://img.shields.io/github/license/lss233/chatgpt-mirai-qq-bot?&amp;color=skyblue&amp;style=for-the-badge" alt="License"></a>
</p>

***

* [交流群（Discord）](https://discord.gg/cc3S2R6RQV)会发布最新的项目动态、问题答疑和交流 [QQ 群](https://jq.qq.com/?_wv=1027&k=XbGuxdTu) 。  
  加群之前先看[这里](https://github.com/lss233/chatgpt-mirai-qq-bot/issues)的内容能不能解决你的问题。  
  如果不能解决，把遇到的问题、**日志**和配置文件准备好后再提问。
* [调试群](https://jq.qq.com/?_wv=1027&k=TBX8Saq7) 这个群里有很多 ChatGPT QQ 机器人，不解答技术问题。 

| ![猫娘问答](https://img.shields.io/badge/-%E7%8C%AB%E5%A8%98%E9%97%AE%E7%AD%94-pink?style=for-the-badge)                     | ![生活助手](https://img.shields.io/badge/-生活助手-orange?style=for-the-badge)                   | ![文字 RPG](https://img.shields.io/badge/-文字RPG-skyblue?style=for-the-badge)            |
|------------------------------|------------------------------|------------------------------|
| ![image](https://user-images.githubusercontent.com/8984680/230702158-73967aa9-01be-44d6-bbd9-24437e333140.png) | ![image](https://user-images.githubusercontent.com/8984680/230702177-de96f89b-053e-4313-a131-715af969db04.png) | ![image](https://user-images.githubusercontent.com/8984680/230702635-fb1de3bf-acbd-46ca-8d6f-caa47368b4d4.png) |




**⚡ 支持**   
* [x] 图片发送
* [x] 关键词触发回复
* [x] 多账号支持
* [x] 百度云内容审核
* [x] 额度限制 
* [x] 人格设定
* [x] 支持 Mirai、 go-cqhttp、 Telegram、Discord  
* [x] 可作为 HTTP 服务端提供 Web API
* [x] 支持 ChatGPT 网页版
* [x] 支持 ChatGPT Plus
* [x] 支持 ChatGPT API
* [x] 支持 Bing 聊天
* [x] 支持 Google bard
* [x] 支持 poe.com 网页版
* [x] 支持 文心一言 网页版
* [x] 支持 ChatGLM-6B 本地版

**🤖 多平台兼容**  

我们支持多种聊天平台。  

| 平台       | 群聊回复 | 私聊回复 | 条件触发 | 管理员指令 | 绘图  | 语音回复 |
|----------|------|------|------|-------|-----|------|
| Mirai    | 支持   | 支持   | 支持   | 支持    | 支持  | 支持   |
| OneBot   | 支持   | 支持   | 支持   | 支持    | 支持  | 支持   |
| Telegram | 支持   | 支持   | 部分支持 | 部分支持  | 支持  | 支持   |
| Discord  | 支持   | 支持   | 部分支持 | 不支持   | 支持  | 支持   |


## 🐎 命令

**你可以在 [Wiki](https://github.com/lss233/chatgpt-mirai-qq-bot/wiki/) 了解机器人的内部命令。**  


## 🔧 搭建

如果你是手机党，可以看这个纯用手机的部署教程（使用 Linux 服务器）：https://www.bilibili.com/video/av949514538

<details>
    <summary>Linux: 通过快速部署脚本部署 （新人推荐)</summary>
执行下面这行命令启动自动部署脚本。  
它会为你安装 Docker、 Docker Compose 和编写配置文件。  

```bash
bash -c "$(curl -fsSL https://gist.githubusercontent.com/lss233/54f0f794f2157665768b1bdcbed837fd/raw/chatgpt-mirai-installer-154-16RC3.sh)"
```

</details>

<details>
    <summary>Linux: 通过 Docker Compose 部署 （自带 Mirai)</summary>
我们使用 `docker-compose.yaml` 整合了 [lss233/mirai-http](https://github.com/lss233/mirai-http-docker) 和本项目来实现快速部署。  
但是在部署过程中仍然需要一些步骤来进行配置。  

你可以在 [Wiki](https://github.com/lss233/chatgpt-mirai-qq-bot/wiki/%E4%BD%BF%E7%94%A8-Docker-Compose-%E9%83%A8%E7%BD%B2%EF%BC%88Mirai---%E6%9C%AC%E9%A1%B9%E7%9B%AE%EF%BC%89) 查看搭建教程。

</details>

<details>
    <summary>Linux: 通过 Docker 部署 （适合已经有 Mirai 的用户)</summary>

1. 找个合适的位置，写你的 `config.cfg`。

2.  执行以下命令，启动 bot：
```bash
# 修改 /path/to/config.cfg 为你 config.cfg 的位置
# XPRA_PASSWORD=123456 中的 123456 是你的 Xpra 密码，建议修改
docker run --name mirai-chatgpt-bot \
    -e XPRA_PASSWORD=123456 \
    -v /path/to/config.cfg:/app/config.cfg \
    --network host \
    lss233/chatgpt-mirai-qq-bot:browser-version
```

3. 启动后，在浏览器访问 `http://你的服务器IP:14500` 可以访问到登录 ChatGPT 的浏览器页面  

</details>

<details>
    <summary>Windows: 快速部署包 (自带 Mirai，新人推荐）</summary>

我们为 Windows 用户制作了一个快速启动包，可以在 [Release](https://github.com/lss233/chatgpt-mirai-qq-bot/releases) 中找到。    

文件名为：`quickstart-windows-amd64.zip`  或者 `Windows快速部署包.zip`

</details>

<details>
    <summary>Mac: 快速部署包 (自带 Mirai，新人推荐）</summary>

Windows快速部署包Mac用户也可以使用，@magisk317 已测试通过，功能基本都正常
不过，需要注意的是，如果需要使用图片模式，由于`wkhtmltoimage.exe`在Mac上无法运行，可以使用`wkhtmltopdf`代替，安装命令：
```
brew install --cask wkhtmltopdf
```
brew的安装及使用方法详见：[链接](https://brew.sh/index_zh-cn)
</details>

<details>
    <summary>手动部署</summary>

提示：你需要 Python >= 3.11 才能运行本项目  

1. 部署 Mirai ，安装 mirai-http-api 插件。

2. 下载本项目:
```bash
git clone https://github.com/lss233/chatgpt-mirai-qq-bot
cd chatgpt-mirai-qq-bot
pip3 install -r requirements.txt
```

3. 参照项目文档调整配置文件。


4. 启动 bot.
```bash
python3 bot.py
```
</details>

**[广告] 免费 OpenAI API Key**  
<img src=https://user-images.githubusercontent.com/50035229/229976556-99e8ac26-c8c3-4f56-902d-a52a7f2e50d5.png width=300px />  
你可以在[这里获取免费的 OpenAI API Key](https://freeopenai.xyz/) 测试使用。
## 🕸 HTTP API

<details>
    <summary>在 `config.cfg` 中加入以下配置后，将额外提供 HTTP API 支持。</summary>

```toml
[http]
# 填写提供服务的端口
host = "0.0.0.0"
port = 8080
debug = false
```
启动后将提供以下接口：  

**POST**    `/v1/chat`  

**请求参数**  

|参数名|必选|类型|说明|
|:---|:---|:---|:---|
|session_id| 是 | String |会话ID，默认：`friend-default_session`|
|username| 是 | String |用户名，默认：`某人`|
|message| 是 | String |消息，不能为空|  

**请求示例**
```json
{
    "session_id": "friend-123456",
    "username": "testuser",
    "message": "ping"
}
```
**响应格式**
|参数名|类型|说明|
|:---|:---|:---|
|message| String |返回信息，HTML 格式|  

**响应示例**  
```json
{
    "message": "pong!"
}
```
</details>

## 🦊 加载预设

如果你想让机器人自动带上某种聊天风格，可以使用预设功能。  

我们自带了 `猫娘` 和 `正常` 两种预设，你可以在 `presets` 文件夹下了解预设的写法。  

使用 `加载预设 猫娘` 来加载猫娘预设。

下面是一些预设的小视频，你可以看看效果：
* MOSS： https://www.bilibili.com/video/av309604568
* 丁真：https://www.bilibili.com/video/av267013053
* 小黑子：https://www.bilibili.com/video/av309604568
* 高启强：https://www.bilibili.com/video/av779555493

关于预设系统的详细教程：[Wiki](https://github.com/lss233/chatgpt-mirai-qq-bot/wiki/%F0%9F%90%B1-%E9%A2%84%E8%AE%BE%E7%B3%BB%E7%BB%9F)

你可以在 [Awesome ChatGPT QQ Presets](https://github.com/lss233/awesome-chatgpt-qq-presets/tree/master) 获取由大家分享的预设。

你也可以参考 [Awesome-ChatGPT-prompts-ZH_CN](https://github.com/L1Xu4n/Awesome-ChatGPT-prompts-ZH_CN) 来调教你的 ChatGPT，还可以参考 [Awesome ChatGPT Prompts](https://github.com/f/awesome-chatgpt-prompts) 来解锁更多技能。

## 📷 文字转图片

在发送代码或者向 QQ 群发送消息失败时，自动将消息转为图片发送。  

字体文件存放于 `fonts/` 目录中。  

默认使用的字体是 [更纱黑体](https://github.com/be5invis/Sarasa-Gothic)。  

## 🎙 文字转语音

自 v2.2.5 开始，我们支持接入微软的 Azure 引擎 和 VITS 引擎，让你的机器人发送语音。

**提示**：在 Windows 平台上使用语音功能需要安装最新的 VC 运行库，你可以在[这里](https://learn.microsoft.com/zh-CN/cpp/windows/latest-supported-vc-redist?view=msvc-170)下载。`

## 🎈 相似项目

如果你自己也有做机器人的想法，可以看看下面这些项目：
 - [Ariadne](https://github.com/GraiaProject/Ariadne) - 一个优雅且完备的 Python QQ 机器人框架 （主要是这个 ！！！）
 - [mirai-api-http](https://github.com/project-mirai/mirai-api-http) - 提供HTTP API供所有语言使用 mirai QQ 机器人
 - [Reverse Engineered ChatGPT by OpenAI](https://github.com/acheong08/ChatGPT) - 非官方 ChatGPT Python 支持库  

本项目基于以上项目开发，所以你可以给他们也点个 star ！


除了我们以外，还有这些很出色的项目：  

* [LlmKira / Openaibot](https://github.com/LlmKira/Openaibot) - 全平台，多模态理解的 OpenAI 机器人
* [RockChinQ / QChatGPT](https://github.com/RockChinQ/QChatGPT) - 基于 OpenAI 官方 API， 使用 GPT-3 的 QQ 机器人
* [fuergaosi233 / wechat-chatgpt](https://github.com/fuergaosi233/wechat-chatgpt) - 在微信上迅速接入 ChatGPT


## 🛠 贡献者名单   

欢迎提出新的点子、 Pull Request。  

<a href="https://github.com/lss233/chatgpt-mirai-qq-bot/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=lss233/chatgpt-mirai-qq-bot" />
</a>

Made with [contrib.rocks](https://contrib.rocks).

## 💪 支持我们

如果我们这个项目对你有所帮助，请给我们一颗 ⭐️
