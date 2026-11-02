# GitHub 推广仓库配置与维护

此仓库用于 TaloKit 商业软件的产品展示、公开文档与反馈，不包含应用源码，也不代表应用按开源许可证分发。

## 检查发现与本轮改造

| 原有情况 | 增量处理 |
| --- | --- |
| 中文首屏已有平台标识、截图和官网链接 | 保留结构，明确产品标题，补功能、入门、最新版和 Release 入口 |
| 英文版比中文版简略，缺版本范围和部分截图 | 对齐平台、专业工具边界、能力限制、FAQ 和文档导航 |
| 最新客户端版本没有统一维护来源 | 以官网下载区为准，不硬编码版本，不使用会暗示已有 Release 的徽章 |
| 文档以功能介绍为主 | 保留旧路径，补教程索引，先深化已有 JSON/Base64 入门 |
| 缺 Social Preview | 用现有品牌图标制作排版式宣传图；不伪造软件截图 |

## Repository About

仓库首页右侧 **About → 齿轮** 中设置：

**Description**

```text
Offline-first developer toolkit for Windows, macOS and Linux.
```

**Website**

```text
https://www.talokit.com/
```

**Topics**（逐个添加）

```text
developer-tools
developer-toolkit
offline-first
kubernetes
docker
yaml
json
sql
electron
cross-platform
```

## Social Preview

在 **Settings → General → Social preview → Edit → Upload an image** 上传 [talokit-social-preview.png](../assets/talokit-social-preview.png)。这一步不能通过提交图片文件自动设置。

- PNG 尺寸：1280 × 640。
- 设计源文件：[talokit-social-preview.svg](../assets/talokit-social-preview.svg)。
- 复用仓库已有图标，使用品牌、跨平台、本地优先与核心工具文字排版；这是宣传图，不是软件截图。
- 不添加虚构评价、Star 数、下载量、版本、开源标识或“完全离线”承诺。

## 版本与 Release 维护

README 的“最新版”链接指向官网实际下载区。Release 入口保留，但在确认真实版本、发布日期与更新内容之前不创建占位 Release。之后如需发布，只填写对应已发布客户端的真实变更，安装包继续指向官方来源；文档提交不触发应用版本发布。

## 真实截图清单

现有图片已用于中英文 README：总览、Kubernetes YAML、Docker 命令、SQL、Diff；JSON 截图在教程中展示。它们来自已有官方素材，不是本轮生成。

后续建议补充以下当前发布版截图，全部使用演示数据、隐藏账号和本地路径：

1. Kubernetes 校验发现错误时的行号和诊断详情。
2. Kubernetes 探针、requests/limits 的配置区域及对应 YAML。
3. 目录 Diff 的两侧目录树、差异状态，以及文件按块合并界面。
4. containerd 的 namespace 筛选和 ctr 命令详情。
5. YAML 语法错误与修正后的结果。

这些是教程增强素材，不阻塞现有产品页使用。截图应与公开发布版一致；不将开发中的集群管理或其他未确认发布能力当作已上线卖点。

## 后续内容节奏

按 [教程计划](tutorials.md) 逐篇补例子和实测记录，完成一篇再发布下一篇。维护文档链接、真实截图和授权边界；GitHub 内容有助于产品发现，但不保证任何搜索引擎收录时间或排名。
