# OpenClaw 中文教程网站 🐕

> 基于官方文档打造的现代化 OpenClaw 中文学习平台

[![GitHub](https://img.shields.io/badge/GitHub-OpenClaw--Tutorial-orange)](https://github.com/wheat868/openclaw-tutorial)
[![Gitee](https://img.shields.io/badge/Gitee-OpenClaw--Tutorial-red)](https://gitee.com/576686357/openclaw-tutorial)
[![License](https://img.shields.io/badge/License-MIT-blue)](LICENSE)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-CSS-38B2AC)](https://tailwindcss.com/)

---

## 📖 项目介绍

本项目是一个完整的 **OpenClaw 中文教程网站**，旨在帮助中文用户快速上手 OpenClaw 框架，从零开始打造属于自己的 AI 助手。

OpenClaw 是一个开源的 AI Agent 框架，提供：
- 🧠 **持久化记忆** - 长期记忆 + 短期工作记忆
- 🔧 **丰富工具链** - 文件读写、终端执行、网页浏览等
- 📱 **多渠道接入** - 微信、Telegram、Discord、飞书等
- 🎯 **灵活配置** - 支持本地 Ollama 大模型、Token 优化等

---

## 🌐 在线访问

| 平台 | 地址 |
|------|------|
| GitHub Pages | https://wheat868.github.io/openclaw-tutorial/ |
| Gitee Pages | https://576686357.gitee.io/openclaw-tutorial/ |

> 💡 Pages 服务需在仓库设置中手动启用

---

## 📁 网站结构

```
openclaw-tutorial-site/
├── index.html          # 首页 - 英雄区 + 功能介绍 + 学习路径
├── beginner.html       # 入门篇 - 环境配置 + 快速启动 + Ollama 接入
├── intermediate.html   # 进阶篇 - 飞书集成 + Token 优化 + 记忆管理
├── advanced.html       # 高级篇 - 权限配置 + 自动化脚本 + 实战案例
├── README.md           # 项目说明文档
└── ...
```

---

## 📄 页面详情

### 1️⃣ index.html - 首页

**核心内容：**
- 🎨 高端大气的 Hero Section（英雄区）
- 🚀 OpenClaw 核心特性介绍
- 📍 三阶段学习路径导航（入门 → 进阶 → 高级）
- 🔗 官方文档及 GitHub 仓库链接

**适合人群：** 首次访问，想了解 OpenClaw 是什么的用户

---

### 2️⃣ beginner.html - 入门篇

**核心内容：**
- ✅ 环境要求清单（Node.js 18+、npm/pnpm、Git）
- 📦 Node.js 安装教程（macOS/Linux/Windows）
- 🚀 `npx openclaw start` 一键启动
- 🤖 本地 Ollama 大模型配置指南
  - Ollama 安装命令
  - 模型下载推荐（qwen2.5:7b/14b）
  - OpenClaw 连接配置示例

**适合人群：** 零基础新手，第一次接触 OpenClaw

**学完收获：** 成功启动自己的第一个 AI 助手

---

### 3️⃣ intermediate.html - 进阶篇

**核心内容：**
- 📱 **飞书机器人集成**
  - 飞书开放平台应用创建
  - 权限配置（消息、群组、事件订阅）
  - OpenClaw 飞书插件配置
  
- 💰 **Cache-TTL 上下文缓存修剪**
  - 工作原理详解
  - 配置参数说明（ttl、maxSize、cleanupInterval）
  - 不同场景的推荐设置
  
- 🗜️ **长文本压缩 (Auto-compaction)**
  - 自动压缩策略配置
  - 压缩效果对比示例
  - threshold 与 targetSize 调优
  
- 💾 **记忆落盘 (Memory Flush)**
  - 自动落盘配置（autoFlush、flushInterval）
  - 手动落盘命令（`/memory flush`）
  - 最佳实践建议

**适合人群：** 已完成入门，想要优化 Token 消耗、集成企业 IM 的开发者

**学完收获：** 掌握生产环境配置技巧，大幅降低使用成本

---

### 4️⃣ advanced.html - 高级篇

**核心内容：**
- ⚠️ **安全警告** - 高风险权限使用说明
- 📂 **文件系统 (fs) 权限**
  - allowedPaths / blockedPaths 配置
  - 可用工具清单（read/write/edit/exec）
  - 风险等级说明
  
- 💻 **终端执行 (runtime) 权限**
  - 命令白名单配置
  - 危险命令拦截（blockedCommands）
  - 强制确认机制（requireConfirmation）
  
- 🎯 **实战案例：自动化项目部署脚本**
  - 完整场景描述
  - 6 步执行流程详解
  - 每步命令及输出示例
  - 完成报告格式
  
- 🔒 **安全最佳实践**
  - ✅ 应该做的（最小权限、白名单、日志审计）
  - ❌ 不应该做的（生产环境启用、系统目录访问）

**适合人群：** 需要自动化能力、想深入理解权限机制的高级用户

**学完收获：** 能够安全地赋予 Agent 自动化能力，编写复杂工作流

---

## 🛠️ 技术栈

| 技术 | 说明 |
|------|------|
| HTML5 | 语义化标签、响应式布局 |
| Tailwind CSS (CDN) | 原子化 CSS 框架，无需构建 |
| 原生 JavaScript | 零依赖，开箱即用 |

**设计特点：**
- 📱 完全响应式，适配手机/平板/桌面
- 🎨 统一的橙色主题色（claw-500/600/700）
- ⚡ 加载速度快，无构建步骤
- 🌈 每个章节独立配色（绿/蓝/紫）

---

## 🚀 本地运行

### 方法一：直接打开
```bash
# 双击文件或在浏览器中打开
file:///path/to/openclaw-tutorial-site/index.html
```

### 方法二：本地服务器
```bash
# 进入项目目录
cd openclaw-tutorial-site

# Python 3
python3 -m http.server 8080

# 或使用 Node.js 的 http-server
npx http-server -p 8080

# 访问 http://localhost:8080
```

---

## 📦 部署到 Pages 服务

### GitHub Pages

1. 访问仓库：https://github.com/wheat868/openclaw-tutorial
2. 进入 **Settings** → **Pages**
3. Source 选择 `Deploy from a branch`
4. Branch 选择 `master`，文件夹选择 `/ (root)`
5. 点击 **Save**，等待部署完成
6. 访问生成的 URL（通常是 `https://wheat868.github.io/openclaw-tutorial/`）

### Gitee Pages

1. 访问仓库：https://gitee.com/576686357/openclaw-tutorial
2. 进入 **管理** → **Gitee Pages**
3. 选择分支 `master`
4. 点击 **启动**
5. 访问生成的 URL（通常是 `https://576686357.gitee.io/openclaw-tutorial/`）

---

## 🤝 贡献指南

欢迎提交 Issue 和 Pull Request！

1. Fork 本仓库
2. 创建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启 Pull Request

---

## 📝 更新日志

### v1.0.0 (2026-02-21)
- ✨ 初始版本发布
- 📄 完成 4 个核心页面
- 🎨 Tailwind CSS 响应式设计
- 📱 移动端适配
- 🔗 GitHub + Gitee 双平台部署

---

## 📄 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情

---

## 🔗 相关链接

| 资源 | 链接 |
|------|------|
| OpenClaw 官方文档 | https://docs.openclaw.ai |
| OpenClaw GitHub | https://github.com/openclaw/openclaw |
| OpenClaw Discord | https://discord.com/invite/clawd |
| Tailwind CSS 文档 | https://tailwindcss.com/docs |
| Ollama 官网 | https://ollama.com |
| 飞书开放平台 | https://open.feishu.cn |

---

## 👨‍💻 关于作者

- **制作：** 二狗 (Èr Gǒu) 🐕
- **基于：** OpenClaw 官方文档
- **时间：** 2026 年 2 月

---

<div align="center">

**🎉 祝你学习愉快，早日打造出自己的 AI 助手！**

⭐ 如果这个项目对你有帮助，请给个 Star 支持一下！

</div>
