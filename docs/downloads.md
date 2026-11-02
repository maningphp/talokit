# TaloKit 下载、文件校验与更新

## 官方下载

唯一推荐入口：<https://www.talokit.com/#downloads>

下载页提供 Windows、macOS 和 Linux 的 x64/ARM64 选项，并根据浏览器报告的系统给出默认推荐。系统识别可能受浏览器和兼容模式影响，最终应以设备真实架构为准。

## 为什么不在本仓库存放安装包

Git 仓库不适合存放持续替换的大型二进制文件，也容易造成下载来源混乱。本仓库只保存公开文档和截图；最新版安装包由官网统一分发。

## SHA-256 校验

官网发布清单会提供安装包 SHA-256。下载后可按系统校验：

Windows PowerShell：

```powershell
Get-FileHash .\TaloKit-安装包文件名.exe -Algorithm SHA256
```

macOS：

```bash
shasum -a 256 TaloKit-安装包文件名.dmg
```

Linux：

```bash
sha256sum TaloKit-安装包文件名.AppImage
```

结果不一致时不要运行文件，应删除并重新从官网下载。

## 更新

TaloKit 每次启动时检查是否存在新版；只有发现更新时才提示。更新包仍来自官方发布地址。需要保留旧版本时，可自行归档安装包和对应 SHA-256，但官网默认只提供最新版本。
