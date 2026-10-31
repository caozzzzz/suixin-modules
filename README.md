# 随心模块 · 多客户端模块与规则

收集和维护 Surge、Clash、Shadowrocket 的模块、覆写与规则，按客户端独立存放。

## 目录

| 客户端 | 内容 | 状态 |
| --- | --- | --- |
| [Surge](Surge/) | `.sgmodule` 模块与规则 | 已收录 SideStore LocalDevVPN |
| [Clash](Clash/) | YAML 覆写与规则集 | 待添加 |
| [Shadowrocket](Shadowrocket/) | 模块与规则 | 待添加 |

## Surge 模块

### SideStore LocalDevVPN

使用 Surge 为 SideStore / LiveContainer 配置 `10.7.0.1` 本机回环。

- [查看模块](Surge/modules/sidestore-localdevvpn.sgmodule)
- [模块下载 / 导入地址](https://raw.githubusercontent.com/caozzzzz/suixin-modules/main/Surge/modules/sidestore-localdevvpn.sgmodule)

在 Surge 的模块管理中使用以上 Raw 地址安装并启用，然后启动 Surge，验证 SideStore / LiveContainer 的连接。

此模块会禁用 IPv6 VIF，并添加 `10.7.0.1/32` 路由和 IP Rewrite。

#### 已验证环境

| 设备 | 系统版本 | Surge 版本 | 测试结果 |
| --- | --- | --- | --- |
| iPhone 16 Pro Max | iOS 27.2 | 5.23.0 | ✅ 测试通过 |

以上为维护者提供的实测结果，其他设备或版本的兼容性待验证。

## 维护约定

- 根据目标客户端放入对应目录，模块、覆写与规则保留其原生格式。
- 每次新增内容时更新本页索引，并写明用途和导入方法。
- 不同客户端的格式与能力有差异，文件不能直接通用。
- 不提交订阅 Token、节点密码、私钥等个人凭据。
