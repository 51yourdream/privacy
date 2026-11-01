# Virtual Memorial Space 隐私政策

**生效日期：2026 年 11 月 1 日**

## 1. 简介

Virtual Memorial Space（以下简称"本 App"、"我们"）是一款 iOS App，用于创建私密的纪念空间、进行纪念仪式和写信。本隐私政策说明本 App 处理哪些信息、这些信息存放在哪里，以及你有哪些选择。

本 App 无需注册账号。你的纪念内容只保存在你的设备上。我们的服务器只用于纪念币——一种可选的 App 内代币，用于使用更精致的供品款式。

使用本 App 即表示你已阅读并理解本隐私政策。

## 2. 我们不收集的信息

本 App 不收集、也不要求提供：

- 你的姓名、电子邮箱、电话号码或任何登录账号
- 纪念空间中的名字、照片、日期、简介、信件或留言
- 整个照片图库的访问权限，以及相机、麦克风、通讯录或位置
- 你的支付卡信息
- 广告标识符（IDFA）。本 App 不会在其他公司的 App 或网站之间跟踪你，也不会弹出"App 跟踪透明度"授权框。
- 统计或使用行为数据。本 App 没有接入任何统计分析 SDK，也没有广告。

## 3. 只保存在你设备上的纪念内容

以下内容保存在你的 iPhone 或 iPad 上本 App 的私有存储中：

- 纪念空间：名字、类型（例如亲人、伴侣、朋友或宠物）、简介、生日、纪念日、主题和提醒设置
- 你为纪念空间添加的照片
- 仪式记录：使用了哪种蜡烛、鲜花或纸钱供品、消耗的纪念币数量、时间，以及你添加的留言
- 你写的信件，包括草稿
- 偏好设置：语言、简化效果、是否显示传统纸钱、是否完成引导、待同步购买标记，以及用于限制评分请求次数的计数
- 上一次从我们服务器获取的纪念币余额，仅用于离线时显示

这些内容不会上传到我们的服务器，不用于广告，也不用于任何人工智能（AI）功能或训练。如果你开启了 iCloud 云备份，iOS 可能会把这些数据包含在设备备份中，由 Apple 在你的 Apple ID 下处理。本 App 自身没有云同步。

**照片。** 你通过系统照片选择器选择照片。本 App 只会收到你选中的照片，不会访问整个照片图库。每张选中的照片会压缩后保存一份副本在本 App 的存储中。

## 4. 纪念币与我们的服务器

纪念币是消耗型 App 内购买项目。为了在重新安装 App 后余额不丢失，余额保存在我们的服务器（"appapi"）上。该服务器部署在 Vercel，数据存储在 Vercel KV（Upstash Redis）中。

服务器只保存：

- 一个随机生成的用户 ID，与你的姓名、邮箱或 Apple ID 无关联
- 为该用户 ID 签发的访问令牌的摘要（哈希值）。服务器不保存令牌本身。
- 你的纪念币余额
- 购买记录：商品 ID、Apple 交易 ID、纪念币数量和时间
- 消费记录：供品 ID（例如某种蜡烛）、纪念币数量、用于防止重复扣币的请求键、消费后的余额和时间
- 一份记录加币、扣币和退款的流水，包括数量及相关的交易 ID 或消费 ID

每次请求服务器时，还会附带 App 版本号和一个设备标识（iOS 的 identifierForVendor），用于校验请求签名。与任何网络服务一样，我们的托管服务商可能会在常规请求日志中处理你的 IP 地址，用于提供和保护服务。

服务器不保存你的姓名、邮箱，也不保存任何关于你所纪念的人或宠物的信息：没有纪念对象的名字、照片、信件或留言。

用户 ID 和令牌保存在你设备的 iOS 钥匙串中，可能会通过 iCloud 钥匙串同步，因此重新安装 App 后，或在登录同一 Apple ID 的其他设备上，你的余额仍然可用。

## 5. 购买

- **Apple（App Store）** 通过你的 Apple ID 处理所有付款。我们不会获取你的支付卡信息。Apple 隐私政策：https://www.apple.com/legal/privacy/
- **RevenueCat** 负责校验交易。RevenueCat 会收到上述随机用户 ID、交易信息（例如商品 ID、Apple 交易 ID 和购买时间），以及基本技术信息，例如 App 版本、操作系统版本和 App Store 国家或地区。我们的服务器向 RevenueCat 确认购买，RevenueCat 也会把购买和退款通知我们的服务器，从而保证每笔购买只加一次币，退款后扣回相应纪念币。RevenueCat 隐私政策：https://www.revenuecat.com/privacy

纪念币没有现实货币价值。退款由 Apple 按其规则处理。使用条款为 Apple 标准许可协议：https://www.apple.com/legal/internet-services/itunes/dev/stdeula/

## 6. 通知（可选）

如果你为某个纪念空间开启纪念日提醒，本 App 会请求通知权限，并在你的设备上安排本地通知。提醒不经过我们的服务器。你可以在 App 内或 iOS"设置"中关闭提醒。

## 7. 我们如何使用信息

我们仅将上述信息用于：

- 在你的设备上显示和保存纪念空间、仪式记录和信件
- 创建你的纪念币钱包，每笔交易只加一次币，在你选择付费供品时扣币，并在退款后扣回纪念币
- 校验请求，防止欺诈或重复加币
- 回复你的支持请求

我们不出售或出租个人信息，不将其用于广告，也不建立广告画像。

## 8. 信息共享

我们只与运营本 App 所必需的服务商共享信息（Apple、RevenueCat，以及提供托管和存储的 Vercel / Upstash），或在法律或有效法律程序要求时共享。

## 9. 删除你的数据

在本 App 的"设置"中：

- **删除全部数据（Delete All Data）** 会删除此设备上的全部纪念内容：纪念空间、照片、仪式记录、信件和留言。
- **删除纪念币数据（Delete Token Data）** 会删除我们服务器上的钱包：用户 ID 记录、令牌哈希、余额、购买与消费记录以及流水。余额会清零且无法恢复。为防止同一笔购买再次入账，我们只保留去掉用户 ID 的 Apple 交易 ID（及其商品 ID）。随后，用户 ID 和令牌也会从你的钥匙串中删除。

删除 App 会移除设备上的本地内容，但删除 App **不会**删除我们服务器上的钱包数据。如需删除，请在删除 App 之前使用"删除纪念币数据"，或联系我们。已删除的本地数据可能仍保留在之前的 iCloud 设备备份中，直到 Apple 替换或删除这些备份。

你也可以请我们向 RevenueCat 申请删除其保存的购买记录。

## 10. 安全与保留期限

与我们服务器、Apple 和 RevenueCat 的连接均使用加密的 HTTPS。请求经过签名，服务器只保存令牌的哈希值，你的身份保存在 iOS 钥匙串中。任何存储或传输方式都无法做到绝对安全。

- 本地内容会一直保留，直到你删除它或删除 App。
- 服务器上的钱包数据会一直保留，直到你使用"删除纪念币数据"或请求我们删除。
- 不含用户 ID 的 Apple 交易 ID 会被保留，用于防止重复入账。
- Apple 和 RevenueCat 会按其自身政策和法律义务保留购买记录。

## 11. 儿童隐私

Virtual Memorial Space 不面向儿童。我们不会故意收集 13 岁以下儿童（或你所在国家规定的最低年龄以下儿童）的个人信息。如果你认为有儿童向我们提供了个人信息，请联系我们，我们会将其删除。

## 12. 跨境处理

我们的托管和存储服务商以及 RevenueCat 可能会在美国或你所在地以外的其他国家处理数据。我们依赖这些服务商的保障措施来进行此类处理。

## 13. 你的权利

根据你所在地区的法律，你可能有权访问、更正、删除或限制处理你的个人信息。大部分数据都在你的设备上，由你自行控制。对于我们服务器上的数据，请使用"删除纪念币数据"或联系我们。我们可能会请你提供有助于找到相关记录的信息。

## 14. 政策变更

我们可能会更新本隐私政策，届时顶部的日期会随之更改。如果本 App 开始收集新类型的数据，我们会先更新本政策。

## 15. 联系我们

如果你对本隐私政策有任何疑问，请联系：

- 邮箱：lpjustdoit@163.com

---

## 其他语言

- [English](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/en/privacy.md)
- [简体中文](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/zh/privacy.md)
- [繁體中文](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/zh-tw/privacy.md)
- [日本語](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ja/privacy.md)
- [한국어](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ko/privacy.md)
- [Deutsch](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/de/privacy.md)
- [Français](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/fr/privacy.md)
- [Español](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/es/privacy.md)
- [Italiano](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/it/privacy.md)
- [Português (Portugal)](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/pt-PT/privacy.md)
- [Português (Brasil)](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/pt-BR/privacy.md)
- [ไทย](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/th/privacy.md)
- [Tiếng Việt](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/vi/privacy.md)
- [Bahasa Indonesia](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/id/privacy.md)
- [Bahasa Melayu](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ms/privacy.md)
- [العربية](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ar/privacy.md)
