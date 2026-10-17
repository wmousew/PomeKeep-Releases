# 拾留 PomeKeep

Windows 本地资料收集与找回工具，提供剪贴板历史、截图标注、录屏、轻量笔记、OCR 与关键词搜索。

本仓库用于发布安装包、更新包和接收反馈，应用源代码保留在私有仓库。GitHub 自动显示的 “Source code” 压缩包仅包含本发布仓库的 README，不包含应用源码。

## 下载

- [最新正式版本](https://github.com/wmousew/PomeKeep-Releases/releases/latest)
- [2.5.2 安装包](https://github.com/wmousew/PomeKeep-Releases/releases/download/v2.5.2/PomeKeep-2.5.2-windows-x64-setup.exe)
- [2.5.2 便携包](https://github.com/wmousew/PomeKeep-Releases/releases/download/v2.5.2/PomeKeep-2.5.2.zip)

安装版运行安装包；便携版完整解压后运行根目录 `PomeKeep.exe`，保留 `app`、`update` 和更新后生成的 `rollback` 目录。

## 2.5.2 更新

- 精简顶部信息，移除重复的版本展示与更新入口；查看版本、检查更新统一在「设置 → 常规」中操作。
- 将 QQ群、微信、GitHub 提交反馈和查看更新说明统一放在页面底部，为帮助内容腾出更多阅读空间。
- 点击 QQ群或微信按钮即可复制号码，左下角显示成功提示，约 2.5 秒后自动消失。
- 切换「快速上手」「常见问题」「诊断报告」时，底部按钮保持位置，方便随时联系与反馈。

**2.4.0 / 2.4.1 用户如果遇到自动更新自行取消，请下载 2.5.2 安装包升级并保留个人数据。** 2.3.x 及更早版本也需要使用安装包切换目录布局。

## 自动更新

设置 → 常规 →「自动更新」：开启后启动时后台检测、下载并准备更新。红点表示更新已准备好，点击版本号完成切换。关闭后，仅在点击版本号时检测、下载并更新。

- 每个版本使用一个完整更新包，由客户端本地比较变化文件，支持跨版本升级。
- 未变化的 DLL 和模型继续使用原文件，只保留最近一次更新的差异回退资料。
- 更新包使用签名验证，试启动失败或更新中断时恢复旧版。
- 个人数据位于 `%APPDATA%/pomekeep`，升级保留数据；本版数据库 Schema 仍为 8。

普通用户选择安装包或便携包即可。`update.json`、`update.sig` 和 update ZIP 供客户端使用；`SHA256SUMS.txt` 提供文件校验信息。

## 帮助与反馈

软件内设置 →「帮助与反馈」可查看使用说明并导出诊断报告。

- QQ 交流群：**460575997**
- 微信：**mouse_zxc**
- [公开 Issues](https://github.com/wmousew/PomeKeep-Releases/issues)：请提供软件版本、Windows 版本和复现步骤。

上传截图和日志前，请确认没有需要保密的内容。

## 测试版（可选）

- [当前测试版 2.5.3-beta.1](https://github.com/wmousew/PomeKeep-Releases/releases/tag/v2.5.3-beta.1)
- [测试更新渠道](https://github.com/wmousew/PomeKeep-Releases/releases/tag/beta)

测试版与正式版分别安装，资料不会自动同步。测试版数据保存在 `%APPDATA%/pomekeep-beta`。首次下载安装测试版，后续通过程序内更新。两版默认快捷键相同，建议退出另一版后使用或分别配置。
