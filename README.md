# Zhou Chenyang Personal Homepage

这是一个适合 GitHub Pages 部署的静态个人主页项目，定位为金融研究、数据分析、风险管理、行业研究与商业分析方向的专业主页。项目使用纯 HTML、CSS 和少量 JavaScript，不依赖 React、Vue 或其他复杂框架。

## 项目简介

主页内容围绕周晨阳的教育背景、专业经历、研究项目、技能、奖项与求职方向展开，适合在简历、求职邮件、LinkedIn 或 GitHub 个人资料中作为个人主页链接使用。

适配方向包括：

- 券商研究所 / 行业研究 / TMT 或金融方向研究
- 互联网公司的金融研究、策略分析、商业分析方向
- 金融科技、风险管理、数据分析相关岗位

## 文件结构

```text
.
├── index.html
├── styles.css
├── script.js
├── README.md
└── assets/
    └── images/
        ├── avatar.jpg
        ├── avatar-placeholder.svg
        ├── business-photo.jpg
        └── business-photo-placeholder.svg
```

## 如何替换照片

图片统一存放在 `assets/images/` 文件夹中。

- 首页商务照：`assets/images/business-photo.jpg`
- 头像/证件照：`assets/images/avatar.jpg`

替换图片时，保持文件名不变即可直接生效。如果想使用其他文件名，请同步修改 `index.html` 中对应的 `src` 路径。不要在网页中使用本地电脑绝对路径，应使用类似 `assets/images/photo-name.jpg` 的项目相对路径。

## 如何在 GitHub Pages 部署

1. 创建一个 GitHub 仓库，例如 `personal-homepage`。
2. 将本项目中的所有文件上传到仓库根目录。
3. 在 GitHub 仓库页面进入 `Settings`。
4. 打开 `Pages` 设置。
5. 在 `Build and deployment` 中选择：
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/root`
6. 保存后等待 GitHub Pages 构建完成。
7. 访问 GitHub 提供的 Pages 地址，例如：

```text
https://your-username.github.io/personal-homepage/
```

如果仓库名是 `your-username.github.io`，则主页通常会部署到：

```text
https://your-username.github.io/
```

## 如何修改个人信息

主要内容都在 `index.html` 中：

- 姓名、标题和首页介绍：修改 Hero 区域
- 教育背景：修改 `Education` 区域
- 实习经历：修改 `Professional Experience` 区域
- 研究项目：修改 `Featured Projects` 区域
- 技能标签：修改 `Skills` 区域
- 奖项荣誉：修改 `Awards & Honors` 区域
- 邮箱、GitHub、LinkedIn：修改 `Contact` 区域

视觉样式在 `styles.css` 中，包括颜色、间距、卡片、响应式布局和 hover 效果。导航交互、滚动高亮和图片 fallback 逻辑在 `script.js` 中。
