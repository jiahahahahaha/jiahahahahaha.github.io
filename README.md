# jiahahahahaha.github.io

个人主页（GitHub Pages），用于 OpenReview 注册的 Homepage 链接。

最终访问地址：**https://jiahahahahaha.github.io**

## 1. 改内容

只需编辑 `index.html`，搜索并替换这些占位标记：

| 标记 | 换成 |
|---|---|
| `[NAME]` | 你的英文姓名（**必须与论文署名完全一致**） |
| `张甲豪` | 中文名（不需要就删掉整个 `<span class="name-cn">`） |
| `[TAGLINE]` | 一句话研究方向 |
| `[AFFIL]` | 单位 / 院系 |
| `[BIO]` | 自我介绍段落（不需要就删掉那行 `<p>[BIO]</p>`） |
| `[EMAIL]` / `first.author@example.edu` | 你的邮箱（建议与 OpenReview 用同一个） |
| `[SCHOLAR]` `[ORCID]` `[DBLP]` `[OPENREVIEW]` | 对应链接；没有的项把整个 `<a>` 删掉 |
| `[PUB-1]` `[PUB-2]` | 论文条目；多余的 `<article class="pub">` 块删掉 |

本地预览：直接双击 `index.html` 用浏览器打开即可。

## 2. 在 GitHub 上创建仓库

打开 https://github.com/new ，填写：

- **Repository name**：`jiahahahahaha.github.io`（必须一字不差，全小写）
- **Visibility**：`Public`（Pages 免费版必须公开）
- 不要勾选 "Add a README file"

然后点 **Create repository**。

## 3. 推送

```powershell
cd c:/Users/14375/CodeBuddy/jiahahahahaha.github.io
git init -b main
git add .
git commit -m "Add personal homepage"
git remote add origin https://github.com/jiahahahahaha/jiahahahahaha.github.io.git
git push -u origin main
```

首次 push 会弹出 Git Credential Manager 的 GitHub 登录窗口，浏览器授权一次即可。

## 4. 等待生效

推送后 1–2 分钟，访问 https://jiahahahahaha.github.io 就能看到。
若 404，去仓库 **Settings → Pages** 确认 Source 是 `Deploy from a branch`、Branch 是 `main` / `(root)`。

## 5. 后续更新

改完 `index.html` 后：

```powershell
git add . ; git commit -m "Update" ; git push
```

## 备注

- 页面是**单文件、零依赖**（CSS 内联、无外部字体/脚本），所以加载快、不会被墙。
- 已适配深色模式（跟随系统）。
- 拿到这个链接后，填进 OpenReview 注册页的 `Homepage URL` 字段即可。
