# Sharon Sharing

Sharon 的个人分享内容仓库，用于沉淀可公开访问的演示页面、分享材料与内容草稿。

## 当前分享

| 主题 | 在线页面 | 内容草稿 |
| --- | --- | --- |
| Codex Sharing 101 | [打开分享页面](https://sharonliao-shopee.github.io/sharon-sharing/codex_sharing_101.html) | [查看 Markdown 大纲](public/codex_sharing_101_draft.md) |
| Codex Sharing 101 — English | [Open the English sharing page](https://sharonliao-shopee.github.io/sharon-sharing/codex_sharing_101_en.html) | [View the English outline](public/codex_sharing_101_en_draft.md) |

> GitHub Pages 首次启用后，在线页面才会生效。后续推送到 `main` 分支时会自动重新部署。

## 仓库结构

```text
.
├── .github/workflows/
│   └── deploy-pages.yml        # GitHub Pages 自动部署
├── public/
│   ├── codex_sharing_101.html  # 可分享的 HTML 页面
│   ├── codex_sharing_101_draft.md
│   ├── codex_sharing_101_en.html       # English sharing page
│   └── codex_sharing_101_en_draft.md   # English outline
└── README.md
```

## 本地预览

直接用浏览器打开 `public/codex_sharing_101.html`，或在仓库根目录启动一个本地静态服务器：

```bash
python3 -m http.server 8000 --directory public
```

然后访问 <http://localhost:8000/codex_sharing_101.html>。

## 发布方式

GitHub Actions 会在以下情况下把 `public/` 目录发布到 GitHub Pages：

- 代码推送到 `main` 分支；
- 在 Actions 页面手动运行 `Deploy GitHub Pages` 工作流。
