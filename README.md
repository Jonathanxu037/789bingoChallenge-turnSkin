# Crown Rush 活动落地页

789Bingo 百级冲级活动的落地页原型与开发需求文档，纯静态文件，无构建步骤。

## 内容

| 文件 | 说明 |
| --- | --- |
| `index.html` | 入口导航页 |
| `pre-launch.html` | 活动预热页原型 |
| `live.html` | 活动进行中页原型 |
| `prd.html` | 开发需求文档（可打印为 PDF） |
| `assets/` | 主视觉、奖品与游戏图片 |
| `support.js` / `doc-page.js` / `image-slot.js` | 页面运行时依赖 |

## 部署到 GitHub Pages

1. 新建仓库并将本目录内所有文件推送到 `main` 分支根目录。
2. 仓库 Settings → Pages → Source 选择 `Deploy from a branch`，分支选 `main`、目录选 `/ (root)`。
3. 等待构建完成后访问 `https://<用户名>.github.io/<仓库名>/`。

如需放在子目录（如 `docs/`），第 2 步的目录选择 `/docs` 即可。

## 本地预览

```bash
python3 -m http.server 8080
# 浏览器打开 http://localhost:8080
```

直接双击 HTML 文件也可打开，但部分浏览器的本地文件策略会阻止脚本加载，建议用上面的本地服务器方式。
