# AnZhiYu 博客项目

这是一个基于 Hexo 静态网站生成器和 AnZhiYu 主题的博客项目。

## 项目结构

```
.
├── .github/              # GitHub Actions 工作流
├── node_modules/         # Node.js 依赖包
├── scaffolds/            # 文章模板
│   ├── draft.md         # 草稿模板
│   ├── page.md          # 页面模板
│   └── post.md          # 文章模板
├── source/              # 博客内容源文件
│   └── _posts/          # 博客文章
│       └── welcome.md   # 欢迎文章示例
├── themes/              # 主题目录
│   └── anzhiyu/        # AnZhiYu 主题
│       ├── layout/      # 模板文件
│       ├── languages/   # 语言文件
│       ├── scripts/     # 脚本文件
│       ├── source/      # 静态资源
│       ├── _config.yml  # 主题配置文件
│       ├── plugins.yml  # 插件配置
│       └── sw-rules.js # Service Worker 规则
├── .gitignore          # Git 忽略文件
├── LICENSE             # 许可证
├── README.md           # 项目说明
├── README_EN.md        # 英文项目说明
├── _config.yml         # Hexo 主配置文件
├── _config.anzhiyu.yml # AnZhiYu 主题配置覆盖
├── package.json        # Node.js 依赖配置
└── package-lock.json   # 依赖锁定文件
```

## 安装依赖

```bash
npm install
```

## 开发命令

- `npm run server` - 启动本地开发服务器
- `npm run generate` - 生成静态文件
- `npm run deploy` - 部署到服务器
- `npm run new <title>` - 创建新文章

## 创建文章

```bash
npm run new "我的新文章"
```

## 本地预览

```bash
npm run server
```

访问 http://localhost:4000 预览博客

## 部署到 Cloudflare Pages

1. 将代码推送到 GitHub 仓库
2. 在 Cloudflare Pages 中连接该仓库
3. 设置构建设置：
   - 构建命令：`npm run generate`
   - 构建输出目录：`public`
   - Node.js 版本：18 或更高

## 主题配置

主题配置文件位于 `_config.anzhiyu.yml`，可以根据需要进行自定义。

## 主要特性

- 响应式设计，适配各种设备
- 支持多种评论系统（Valine, Waline, Twikoo 等）
- 内置搜索功能
- 代码高亮
- 数学公式支持
- Service Worker 支持
- PWA 特性

## 技术栈

- Hexo 静态网站生成器
- AnZhiYu 主题
- Pug 模板引擎
- Stylus CSS 预处理器
- Cloudflare Pages 部署

## 许可证

GPL-3.0