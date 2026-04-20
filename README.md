# Ji-Xuan He — Personal Homepage

## 本地预览

```bash
cd ~/personal-homepage
open index.html          # macOS 直接浏览器打开
# 或起一个本地 server：
python3 -m http.server 8000
# 访问 http://localhost:8000
```

## 部署到 GitHub Pages

```bash
cd ~/personal-homepage
git init
git add .
git commit -m "init: personal homepage"
git branch -M main
# 在 GitHub 上创建仓库：JXVision.github.io（仓库名必须等于 username.github.io）
git remote add origin git@github.com:JXVision/JXVision.github.io.git
git push -u origin main
```

推送完成后 1–2 分钟，访问 **https://JXVision.github.io** 即可。

## 需要你替换的内容（已在 HTML 中用占位符标出）

- 头像：把图片放到 `assets/photo.jpg`，然后取消 `index.html` 里对应 `<img>` 注释
- ICME 论文：
  - `DTP: [full paper title]` → 换成完整标题
  - Co-author 列表 → 换成真实作者顺序
  - `[paper]` 链接 → 换成 IEEE Xplore 或 arXiv 链接
- 在投论文标题 → 可先保持匿名或写"Under review"
- 本科学校 / 专业 → 在 Education 部分补上
- Google Scholar 链接 → 如果有的话
- CV PDF → 放到 `assets/cv.pdf`

## 目录结构建议

```
personal-homepage/
├── index.html
├── README.md
└── assets/
    ├── photo.jpg          # 你的头像
    ├── cv.pdf             # 简历 PDF
    ├── dtp.png            # ICME 论文 teaser 图
    └── favicon.ico        # （可选）
```
