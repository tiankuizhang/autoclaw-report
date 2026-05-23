# AutoClaw 市场日报站点

这个仓库用于托管由 AutoClaw 每日市场报告归档自动生成的公开静态网站。

源 Markdown 日报和站点生成脚本位于私有仓库 `AutoClaw`。本仓库只应保存生成后的静态站点文件，以及必要的仓库元数据。

不要手动修改生成文件，例如 `index.html`、`assets/site.css`、`markets/*.html` 或 `reports/**/*.html`。这些文件会在下一次 AutoClaw 站点构建时被覆盖。

## GitHub Pages 配置

本仓库的 GitHub Pages 应配置为：

- Source: Deploy from a branch
- Branch: `main`
- Folder: `/root`

站点地址：

https://tiankuizhang.github.io/autoclaw-report/

## 本地构建

在私有 AutoClaw 仓库根目录运行：

```powershell
python scripts/build_report_site.py --site-dir ../autoclaw-report
```
