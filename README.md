# 拾留 PomeKeep

Windows 本地资料收集与找回工具，提供剪贴板历史、截图标注、录屏、轻量笔记、OCR 与关键词搜索。

本仓库用于发布安装包、更新包和接收反馈，应用源代码保留在私有仓库。GitHub 自动显示的 “Source code” 压缩包仅包含本发布仓库的 README，不包含应用源码。

## 下载

- [最新正式版本](https://github.com/wmousew/PomeKeep-Releases/releases/latest)
- [2.5.1 安装包](https://github.com/wmousew/PomeKeep-Releases/releases/download/v2.5.1/PomeKeep-2.5.1-windows-x64-setup.exe)
- [2.5.1 便携包](https://github.com/wmousew/PomeKeep-Releases/releases/download/v2.5.1/PomeKeep-2.5.1.zip)

安装版运行安装包；便携版完整解压后运行根目录 `PomeKeep.exe`，保留 `app`、`update` 和更新后生成的 `rollback` 目录。

## 2.5.1 更新

- 新增“帮助与反馈”：离线使用说明、QQ/微信联系方式、公开 Issues 入口。
- 支持用户主动预览并导出诊断报告，无自动上传，不含采集内容和日志原文。
- 修复更新准备完成后客户端自行取消的问题。
- 下载时显示进度条、百分比和已下载/总大小，异常退出显示错误信息。

**2.4.0 / 2.4.1 用户如果遇到自动更新自行取消，请下载 2.5.1 安装包升级并保留个人数据。** 2.3.x 及更早版本也需要使用安装包切换目录布局。

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
