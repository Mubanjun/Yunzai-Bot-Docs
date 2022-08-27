---
title: 部署说明
icon: note
index: true
---

你可以使用 docker 快速部署一个云崽机器人，也可以手动本地部署。

::: tip

我们推荐使用 docker。

:::

## 目录

### Linux

- [Docker 部署](linux/docker.md)
- [本地手动部署](linux/local.md)

### Windows

- [Docker 部署](windows/docker.md)
- [本地手动部署](windows/local.md)

### Android

- [安卓手机部署](android/README.md)

## 为什么选择 docker？

- **开箱即用**的云崽机器人，近乎一键安装，无需考虑 redis 和 nodejs 环境安装和依赖安装、项目更新等问题
- **不会破坏主机环境**，跑路时仅需删除 docker 容器即可
- 毋庸担心本项目环境与本机其他项目所需要的环境相互干扰的问题
- 可在任意支持 docker 的 **amd64 架构或 arm64 架构**的操作系统（包括 Linux、Windows、MacOS 等）上轻松运行
- 结合 docker 部署脚本，可以交互式**配置喵喵插件和 Python 插件**，免除手动安装插件、配置环境和编译 ffmpeg 的烦恼
- 所有用户数据均已映射到主机，**方便备份和迁移**
- 每次重启容器即可完成对云崽本体和喵喵插件、Python 插件（若存在）的更新，方便快捷
- 可配合 [portainer](https://www.portainer.io/) 进行图形化管理
- 可通过创建多个 service 轻松实现**多开**
