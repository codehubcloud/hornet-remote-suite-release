# Hornet Remote Suite

Hornet Remote Suite 二进制安装包发布仓库。项目源码保留在私有仓库，本仓库只包含下载说明、版本说明与校验文件。

当前最新版本为 **[0.0.5](https://github.com/codehubcloud/hornet-remote-suite-release/releases/tag/v0.0.5)**。补齐后台无响应时的退出保障：关闭提示不再等待后台查询，取消后继续运行；确认退出后清理最多等待 5 秒，避免后台或界面卡住时迟迟无法退出。

包含 0.0.4 的后台存活检测、SFTP 错误处理和大文件完整 SHA-256 校验优化：服务器支持时在远端计算摘要，上传后无需回下载整个文件；不支持时自动回退流式校验。继续包含终端复制/粘贴、右键菜单及历史数据库启动兼容性修复；覆盖安装即可，原有连接与配置保留，不需要删除数据库。

从 [Releases](https://github.com/codehubcloud/hornet-remote-suite-release/releases) 下载，首个版本为 **0.0.1**。

| 系统 | 架构 | 格式 |
| --- | --- | --- |
| Windows | x64 | EXE 安装程序 |
| macOS | Intel x64 / Apple Silicon ARM64 | DMG |
| Linux | x64 / ARM64 | AppImage、DEB |

请按系统和架构选择安装包，并用每个版本附带的 `SHA256SUMS` 核对 SHA-256。

Windows：`Get-FileHash <安装包路径> -Algorithm SHA256`。

macOS：`shasum -a 256 <安装包路径>`；Linux：`sha256sum <安装包路径>`。

AppImage 下载后需要赋予执行权限：`chmod +x <安装包路径>`。DEB 适用于 Debian/Ubuntu 系统。

SSH/SFTP、FTP/FTPS、Telnet、会话管理、多语言和主题为通用能力。当前原生 RDP、VcXsrv 管理、本地 PowerShell/CMD、串口及系统打印提交使用 Windows 专用适配器。VcXsrv 不随安装包分发，需自行安装。

当前发行版未配置商业代码签名或 Apple 公证。

公开提供安装包不代表项目源码开源，也不授予开源许可；第三方组件按随附许可分发。问题反馈请使用本仓库的 Issues。
