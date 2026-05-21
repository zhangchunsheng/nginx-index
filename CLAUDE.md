# CLAUDE.md

本文件为 Claude Code (claude.ai/code) 在此仓库中工作时提供指导。

## 项目概述

此仓库托管烙馍网（luomor.com）的静态 HTML 页面，作为 Nginx 的默认首页。网站自 2015 年起运营至今。

## 文件结构

| 文件 | 说明 |
|------|------|
| `index.html` | 主页面 — "AI与生活" 主题，深色科技风 |
| `index1.html` | 备选页面 — 烙馍饮食文化主题，暖色调 |
| `docs/log.txt` | AI 会话生成记录 |
| `docs/README.md` | 生成页面的原始提示词 |
| `centos/` | CentOS 默认 HTML 文档（参考资料，非站点内容） |

## 开发

- **无构建流程** — 页面为纯 HTML + 内联 CSS，无框架、无依赖
- **本地预览**：直接在浏览器中打开 `index.html`，或使用 `python3 -m http.server` 启动服务
- **部署**：提交并推送，Nginx 从此目录提供 `index.html`

## 编码规范

- 单文件页面，样式内联在 `<style>` 中，无外部 CSS/JS 文件
- 纯 HTML + CSS，无 JavaScript 框架或构建工具
- 响应式设计，使用 `@media (max-width: 768px)` 断点
- 页面语言为中文（`lang="zh-CN"`）
- 使用 Emoji/Unicode 实体作为装饰图标（如 `&#129652;`）
