# TaloKit 实用教程索引与扩展计划

这里按真实开发任务组织教程，先完善已有页面，再逐步增加独立专题。标为“待扩展”的条目是文档计划，不代表尚未发布的产品能力，也不提供空白教程链接。当前教程为中文。

## 已有入门与功能说明

| 任务 | 当前可读内容 | 内容层级 |
| --- | --- | --- |
| JSON 格式化与校验 | [输入输出、错误修复与操作步骤](json-and-base64.md#json-格式化与校验) | 入门教程 |
| Base64 编码解码 | [文本示例、乱码与常见错误](json-and-base64.md#base64-编码与解码) | 入门教程 |
| YAML 格式整理 | [YAML 与 JSON 类型差异](json-and-base64.md#yaml-与-json-的差异) | 基础说明，待扩展完整排错教程 |
| Kubernetes 清单 | [YAML 工作台操作与校验边界](kubernetes-yaml.md) | 功能指南 |
| Docker / containerd 命令 | [命令搜索、版本与执行边界](container-command-library.md) | 功能指南 |
| SQL / 文本与目录 Diff | [方言选择、检查与对比流程](sql-and-diff.md) | 功能指南 |

## 下一阶段：逐篇验证后发布

| 优先级 | 教程主题 | 要解决的问题与验收示例 | 扩展位置 |
| --- | --- | --- | --- |
| 1 | YAML 格式化与校验 | 缩进、Tab、重复键、字符串类型；错误输入与修正对照，区分语法和资源规则 | 深化现有 JSON/YAML 文档，篇幅足够再拆分并保留回链 |
| 1 | Kubernetes Deployment YAML 示例 | labels 与 selector 对齐、镜像、端口、Service；完整可解析清单和验证步骤 | 从 Kubernetes 指南链接独立专题 |
| 1 | Readiness Probe / Liveness Probe | 区分流量就绪与重启判断，说明 startupProbe、路径、阈值及常见误配 | Kubernetes 专题 |
| 1 | CPU / Memory requests 与 limits | `m`、`Mi`、`Gi` 单位，调度、限流和 OOM；完整容器配置 | Kubernetes 专题 |
| 2 | Docker 常用命令 | 从容器查看、日志到端口检查；区分只读命令与清理写操作 | 容器命令指南的专题 |
| 2 | containerd ctr 命令 | namespace、镜像与任务的区别；说明 ctr、crictl 与 nerdctl 的适用边界 | 容器命令指南的专题 |
| 2 | SQL 格式化与常见风险检查 | 方言差异、无 WHERE 写操作、NULL 陷阱；修正前后对比和静态检查局限 | 深化现有 SQL / Diff 页面，必要时拆分 |
| 2 | 文本与目录 Diff | 双栏差异、按块合并、左右方向、保存后刷新；最小目录样例 | 深化现有 SQL / Diff 页面，必要时拆分 |

JSON 和 Base64 入门继续复用现有页面，不另建同题页面。每篇新增教程都应包含适用场景、可复现输入与预期结果、具体操作、常见错误、版本或环境前提，以及对应功能指南、[官方下载](https://www.talokit.com/#downloads)和[反馈入口](https://github.com/maningphp/talokit/issues)。

## 发布质量要求

- 示例先用对应解析器或隔离环境验证；涉及集群或数据库的命令明确哪些步骤需要真实环境。
- 静态 YAML / SQL 检查不能写成“保证可上线”，命令知识库不能写成远程执行或集群管理平台。
- 使用真实软件截图；没有截图时保留文字和可复现实例，不用界面概念图替代。
- 用标题、说明性链接和解决问题的内容帮助检索，不堆砌关键词，不制造近似重复页面。

[功能地图](features.md) · [快速开始](getting-started.md) · [隐私说明](privacy.md) · [官网](https://www.talokit.com/)
