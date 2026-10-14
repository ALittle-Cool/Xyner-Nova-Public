# 使用帮助与反馈

下载与更新见 [Releases](https://github.com/ALittle-Cool/Xyner-Nova-Public/releases)。项目当前处于内测，登录、申请、功能权益和云备份资格以应用内提示为准。

## 常见问题

**安装后为什么没有功能？**

确认 Xposed / LSPosed 已正常工作、Nova 已启用，并勾选当前宿主作用域；彻底结束宿主后重新打开。普通抖音与极速版需要分别选择。随后检查登录状态、功能开关及适配提示。

**更新后提示模块版本不一致？**

确认框架启用的是新安装的 Nova，彻底结束宿主后重开。请保留应用数据；先按提示重新授权，不要把卸载或清空数据作为第一步。

**下载了 Source code 为什么不能安装？**

安装包是 Release 的 Assets 中以 `.apk` 结尾的附件。Source code 是公开介绍资料压缩包。

**为什么设置页没有某项功能？**

功能入口受宿主版本、适配状态与账号权益影响；部分高等级功能未授权时不会展示。注册的宿主范围不等于所有版本和功能均已验证。

**云备份会包含所有文件吗？**

备份保存允许导出的设置、业务记录与关联资源；新备份不包含音频、视频资源和账号凭据。共享配置会移除私人信息，导入的自动任务默认关闭。恢复前请看清合并或覆盖选项。

## 选择反馈入口

| 需求 | 入口 |
| --- | --- |
| 功能错误、崩溃、显示异常 | [Bug 反馈](https://github.com/ALittle-Cool/Xyner-Nova-Public/issues/new?template=bug_report.yml) |
| 某个宿主或版本不兼容 | [宿主适配反馈](https://github.com/ALittle-Cool/Xyner-Nova-Public/issues/new?template=compatibility_report.yml) |
| 新功能或交互建议 | [功能建议](https://github.com/ALittle-Cool/Xyner-Nova-Public/issues/new?template=feature_request.yml) |
| 安装使用问题、经验分享 | [Discussions](https://github.com/ALittle-Cool/Xyner-Nova-Public/discussions) |
| 安全漏洞 | [私密报告方式](SECURITY.md) |

一个问题使用一个话题。请提供 Nova 版本、宿主名称／包名／版本、Android 版本、框架版本、复现步骤和预期／实际结果。可附脱敏截图或应用提供的适配报告；不要上传完整聊天记录、数据库、备份包、密码、令牌或签名密钥。
