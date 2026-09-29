# 789Bingo 需求与原型中心

流水闯关活动（完整需求 + v1.0 / v1.1 / v1.2 迭代）与圣诞换肤需求的全部原型页面和文档，纯静态文件，无需构建。

## 目录结构

```
index.html                 入口：左侧按项目 › 版本 › 文件的树形目录，右侧显示内容
项目导航.dc.html            项目导航页（默认首页）
crown-rush/                流水闯关活动 · 完整需求（基线）
  v1.0/                    v1.0 迭代：前台全量 + 后台精简
  v1.1/                    v1.1 迭代：仅后台（库存与机器人完善）
  v1.2/                    v1.2 迭代：仅后台（达到完整需求）
xmas-skin/                 圣诞换肤：需求文档、后台与页面原型
assets/                    图片素材
support.js / doc-page.js / image-slot.js   页面运行时
.nojekyll                  关闭 Jekyll 处理
```

每个版本目录包含：开发需求 PRD、需求速览、开发自查清单、后台操作手册、后台原型；完整需求与 v1.0 另含三个前台活动页。

## 部署到 GitHub Pages

1. 将本目录全部内容（包括 `.nojekyll`）推送到仓库根目录，例如 `main` 分支。
2. 仓库 Settings → Pages → Build and deployment → Source 选择 `Deploy from a branch`，分支 `main`，目录 `/ (root)`。
3. 等待部署完成后访问 `https://<用户名>.github.io/<仓库名>/`。

如需放在子目录（如 `docs/`），把本目录内容放进 `docs/`，第 2 步目录选 `/docs`。

## 使用说明

- 左侧目录按「项目 › 版本 › 文件」展开，点击文件在右侧打开；支持搜索。
- 地址栏会记录当前打开的文件（如 `#/crown-rush/v1.0/Crown Rush PRD.dc.html`），可直接分享链接。
- 页面内的跳转（如需求速览 → 查看 PRD）会同步更新左侧选中项。
- 右上角「新窗口打开」可单独查看当前页面。

## 本地预览

```bash
python3 -m http.server 8080
# 浏览器打开 http://localhost:8080
```

请通过本地服务器访问；直接双击 HTML 文件时，浏览器的本地文件限制可能导致页面无法加载。
