# 漂移高手第三方信息共享清单 / Drift Master Third-Party Data Sharing List

**生效日期 / Effective Date:** 2026-09-14  
**最后更新 / Last Updated:** 2026-09-27
**开发者 / Developer:** SPIELPHANTOMLIMITED

## 1. 共享原则 / Sharing Principles

开发者不出售玩家个人信息。以下共享仅用于实现游戏功能、运行在线服务、维护稳定性或履行法律义务。

The developer does not sell player personal information. The sharing described below is only for game features, online services, stability, or legal compliance.

## 2. Google Play Games Services

| 项目 / Item | 中文 / Chinese | English |
| --- | --- | --- |
| 服务提供方 | Google LLC | Google LLC |
| 使用场景 | Google 登录、玩家身份识别、Saved Games 云端存档 | Google sign-in, player identity, and Saved Games cloud saves |
| 可能共享信息 | Play Games 玩家 ID、显示名称、登录状态、登录令牌、游戏存档数据 | Play Games player ID, display name, sign-in status, sign-in token, and game-save data |
| 共享触发条件 | 玩家主动使用 Google Play Games 登录，或登录后使用云端存档 | When the player signs in with Google Play Games or uses cloud saves after sign-in |
| 隐私政策 | Google 隐私权政策 / Google Privacy Policy | [Google Privacy Policy](https://policies.google.com/privacy) |

## 3. Unity Gaming Services

| 项目 / Item | 中文 / Chinese | English |
| --- | --- | --- |
| 服务提供方 | Unity Technologies / Unity Software Inc. | Unity Technologies / Unity Software Inc. |
| 使用场景 | 匿名身份验证、排行榜、服务初始化、崩溃与性能诊断 | Anonymous authentication, leaderboards, service initialization, crash and performance diagnostics |
| 可能共享信息 | Unity 安装 ID、匿名玩家 ID、排行榜成绩、设备型号、操作系统、应用版本、IP 地址和错误日志 | Unity installation ID, anonymous player ID, leaderboard scores, device model, OS version, app version, IP address, and error logs |
| 当前开关 | Leaderboards 已启用；UGS Cloud Save 当前未启用 | Leaderboards enabled; UGS Cloud Save currently disabled |
| 隐私政策 | Unity 隐私政策 / Unity Privacy Policy | [Unity Privacy Policy](https://unity.com/legal/privacy-policy) |

## 3.1 Google AdMob

| 项目 / Item | 中文 / Chinese | English |
| --- | --- | --- |
| 服务提供方 | Google LLC | Google LLC |
| 使用场景 | 横幅广告、插屏广告和激励视频广告展示、广告加载、展示统计与用户同意管理 | Banner, interstitial, and rewarded video ads, ad loading, impression reporting, and consent management |
| 可能共享信息 | Android 广告标识、设备型号、操作系统、应用版本、网络状态、IP 地址、广告交互信息和激励视频完成状态 | Android advertising ID, device model, OS version, app version, network state, IP address, ad interaction data, and rewarded-video completion status |
| 共享触发条件 | 用户完成 UMP 同意流程，并且进入展示广告的场景 | After the UMP consent flow is complete and the player enters an ad-supported scene |
| 隐私政策 | Google 隐私权政策 / Google Privacy Policy | [Google Privacy Policy](https://policies.google.com/privacy) |

## 4. Google Play 和应用商店 / Google Play and App Stores

应用商店和操作系统可能为下载、安装、更新、账号管理、付款或安全审核处理设备标识、商店账号状态和应用版本信息。此类处理受对应商店政策约束。当前版本没有应用内购买。

App stores and operating systems may process device identifiers, store-account status, and app-version information for download, installation, updates, account management, payments, or security review. Such processing is governed by the relevant store policies. The current version has no in-app purchases.

## 5. 未启用的服务 / Services Not Currently Active

- Unity Analytics：当前构建未启用主动分析。  
  Unity Analytics: active analytics is not enabled in the current build.
- Unity Cloud Save：UGS 设置中当前为关闭状态。  
  Unity Cloud Save: currently disabled in the UGS settings.
- Rewarded 广告：已接入。仅在玩家主动选择观看时展示；完成观看后发放游戏内奖励，玩家不观看也可以继续使用不依赖该奖励的功能。  
  Rewarded ads: integrated. They are shown only when the player chooses to watch; the reward is granted after completion, and the player can continue using features that do not depend on the reward without watching.
- 第三方登录以外的社交网络：当前未接入公共社交功能。  
  Social networks other than third-party sign-in: no public social features are integrated.

## 6. Android 权限 / Android Permissions

| 权限 / Permission | 用途 / Purpose |
| --- | --- |
| `android.permission.INTERNET` | 登录、排行榜、云端存档和网络诊断 |
| `android.permission.ACCESS_NETWORK_STATE` | 判断网络是否可用及连接状态 |
| `com.google.android.gms.permission.AD_ID` | AdMob 广告标识，用于广告投放、频次控制和反作弊；玩家可在系统设置中重置或删除广告 ID |
| `android.permission.ACCESS_ADSERVICES_AD_ID` | Android 广告服务访问广告 ID，由 AdMob SDK 合并加入 |
| `android.permission.ACCESS_ADSERVICES_ATTRIBUTION` | Android 广告服务归因，由 AdMob SDK 合并加入 |
| `android.permission.ACCESS_ADSERVICES_TOPICS` | Android 广告服务主题，由 AdMob SDK 合并加入 |
| `android.permission.WAKE_LOCK` | 广告 SDK 在展示广告或视频时保持必要的唤醒状态 |
| `android.permission.FOREGROUND_SERVICE` | 广告 SDK 在特定场景下使用前台服务能力 |

## 7. 联系与更新 / Contact and Updates

如对本清单有疑问，请联系 `kawhijimmy@spielphantom.com`。第三方服务调整或新增 SDK 时，本清单将同步更新。

For questions about this list, contact `kawhijimmy@spielphantom.com`. This list will be updated when third-party services or SDKs change.
