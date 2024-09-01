# Telegram 搭建私聊bot教程

Telegram（电报）现在在国内码农圈用的人越来越多，之前 Telegram 为了防止 spam，直接无差别的关闭了所有以 +86 开头手机号注册的 Telegram 账号的私聊权限。本文老王介绍下如何在 Telegram 搭建一个私聊机器人，用于转发别人的私聊信息，同时也可以保护自己的隐私。

&#x20;

搭建 Telegram 私聊机器人时，我们需要两个 bot：

@BotFather

@LivegramBot

这两个机器人都是 Telegram 官方的，工作原理也很简单，就是别人私聊给你的信息都是通过 LivegramBot 转发给你的。

&#x20;

直接私聊给你创建的私聊机器人；

收到私聊后，这个私聊机器人会将信息通过 LivegramBot 转发给你（你可以看到发送消息人的信息，也就是这个私聊是谁发给私聊机器人的）；

你直接在私聊机器人的聊天窗口回复那条消息，LivegramBot 就会把你回复的信息通过私聊机器人再次转发给你。

### 搭建教程 <a href="#heading-1" id="heading-1"></a>

**1、找** [**BotFather**](https://t.me/botfather) **创建一个私聊机器人**

直接给 [BotFather](https://t.me/botfather) 发送 `/newbot` 指令创建机器人，之后需要你给机器人取个名字，必须以 bot 结尾，如果没有问题就会创建成功，你会得到一个机器人的 URL 和 API token：

**2、找** [**LivegramBot**](https://t.me/LivegramBot) **创建私聊机器人**

继续联系 [LivegramBot](https://t.me/LivegramBot) 发送 `/addbot` 指令创建私聊机器人，之后回复刚才创建的机器人的 API token：

**3、私聊机器人使用**

首先你自己私聊自己的私聊机器人，`/start` 开始对话。之后别人再想通过 Telegram 私聊你时，只需要联系这个机器人就行了，消息会自动通过你的私聊机器人转发给你，你只需要把机器人的 URL 或者 bot 的 username 告诉别人就行。
