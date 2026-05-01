<div align="center">

# 文物智鉴 · ArtiGuide

**深色科技风格展示页面框架 | 适用于项目答辩、产品展示、技术演示**

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![GSAP](https://img.shields.io/badge/GSAP-88CE02?style=flat&logo=greensock&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-blue.svg)

[English](#english) | 中文

</div>

---

## 项目简介

这是一个精心设计的深色主题展示页面框架，专为**项目答辩**、**产品发布**、**技术演示**和**作品集展示**等场景打造。页面采用现代前端技术栈，集成了丰富的交互动画效果，开箱即用，只需替换内容即可快速搭建专业的展示页面。

## 效果预览

> 💡 建议：可录制 GIF 或截图放置于此处展示效果

<!-- ![预览截图](./preview.gif) -->

### 核心特性

| 特性 | 说明 |
|------|------|
| 粒子动画背景 | 基于 tsparticles 的动态粒子网络，支持交互抓取 |
| 鼠标跟踪光晕 | 鼠标移动时产生柔和的光晕跟随效果 |
| 3D 卡片倾斜 | VanillaTilt.js 实现的卡片 3D 倾斜与光泽反射 |
| 滚动触发动画 | GSAP + ScrollTrigger 实现的滚动入场动画 |
| Tab 标签页切换 | 平滑的标签页切换动画与粒子颜色过渡 |
| PPT 幻灯片展示 | 全屏幻灯片模式，支持键盘导航与指示器 |
| 聚光灯效果 | 悬停卡片时其他卡片自动淡化 |
| 数字滚动动画 | 首页统计数据的动态计数效果 |
| 响应式设计 | 完美适配桌面端与移动端 |

## 快速开始

### 方式一：直接下载

1. 点击页面上方绿色 `Code` 按钮 → `Download ZIP`
2. 解压后用浏览器打开 `perform.html` 即可预览

### 方式二：Git 克隆

```bash
git clone https://github.com/zgy123454zgy-afk/arti-guide-showcase.git
cd arti-guide-showcase
# 直接用浏览器打开 perform.html
```

### 方式三：GitHub Pages 部署

1. Fork 本仓库
2. 进入仓库 `Settings` → `Pages`
3. Source 选择 `Deploy from a branch`
4. Branch 选择 `main`，文件夹选择 `/ (root)`
5. 点击 `Save`，等待部署完成
6. 访问 `https://<你的用户名>.github.io/arti-guide-showcase/`

## 项目结构

```
arti-guide-showcase/
│
├── perform.html              # 主页面（HTML + CSS + JavaScript 一体化）
│
├── ppt/                      # PPT 图片存放目录
│   └── README.md             # PPT 配置详细说明
│
├── .gitignore                # Git 忽略规则
├── LICENSE                   # MIT 开源协议
└── README.md                 # 项目说明文档（本文件）
```

> **设计说明：** 本项目采用单文件架构（Single File Architecture），将 HTML、CSS、JavaScript 整合在同一文件中，便于分发和部署，无需构建工具。

## 使用指南

### 1. 修改页面内容

#### 修改标题与描述

在 `perform.html` 中找到 Hero 区域：

```html
<!-- ==============================================
HERO
============================================== -->
<header class="hero" id="hero">
    <h1 id="hero-title">
        <span>你的主标题</span>
        <span class="highlight">你的副标题</span>
    </h1>
    <p id="hero-desc">你的项目描述文字...</p>
</header>
```

#### 修改统计数据

```html
<div class="hero-stat">
    <div class="num" data-target="1115">0</div>  <!-- 修改数字 -->
    <div class="label">文物藏品</div>              <!-- 修改标签 -->
</div>
```

#### 修改数据卡片

在 JavaScript 部分找到数据数组并修改：

```javascript
const dataSources = [
    {
        name: "卡片标题",
        field: "分类标签",
        desc: "卡片描述内容...",
        tags: ["标签1", "标签2", "标签3"],
        url: "https://链接地址"
    },
    // 添加更多卡片...
];

const features = [
    // 同上结构
];
```

### 2. 配置 PPT 幻灯片展示

本项目支持嵌入 PPT 展示功能，适用于答辩场景：

**步骤：**

1. 将你的 PPT 导出为图片格式（推荐 PNG，支持 JPG）
2. 在项目根目录下创建 `ppt` 文件夹
3. 将图片按顺序放入，命名为 `1.png`、`2.png`、`3.png`...
4. 修改 `perform.html` 中的配置：

```javascript
// ========== PPT 配置区域 ==========
const PPT_TOTAL = 17;           // ← 修改为你的 PPT 图片总数
const PPT_PATH = './ppt/';      // ← 图片存放路径
const PPT_IMAGES = [];          // ← 可选：自定义文件名数组
// ========== 配置区域结束 ==========
```

**自定义文件名示例：**

```javascript
const PPT_TOTAL = 10;
const PPT_PATH = './ppt/';
const PPT_IMAGES = [
    'title.png',
    'overview.png',
    'architecture.png',
    'demo.png',
    'results.png',
    'comparison.png',
    'future.png',
    'team.png',
    'thanks.png',
    'q&a.png'
];
```

**PPT 图片导出建议：**

| 项目 | 推荐值 |
|------|--------|
| 图片格式 | PNG（画质最佳）或 JPG |
| 分辨率 | 1920 × 1080（16:9） |
| 单张大小 | < 2MB |
| 命名方式 | 数字序号或有意义的英文名 |

> 详细配置说明请查看 [`ppt/README.md`](./ppt/README.md)

### 3. 自定义样式主题

#### 修改颜色方案

在 `perform.html` 的 CSS `:root` 变量中修改：

```css
:root {
    --bg-dark: #030307;           /* 页面背景色 */
    --bg-card: rgba(13,13,23,0.6);/* 卡片背景色 */
    --text-primary: #ffffff;      /* 主文字颜色 */
    --text-secondary: rgba(255,255,255,0.6); /* 次文字颜色 */
    --accent-glow: #d4a843;       /* 主强调色（金色） */
    --accent-purple: #2e8b57;     /* 次强调色（绿色） */
    --accent-jade: #3aaf7c;       /* 辅助强调色 */
    --glass-border: rgba(255,255,255,0.06); /* 玻璃边框色 */
    --glass-bg: rgba(255,255,255,0.03);     /* 玻璃背景色 */
}
```

#### 配色方案参考

| 风格 | accent-glow | accent-purple | 效果 |
|------|-------------|---------------|------|
| 金色科技（默认） | `#d4a843` | `#2e8b57` | 高端、科技感 |
| 蓝色海洋 | `#4a9eff` | `#1a6bff` | 清新、专业 |
| 紫色梦幻 | `#9b59b6` | `#8e44ad` | 神秘、创意 |
| 红色中国 | `#e74c3c` | `#c0392b` | 喜庆、传统 |

#### 修改粒子效果

```javascript
tsParticles.load("tsparticles", {
    particles: {
        number: { value: 80 },        // 粒子数量
        color: { value: "#d4a843" },   // 粒子颜色
        links: {
            distance: 150,             // 连线距离
            color: "#d4a843",          // 连线颜色
            opacity: 0.2               // 连线透明度
        },
        move: { speed: 1 }            // 移动速度
    }
});
```

## 技术栈

| 技术 | 版本 | 用途 |
|------|------|------|
| HTML5 | - | 页面结构 |
| CSS3 | - | 样式与动画 |
| JavaScript | ES6+ | 交互逻辑 |
| [tsparticles](https://particles.js.org/) | 2.12.0 | 粒子动画背景 |
| [VanillaTilt](https://micku7zu.github.io/vanilla-tilt.js/) | 1.8.1 | 卡片 3D 倾斜效果 |
| [GSAP](https://greensock.com/gsap/) | 3.12.2 | 动画引擎 |
| [ScrollTrigger](https://greensock.com/scrolltrigger/) | 3.12.2 | 滚动触发动画 |
| [Google Fonts](https://fonts.google.com/) | - | Inter 字体 |

## 浏览器兼容性

| 浏览器 | 最低版本 |
|--------|----------|
| Chrome | 80+ |
| Firefox | 75+ |
| Safari | 13+ |
| Edge | 80+ |

> 本项目使用了 CSS Custom Properties、backdrop-filter、CSS Grid 等现代特性，请确保目标浏览器支持。

## 常见问题

### Q: 页面打开后背景是黑色的，没有粒子效果？

A: 粒子动画依赖外部 CDN 加载，请确保网络可以访问 `cdn.jsdelivr.net` 和 `cdnjs.cloudflare.com`。

### Q: PPT 图片无法显示？

A: 请检查：
1. `ppt` 文件夹是否存在且包含图片
2. `perform.html` 中 `PPT_TOTAL` 是否正确设置
3. 图片格式是否为 PNG 或 JPG
4. 图片命名是否与配置一致

### Q: 移动端体验不佳？

A: 本项目已做响应式适配，但部分 3D 效果在移动端会自动禁用以提升性能。

### Q: 如何添加新的 Tab 页面？

A: 参考现有代码结构，在 HTML 中添加 `.tab-panel`，在 JavaScript 中添加对应的数据数组和渲染函数。

## 贡献指南

欢迎提交 Issue 和 Pull Request！

1. Fork 本仓库
2. 创建特性分支：`git checkout -b feature/your-feature`
3. 提交更改：`git commit -m 'Add some feature'`
4. 推送分支：`git push origin feature/your-feature`
5. 提交 Pull Request

## 开源协议

本项目基于 [MIT License](./LICENSE) 开源。

```
MIT License

Copyright (c) 2026

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software...
```

## 致谢

- [tsparticles](https://particles.js.org/) - 粒子动画库
- [GSAP](https://greensock.com/) - 专业级动画引擎
- [VanillaTilt.js](https://micku7zu.github.io/vanilla-tilt.js/) - 轻量级倾斜效果库
- [Google Fonts](https://fonts.google.com/) - Inter 字体

---

<div align="center">

**如果这个项目对你有帮助，请给一个 ⭐ Star 支持一下！**

Made with ❤️

</div>
