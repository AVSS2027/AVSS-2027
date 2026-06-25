# AVSS 2027 Website

This repository contains a Markdown-based GitHub Pages site for AVSS 2027.
The homepage content is written in Markdown and rendered by GitHub Pages/Jekyll.

这个仓库是一个 Markdown 驱动的 GitHub Pages 会议网站模板，首页内容主要写在
`index.md` 里，由 GitHub Pages/Jekyll 自动渲染。

## How It Renders

- `index.md` is the homepage content.
- `_layouts/default.html` is the Jekyll page shell.
- `assets/css/site.css` controls the visual style.
- `assets/images/hero-avss-2027.png` is the hero background image.

GitHub Pages can render this directly with Jekyll.

## Publish On GitHub Pages

1. Open the repository on GitHub.
2. Go to **Settings** -> **Pages**.
3. Set **Source** to **Deploy from a branch**.
4. Select the `main` branch and the repository root folder `/`.
5. Save. GitHub will build `index.md` into the website homepage.

## Edit Content

Most conference text is in `index.md`. Update the placeholder fields for dates,
location, chairs, speakers, and deadlines when confirmed.

主要内容都在 `index.md`，确认会议日期、地点、主席、讲者和截稿时间后，直接改
这个文件即可。

## Local Preview

Jekyll is available from the conda `base` environment on this machine:

```bash
conda run -n base jekyll build
conda run -n base jekyll serve --host 127.0.0.1 --port 4000
```

If `conda run` keeps the server attached in an awkward way, the linked base
command can also be called directly:

```bash
/opt/miniconda3/bin/jekyll serve --host 127.0.0.1 --port 4000
```
