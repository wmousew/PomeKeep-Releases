# 拾留 PomeKeep

Windows 本地资料收集与查找工具，提供剪贴板历史、截图标注、录屏、轻量笔记、OCR 和关键词搜索。

本仓库仅用于公开说明和发布附件。应用源码保存在私有仓库。GitHub 自动生成的 Source code 压缩包仅包含本仓库的 README，不包含应用源码。

## 下载

- [最新正式版本](https://github.com/wmousew/PomeKeep-Releases/releases/latest)
- [2.5.4 安装包](https://github.com/wmousew/PomeKeep-Releases/releases/download/v2.5.4/PomeKeep-2.5.4-windows-x64-setup.exe)
- [2.5.4 便携包](https://github.com/wmousew/PomeKeep-Releases/releases/download/v2.5.4/PomeKeep-2.5.4.zip)

安装包运行安装；便携包完整解压后，运行根目录 `PomeKeep.exe`。请保留 `app`、`update` 及更新后生成的 `rollback` 目录。

## 2.5.4 更新

- 截图工具栏“更多 → 复制文字（OCR）”：识别当前选区和标注，查看、修改后复制。
- 新增半透明荧光笔（H），支持颜色与线宽记忆、撤销重做及历史编辑。
- 搜索关键词高亮、命中摘要、命中来源和预览定位；优化大量记录下的查询响应。
- [完整更新说明](https://github.com/wmousew/PomeKeep-Releases/releases/tag/v2.5.4)

**本次涉及数据库结构升级，请使用安装包升级。** 旧版自动更新入口会提示改用安装包。安装时保留用户数据，首次启动创建升级前数据库快照，再迁移到 schema 9。需要退回旧版时，先备份当前资料并恢复升级前快照；旧版不能直接打开新版数据库。

## 自动更新

在“设置 → 常规”开启自动更新，可在后台检查并准备兼容的替换更新；准备完成后出现红点，点击版本号执行更新。关闭自动更新后，点击版本号再检查。特殊升级会提示使用安装包。

- 每版发布完整更新包，客户端本地比较文件；相同结构版本支持跨版本替换。
- 未变化的文件继续使用，只保留最近一次更新的差异回退文件。
- 更新清单使用签名校验；兼容的替换更新启动失败或中断时恢复旧程序。
- 用户资料位于 `%APPDATA%/pomekeep`，与程序目录分开。卸载默认保留资料，主动勾选删除后才删除。

普通用户选择安装包或便携包即可。`update.json`、`update.sig` 和 update ZIP 供客户端使用；`SHA256SUMS.txt` 提供文件校验信息。

## 帮助与反馈

在“设置 → 帮助与反馈”查看使用说明、常见问题和诊断报告。

- QQ 交流群：**460575997**
- 微信：**mouse_zxc**
- [提交反馈](https://github.com/wmousew/PomeKeep-Releases/issues)：请提供软件版本、Windows 版本和复现步骤。上传截图或日志前，请确认没有需要保密的内容。

## 测试版（可选）

- [当前公开测试版 2.5.3-beta.3](https://github.com/wmousew/PomeKeep-Releases/releases/tag/v2.5.3-beta.3)
- [测试更新渠道](https://github.com/wmousew/PomeKeep-Releases/releases/tag/beta)

测试版与正式版分开安装，资料不合并、不自动同步。测试版数据位于 `%APPDATA%/pomekeep-beta`。首次下载安装测试版，后续可在测试版内更新。两版默认快捷键相同，建议退出另一版后使用或分别设置。
