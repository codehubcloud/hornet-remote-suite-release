# Hornet Remote Suite

Hornet Remote Suite 二进制安装包发布仓库，提供下载说明、版本说明和安装包。

当前最新版本为 **[0.0.36](https://github.com/codehubcloud/hornet-remote-suite-release/releases/tag/v0.0.36)**。

- **传输历史清除**：任务中心传输列表右键可清除单条记录，或批量清除已完成、已取消和失败记录；保留进行中、已暂停及冲突任务。
- **持久化与多窗口同步**：已清除的传输历史在刷新和重启后不会恢复，其他工作台窗口同步更新，传输文件保持不变。
- **日志清空**：日志页右键可清空当前日志，后续状态变化继续记录；刷新或切换页签不会回填已清空的日志。菜单支持 Shift+F10、方向键和 Esc。

其他功能：

- **快速命令**：命令栏、窗格、管理器、命令集、导入导出与快捷键；按钮支持纯色、线性/径向渐变、文字颜色、预设及预览，右键按钮即可编辑。
- **会话属性**：分类配置、相邻的用户名/密码和密码查看按钮；底部显示当前终端名称、主机、账号、协议、端口及用户填写的说明。每会话支持终端/键盘/外观/保活/目录/快速命令设置，可选择启用异常断线自动重连，不重发历史命令。
- **工具栏**：顶部右键可显示/隐藏菜单栏、标准按钮、地址栏、链接栏，解锁后调整顺序；修复隐藏菜单后无法右键重新勾选。
- **帮助**：F1 离线指南、离线生成 PDF、网站、技术支持、反馈、检查更新和关于。帮助正文提供中文/英文；其他界面语言使用英文正文。更新检查显示稳定版本与发布说明，支持失败重试，由用户选择下载安装包，不自动安装。

继续包含 SSH 断线提示、Xshell 风格标签菜单与分屏、加密保存密码、透明 Logo 和合并标题菜单、Ctrl＋滚轮字号缩放、大文件 SHA-256 校验优化及后台无响应退出保障。覆盖安装保留连接、分组和配置，无需删除数据库。

从 [Releases](https://github.com/codehubcloud/hornet-remote-suite-release/releases) 下载。首个版本为 **0.0.1**。

| 系统 | 架构 | 格式 |
| --- | --- | --- |
| Windows | x64 | EXE 安装程序 |
| macOS | Intel x64 / Apple Silicon ARM64 | DMG |
| Linux | x64 / ARM64 | AppImage、DEB |

请按系统和架构选择安装包，并用每个版本附带的 `SHA256SUMS` 核对 SHA-256。

Windows：`Get-FileHash <安装包路径> -Algorithm SHA256`。macOS：`shasum -a 256 <安装包路径>`；Linux：`sha256sum <安装包路径>`。

AppImage 下载后需赋予执行权限：`chmod +x <安装包路径>`。DEB 适用于 Debian/Ubuntu。

SSH/SFTP、FTP/FTPS、Telnet、会话管理、多语言和主题为通用能力。本地 PowerShell/CMD、串口、原生 RDP、VcXsrv 管理和系统打印提交目前使用 Windows 适配器；VcXsrv 需另行安装。尚未实现的 Xshell 功能仍显示为不可用，本软件不宣称完整覆盖其全部功能。

当前发行版未配置商业代码签名或 Apple 公证。

公开提供安装包不代表源码开源，也不授予开源许可；第三方组件按随附许可分发。问题反馈请使用本仓库的 [Issues](https://github.com/codehubcloud/hornet-remote-suite-release/issues)，不要包含密码、私钥或敏感日志。
