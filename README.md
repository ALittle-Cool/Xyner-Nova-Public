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
| 当前发行 | **0.1.32（33） · 内测** |
| 发布页 | [Xyner Nova 0.1.32](https://github.com/ALittle-Cool/Xyner-Nova-Public/releases/tag/v0.1.32) |
| APK 下载 | [Xyner-Nova-0.1.32.apk](https://github.com/ALittle-Cool/Xyner-Nova-Public/releases/download/v0.1.32/Xyner-Nova-0.1.32.apk) |
| 文件大小 | 21,599,159 字节（约 20.60 MiB） |
| 应用包名 | `cn.xyner.nova` |
| 最低系统 | Android 9（API 28） |
| 框架要求 | 兼容 Xposed 的运行环境；模块声明最低 Xposed API 93 |
| APK 架构 | arm64-v8a、armeabi-v7a、x86、x86_64 |
| 界面语言 | 中文 / English，跟随系统语言 |

SHA-256：

```text
e3d87c650bec821198502067dc77bd001fb15a378ace552554414a97e9f07153
```

可以使用发布附件中的 [SHA256SUMS.txt](https://github.com/ALittle-Cool/Xyner-Nova-Public/releases/download/v0.1.32/SHA256SUMS.txt) 核对 APK。请在 **Assets** 中下载 APK；GitHub 自动提供的 Source code 压缩包是本介绍仓库的文件。

## 主要功能

| 场景 | 功能举例 |
| --- | --- |
| 陌陌 | 防撤回与系统提示、媒体保存、定位、自动化发送、聊天气泡和底栏外观、主动 AI 工具 |
| 微信 | 主页顶栏与浮动底栏、头像与输入区外观、密友隐藏、朋友圈关键词及好友选择、自动任务管理；朋友圈防撤回、评论防撤回及本机缓存可见性提供独立开关，真实删除／撤回效果待验证 |
| 抖音与抖音极速版 | 顶部 Tab 与分享提示、Live 图集保存、快捷悬浮条、倍速与手势、私聊／评论语音替换及社区语音来源、收藏语音分享到素材社区，两个应用分别适配 |
| Soul | 虚拟定位与地图收藏、动态筛选／自动点赞、自定义注册徽章、私聊／群聊防撤回与隐私、语音收藏／替换／文字转语音、气泡与聊天玩法、会话管理及消息自动化、相册与资料工具、瞬间／评论素材；部分选项待更多样本确认 |
| TikTok | 地区与匹配运营商、无水印保存与下载限制解除、自动倍速与翻页、内容筛选、双击与长按控制、沉浸式全屏、顶部频道及拍摄入口隐藏、原生预留间距移除、本人主页本地计数；广告／升级／插入拦截选项仍待实际样本确认 |
| 百度贴吧 | 自动签到与新关注补签，支持账号和日期隔离 |
| 红果短剧 | 右侧控件、上下控件与全屏按钮分别隐藏，播放手势、暂停控制与自动最高画质选项 |
| 快手与快手极速版 | 无水印图片／视频保存、解除普通视频下载限制、首页／发现与精选推荐筛选 |
| Nova 更新 | 新版提醒、手动检查、跨宿主提醒同步、后台下载与断点续传、另存安装包 |
| 云备份 | 创建和管理宿主设置、业务记录及关联资源备份，支持合并或覆盖恢复；需要云备份资格 |
| 共享社区 | 发布、搜索、预览、导入和撤回可共享的配置、规则及任务模板 |
| 素材社区 | 图片／表情／语音分类、搜索、预览、评论、点赞与收藏；支持宿主选用和收藏语音分享，发布／下载／完整预览／试听需云备份资格 |

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

0.1.32：

本版为内测预发布，新增 Soul 功能与素材社区。更新后请彻底结束并重开需要使用的宿主。Soul 按官方 6.38.0 适配，新功能默认关闭，按需开启。

- [新增] Soul 虚拟定位，支持地图选点、地点与城市搜索、普通／卫星图层、常用位置收藏；位置及收藏支持私人云备份。
- [新增] Soul 去广告、更新与青少年提醒拦截、进入前台清除通知、关闭匹配背景音乐、禁用智能打招呼和关闭挚友邀请等选项。
- [新增] Soul 动态筛选和自动点赞，两套条件独立设置，支持多关键词、性别、注册天数、VIP／SSR、关注关系、在线状态和内容类型等筛选。
- [新增] Soul 作者昵称、注册天数徽章和外观自定义，支持恢复默认样式；提供本地分享限制解除及隐身小助手作者入口。查看隐身小助手作者需等级 ≥3，并显示“个性”标识。
- [新增] Soul 瞬间与聊天语音的下载、收藏、试听、进度控制和链接复制；收藏显示可取得的作者头像、昵称、备注和收藏时间。
- [新增] Soul 聊天录音及瞬间、评论语音替换，支持本地文件、收藏语音和社区语音、完整导入瞬间语音；选用评论语音可直接评论。
- [新增] Soul 聊天、瞬间及评论文字转语音，复用 Fish Audio；聊天支持自定义前缀，默认 #，并可选择发送前试听。
- [新增] Soul 私聊／群聊防撤回、独立撤回提示和自定义文案、聊天时间显示间隔，以及本人消息的本地撤回时限选项；撤回结果仍受 Soul 服务规则影响。
- [新增] Soul 聊天图片和表情保存、图片／视频预览、消息详情，以及文字、图片、视频、语音转发。
- [新增] Soul 本机文字显示编辑，退出聊天或重开后保留，可手动恢复原文。该功能需等级 ≥3，资格不足时隐藏，并显示“个性”标识；仅改变本机显示。
- [新增] Soul 清除未读、扩展会话列表、隐藏选定会话及收到新消息时恢复隐藏；提供关键词回复、定时发送、好友和群组群发。
- [新增] Soul 阻止已读回执、隐藏输入状态、隐藏关注按钮、屏蔽轻互动、推荐表情及自动拒接语音来电等聊天选项。
- [新增] Soul 自定义私聊气泡及静态／动态预览，支持全局与单聊选择；自选骰子、猜拳和发送类工具位于输入栏笑脸长按菜单，轻点保持原生操作；支持回车发送。
- [新增] Soul 相册多选与时长扩展、原图／编辑／拍摄入口，公开资料复制及头像／背景浏览保存、校园吧主页入口、本地登录数量限制与 VIP 显示选项、自动签到、上线隐身和本人主页本地计数。
- [新增] Soul 语音房消息尾巴、彩色文字、自动欢迎，群聊彩色文字及聊天话题卡文案编辑；提供手动批量取消关注、调整本人瞬间可见范围、主页动态批量下载和点赞。
- [新增] 素材社区支持图片、表情和语音分类、搜索、发现／收藏／我的、评论、点赞与收藏；可在全局服务中打开，并供 Soul 相关聊天、瞬间及评论功能选用。
- [新增] Soul、抖音与抖音极速版的收藏语音支持“分享到素材社区”，带入可编辑标题，由用户确认发布；抖音两版的私聊和评论语音替换支持社区语音来源。
- [优化] 素材社区列表、缩略图、预览和下载缓存，重复使用及重开宿主时复用已验证素材；不同宿主和账号分别隔离，支持手动刷新。
- [优化] Soul 设置整理为五个顶级分类及二三级菜单；多关键词改为逐条新增、编辑和删除，相关设置纳入相应云备份范围。
- [修复] Soul 部分发送操作需重进聊天才显示、发送状态持续转圈、气泡样式延迟更新和群语音重复显示的问题；修复会话工具导致列表异常或旧会话重新出现的问题。
- [修复] Fish Audio 中转试听暂时不可用，以及模块检查更新只闪一下、结果不显示的问题；改善更新弹窗的内容滚动和按钮布局。
- [调整] LSPosed 推荐作用域移除旧 Xyner 工具。

素材社区规则：所有用户可浏览素材列表；发布、下载、完整预览和语音试听需要云备份权限。普通用户每份素材不超过 1MiB，默认每天可分享 10 份；无云备份权限用户可点赞、收藏，评论默认关闭，以当前规则为准。发布违法违规内容将直接封禁整个 Nova 账号。

验证范围：已完成多项 Soul 私聊／群聊、定位、筛选、语音、气泡、会话管理及社区流程的实机核对。每日签到、本地 VIP 显示、部分提醒拦截、旧楼层评论广告过滤、聊天话题卡、部分批量／定时操作、瞬间话题前缀转换，以及抖音两版新增收藏分享的完整发布仍待更多样本确认；本地撤回时限选项不保证服务器接受。请按应用内权限和适配结果使用。

完整版本说明与下载文件见 [全部 Releases](https://github.com/ALittle-Cool/Xyner-Nova-Public/releases)。

## 反馈与交流

- **故障反馈**：[提交 Bug](https://github.com/ALittle-Cool/Xyner-Nova-Public/issues/new?template=bug_report.yml)，提供版本、复现步骤与实际表现。
- **版本兼容**：[提交宿主适配反馈](https://github.com/ALittle-Cool/Xyner-Nova-Public/issues/new?template=compatibility_report.yml)，注明宿主包名、版本和设备环境。
- **功能建议**：[提交建议](https://github.com/ALittle-Cool/Xyner-Nova-Public/issues/new?template=feature_request.yml)，描述使用场景与期望效果。
- **使用问答**：[Q&A](https://github.com/ALittle-Cool/Xyner-Nova-Public/discussions/categories/q-a)；**设置经验与分享**：[Discussions](https://github.com/ALittle-Cool/Xyner-Nova-Public/discussions)。
- **交流导航**：[欢迎交流与反馈指引](https://github.com/ALittle-Cool/Xyner-Nova-Public/discussions/2)；**本版本交流**：[0.1.32 讨论](https://github.com/ALittle-Cool/Xyner-Nova-Public/discussions/37)。

反馈前请搜索已有话题；截图和报告请先移除账号凭据、联系方式与聊天内容。查看 [反馈说明](SUPPORT.md) 和 [安全问题报告方式](SECURITY.md)。

维护者：[ALittle-Cool](https://github.com/ALittle-Cool)。可以在仓库的 **Watch → Custom** 中订阅 Releases，接收版本发布通知。
