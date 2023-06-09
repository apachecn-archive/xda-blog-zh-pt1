# 脸书解释了 WhatsApp 的端到端加密备份是如何工作的

> 原文：<https://www.xda-developers.com/facebook-whatsapp-end-to-end-backups/>

脸书旗下的 WhatsApp 提供端到端加密信息服务已经有一段时间了，不过这种额外的安全性在过去并没有应用于备份。它也不适用于媒体，并且您依赖于您所支持的云提供商提供的加密服务。如果需要的话，这些云提供商也可以解密它们，对于注重隐私的人来说，这显然不太理想。

该公司开始在 WhatsApp 的测试版中测试端到端的加密备份，现在，在更大范围的推广之前，脸书已经向 T2 解释了这些加密备份是如何工作的。

## WhatsApp 的端到端加密备份是如何工作的

### 生成加密密钥和密码

脸书表示，它已经开发了一个全新的加密密钥存储系统，可以在 iOS 和 Android 上运行。备份使用唯一的随机密钥加密，该密钥可以手动存储，也可以使用密码存储。如果用户想用密码存储它，他们可以访问基于硬件安全模块的备份密钥库，以检索他们的加密密钥并解密备份。该保险库负责强制执行密码验证尝试，并在多次尝试访问失败后使密钥永久不可访问。这可以防止暴力攻击，WhatsApp 永远不会知道密钥。

### 存储密钥

WhatsApp 使用一种名为 ChatD 的前端服务，该服务处理客户端连接和客户端-服务器认证。它将实现一个协议，在 WhatsApp 的服务器之间发送备份密钥，客户端和密钥库交换加密消息。备份是作为对称加密的连续数据流生成的，也就是说，用于加密的密钥也可以用于解密。加密后，备份可以存储在异地的任何地方，包括 Google Drive 或 iCloud。

脸书表示，为了帮助应对依赖 WhatsApp 的用户数量，在发生宕机的情况下，密钥库服务将在地理上分布在多个数据中心。脸书还发布了两张图片，展示了当使用密钥解密备份或使用用户密码解密时，端到端加密是如何工作的。

### 使用密码时的加密和解密过程

如果帐户所有者使用密码来访问他们的备份，那么它将通过以下过程从密钥库中检索密钥。

1.  他们输入密码，该密码被加密，然后由备份密钥库验证。
2.  一旦验证了密码，备份密钥库就会将加密密钥发送回 WhatsApp 客户端。
3.  有了密钥，WhatsApp 客户端就可以解密备份了。

如果使用的是 64 位密钥，那么用户需要自己手动保存并输入密钥。