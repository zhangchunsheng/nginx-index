# nginx-index

烙馍网（luomor.com）的 Nginx 默认首页。

## 用途

当访问域名根路径时，Nginx 输出此目录下的 `index.html`，作为烙馍网的引导介绍页面。

## 文件说明

| 文件 | 说明 |
|------|------|
| `index.html` | 主页面 — "AI与生活" 主题，深色科技风 |
| `index1.html` | 备选页面 — 烙馍饮食文化主题，暖色调 |
| `docs/` | 生成记录与日志 |
| `centos/` | CentOS 默认 HTML 文档（参考资料，非站点内容） |

## 开发

纯静态 HTML + 内联 CSS，无构建流程、无外部依赖。

```bash
# 本地预览
python3 -m http.server 8080

# 部署
git add . && git commit -m "your message" && git push
```

## 运营信息

- 域名：luomor.com
- 服务器：CentOS
- 静态目录：`/usr/share/doc/HTML`
- 主题：基于 Puock（WordPress）构建
