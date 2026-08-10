# codermali.com

马力的个人名片页 — [codermali.com](https://codermali.com)

一个零依赖、零构建的纯静态单页：手写 HTML/CSS，十几行原生 JS（鼠标聚光灯与
滚动导航高亮），无任何框架和第三方库。

## 结构

```
index.html            # 整个网站
CNAME                 # 自定义域名（GitHub Pages）
assets/wechat-qr.png  # 微信二维码（不存在时页面自动降级提示）
```

## 本地预览

```bash
python3 -m http.server 8000
# 打开 http://localhost:8000
```

## 部署

```
本地 ──push──▶ GitLab（自建） ──Push Mirroring──▶ GitHub ──▶ GitHub Pages ──▶ codermali.com
```

日常只推 `origin`（GitLab），由镜像自动同步到 GitHub 触发 Pages 部署。
不要直接在 GitHub 侧修改代码，避免两边历史分叉。

## 相关

- 博客（独立 Hexo 项目）：[blog.codermali.com](https://blog.codermali.com)
