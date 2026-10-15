# 拾留 PomeKeep

Windows 本地资料收集与找回工具，提供剪贴板历史、截图标注、录屏、轻量笔记、OCR 与关键词搜索。

本仓库用于发布安装包、更新包和接收反馈。应用源代码保留在私有仓库。

## 下载

- [最新正式版本](https://github.com/wmousew/PomeKeep-Releases/releases/latest)
- [2.4.0 安装包](https://github.com/wmousew/PomeKeep-Releases/releases/download/v2.4.0/PomeKeep-2.4.0-windows-x64-setup.exe)
- [2.4.0 便携包](https://github.com/wmousew/PomeKeep-Releases/releases/download/v2.4.0/PomeKeep-2.4.0.zip)

安装版运行安装包；便携版完整解压后运行根目录的 `PomeKeep.exe`，保留 `app`、`update` 和更新后生成的 `rollback` 目录。

## 自动更新

2.4.0 起，在「设置 → 常规」开启「自动更新」，启动后在后台检测、下载并准备更新。红点表示更新已准备好，点击版本号完成切换。

关闭自动更新后，仅在点击版本号时检测、下载并更新。后台下载期间点击版本号会接续已有任务。

- 每个版本发布一个完整更新包，客户端本地比较变化文件，支持跨版本升级。
- 只保留最近一次更新的差异回退资料；未变化的 DLL 和模型不重复保存。
- 更新包和版本清单使用签名验证。
- 2.3.x 及更早版本首次切换新布局需要使用安装包升级；用户数据位于 `%APPDATA%/pomekeep`，升级保留数据。
- 2.4.0 已正式发布供在线更新验证，自动化及实机更新、回退验收尚未完成。当前安装的版本与最新版本相同时显示「已是最新版本」；完整替换更新需要更高版本触发。

Release 中的 `update.json`、`update.sig` 和 update ZIP 供客户端使用；普通用户选择安装包或便携包即可。`SHA256SUMS.txt` 提供文件完整性校验信息。

## 反馈

请通过 [Issues](https://github.com/wmousew/PomeKeep-Releases/issues) 提交问题，注明软件版本、Windows 版本和复现步骤。上传截图和日志前，请确认没有需要保密的内容。
