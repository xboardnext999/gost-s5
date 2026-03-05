# 🚀 gost-s5 超轻量多端口 SOCKS5 管理工具



**gost-s5** 是一款基于 **GOST** 引擎开发的 SOCKS5 代理一键管理工具。专为小内存 VPS（如 **200MB RAM** 廉价节点）进行深度优化，支持多端口独立管理、全自动配置及开机自启。

## ✨ 功能特性

- **极致轻量**：针对极小内存环境优化，每个端口实例通过 Systemd 严格限制 **60MB** 内存占用。
- **多端口独立管理**：支持无限添加端口，每个端口作为独立服务运行，支持单独 启动/停止/删除。
- **人性化流程**：安装流程采用“先设账号密码，后设端口”的逻辑，支持回车全随机生成。
- **智能 IP 探测**：全自动识别服务器 IPv4 和 IPv6 地址，并生成对应的双栈 SOCKS5 链接。
- **零依赖运行**：改用系统原生 `ss` 命令检测端口，无需安装 `net-tools`，适配精简版系统。
- **快捷命令注册**：支持 `gost-s5`、`sock5`、`socks5` 三种指令快速调出菜单。
- **彻底卸载**：选项 6 提供“自我销毁”功能，清理所有进程、配置目录 `/etc/gost-s5` 及快捷命令。

## 🚀 一键安装

```bash
bash <(curl -Ls [https://raw.githubusercontent.com/xboardnext999/gost-s5/main/gost-s5.sh](https://raw.githubusercontent.com/xboardnext999/gost-s5/main/gost-s5.sh))

安装后执行：
```bash
gost-s5
