# 789Bingo 需求与原型中心

流水闯关活动与圣诞换肤两套需求的全部原型页面与文档，纯静态文件，无需构建。

## 目录结构

```
index.html        入口：左侧「流水闯关 / 圣诞换肤」两个标签切换各自的树形目录，右侧显示内容
nav.dc.html       项目导航页（默认首页）
crown-rush/plan/
  latest/v1.1/    最新需求记录：full（完整需求）、v1.0 / v1.1 / v1.2 迭代
  history/v1.0/   历史需求记录（已归档）
xmas-skin/
  latest/v1.1/    最新需求记录
  history/v1.0/   历史需求记录（已定稿）
assets/           图片素材
support.js / doc-page.js / image-slot.js   页面运行时
.nojekyll         关闭 Jekyll 处理
```

## 部署到 GitHub Pages

1. 将本目录全部内容（包括 `.nojekyll`）推送到仓库根目录，例如 `main` 分支。
2. 仓库 Settings → Pages → Source 选择 `Deploy from a branch`，分支 `main`，目录 `/ (root)`。
3. 部署完成后访问 `https://<用户名>.github.io/<仓库名>/`。

如需放在子目录（如 `docs/`），把本目录内容放进 `docs/`，第 2 步目录选 `/docs`。

## 使用说明

- 左侧顶部点「流水闯关」「圣诞换肤」切换需求；默认展开状态与项目导航一致（流水闯关只展开最新需求记录 v1.1 下的 v1.0 迭代，圣诞换肤展开最新需求记录 v1.1 下全部目录），可用「全部展开」「恢复默认」切换。
- 搜索框只搜索当前标签下的页面和文档。
- 地址栏记录当前打开的文件，可直接分享链接；从链接打开时会自动切到对应标签并展开所在目录。
- 所有文件名均为英文，避免解压或上传时中文文件名乱码。

## 本地预览

```bash
python3 -m http.server 8080
# 浏览器打开 http://localhost:8080
```
