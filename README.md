# jiahahahahaha.github.io

个人主页（GitHub Pages），用于 OpenReview 注册的 Homepage 链接。

最终访问地址：**https://jiahahahahaha.github.io**

## 1. 改内容

只需编辑 `index.html`。已填好的信息（无需改动）：

- 姓名：Longjie Jia / 贾龙杰
- 单位：College of Computer Science and Technology, National University of Defense Technology (NUDT), Changsha, China
- 邮箱：jialongjie@nudt.edu.cn

还需要你补的占位标记：

| 标记 | 换成 |
|---|---|
| `[COAUTHORS]` | 论文合作者，按署名顺序，例如 `Jane Doe, Wei Wang` |
| `[VENUE]` | 会议/期刊或状态，例如 `Under review`、`IMC 2027` |
| `PDF` / `Code` / `DOI` 三条链接 | 真实链接；没有的整条 `<a>` 删掉 |

> **姓名必须与论文署名完全一致**（英文名顺序按你论文里的写法；若论文用 `Jia, Longjie`，就把 `Longjie Jia` 改成对应写法）。

另外 HTML 里有三处被注释掉、等你拿到链接后启用的按钮，把 `<!--` 和 `-->` 去掉再填 URL 即可：

```html
<!-- <a href="[SCHOLAR]">Google Scholar</a> -->
<!-- <a href="[ORCID]">ORCID</a> -->
<!-- <a href="[DBLP]">DBLP</a> -->
<!-- <a href="[OPENREVIEW]">OpenReview</a> -->
```

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
