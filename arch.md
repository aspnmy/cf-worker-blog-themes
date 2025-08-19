# 架构文档

## 项目概述
本项目是一个基于 Cloudflare Workers 的博客主题系统，包含多个主题模板，用于快速构建博客网站。

## 目录结构
```
cf-worker-blog-themes/
├── LICENSE
├── README.md
└── themes/
    ├── default/
    │   ├── articleList.html
    │   ├── articleListItem.html
    │   ├── articleListItemCategory.html
    │   ├── articleListItemImg.html
    │   ├── articleListItemTags.html
    │   ├── articleListNewer.html
    │   ├── articleListOlder.html
    │   ├── articleSingle.html
    │   ├── articleSingleArticle.html
    │   ├── articleSingleArticleCategory.html
    │   ├── articleSingleArticleTags.html
    │   ├── articleSingleComment.html
    │   ├── articleSingleNewer.html
    │   ├── articleSingleOlder.html
    │   ├── favicon.ico
    │   ├── index.html
    │   ├── style.css
    │   ├── widgetCategory.html
    │   ├── widgetCategoryItem.html
    │   ├── widgetMenu.html
    │   ├── widgetMenuItem.html
    │   ├── widgetRecently.html
    │   ├── widgetRecentlyItem.html
    │   ├── widgetTags.html
    │   ├── widgetTagsItem.html
    │   ├── wp-embed.min.js
    │   ├── wp-emoji-release.min.js
    │   └── admin/
    ├── default2.0/
    ├── JustNews/
    ├── JustNews2/
    └── yinwang/
```

## 核心组件
1. **主题模板** (`themes/default/`)
   - `index.html`: 主页面模板，包含博客的基本结构和布局。
   - `style.css`: 主题样式文件，定义了博客的外观和响应式设计。
   - 文章列表和单篇文章的模板文件（如 `articleList.html`, `articleSingle.html`）。
   - 小部件模板（如 `widgetCategory.html`, `widgetRecently.html`）。

2. **静态资源**
   - `favicon.ico`: 网站图标。
   - JavaScript 文件（如 `wp-embed.min.js`, `wp-emoji-release.min.js`）。

3. **管理界面** (`themes/default/admin/`)
   - 提供博客后台管理的相关功能。

## 技术栈
- **前端**: HTML5, CSS3, JavaScript
- **部署**: Cloudflare Workers

## 架构特点
1. **模块化设计**: 主题模板通过多个 HTML 文件实现模块化，便于维护和扩展。
2. **响应式布局**: 使用 CSS3 实现自适应设计，支持多种设备屏幕。
3. **轻量级**: 静态资源经过压缩，确保快速加载。

## 后续建议
1. 增加更多主题模板以满足不同需求。
2. 优化静态资源加载性能。
3. 提供主题配置选项，支持用户自定义样式。