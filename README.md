# 拾留 PomeKeep

Windows 本地资料收集与找回工具，提供剪贴板历史、截图标注、录屏、轻量笔记、OCR 与关键词搜索。

本仓库用于发布安装包、更新包和接收反馈，应用源代码保留在私有仓库。

## 下载

- [最新正式版本](https://github.com/wmousew/PomeKeep-Releases/releases/latest)
- [2.4.1 安装包](https://github.com/wmousew/PomeKeep-Releases/releases/download/v2.4.1/PomeKeep-2.4.1-windows-x64-setup.exe)
- [2.4.1 便携包](https://github.com/wmousew/PomeKeep-Releases/releases/download/v2.4.1/PomeKeep-2.4.1.zip)

安装版运行安装包；便携版完整解压后运行根目录 `PomeKeep.exe`，保留 `app`、`update` 和更新后生成的 `rollback` 目录。

## 自动更新

设置 → 常规 →「自动更新」：开启后启动时后台检测、下载并准备更新。红点表示更新已准备好，点击版本号完成切换。关闭后，仅在点击版本号时检测、下载并更新。

- 每个版本使用一个完整更新包，由客户端本地比较变化文件，支持跨版本升级。
- 未变化的 DLL 和模型继续使用原文件，只保留最近一次更新的差异回退资料。
- 更新包使用签名验证，试启动失败或更新中断时恢复旧版。
- 2.4.0 用户可直接更新到 2.4.1；2.3.x 及更早版本首次切换目录布局需要使用安装包。
- 个人数据位于 `%APPDATA%/pomekeep`，升级保留数据。

2.4.1 修复了 Windows 更新 ZIP 路径、空目录及重复更新器交接问题，并补充了自动下载、差异替换和失败回退测试。验收范围见 Release 附带的更新功能验收报告。

普通用户选择安装包或便携包即可。`update.json`、`update.sig` 和 update ZIP 供客户端使用；`SHA256SUMS.txt` 提供文件校验信息。

## 反馈

请通过 [Issues](https://github.com/wmousew/PomeKeep-Releases/issues) 提交软件版本、Windows 版本和复现步骤。上传截图和日志前，请确认没有需要保密的内容。
