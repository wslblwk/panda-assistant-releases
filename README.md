# 熊猫助手 · 发布产物

本仓库**只存放**熊猫助手桌面版的发布产物，不包含源代码。

- `latest.json`：自动更新清单（版本号、下载地址、大小、SHA-256、更新说明）
- `PandaAssistant-<版本>-win-x64.zip`：绿色版程序包
- `SHA256SUMS.txt`：安装包校验值

源码仓库为私有；客户端只从本仓库的 Release 读取更新。

## 给用户

下载最新 Release 里的 zip，解压到新文件夹即可。旧版数据会从同级旧目录或 `%APPDATA%` 自动迁移；也可以手动把 `data`、`images`、`game-assets` 复制到新文件夹。
