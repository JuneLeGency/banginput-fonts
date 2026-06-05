# BangInput 隐私政策 / Privacy Policy

**生效日期 / Effective date**: 2026-06-05

---

## 中文版

### 核心承诺

BangInput 是一款**默认完全离线**的输入法。你键入的每一个字符都只在你的设备本地处理：

- **我们不收集、不存储、不上传你的任何输入内容。**
- 我们没有自己的服务器，不存在「输入数据回传」的通道。
- 系统在启用第三方输入法时会显示通用警告（「此输入法可能会收集您键入的所有文字」）——这是 Android 对所有第三方键盘的统一提示。BangInput 的回应是架构层面的：解码、联想、纠错、用户词典全部在设备上完成，应用不含任何分析/广告/追踪 SDK。

### 数据在哪里

| 数据 | 位置 | 说明 |
|---|---|---|
| 输入内容（按键、拼音、候选） | 仅设备内存 | 处理后即弃，不写盘不上传 |
| 用户词典（你打过的新词） | 仅设备本地存储 | 卸载即删；**密码输入框自动禁用学习与联想** |
| 剪贴板历史 | 仅设备本地存储 | 仅在你打开该功能时记录，可随时清空 |
| 输入统计（命中率等聚合数字） | 仅设备本地存储 | 不含任何输入文本，仅供你在设置页自查 |
| 崩溃日志 | 仅设备本地文件 | 不自动上报；只有你主动复制发送才会离开设备 |
| 语音（离线模型） | 仅设备处理 | 音频不离开设备 |

### 哪些功能会联网（均为可选，且可一键关闭）

1. **版本更新检查**：向 GitHub / Gitee 的公开接口查询新版本号。不携带任何个人数据或输入内容。
2. **资产下载**：词库包、语音模型、字体、重排模型按需从公开仓库下载（HTTPS + 校验）。下载请求不含个人数据。
3. **云 AI / 云语音（默认关闭，需你自行配置）**：如果你主动填写了第三方 AI 服务（OpenAI 兼容端点）的地址与密钥，则在你触发相应功能时，相关文本或语音会发送到**你指定的**第三方服务。该传输受对应第三方的隐私政策约束，BangInput 仅做转发，不经手任何中间服务器。不配置则完全不存在此数据流。
4. **单机模式**：设置中开启后，应用内所有网络功能（含更新检查与下载）全部禁用。

### 权限用途

| 权限 | 用途 |
|---|---|
| 网络（INTERNET） | 上述更新检查 / 资产下载 / 可选云功能 |
| 麦克风（RECORD_AUDIO） | 语音输入：仅在你按下语音按钮时录音；离线模型下音频不离开设备 |
| 震动（VIBRATE） | 按键触感反馈 |
| 使用情况访问（可选） | T9 查找器按使用频度排列应用，仅本地统计，需你在系统设置中手动授予 |

### 数据删除

所有本地数据（用户词典、剪贴板、统计、已下载模型）随应用卸载即彻底删除；也可在设置中分项清除。

### 儿童

本应用非儿童导向，不针对 13 岁以下儿童收集任何信息（事实上对任何人都不收集）。

### 政策变更与联系方式

政策若有实质变更，将在应用更新说明中提示。问题或反馈：
- GitHub Issues: https://github.com/JuneLeGency/BangInput/issues
- Email: lichen900210@gmail.com

---

## English Version

### Core Commitment

BangInput is an **offline-first** input method. Every character you type is processed locally on your device:

- **We do not collect, store, or transmit anything you type.**
- We operate no servers; there is no channel through which input data could be sent back.
- Android shows a generic warning when enabling any third-party keyboard ("may be able to collect all the text you type"). BangInput's answer is architectural: decoding, prediction, correction, and the user dictionary all run on-device, and the app contains no analytics, advertising, or tracking SDKs.

### Where Your Data Lives

| Data | Location | Notes |
|---|---|---|
| Input content (keystrokes, pinyin, candidates) | Device memory only | Discarded after processing; never written or uploaded |
| User dictionary (new words you typed) | Local storage only | Deleted on uninstall; **learning is disabled in password fields** |
| Clipboard history | Local storage only | Recorded only if you enable the feature; clearable anytime |
| Input statistics (aggregate numbers) | Local storage only | Contains no text; visible only to you in Settings |
| Crash logs | Local file only | Never auto-reported; leaves the device only if you manually share it |
| Voice (offline models) | On-device only | Audio never leaves the device |

### Network Features (all optional, all disableable)

1. **Update check**: queries public GitHub/Gitee endpoints for the latest version number. Carries no personal data.
2. **Asset downloads**: dictionaries, speech models, fonts, and ranking models are downloaded on demand from public repositories (HTTPS, checksum-verified). Requests contain no personal data.
3. **Cloud AI / Cloud ASR (off by default, user-configured)**: if you choose to configure a third-party AI service (OpenAI-compatible endpoint) with your own URL and key, the relevant text or audio is sent to **the service you specified** when you trigger those features, governed by that third party's privacy policy. BangInput forwards directly with no intermediary server. Without configuration, this data flow does not exist.
4. **Offline mode**: a single switch in Settings disables all in-app network activity, including update checks and downloads.

### Permissions

| Permission | Purpose |
|---|---|
| INTERNET | Update check / asset downloads / optional cloud features above |
| RECORD_AUDIO | Voice input: records only while you hold the voice button; with offline models audio never leaves the device |
| VIBRATE | Keypress haptic feedback |
| Usage access (optional) | Sorts apps by usage frequency in the T9 app finder; local-only statistics; must be granted manually in system settings |

### Data Deletion

All local data (user dictionary, clipboard, statistics, downloaded models) is permanently removed when the app is uninstalled, and can also be cleared per-category in Settings.

### Children

This app is not directed at children and collects no information from anyone, including children under 13.

### Changes & Contact

Material changes will be announced in release notes.
- GitHub Issues: https://github.com/JuneLeGency/BangInput/issues
- Email: lichen900210@gmail.com
