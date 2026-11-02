# JSON 格式化、YAML 转换与 Base64 编解码

接口调试时，常见任务并不是编写新代码，而是看清一段响应、定位一个非法字符，或还原一个编码字段。TaloKit 将这些高频操作放在本地桌面工具中。

![TaloKit JSON 格式化与数据转换界面](../assets/json-formatting-workbench.png)

## JSON 格式化与校验

在顶部搜索框输入 `JSON`，打开工具并粘贴以下内容：

```json
{"product":"TaloKit","localFirst":true,"platforms":["Windows","macOS","Linux"]}
```

执行格式化后，可按层次阅读：

```json
{
  "product": "TaloKit",
  "localFirst": true,
  "platforms": [
    "Windows",
    "macOS",
    "Linux"
  ]
}
```

若输入包含尾逗号、未闭合引号或非法转义，先根据编辑器诊断修正语法，再复制结果。格式化不会替你判断业务字段值是否正确。

## YAML 与 JSON 的差异

同一数据的 YAML 表达可以是：

```yaml
product: TaloKit
localFirst: true
platforms:
  - Windows
  - macOS
  - Linux
```

使用数据转换工具前，留意数字、布尔值、日期与字符串的类型。YAML 注释、锚点和样式不一定能在 JSON 中原样保留；转换后应检查关键字段。

## Base64 编码与解码

在全局搜索中输入 `Base64`，选择编码或解码方向：

| 操作 | 输入 | 输出 |
| --- | --- | --- |
| 编码 | `TaloKit` | `VGFsb0tpdA==` |
| 解码 | `VGFsb0tpdA==` | `TaloKit` |

Base64 适合文本传输和开发调试，**不能隐藏内容，也不能替代加密**。中文内容出现乱码时，应检查原始字符集，而不是反复编码。

## 相关工具

- URL 编解码：处理查询参数中的空格、中文和保留字符；
- Unicode / Hex：检查字符和字节表示；
- Hash：计算摘要并核对内容一致性；
- [文本 Diff](sql-and-diff.md)：比较格式化、转换前后的变化；
- [隐私说明](privacy.md)：了解本地处理和联网场景。

[下载 TaloKit](https://www.talokit.com/#downloads) · [返回功能地图](features.md)
