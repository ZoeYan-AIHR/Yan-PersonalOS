# 严琰｜Personal OS

> **企业级组织与人才战略转型实践者｜AI‑Native 组织研究者｜AI + HR Practitioner**  
> 把人、组织、技术与生活放在同一张地图上。

[在线访问](https://<你的-GitHub-用户名>.github.io/<仓库名>/) · [本地打开](#本地预览) · [部署到-github-pages](#部署到-github-pages)

---

## 关于这个项目

这是严琰的个人叙事地图（Personal OS）：以一个可交互的单页网页，串联组织与人才战略实践、AI‑Native 组织研究、学习、摄影与长期训练。

它不是一份静态简历，而是一套持续生长的个人工作与生活操作系统：既记录组织现场的真实问题和实践，也保留对技术、学习、创作与身体的长期投入。

### 五个场域

- **组织与人才战略实践**：扎根业务现场，围绕组织、人才与效率问题持续行动。
- **AI‑Native 组织研究**：探索 AI 如何重塑组织机制、管理方式与人才工作。
- **复旦 MBA · MIT 游学**：用系统学习和跨学科视角扩展管理认知。
- **摄影**：以观察和叙事保留真实的瞬间。
- **训练**：通过长期、稳定的身体训练，建立可持续的节奏与韧性。

---

## 体验亮点

- **单文件交付**：全部页面结构、样式、交互逻辑与人物图像均收纳于一个 `index.html` 文件；不依赖构建工具、CDN 或 `assets` 文件夹。
- **直接可打开**：下载后可直接双击打开，也可以部署到任意静态网站服务。
- **交互式场域探索**：点击场域卡片或导航，右侧信息面板随之切换，呈现每个场域此刻的叙事与状态。
- **可分享的状态链接**：支持 URL Hash 跳转，例如 `#field`、`#lab`、`#learning`、`#photo`、`#training`。
- **轻量动效语言**：借鉴 ThreeUI 的“环境层、焦点反馈、状态信号”思路，以低干扰、可感知的交互反馈增强浏览体验。
- **隐私友好**：当前页面未配置公开邮箱；若未来希望开放联系入口，可在页面脚本中填写 `publicEmail` 变量。

---

## 技术说明

| 项目 | 说明 |
| --- | --- |
| 页面形态 | 原生 HTML / CSS / JavaScript 单页网站 |
| 依赖 | 无 npm、无框架、无构建步骤 |
| 图片策略 | 人物素材以 Base64 形式内嵌，页面无需额外图片目录 |
| 动效策略 | CSS 与轻量 JavaScript 交互，不引入重型 WebGL 场景 |
| 推荐浏览器 | 桌面端 Chrome、Edge、Safari、Firefox 的较新版本 |
| 发布方式 | GitHub Pages 或任意静态托管服务 |

---

## 本地预览

1. 下载仓库中的 `index.html`。
2. 直接双击该文件，或用 Chrome / Edge 打开。
3. 点击场域卡片、顶部导航和右侧导航轨道，体验内容切换与动效反馈。

> 建议优先使用桌面端 Chrome 或 Edge 预览，以获得完整的卡片悬停与鼠标交互效果。

---

## 部署到 GitHub Pages

### 1. 准备文件

请确保仓库根目录至少包含以下两个文件：

```text
.
├── index.html     # 网站主文件（由单文件版本重命名而来）
└── README.md      # 本说明文档
```

> `index.html` 是 GitHub Pages 默认识别的首页文件。项目运行时**不需要** `assets` 文件夹。

### 2. 创建仓库

1. 登录 [GitHub](https://github.com)，点击右上角 **+ → New repository**。
2. 仓库名称建议使用：`YanYan-PersonalOS`。
3. 若希望任何人都可访问作品集，选择 **Public**；若仅用于内部预览，选择 **Private** 并确认你的账号或组织支持 GitHub Pages。
4. 为避免首次上传发生文件冲突，可以暂时不要勾选 “Add a README file”。
5. 点击 **Create repository**。

### 3. 上传网站

1. 将当前单文件网页重命名为 `index.html`。
2. 在新仓库中点击 **Add file → Upload files**。
3. 同时上传 `index.html` 与 `README.md`。
4. 填写提交说明，例如：`feat: publish Personal OS`。
5. 点击 **Commit changes**。

### 4. 启用 GitHub Pages

1. 进入仓库的 **Settings → Pages**。
2. 在 **Build and deployment** 中，将 Source 设置为 **Deploy from a branch**。
3. Branch 选择 `main`，目录选择 `/(root)`，然后点击 **Save**。
4. 等待 GitHub 完成部署。发布地址通常为：

```text
https://<你的-GitHub-用户名>.github.io/YanYan-PersonalOS/
```

### 5. 验证页面

部署完成后，访问上述地址，并分别测试以下链接：

```text
/#overview
/#field
/#lab
/#learning
/#photo
/#training
```

---

## 后续更新

网页内容或动效更新后，只需要：

1. 用新版文件替换仓库根目录的 `index.html`；
2. 在 GitHub 页面提交变更，或通过 Git 执行 `git add`、`git commit`、`git push`；
3. 等待 GitHub Pages 重新发布后刷新访问链接。

推荐使用清晰的提交信息，例如：

```text
feat: refresh AI-Native field narrative
fix: refine learning character edge
style: strengthen field-card interaction feedback
```

---

## 可选：启用社交分享封面

当前网页可保持“运行时单 HTML 文件”的交付方式。不过，Open Graph / 微信 / LinkedIn 等平台的分享卡片通常需要一个可公开访问的独立图片 URL，**无法读取 HTML 内嵌的 Base64 图片**。

如需让分享链接带封面图，可以额外在仓库根目录放置一张 `og-cover.png`，并将页面中的 `og:image` 修改为完整地址：

```html
<meta property="og:image" content="https://<你的-GitHub-用户名>.github.io/YanYan-PersonalOS/og-cover.png" />
```

这张图只服务于社交平台预览；网页本身仍然是一个无需 `assets` 文件夹的独立 HTML 文件。

---

## 使用与版权

本仓库用于展示严琰的个人职业实践、研究与生活叙事。

- 页面中的文字、视觉叙事与人物形象，除另有说明外，版权归严琰所有。
- 未经授权，请勿将人物形象、个人照片或内容用于商业宣传、二次发布或训练用途。
- 如需引用或交流，欢迎通过 GitHub Issue 或未来开放的联系入口留言。

© 2026 严琰. All rights reserved.
