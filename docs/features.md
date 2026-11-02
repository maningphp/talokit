# TaloKit 功能地图

本文按使用场景介绍 TaloKit 的主要工具，便于搜索“离线开发工具”“程序员工具箱”“JSON 格式化”“Kubernetes YAML 生成”等需求时快速判断是否匹配。具体能力以当前公开版本客户端为准。

## 格式化与结构化数据

- JSON 格式化、压缩、语法检查与编辑；
- XML、YAML、TOML、Properties、Query 等格式整理和转换辅助；
- 代码美化、序列化结果整理、SQL 参数填充；
- 带行号、搜索、错误提示和复制反馈的代码编辑区域。

## 编码、压缩与字符转换

- Base64 编码与解码；
- URL 编码、Unicode、ASCII、文本与 Hex 互转；
- HTML 实体、二进制表示、进制转换；
- Gzip 压缩与解压辅助。

Base64 不是加密算法，不应把它用于保护密码或敏感数据。

## 加密、安全与校验

- MD5、SHA 系列等 Hash 摘要；
- HMAC、JWT、bcrypt；
- AES、DES、3DES、RC4、Rabbit、RSA；
- SM2、SM4 等国密辅助；
- 签名、校验和、随机密钥与安全字符串生成。

这些工具适合开发调试，不替代经过审计的生产密钥管理系统。

## 时间、文本与生成器

- 秒/毫秒时间戳与日期转换、时区和日期计算；
- Cron 表达式解释；
- 正则表达式测试、文本统计、排序、去重与替换；
- 拼音、变量命名风格转换；
- UUID、随机字符串、二维码和条形码。

## 网络辅助

- IPv4/IPv6 和 CIDR 计算；
- 子网、地址范围和掩码辅助；
- URL 解析、HTTP 请求片段；
- WebSocket 调试辅助；
- IP 归属查询。

IP 归属查询、WebSocket 和用户指定的网络目标需要联网。

## SQL 与数据库

- MySQL、PostgreSQL、SQLite、SQL Server 方言格式化；
- 无 WHERE 的 UPDATE/DELETE 等高风险模式提示；
- CTE、窗口函数、分页、Upsert 等方言与版本提示；
- 查询知识库和可复制的示例；
- SQL 占位参数填充与修正结果。

静态检查不连接生产数据库，不能代替真实数据库解析、权限检查、执行计划或事务验证。

## 文件与目录比较

- 双栏文本和文件 Diff；
- 行内差异高亮与差异导航；
- 按差异块从左向右或从右向左合并；
- 目录树比较与状态筛选；
- 差异文件预览和安全覆盖操作。

## Kubernetes 与容器云原生

- Kubernetes YAML 模板生成、源码编辑、静态检查和版本规则；
- Kubernetes 资源、操作和任务导向的 kubectl 命令知识库；
- Docker 容器、镜像、网络、日志、清理命令；
- containerd、ctr、crictl 命令与版本说明；
- Docker Compose 部署 YAML 辅助；
- Helm Chart/values 模板和命令参考。

命令知识库不会自动执行命令。应用前必须理解目标环境、权限和风险。
