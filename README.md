# cyber漫剧

Windows x64 安装包与正式更新发布仓库。

[下载最新版](https://github.com/shiyu54/cyber-manju-releases/releases/latest) · [全部版本](https://github.com/shiyu54/cyber-manju-releases/releases)

## 安装与更新

1. 从 Releases 下载 `cyber-manju-版本号-win-x64-setup.exe`。
2. 等待图片、视频等生成任务结束，保存项目并正常退出 cyber漫剧。
3. 运行安装包。覆盖安装时确认安装目录与现有 cyber漫剧目录一致。
4. 启动软件，在“设置 → 关于”中检查版本。

从 v1.2.1 起，软件从本仓库的 GitHub Releases 检查正式更新。发现新版本后可在软件内下载安装包，下载完成会核对大小与 SHA-256。点击“查看安装包”，正常退出软件后双击安装包进行更新。

自动检查可在设置中关闭；关闭后不执行启动或定时检查，仍可手动检查。检查更新无需登录原厂账号，不会自动退出软件或中断生成任务。

## 发行配置

- 只预置“聚合中转 8877（自建）”供应商，API Key 为空，由用户自行填写。
- 不附带米核、Ark 或聚合中转供应商插件包，不会自动导入这些插件。
- 图片、视频模型需要相应适配器时，请手动导入兼容插件，并确认所用 Key 已获得模型权限。
- 保留通用插件管理、程序内置适配器与 Agent 功能；原厂软件更新、官方插件在线更新及官方插件更新缓存加载已关闭。
- 安装包不包含用户项目、账号数据或用户配置。覆盖安装保留本机已有配置，因此已有电脑可能继续显示原来保存的密钥。

本仓库只提供发行文件与说明，不包含应用项目源码。第三方组件的版权与许可见安装目录随附文件。

## 更新文件

每个正式 Release 包含：

- Windows 安装包；
- `cyber-update.json`：应用标识、版本、更新说明、安装包地址、字节数与 SHA-256；
- `SHA256SUMS.txt`：供手动校验的哈希；
- 安装说明。

固定检查地址：

`https://github.com/shiyu54/cyber-manju-releases/releases/latest/download/cyber-update.json`

仅使用 GitHub Releases，不需要额外更新服务器。访问速度取决于用户网络到 GitHub 的连通情况。
