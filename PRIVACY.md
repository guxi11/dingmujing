# 定目镜（Steadeye）隐私政策

生效日期：2026 年 10 月 28 日

**一句话：相机、面部和运动数据仅在设备上用于实时取景与跟踪，不会发送给开发者或第三方。若你主动发送邮件反馈，开发者会收到邮件及其中的内容。开发者没有账号系统、服务器、广告或分析服务。**

## 相机

前置摄像头帧在设备内存中用于本机眼部分析、放大窗画面及引导箭头。信息卡以取景叠层显示，打开信息卡不会停止采集。应用在支持 ARKit 面部追踪的设备上启用该功能；TrueDepth 是部分支持设备使用的硬件能力，并非应用可用的必要条件。取景期间会在内存中缓存多帧像素和放大画面，并暂存眼部位置、标定偏移及追踪状态；这些数据可能跨帧使用，也可能在画面短暂冻结时继续保留。停止采集不会主动清空这些内存数据；它们随缓存覆盖、重置或对象释放而释放，最迟在应用进程结束时释放。相机画面及由此产生的数据不写入文件、不上传或共享给开发者或第三方。

## 面部数据（ARKit / 原深感摄像头）

应用通过 `ARFaceTrackingConfiguration.isSupported` 判断是否启用 ARKit 面部追踪。支持设备可能使用 TrueDepth 硬件；TrueDepth 并非应用可用的必要条件。应用读取头部和双眼的相对位姿，用于放大窗定位与稳定、丢失后的跟踪找回及眼部贴图。设备支持时还会启用 world tracking，读取相机运动和位姿以辅助掉锚跟踪。应用不读取原始深度图或 Face ID 身份信息，也不会写入、保存或上传空间地图。

- **用途**：用于实时眼部追踪、放大窗定位与稳定、跟踪找回和贴图。
- **保存与保留**：眼部位置、追踪状态及运动位姿会在内存中缓存并可能跨帧使用；停止采集不会主动清空，数据随缓存覆盖、重置或对象释放而释放，最迟在应用进程结束时释放。不写入文件。
- **共享**：面部追踪数据不发送给开发者或任何第三方。
- **限制**：不用于身份识别、广告、营销或数据分析。

## 运动传感器

Core Motion 读取重力、姿态、旋转速率和用户加速度，用于引导箭头、界面朝向及跟踪。相关运动数据在设备内存中用于处理，不写入文件、不上传或共享。应用不读取 GPS 位置。

## 保存在设备上的内容

定目镜只在本机（App 自己的设置存储里）保存两项与你身份无关的内容：

- 你选择的虹膜贴图样式；
- 一个「最近见过的时间」记号，用于判断购买权益时防止系统时间回拨。

App 不会主动上传这些设置。iOS 是否将 App 数据纳入系统备份由 iOS 和你的设备设置决定，因此这些内容不一定始终只保留在本机。删除 App 后，设备上的 App 数据按 iOS 的行为处理。新版不再写入或读取旧测试版留在钥匙串中的试用计时项；启动时会尝试删除该项，但删除失败时可能残留。App 也不保存首次启动时间。

## 网络、账号与第三方

定目镜没有账号系统、开发者服务器、广告或分析服务，也没有第三方 SDK。购买和恢复购买时，StoreKit 会与 Apple 通信。你点击政策或 GitHub Issues 链接后，浏览器会访问 GitHub Pages 或 GitHub；访问会涉及 IP 地址等网络信息，并受相应服务方的隐私政策约束。

## 购买与试用

App 启动时会通过 StoreKit 向 Apple 加载商品信息；购买与恢复购买由 Apple 处理。试用为 3 天、0 元的非消耗型内购，从原始交易日期起算且不会自动续费；买断为一次性付费。App 通过 StoreKit 读取交易权益以决定是否解锁。Apple 按其政策管理交易记录；开发者不运营账号或服务器。相关处理适用 [Apple 隐私政策](https://www.apple.com/legal/privacy/)。

## 反馈

在 App 里点「写邮件反馈」会打开你的邮件 App，并在正文预填机型代号、iOS 版本和 App 版本，方便排查问题；发不发、写什么都由你决定，预填内容可以删改。点击时 App 会将开发者邮箱复制到剪贴板，不会读取剪贴板内容。你主动发送的邮件会由开发者收到，并按回复和排查问题所需予以保留；如需删除已发送邮件中的内容，请联系下方邮箱提出请求。

在 GitHub Issues 提交的内容公开可见，并适用 GitHub 的隐私条款；请不要在 Issues 里上传带有你面部的照片或录屏。

## 儿童

相机、面部和运动数据不会发送给开发者。儿童或其监护人若主动发送邮件反馈，开发者会收到邮件及其中的个人信息；请只提供处理问题所需的内容，并可联系下方邮箱请求删除已发送邮件中的内容。

## 政策变更

如有变更，会更新本页并修改上方的生效日期。

## 联系

- 邮箱：2364194350@qq.com
- GitHub Issues：<https://github.com/Guxi11/dingmujing/issues>

---

<a id="english"></a>

# Steadeye Privacy Policy

Effective: October 28, 2026

**In short: Camera, face, and motion data are used on your device for live viewing and tracking and are not sent to the developer or third parties. If you choose to email feedback, the developer receives your email and its contents. The developer has no accounts, servers, advertising, or analytics service.**

## Camera

Front-camera frames are analyzed for the eyes on device and used for the magnified view and guide arrow. The information card is an overlay on the viewfinder; opening it does not stop capture. The app enables ARKit face tracking on devices where it is supported; TrueDepth is hardware used by some supported devices, but is not required for the app to work. During viewing, the app buffers multiple frames of pixels and magnified images and temporarily retains eye positions, calibration offsets, and tracking state. These data may be used across frames or retained while the display briefly freezes. Stopping capture does not actively clear these in-memory data; they are released as buffers are overwritten, state is reset, or related objects are released, and no later than when the app process ends. Camera frames and derived data are not written to files or uploaded or shared with the developer or third parties.

## Face data (ARKit / TrueDepth camera)

The app checks `ARFaceTrackingConfiguration.isSupported` to determine whether to enable ARKit face tracking. Supported devices may use TrueDepth hardware; TrueDepth is not required for the app to work. The app reads the relative poses of the head and both eyes to position and stabilize the magnified view, recover tracking, and place eye stickers. When supported, world tracking is also enabled to read camera motion and pose for tracking recovery. The app does not read raw depth maps or Face ID identity information, and does not write, store, or upload a spatial map.

- **Use**: live eye tracking, positioning and stabilizing the magnified view, tracking recovery, and sticker placement.
- **Storage and retention**: eye positions, tracking state, and motion poses are buffered in memory and may be used across frames. Stopping capture does not actively clear them; they are released as buffers are overwritten, state is reset, or related objects are released, and no later than when the app process ends. They are not written to files.
- **Sharing**: face-tracking data is not sent to the developer or any third party.
- **Restrictions**: not used for identification, advertising, marketing, or analytics.

## Motion sensors

Core Motion reads gravity, attitude, rotation rate, and user acceleration for the guide arrow, interface orientation, and tracking. Motion data is processed in device memory and is not written to files, uploaded, or shared. The app does not access GPS location.

## What stays on your device

Steadeye stores only two items on the device (in the app's own settings storage), neither of which identifies you:

- the iris sticker style you chose;
- a "latest time seen" marker, used to prevent system clock rollback from affecting purchase entitlement checks.

The app does not actively upload these settings. Whether iOS includes app data in a system backup depends on iOS and your device settings, so this data may not always remain only on your device. App data on the device is handled according to iOS behavior when you delete the app. The current version no longer writes or reads the legacy trial timer stored in the keychain; at launch, it attempts to delete that item, but it may remain if deletion fails. The app does not store when you first launched it.

## Network, accounts, and third parties

Steadeye has no account system, developer server, advertising, or analytics service, and no third-party SDKs. StoreKit communicates with Apple for purchases and restoration. When you tap a policy or GitHub Issues link, your browser visits GitHub Pages or GitHub; that access involves network information such as your IP address and is governed by the service provider's privacy policy.

## Purchases and trial

At launch, the app uses StoreKit to load product information from Apple; Apple processes purchases and restoration. The trial is a free, non-consumable in-app purchase for three days, starting from the original transaction date and not auto-renewing. The full version is a one-time purchase. The app reads transaction entitlements through StoreKit to determine access. Apple manages transaction records under its policies; the developer does not operate an account system or server. See the [Apple Privacy Policy](https://www.apple.com/legal/privacy/).

## Feedback

Tapping "Email Feedback" opens your mail app with your device model code, iOS version, and app version pre-filled to help diagnose issues. Whether and what you send is up to you, and you can edit or delete the pre-filled text. When tapped, the app copies the developer's email address to the clipboard and does not read clipboard contents. Emails you choose to send are received by the developer and retained as needed to reply and troubleshoot. To request deletion of content in an email you sent, contact the email address below.

Content posted to GitHub Issues is public and subject to GitHub's privacy terms. Please don't upload photos or recordings of your face there.

## Children

Camera, face, and motion data are not sent to the developer. If a child or their guardian chooses to email feedback, the developer receives the email and personal information it contains. Please provide only what is needed to address the issue; you may contact the email address below to request deletion of content in an email you sent.

## Changes

Any changes will be posted on this page with an updated effective date.

## Contact

- Email: 2364194350@qq.com
- GitHub Issues: <https://github.com/Guxi11/dingmujing/issues>
