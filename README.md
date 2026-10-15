<p align="center"><img src="assets/nova-logo.svg" width="96" alt="Xyner Nova Logo"></p>

<h1 align="center">Xyner Nova</h1>

<p align="center">Android 多应用增强模块 · 界面定制 · 功能设置 · 云备份与共享</p>

<p align="center">
  <a href="https://github.com/ALittle-Cool/Xyner-Nova-Public/releases">下载与更新</a> ·
  <a href="https://github.com/ALittle-Cool/Xyner-Nova-Public/issues/new/choose">问题反馈</a> ·
  <a href="https://github.com/ALittle-Cool/Xyner-Nova-Public/discussions">交流问答</a> ·
  <a href="SUPPORT.md">使用帮助</a>
</p>

Xyner Nova 通过 Xposed 框架为已接入的 Android 应用提供界面与交互定制、实用功能和配置管理。各应用的功能独立设置，实际可用项目会随宿主版本、适配情况和账号权益变化。

本仓库是 Xyner Nova 的公开介绍、反馈交流与发行入口。项目目前处于内测阶段，下载 APK 后仍需符合应用内的账号与功能资格要求。

## 下载与版本

| 项目 | 信息 |
| --- | --- |
| 当前发行 | **0.1.24（25） · 内测** |
| 发布页 | [Xyner Nova 0.1.24](https://github.com/ALittle-Cool/Xyner-Nova-Public/releases/tag/v0.1.24) |
| APK 下载 | [Xyner-Nova-0.1.24.apk](https://github.com/ALittle-Cool/Xyner-Nova-Public/releases/download/v0.1.24/Xyner-Nova-0.1.24.apk) |
| 文件大小 | 19,613,089 字节（约 18.70 MiB） |
| 应用包名 | `cn.xyner.nova` |
| 最低系统 | Android 9（API 28） |
| 框架要求 | 兼容 Xposed 的运行环境；模块声明最低 Xposed API 93 |
| APK 架构 | arm64-v8a、armeabi-v7a、x86、x86_64 |
| 界面语言 | 中文 / English，跟随系统语言 |

SHA-256：

```text
575a4119410128686646d33b67795810c975e1cf0046a10472dff82c138dca78
```

可以使用发布附件中的 [SHA256SUMS.txt](https://github.com/ALittle-Cool/Xyner-Nova-Public/releases/download/v0.1.24/SHA256SUMS.txt) 核对 APK。请在 **Assets** 中下载 APK；GitHub 自动提供的 Source code 压缩包是本介绍仓库的文件。

## 主要功能

| 场景 | 功能举例 |
| --- | --- |
| 陌陌 | 防撤回与系统提示、媒体保存、定位、自动化发送、聊天气泡和底栏外观、主动 AI 工具 |
| 微信外观与交互 | 主页顶栏、头像形状、输入区外观、部分页面入口隐藏；以设置页展示的项目为准 |
| 抖音与抖音极速版 | 顶部 Tab 隐藏与排序、分享提示管理、快捷悬浮条等；两个应用分别适配 |
| 红果短剧 | 播放页面控件精简、播放手势、暂停控制与自动最高画质选项 |
| 云备份 | 创建和管理宿主设置、业务记录及关联资源备份，支持合并或覆盖恢复；需要云备份资格 |
| 共享社区 | 发布、搜索、预览、导入和撤回可共享的配置、规则及任务模板 |

新云备份排除音频和视频资源。每个资源压缩封装后最多 10 MiB，整份上传包最多 64 MiB。自动备份和红果自动最高画质默认关闭；社区导入的自动任务默认停用。

## 宿主接入范围

下面列出当前版本已注册的宿主范围。**接入范围不等于所有功能均可用，也不保证任意版本或分身环境都兼容**；请以应用内的功能列表、授权提示和适配结果为准。

| 应用 | 包名 |
| --- | --- |
| 微信 | `com.tencent.mm` |
| 陌陌 | `com.immomo.momo` |
| 抖音 | `com.ss.android.ugc.aweme` |
| 抖音极速版 | `com.ss.android.ugc.aweme.lite` |
| 红果短剧 | `com.phoenix.read` |
| 快手 | `com.smile.gifmaker` |
| 快手极速版 | `com.kuaishou.nebula` |
| 小红书 | `com.xingin.xhs` |
| 番茄小说 | `com.dragon.read` |
| 番茄畅听 | `com.xs.fm` |
| 百度贴吧 | `com.baidu.tieba` |
| 七猫免费小说 | `com.kmxs.reader` |
| 盐言故事 | `com.zhihu.vip.android` |
| 多邻国 | `com.duolingo` |
| ES 文件浏览器 | `com.estrongs.android.pop` |
| 皮皮虾 | `com.sup.android.superb` |
| 皮皮搞笑 | `cn.xiaochuankeji.zuiyouLite` |
| 最右 | `cn.xiaochuankeji.tieba` |
| 西瓜视频 | `com.ss.android.article.video` |
| Soul | `cn.soulapp.android` |
| TikTok | `com.zhiliaoapp.musically` |

## 安装与使用

1. 从 [Releases](https://github.com/ALittle-Cool/Xyner-Nova-Public/releases) 下载 APK，并安装或覆盖更新 Xyner Nova。
2. 在已正确安装的 Xposed / LSPosed 环境中启用模块，为需要使用的宿主勾选作用域。设备是否需要 Root、框架如何安装，以所用框架的官方说明为准。
3. 打开 Nova，按应用内提示登录并完成资格确认。符合条件的旧账号可从登录页提交内测申请并查询审核结果；申请条件以页面提示为准。
4. 彻底结束需要使用的宿主应用，再重新打开；进入该宿主的 Nova 设置入口，按需启用功能。
5. 更新模块后如提示仍加载旧版本，确认框架启用了当前 Nova，再彻底结束并重开宿主。更多排查步骤见 [使用帮助](SUPPORT.md)。

## 最新更新

0.1.24：

- [适配] 新增陌陌支持，按需开启各项功能。
- [新增] 陌陌防撤回、聊天流撤回提示、精确消息时间，以及语音、头像、动态视频保存。
- [新增] 陌陌阻止发送已读回执、好友和群组群发、关键词自动回复；支持文字、图片、视频和语音，每条关键词规则可单独设置冷却时间。
- [新增] 陌陌定时发送支持单次、每天、周一至周五、周末、自选星期、倒计时与固定间隔循环。目标选择支持头像、备注、群聊及批量选择。
- [新增] 陌陌虚拟定位、地图选点及账号独立定位；支持去广告、隐藏底栏与动态中的直播入口。
- [新增] 陌陌自定义聊天气泡颜色、圆角与图片，可分别调整上下留白及相邻消息间距；支持底栏文字、图标大小和颜色设置。
- [新增] 陌陌主动 AI 回复建议、聊天总结、翻译与润色，先预览再生成，结果不会自动发送。
- [新增] 首页问题反馈入口，便于提交使用问题。
- [修复] 陌陌私人云备份恢复位置、功能开关及自动化规则；恢复的定时任务保持暂停。
- [优化] 授权无法发起时提供“打开 Nova”和“原方式授权”入口，改善模块不可见时的提示体验。

使用说明：更新后请在框架中勾选陌陌作用域，并彻底结束、重新打开需要使用的宿主。AI 需自行配置可用服务；语音转文字、聊天图片高清加载及视频倍速暂为试验功能。定时发送需保持陌陌进程运行；周一至周五不判断法定节假日调休。

完整版本说明与下载文件见 [全部 Releases](https://github.com/ALittle-Cool/Xyner-Nova-Public/releases)。

## 反馈与交流

- **故障反馈**：[提交 Bug](https://github.com/ALittle-Cool/Xyner-Nova-Public/issues/new?template=bug_report.yml)，提供版本、复现步骤与实际表现。
- **版本兼容**：[提交宿主适配反馈](https://github.com/ALittle-Cool/Xyner-Nova-Public/issues/new?template=compatibility_report.yml)，注明宿主包名、版本和设备环境。
- **功能建议**：[提交建议](https://github.com/ALittle-Cool/Xyner-Nova-Public/issues/new?template=feature_request.yml)，描述使用场景与期望效果。
- **使用问答**：[Q&A](https://github.com/ALittle-Cool/Xyner-Nova-Public/discussions/categories/q-a)；**设置经验与分享**：[Discussions](https://github.com/ALittle-Cool/Xyner-Nova-Public/discussions)。
- **交流导航**：[欢迎交流与反馈指引](https://github.com/ALittle-Cool/Xyner-Nova-Public/discussions/2)；**本版本交流**：[0.1.24 讨论](https://github.com/ALittle-Cool/Xyner-Nova-Public/discussions/4)。

反馈前请搜索已有话题；截图和报告请先移除账号凭据、联系方式与聊天内容。查看 [反馈说明](SUPPORT.md) 和 [安全问题报告方式](SECURITY.md)。

维护者：[ALittle-Cool](https://github.com/ALittle-Cool)。可以在仓库的 **Watch → Custom** 中订阅 Releases，接收版本发布通知。
