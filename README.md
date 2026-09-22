# Crown Rush 活动落地页与需求文档

789Bingo 百关闯关活动（Crown Rush）的三个前台原型页面与开发需求文档，纯静态文件，无需构建。

## 内容

| 文件 | 说明 |
| --- | --- |
| `index.html` | 入口导航（左侧栏切换页面，PRD 带目录跳转） |
| `pre-launch.html` | 活动预热页原型（英文版） |
| `live.html` | 活动进行中页原型（英文版） |
| `ended.html` | 活动结束页原型（英文版，领奖缓冲期） |
| `prd.html` | 开发需求文档 PRD（中文，可打印为 PDF） |
| `assets/` | 主视觉、奖品、游戏与弹窗素材 |
| `support.js` / `doc-page.js` / `image-slot.js` | 页面运行时依赖 |

## 使用

- 打开 `index.html`，左侧栏点选即可在右侧区域切换四个页面。
- 选中「开发需求文档 PRD」时，左侧栏下方展开章节目录，点击任意章节可直接跳转到文档对应位置。
- 地址栏 hash 会记录当前页面与章节（如 `#prd:sec-8-3`），可直接分享定位链接。
- 每个页面也可单独打开：`pre-launch.html`、`live.html`、`ended.html`、`prd.html`。

## 部署到 GitHub Pages

1. 新建仓库，将本目录内所有文件（含 `assets/`、`.nojekyll`）推送到 `main` 分支根目录。
2. 仓库 Settings → Pages → Source 选择 `Deploy from a branch`，分支 `main`、目录 `/ (root)`。
3. 构建完成后访问 `https://<用户名>.github.io/<仓库名>/`。

放在子目录（如 `docs/`）时，第 2 步目录选择 `/docs` 即可。

## 本地预览

```bash
python3 -m http.server 8080
# 浏览器打开 http://localhost:8080
```

建议使用本地服务器方式预览；直接双击 HTML 文件时，部分浏览器的本地文件策略会阻止脚本与 iframe 加载。
