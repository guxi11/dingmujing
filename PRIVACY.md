# 定目镜（Steadeye）隐私政策

生效日期：2026 年 10 月 5 日

**一句话：定目镜不收集、不保存、不上传你的任何个人数据。所有计算都在你的 iPhone 上实时完成，开发者没有服务器。**

## 相机

前置摄像头画面只用于实时识别眼睛位置、在放大窗里显示放大画面和引导箭头。画面只在内存中逐帧处理：不保存、不截图、不录像、不上传。离开取景即停止采集。

## 面部数据（ARKit / 原深感摄像头）

在带原深感（TrueDepth）摄像头的机型上，定目镜使用 Apple ARKit 人脸追踪读取眼部的位置与朝向。

- **用途**：仅用于实时定位眼睛、放大取景和绘制引导箭头。
- **保存与保留**：只在内存中参与当前画面的计算，算完即丢弃，不写入任何存储。
- **共享**：不发送给开发者或任何第三方。
- **限制**：不用于身份识别、广告、营销或任何数据分析。

## 运动传感器

只读取重力方向，用来让引导箭头指向物理上方。不记录、不上传。

## 保存在设备上的内容

定目镜只在本机（App 自己的设置存储里）保存两项与你身份无关的内容：

- 你选择的虹膜贴图样式；
- 一个「最近见过的时间」记号，只用于判断试用是否到期时防止把系统时间往回拨。

它们都不会离开你的设备，删除 App 即一并清除。定目镜不在钥匙串中保存任何内容，也不保存首次启动时间（早期测试版曾写入的试用计时项会在启动时自动删除）。

## 网络、账号与第三方

定目镜本身不发起任何网络请求（下方「购买与试用」经 Apple StoreKit 与 App Store 通信的除外）；没有账号，没有广告，没有统计分析，也没有任何第三方 SDK。

## 购买与试用

3 天试用与买断都是 Apple App Store 内购：试用是一件 0 元的「3-day Trial」，试用期从你领取它的交易日期起算；买断是一次性付费。交易与付款都由 Apple 处理并记在你的 Apple ID 上，开发者接触不到你的 Apple ID 或支付信息；App 只通过 Apple 的 StoreKit 读取这两件商品的交易状态（包括试用的交易日期）来决定是否解锁。相关处理适用 [Apple 隐私政策](https://www.apple.com/legal/privacy/)。

## 反馈

在 App 里点「写邮件反馈」会打开你的邮件 App，并在正文预填机型代号、iOS 版本和 App 版本，方便排查问题；发不发、写什么都由你决定，预填内容可以删改。你发来的邮件只用于回复和排查问题。

在 GitHub Issues 提交的内容公开可见，并适用 GitHub 的隐私条款；请不要在 Issues 里上传带有你面部的照片或录屏。

## 儿童

定目镜不收集任何人的个人数据，包括儿童。

## 政策变更

如有变更，会更新本页并修改上方的生效日期。

## 联系

- 邮箱：2364194350@qq.com
- GitHub Issues：<https://github.com/Guxi11/dingmujing/issues>

---

<a id="english"></a>

# Steadeye Privacy Policy

Effective: October 5, 2026

**In short: Steadeye does not collect, store, or upload any of your personal data. Everything is computed in real time on your iPhone, and the developer runs no servers.**

## Camera

Front-camera frames are used only to locate your eye in real time and to show the magnified view and the guide arrow. Frames are processed in memory, one at a time: they are never saved, captured, recorded, or uploaded. Capture stops when you leave the viewfinder.

## Face data (ARKit / TrueDepth camera)

On devices with a TrueDepth camera, Steadeye uses Apple ARKit face tracking to read the position and orientation of your eyes.

- **Use**: only to locate your eye in real time, frame the magnified view, and draw the guide arrow.
- **Storage and retention**: used in memory for the current frame only and discarded right after; never written to storage.
- **Sharing**: never sent to the developer or any third party.
- **Restrictions**: never used for identification, advertising, marketing, or any kind of analytics.

## Motion sensors

Only the direction of gravity is read, so the guide arrow can point physically upward. Nothing is recorded or uploaded.

## What stays on your device

Steadeye stores only two items on the device (in the app's own settings storage), neither of which identifies you:

- the iris sticker style you chose;
- a "latest time seen" marker, used only to stop the trial check from being fooled by setting the system clock back.

Neither ever leaves your device, and both are removed when you delete the app. Steadeye stores nothing in the keychain and does not record when you first launched it (a trial timer written by early test builds is deleted automatically at launch).

## Network, accounts, and third parties

Steadeye itself makes no network requests, apart from StoreKit communicating with the App Store as described under "Purchases and trial". There are no accounts, no ads, no analytics, and no third-party SDKs.

## Purchases and trial

Both the 3-day trial and the one-time purchase are Apple App Store in-app purchases: the trial is a free "3-day Trial" item, and the trial period runs from the date of that transaction; the full version is a one-time payment. Apple processes the transactions and payment and records them on your Apple ID; the developer never sees your Apple ID or payment details. The app only reads the status of these two items through Apple's StoreKit (including the trial's transaction date) to decide what to unlock. See the [Apple Privacy Policy](https://www.apple.com/legal/privacy/).

## Feedback

Tapping "Email Feedback" opens your mail app with your device model code, iOS version, and app version pre-filled to help diagnose issues. Whether and what you send is up to you, and you can edit or delete the pre-filled text. Emails are used only to reply and troubleshoot.

Content posted to GitHub Issues is public and subject to GitHub's privacy terms. Please don't upload photos or recordings of your face there.

## Children

Steadeye collects no personal data from anyone, including children.

## Changes

Any changes will be posted on this page with an updated effective date.

## Contact

- Email: 2364194350@qq.com
- GitHub Issues: <https://github.com/Guxi11/dingmujing/issues>
