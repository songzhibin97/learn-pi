# learn-pi · pi 闯关教程

一个**交互式、闯关式**的网页教程 —— 用 8 个关卡，带你从零搞懂 [pi](https://github.com/earendil-works/pi-mono)（一个用来构建 AI Agent 的开源框架），以及一个更普适的问题：**一个 AI Agent 到底是怎么跑起来的**。

> 🎮 在线体验：<https://songzhibin97.github.io/learn-pi/>

## 特点

- **纯静态、离线可用** —— 单个 `index.html`，双击即在浏览器打开，无需安装、无需联网、无需 API key。
- **闯关式学习** —— 8 关循序渐进，每关若干小步骤 + 一道通关测验，答对解锁下一关、获得经验值。
- **概念 + 源码并重** —— 既用生活化比方讲清原理，也对照 pi 的真实源码片段（每段代码都配「人话」翻译）。
- **可交互 Demo** —— 流式播放器、工具调用、Agent Loop 单步模拟器、事件流可视化、steering 插话等，全部离线模拟。
- 浅色 / 深色主题切换，学习进度本地保存。

## 8 个关卡

| 关卡 | 主题 |
|------|------|
| 1 | 总览 —— pi 是什么 |
| 2 | 一次 LLM 对话的本质 —— Context 与无状态 |
| 3 | 流式输出与事件 —— 逐字拼装消息 |
| 4 | 工具调用 —— 让 LLM 行动起来 |
| 5 | Agent Loop —— 整个 pi 的心脏 |
| 6 | 事件流 —— Agent 如何驱动 UI |
| 7 | 进阶控制 —— steering / 钩子 / 上下文压缩 |
| 8 | 从框架到产品 —— pi-coding-agent |

## 本地使用

直接双击 `index.html` 即可。或启动一个本地服务器：

    python3 -m http.server 8000
    # 然后访问 http://localhost:8000

## 部署

推送到 `main` 分支后，GitHub Actions 会自动将站点部署到 GitHub Pages，配置见 [`.github/workflows/deploy.yml`](.github/workflows/deploy.yml)。

首次部署前需在仓库 **Settings → Pages → Build and deployment → Source** 选择 **GitHub Actions**。

## 致谢

教程内容基于开源项目 [pi](https://github.com/earendil-works/pi-mono)（`@earendil-works/pi-*`，MIT 许可证）。本教程为非官方学习材料。
