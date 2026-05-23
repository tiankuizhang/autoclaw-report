# AutoClaw Report Site

This repository hosts the public static website generated from AutoClaw daily market report archives.

The source Markdown reports and site generation logic live in the private `AutoClaw` repository. This repository should contain only generated static site files and minimal repository metadata.

Do not manually edit generated HTML or CSS files such as `index.html`, `assets/site.css`, `markets/*.html`, or `reports/**/*.html`. They are overwritten by the next AutoClaw site build.

## GitHub Pages

Configure GitHub Pages for this repository as:

- Source: Deploy from a branch
- Branch: `main`
- Folder: `/root`

The expected project site URL is:

https://tiankuizhang.github.io/autoclaw-report/

## Local Build

From the private AutoClaw repository root, run:

```powershell
python scripts/build_report_site.py --site-dir ../autoclaw-report
```
