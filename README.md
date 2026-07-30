# ForU伴学官网发布版

这是本次可直接上传到 GitHub 的静态官网版本。

## 文件说明

- `index.html`：官网主页，CSS 和 JS 已内联。
- `students.json`：成长星球学员城市、简介和链接数据。
- `public/logo.png`：网站 Logo 与路径图水印。
- `public/wechat-qr.jpg`：JoJo 老师微信二维码。
- `public/favicon.png`：浏览器标签页图标。
- `public/phonics-audio/`：自然拼读练习室 AI 英音示范音频；以后可用正式 AI 音频覆盖同名文件。

## 上传 GitHub 时只上传这些内容

请上传本文件夹 `foru-homepage-github-release` 里面的文件，不要上传外层目录里的旧版本、压缩包、`.next`、`node_modules` 或备份文件。

推荐仓库结构：

```text
your-github-repo/
├── index.html
├── students.json
├── README.md
├── .nojekyll
└── public/
    ├── favicon.png
    ├── logo.png
    ├── wechat-qr.jpg
    └── phonics-audio/
        ├── prompt-set-01-core.mp3
        ├── sound-s.mp3
        └── word-sat.mp3
```

## 预览注意

成长星球需要通过网页服务器读取 `students.json`。如果直接双击打开 `index.html`，部分浏览器可能拦截 JSON 读取；上传 GitHub Pages、Vercel 或用本地 `http://localhost` 预览都可以正常读取。
