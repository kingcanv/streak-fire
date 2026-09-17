# 打卡小火苗 · Streak Fire

高保真的「健身步数连胜」小组件可视化页面，包含：

- 水滴火焰矢量图（SVG 动效：外焰摆动 + 内芯跳动）
- 左上 → 右下的模糊粉色辉光背景
- 主卡片 / 周打卡胶囊 / 进度条轨道的毛玻璃质感
- 步数与目标滑块、连点打卡交互

## 在线预览

部署完成后会自动发布到 GitHub Pages：

```
https://<owner>.github.io/streak-fire/
```

> 首次启用 Pages 后大约 30 秒生效。

## 本地预览

页面是单文件（Tailwind 走 CDN），无需安装依赖：

```bash
python -m http.server 8080
# 或
npx serve .
```

打开 <http://localhost:8080>。

## 仓库内容

- `index.html` — 完整页面（HTML + CSS + JS 全在一份）
- `.gitignore` — 忽略 macOS 系统文件

## 一键复刻

```bash
git init -b main
git add . && git commit -m "feat: 初始版本"
gh repo create streak-fire --public --source=. --remote=origin --push
gh repo edit streak-fire --enable-pages --branch main --path /
```