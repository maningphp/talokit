# TaloKit 快速开始：下载、安装与首次使用

TaloKit 是 Windows、macOS 和 Linux 桌面开发者工具箱。请始终从 [官方网站下载区](https://www.talokit.com/#downloads) 获取最新版，避免使用来源不明的网盘或镜像。

## 1. 选择系统和架构

| 系统 | 如何选择 |
| --- | --- |
| Windows x64 | 绝大多数 Intel/AMD 处理器的 Windows 10/11 电脑 |
| Windows ARM64 | 使用 ARM 处理器的 Windows 11 设备 |
| macOS Intel | “关于本机”中显示 Intel 处理器 |
| macOS Apple Silicon | M1、M2、M3、M4 或更新的 Apple 芯片 |
| Linux x64 | Intel/AMD 64 位发行版，优先选 AppImage 或对应 deb |
| Linux ARM64 | ARM64 Linux 设备 |

不确定时，不要只根据操作系统名称猜测架构。Windows 可在“设置 → 系统 → 系统信息”查看系统类型；macOS 可在“苹果菜单 → 关于本机”查看芯片。

## 2. 安装

### Windows

下载 `win-x64-setup.exe` 或 `win-arm64-setup.exe`，运行安装程序并选择安装目录。尚未建立足够签名信誉的发行包可能触发系统或安全软件提示，应先核对下载来源和官网公布的 SHA-256，不要关闭系统整体安全防护。

### macOS

下载与芯片匹配的 DMG，打开后将 TaloKit 拖入“应用程序”。如果系统提示无法验证开发者，请核对官网说明、安装包名称和校验值，不要全局关闭 Gatekeeper。

### Linux

AppImage 需要执行权限：

```bash
chmod +x TaloKit-*-linux-*.AppImage
./TaloKit-*-linux-*.AppImage
```

Debian/Ubuntu 系也可选择官网提供的 `.deb` 包。

## 3. 首次使用

1. 使用顶部搜索输入工具名、格式名或任务，例如 `JSON`、`CIDR`、`Docker 日志`、`Kubernetes Deployment`。
2. 左侧导航按通用工具、容器云原生、数据库等场景组织；常用工具可加入收藏。
3. 免费工具可直接使用。需要 Pro 的功能会展示登录或订阅入口。
4. 重要内容处理完成后及时复制或导出。不要把桌面工具当作唯一的数据存储位置。

## 4. 更新

应用启动时会检查更新，并在发现新版本后提示。更新安装前可备份重要工作区内容。下载失败时可回到官网手动下载最新版。

## 5. 遇到问题

提交 Issue 时请提供：TaloKit 版本、操作系统与架构、安装包文件名、复现步骤、完整错误文字和已脱敏截图。不要提交账号密码、授权码、支付密钥、生产令牌或包含敏感内容的原始配置。
