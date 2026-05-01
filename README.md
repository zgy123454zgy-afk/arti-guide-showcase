<div align="center">

# 文物智鉴 · ArtiGuide

### 深色科技风格展示页面框架

**适用于项目答辩 · 产品发布 · 技术演示 · 作品集展示**

<br>

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![GSAP](https://img.shields.io/badge/GSAP-3.12-88CE02?style=for-the-badge&logo=greensock&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-007ACC?style=for-the-badge)
![Stars](https://img.shields.io/github/stars/zgy123454zgy-afk/arti-guide-showcase?style=for-the-badge)
![Forks](https://img.shields.io/github/forks/zgy123454zgy-afk/arti-guide-showcase?style=for-the-badge)

<br>

**[English](./README_EN.md)** | 中文

<br>

![demo](https://img.shields.io/badge/🎬_在线预览-GitHub_Pages-238636?style=for-the-badge&logo=github)
![download](https://img.shields.io/badge/📦_下载源码-ZIP-007ACC?style=for-the-badge&logo=github)

</div>

---

## 📑 目录

- [项目简介](#-项目简介)
- [核心特性](#-核心特性)
- [效果预览](#-效果预览)
- [快速开始](#-快速开始)
- [项目结构](#-项目结构)
- [使用指南](#-使用指南)
  - [修改页面内容](#1-修改页面内容)
  - [配置 PPT 幻灯片](#2-配置-ppt-幻灯片展示)
  - [自定义样式主题](#3-自定义样式主题)
  - [修改粒子效果](#4-修改粒子效果)
  - [修改导航栏](#5-修改导航栏)
- [技术栈详解](#-技术栈详解)
- [浏览器兼容性](#-浏览器兼容性)
- [部署指南](#-部署指南)
- [常见问题](#-常见问题)
- [更新日志](#-更新日志)
- [贡献指南](#-贡献指南)
- [开源协议](#-开源协议)
- [致谢](#-致谢)
- [联系方式](#-联系方式)

---

## 📖 项目简介

**文物智鉴 · ArtiGuide** 是一个精心设计的深色主题展示页面框架，专为需要高质量视觉呈现的场景打造。

### 适用场景

| 场景 | 说明 |
|------|------|
| 🎓 项目答辩 | 毕业设计、课程项目、课题汇报 |
| 🚀 产品发布 | 新功能上线、版本更新公告 |
| 💻 技术演示 | 技术分享、架构设计展示 |
| 🎨 作品集 | 设计师、开发者个人作品展示 |
| 📊 数据报告 | 数据分析结果可视化展示 |
| 🏢 公司官网 | 产品官网、企业介绍页面 |

### 为什么选择这个框架？

- **开箱即用** - 单文件架构，无需安装任何依赖，下载即用
- **高度可定制** - 所有内容、样式、动画均可轻松修改
- **专业视觉效果** - 粒子动画、3D 卡片、平滑过渡等专业级效果
- **响应式设计** - 完美适配从手机到桌面的各种屏幕尺寸
- **零学习成本** - 代码结构清晰，注释完善，易于理解和修改

---

## ✨ 核心特性

### 视觉效果

| 特性 | 描述 | 技术实现 |
|------|------|----------|
| 粒子动画背景 | 动态粒子网络，鼠标可交互抓取 | tsparticles 2.12 |
| 鼠标跟踪光晕 | 柔和的光晕跟随鼠标移动 | JavaScript + CSS |
| 3D 卡片倾斜 | 鼠标悬停时卡片产生 3D 倾斜效果 | VanillaTilt.js |
| 卡片呼吸光效 | 卡片边框缓慢闪烁的呼吸动画 | CSS Animation |
| 光泽扫过效果 | 悬停时光泽从卡片表面扫过 | CSS Transform |
| 数字滚动动画 | 统计数据从 0 动态增长到目标值 | GSAP |

### 交互功能

| 特性 | 描述 | 技术实现 |
|------|------|----------|
| Tab 标签页切换 | 平滑切换内容区域，粒子颜色随之变化 | GSAP |
| 聚光灯效果 | 悬停卡片时其他卡片自动淡化 | CSS + JavaScript |
| 滚动触发动画 | 元素进入视口时自动播放入场动画 | ScrollTrigger |
| PPT 幻灯片展示 | 全屏模式浏览演示文稿 | JavaScript |
| 返回顶部按钮 | 滚动后自动显示，点击平滑回顶 | JavaScript |
| 卡片涟漪按钮 | 点击按钮产生扩散涟漪效果 | CSS Animation |

### 布局设计

| 特性 | 描述 |
|------|------|
| 响应式网格 | 自动适应屏幕宽度的卡片网格布局 |
| 粘性导航栏 | 滚动时导航栏固定在顶部 |
| 滚动指示器 | 首页底部的向下滚动提示 |
| 玻璃拟态 | 半透明模糊背景的现代 UI 风格 |

---

## 🎬 效果预览

> 💡 **提示：** 建议在此处添加项目截图或 GIF 动图

<!-- 
### 首页效果
![首页预览](./screenshots/hero.png)

### 卡片效果
![卡片预览](./screenshots/cards.png)

### PPT 展示
![PPT预览](./screenshots/ppt.png)

### 移动端适配
![移动端预览](./screenshots/mobile.png)
-->

**如何添加预览截图：**

1. 在项目根目录创建 `screenshots` 文件夹
2. 将截图放入该文件夹
3. 取消上面注释并修改图片路径

---

## 🚀 快速开始

### 方式一：直接下载（推荐新手）

```
1. 点击页面上方绿色 [Code] 按钮
2. 选择 [Download ZIP]
3. 解压下载的文件
4. 双击用浏览器打开 perform.html
```

### 方式二：Git 克隆

```bash
# 克隆仓库
git clone https://github.com/zgy123454zgy-afk/arti-guide-showcase.git

# 进入项目目录
cd arti-guide-showcase

# 用浏览器打开（Windows）
start perform.html

# 用浏览器打开（Mac）
open perform.html

# 用浏览器打开（Linux）
xdg-open perform.html
```

### 方式三：GitHub Pages 在线部署

```bash
# 1. Fork 本仓库到你的账号
# 2. 进入你 Fork 的仓库
# 3. Settings → Pages
# 4. Source: Deploy from a branch
# 5. Branch: main, 文件夹: / (root)
# 6. 点击 Save
# 7. 等待 1-2 分钟，访问: https://<你的用户名>.github.io/arti-guide-showcase/
```

### 方式四：本地服务器运行

```bash
# 使用 Python
python -m http.server 8080

# 使用 Node.js (需安装 http-server)
npx http-server -p 8080

# 使用 PHP
php -S localhost:8080

# 然后访问 http://localhost:8080
```

---

## 📁 项目结构

```
arti-guide-showcase/
│
├── perform.html                # 主页面文件（HTML + CSS + JavaScript）
│   │
│   ├── <style>                 # 所有 CSS 样式
│   │   ├── 变量定义            # :root CSS Variables
│   │   ├── 布局样式            # Grid, Flexbox
│   │   ├── 组件样式            # Cards, Buttons, Navigation
│   │   ├── 动画定义            # @keyframes
│   │   └── 响应式              # @media queries
│   │
│   ├── <body>                  # HTML 结构
│   │   ├── Navigation          # 顶部导航栏
│   │   ├── Hero                # 首页大图区域
│   │   ├── Highlights Banner   # 滚动高亮横幅
│   │   ├── Tab Switcher        # 标签页切换器
│   │   ├── Content Panels      # 内容面板
│   │   ├── PPT Modal           # PPT 弹窗
│   │   └── Footer              # 页脚
│   │
│   └── <script>                # JavaScript 逻辑
│       ├── 数据定义            # dataSources, features
│       ├── 动画初始化          # GSAP, tsparticles
│       ├── 交互逻辑            # Tab, Filter, PPT
│       └── 工具函数            # Helpers
│
├── ppt/                        # PPT 图片存放目录
│   ├── 1.png                   # 第 1 页幻灯片
│   ├── 2.png                   # 第 2 页幻灯片
│   ├── ...                     # 更多幻灯片
│   └── README.md               # PPT 配置说明
│
├── screenshots/                # 项目截图（可选）
│   ├── hero.png
│   ├── cards.png
│   └── mobile.png
│
├── .gitignore                  # Git 忽略规则
├── LICENSE                     # MIT 开源协议
├── README.md                   # 中文说明文档
└── README_EN.md                # 英文说明文档
```

### 设计理念

> **单文件架构（Single File Architecture）**
> 
> 本项目将所有代码整合在单个 HTML 文件中，这是有意为之的设计选择：
> - ✅ 便于分发 - 只需一个文件即可分享
> - ✅ 便于部署 - 上传到任何静态服务器即可运行
> - ✅ 便于理解 - 所有代码集中在一起，易于学习
> - ✅ 无需构建 - 不需要 npm、webpack 等工具
> 
> 如果需要拆分为多文件结构，可自行重构。

---

## 📘 使用指南

### 1. 修改页面内容

#### 修改网站标题

```html
<!-- 在 <head> 中修改 -->
<title>你的项目名称 | 你的项目副标题</title>

<!-- 在导航栏中修改 -->
<div class="logo">你的项目名称</div>
```

#### 修改 Hero 区域

```html
<header class="hero" id="hero">
    <!-- 主标题 - 支持两行 -->
    <h1 id="hero-title">
        <span>第一行标题</span>
        <span class="highlight">第二行标题（高亮）</span>
    </h1>
    
    <!-- 描述文字 -->
    <p id="hero-desc">你的项目描述，建议控制在 100-200 字...</p>
    
    <!-- 统计数据 -->
    <div class="hero-stats" id="hero-stats">
        <div class="hero-stat">
            <div class="num" data-target="1000">0</div>
            <div class="label">数据指标1</div>
        </div>
        <div class="hero-stat">
            <div class="num" data-target="50">0</div>
            <div class="label">数据指标2</div>
        </div>
        <div class="hero-stat">
            <div class="num" data-target="100">0</div>
            <div class="label">数据指标3</div>
        </div>
        <div class="hero-stat">
            <div class="num" data-target="5000">0</div>
            <div class="label">数据指标4</div>
        </div>
    </div>
</header>
```

#### 修改高亮横幅

```html
<div class="highlights-track" id="highlights-track">
    <span class="highlight-item">
        <span class="dot"></span>
        你的高亮文字<strong>重点内容</strong>
    </span>
    <!-- 复制以上结构添加更多项，注意需要重复一遍以实现无缝滚动 -->
</div>
```

#### 修改数据卡片

```javascript
// 在 JavaScript 部分找到并修改

const dataSources = [
    {
        name: "卡片标题",           // 显示在左上角
        field: "分类标签",          // 显示在右上角的标签
        desc: "卡片描述内容...",    // 中间的描述文字
        tags: ["标签1", "标签2"],   // 底部标签列表
        url: "https://..."         // 按钮链接地址
    },
    // 继续添加更多卡片...
];

const sourceCategories = ["全部", "分类1", "分类2", "分类3"];

const features = [
    // 同样的结构...
];

const featureCategories = ["全部", "分类A", "分类B", "分类C"];
```

#### 修改导航栏链接

```html
<nav>
    <div class="logo">文物智鉴 · ArtiGuide</div>
    <div class="nav-links">
        <a onclick="switchTab('sources')">数据来源</a>        <!-- 切换到数据来源标签 -->
        <a onclick="switchTab('features')">核心功能</a>       <!-- 切换到核心功能标签 -->
        <a onclick="openPPT()">答辩PPT</a>                   <!-- 打开PPT弹窗 -->
        <a href="https://github.com/..." target="_blank">GitHub</a>  <!-- 外部链接 -->
    </div>
</nav>
```

#### 修改页脚

```html
<div class="footer">
    <p>&copy; 2026 <strong>你的项目名称</strong> — 你的项目描述</p>
    <p style="margin-top: 8px; font-size: 12px;">
        技术栈1 · 技术栈2 · 技术栈3
    </p>
</div>
```

---

### 2. 配置 PPT 幻灯片展示

#### 基本配置

```javascript
// 在 perform.html 的 JavaScript 部分找到：

// ========== PPT 配置区域 ==========
const PPT_TOTAL = 17;              // ← 修改为你的 PPT 图片总数
const PPT_PATH = './ppt/';         // ← 图片存放路径
const PPT_IMAGES = [];             // ← 可选：自定义文件名数组
// ========== 配置区域结束 ==========
```

#### 使用默认命名（推荐）

将图片命名为 `1.png`、`2.png`... 放入 `ppt` 文件夹：

```javascript
const PPT_TOTAL = 10;              // 你有 10 张图片
const PPT_PATH = './ppt/';
const PPT_IMAGES = [];             // 留空，自动使用 1.png ~ 10.png
```

#### 使用自定义命名

```javascript
const PPT_TOTAL = 5;
const PPT_PATH = './ppt/';
const PPT_IMAGES = [
    '封面.png',
    '目录.png',
    '内容1.png',
    '内容2.png',
    '总结.png'
];
```

#### PPT 图片导出指南

| 软件 | 导出方式 |
|------|----------|
| Microsoft PowerPoint | 文件 → 另存为 → PNG/JPG |
| WPS 演示 | 文件 → 输出为图片 |
| Google Slides | 文件 → 下载 → PNG 图像 |
| Keynote | 文件 → 导出到 → 图像 |
| LibreOffice Impress | 文件 → 导出 → PNG |

**推荐设置：**

- 格式：PNG（无损压缩，画质最佳）
- 分辨率：1920 × 1080（16:9 宽屏）
- 单张大小：< 2MB（保证加载速度）

---

### 3. 自定义样式主题

#### CSS 变量一览

```css
:root {
    /* ===== 背景色 ===== */
    --bg-dark: #030307;                        /* 页面主背景 */
    --bg-card: rgba(13, 13, 23, 0.6);          /* 卡片背景 */
    
    /* ===== 文字颜色 ===== */
    --text-primary: #ffffff;                    /* 主文字 */
    --text-secondary: rgba(255, 255, 255, 0.6); /* 次文字 */
    
    /* ===== 强调色 ===== */
    --accent-glow: #d4a843;                     /* 主强调色 */
    --accent-purple: #2e8b57;                   /* 次强调色 */
    --accent-jade: #3aaf7c;                     /* 辅助色 */
    
    /* ===== 玻璃效果 ===== */
    --glass-border: rgba(255, 255, 255, 0.06);  /* 边框 */
    --glass-bg: rgba(255, 255, 255, 0.03);      /* 背景 */
    
    /* ===== 字体 ===== */
    --font-main: 'Inter', -apple-system, sans-serif;
    
    /* ===== 缓动函数 ===== */
    --ease-out-expo: cubic-bezier(0.19, 1, 0.22, 1);
}
```

#### 预设配色方案

**方案 A：金色科技（默认）**
```css
--accent-glow: #d4a843;
--accent-purple: #2e8b57;
--accent-jade: #3aaf7c;
```

**方案 B：蓝色海洋**
```css
--accent-glow: #4a9eff;
--accent-purple: #1a6bff;
--accent-jade: #00d4ff;
```

**方案 C：紫色星空**
```css
--accent-glow: #9b59b6;
--accent-purple: #8e44ad;
--accent-jade: #c39bd3;
```

**方案 D：红色中国风**
```css
--accent-glow: #e74c3c;
--accent-purple: #c0392b;
--accent-jade: #f39c12;
```

**方案 E：青色极简**
```css
--accent-glow: #00bcd4;
--accent-purple: #0097a7;
--accent-jade: #4dd0e1;
```

---

### 4. 修改粒子效果

```javascript
tsParticles.load("tsparticles", {
    fpsLimit: 120,
    particles: {
        number: { 
            value: 80,                    // 粒子数量（50-150 较好）
            density: { enable: true, area: 800 }
        },
        color: { value: "#d4a843" },      // 粒子颜色
        shape: { type: "circle" },        // 形状：circle / edge / triangle / polygon / star
        opacity: { 
            value: 0.5,                   // 透明度
            random: true,                 // 随机透明度
            anim: { enable: true, speed: 1, opacity_min: 0.1 }
        },
        size: { value: 1, random: true }, // 大小
        links: { 
            enable: true,                 // 是否显示连线
            distance: 150,                // 连线距离
            color: "#d4a843",             // 连线颜色
            opacity: 0.2,                 // 连线透明度
            width: 1                      // 连线宽度
        },
        move: { 
            enable: true, 
            speed: 1,                     // 移动速度（0.5-3）
            direction: "none", 
            random: true, 
            straight: false, 
            outModes: "out" 
        }
    },
    interactivity: {
        events: { 
            onHover: { enable: true, mode: "grab" },    // 悬停：grab / bubble / repulse
            onclick: { enable: true, mode: "push" }     // 点击：push / remove / bubble
        },
        modes: { 
            grab: { distance: 200, links: { opacity: 0.5 } } 
        }
    },
    detectRetina: true
});
```

#### 粒子效果预设

**密集星空** - 适合科技主题
```javascript
number: { value: 150 },
size: { value: 1.5, random: true },
links: { distance: 120, opacity: 0.15 },
move: { speed: 0.5 }
```

**稀疏优雅** - 适合简约主题
```javascript
number: { value: 40 },
size: { value: 2, random: true },
links: { distance: 200, opacity: 0.3 },
move: { speed: 0.8 }
```

**快速动态** - 适合活泼主题
```javascript
number: { value: 60 },
size: { value: 1 },
links: { distance: 180, opacity: 0.25 },
move: { speed: 3, random: false }
```

---

### 5. 修改导航栏

#### 添加新导航项

```html
<nav>
    <div class="logo">你的项目名</div>
    <div class="nav-links">
        <!-- 内部标签切换 -->
        <a onclick="switchTab('sources')">数据来源</a>
        <a onclick="switchTab('features')">核心功能</a>
        
        <!-- 打开 PPT -->
        <a onclick="openPPT()">PPT展示</a>
        
        <!-- 外部链接 -->
        <a href="https://github.com/你的用户名/仓库名" target="_blank">GitHub</a>
        <a href="https://你的博客地址" target="_blank">博客</a>
        <a href="mailto:你的邮箱@example.com">联系我</a>
        
        <!-- 锚点跳转 -->
        <a href="#footer" onclick="document.getElementById('footer').scrollIntoView({behavior:'smooth'})">联系我们</a>
    </div>
</nav>
```

#### 导航栏样式调整

```css
/* 修改导航栏高度 */
nav {
    height: 72px;  /* 修改此值 */
    padding: 0 5%; /* 左右间距 */
}

/* 修改导航链接间距 */
.nav-links { 
    display: flex; 
    gap: 24px; /* 修改此值调整间距 */
}

/* 修改 Logo 样式 */
.logo {
    font-size: 22px;    /* 字体大小 */
    font-weight: 800;   /* 字体粗细 */
}
```

---

## 🔧 技术栈详解

### 前端基础

| 技术 | 版本 | 说明 | 官网 |
|------|------|------|------|
| HTML5 | - | 页面结构，语义化标签 | [MDN](https://developer.mozilla.org/zh-CN/docs/Web/HTML) |
| CSS3 | - | 样式布局，动画效果 | [MDN](https://developer.mozilla.org/zh-CN/docs/Web/CSS) |
| JavaScript | ES6+ | 交互逻辑，动态效果 | [MDN](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript) |

### 第三方库

| 库 | 版本 | 大小 | 用途 | CDN |
|----|------|------|------|-----|
| tsparticles | 2.12.0 | ~60KB | 粒子动画背景 | [jsDelivr](https://cdn.jsdelivr.net/npm/tsparticles@2.12.0/) |
| VanillaTilt | 1.8.1 | ~8KB | 卡片 3D 倾斜效果 | [cdnjs](https://cdnjs.cloudflare.com/ajax/libs/vanilla-tilt/1.8.1/) |
| GSAP | 3.12.2 | ~30KB | 专业级动画引擎 | [cdnjs](https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/) |
| ScrollTrigger | 3.12.2 | ~15KB | 滚动触发动画插件 | [cdnjs](https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/) |
| Inter Font | - | ~30KB | 界面字体 | [Google Fonts](https://fonts.googleapis.com/css2?family=Inter) |

### CSS 特性

| 特性 | 用途 | 兼容性 |
|------|------|--------|
| CSS Custom Properties | 主题颜色变量 | Chrome 49+ |
| CSS Grid | 卡片网格布局 | Chrome 57+ |
| Flexbox | 各种布局场景 | Chrome 29+ |
| backdrop-filter | 玻璃模糊效果 | Chrome 76+ |
| @keyframes | 动画定义 | Chrome 43+ |
| perspective / transform-style | 3D 效果 | Chrome 36+ |

### JavaScript API

| API | 用途 |
|-----|------|
| requestAnimationFrame | 流畅动画循环 |
| IntersectionObserver | 元素可见性检测 |
| Web Audio API | 音频可视化（可选） |
| KeyboardEvent | 键盘快捷键支持 |
| MouseEvent | 鼠标交互效果 |

---

## 🌐 浏览器兼容性

| 浏览器 | 最低版本 | 完全支持 | 备注 |
|--------|----------|----------|------|
| Google Chrome | 80+ | ✅ | 推荐使用 |
| Microsoft Edge | 80+ | ✅ | 基于 Chromium |
| Mozilla Firefox | 75+ | ✅ | - |
| Apple Safari | 13+ | ✅ | macOS / iOS |
| Opera | 67+ | ✅ | 基于 Chromium |
| Samsung Internet | 13+ | ✅ | 移动端 |
| IE | 11 | ⚠️ | 部分功能不可用 |

> **注意：** 本项目使用了 `backdrop-filter`、`CSS Grid`、CSS Variables 等现代特性，在较旧的浏览器中可能无法正常显示所有效果。

---

## 🚀 部署指南

### GitHub Pages（推荐）

```bash
# 步骤 1: Fork 本仓库
# 步骤 2: 进入你 Fork 的仓库
# 步骤 3: Settings → Pages
# 步骤 4: Source 选择 "Deploy from a branch"
# 步骤 5: Branch 选择 "main"，文件夹选择 "/ (root)"
# 步骤 6: 点击 Save
# 步骤 7: 等待 1-2 分钟
# 步骤 8: 访问 https://<你的用户名>.github.io/arti-guide-showcase/
```

### Vercel

```bash
# 1. 注册 Vercel: https://vercel.com
# 2. 导入你的 GitHub 仓库
# 3. 保持默认设置，点击 Deploy
# 4. 完成后获得免费域名
```

### Netlify

```bash
# 1. 注册 Netlify: https://netlify.com
# 2. 拖拽项目文件夹到 Netlify 页面
# 3. 或连接 GitHub 仓库自动部署
# 4. 完成后获得免费域名
```

### 传统服务器

```bash
# 将 perform.html 和 ppt 文件夹上传到服务器即可
# 确保服务器支持静态文件托管

# Nginx 配置示例
server {
    listen 80;
    server_name your-domain.com;
    root /path/to/arti-guide-showcase;
    index perform.html;
}
```

---

## ❓ 常见问题

### 基础问题

**Q: 页面打开后是空白/黑色的？**

A: 可能的原因：
1. 网络问题 - 本项目依赖 CDN 加载第三方库，请确保网络畅通
2. 浏览器版本过低 - 请升级到推荐版本
3. 控制台报错 - 按 F12 打开开发者工具查看错误信息

**Q: 粒子动画不显示？**

A: 粒子动画依赖 tsparticles 库，需要从 CDN 加载。请检查：
- 网络是否可以访问 `cdn.jsdelivr.net`
- 是否有广告拦截插件阻止了加载

**Q: 卡片没有 3D 倾斜效果？**

A: VanillaTilt.js 需要从 CDN 加载。请检查：
- 网络是否可以访问 `cdnjs.cloudflare.com`
- 浏览器是否支持 CSS 3D Transform

### PPT 相关

**Q: PPT 图片无法显示？**

A: 请按以下步骤排查：
1. 确认 `ppt` 文件夹存在且包含图片
2. 确认 `perform.html` 中 `PPT_TOTAL` 已正确设置
3. 确认图片格式为 PNG 或 JPG
4. 确认图片命名与配置一致
5. 如果是本地打开，部分浏览器可能限制本地文件访问

**Q: PPT 图片太大导致加载慢？**

A: 建议：
- 使用图片压缩工具（如 TinyPNG）
- 将分辨率降低到 1920×1080
- 使用 JPG 格式代替 PNG
- 单张图片控制在 1MB 以内

### 自定义问题

**Q: 如何添加更多的 Tab 页面？**

A: 
1. 在 HTML 中添加新的 `.tab-panel`
2. 在 JavaScript 中添加对应的数据数组
3. 修改 `switchTab` 函数逻辑
4. 添加对应的 Tab 按钮

**Q: 如何修改字体？**

A: 
1. 在 `<head>` 中引入新字体
2. 修改 `:root` 中的 `--font-main` 变量

**Q: 如何禁用某些动画效果？**

A: 在 JavaScript 中找到对应的初始化代码并注释掉：
- 禁用粒子：注释 `tsParticles.load(...)` 
- 禁用倾斜：移除 `VanillaTilt.init(...)` 
- 禁用滚动动画：移除 `ScrollTrigger` 相关代码

---

## 📝 更新日志

### v1.0.0 (2026-05-01)

- 🎉 初始版本发布
- ✨ 粒子动画背景
- ✨ 3D 卡片倾斜效果
- ✨ Tab 标签页切换
- ✨ PPT 幻灯片展示
- ✨ 响应式布局设计
- ✨ 滚动触发动画

---

## 🤝 贡献指南

欢迎所有形式的贡献！

### 如何贡献

1. **Fork** 本仓库
2. 创建你的特性分支：`git checkout -b feature/AmazingFeature`
3. 提交你的修改：`git commit -m 'Add some AmazingFeature'`
4. 推送到分支：`git push origin feature/AmazingFeature`
5. 打开一个 **Pull Request**

### 贡献类型

- 🐛 Bug 修复
- ✨ 新功能
- 📝 文档改进
- 🎨 样式优化
- ⚡ 性能优化
- 🔧 代码重构

### 代码规范

- 保持代码简洁清晰
- 添加必要的注释
- 遵循现有代码风格
- 确保兼容性

---

## 📄 开源协议

本项目基于 [MIT License](./LICENSE) 开源。

```
MIT License

Copyright (c) 2026

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## 🙏 致谢

感谢以下开源项目：

| 项目 | 作者 | 协议 |
|------|------|------|
| [tsparticles](https://particles.js.org/) | Matteo Bruni | MIT |
| [GSAP](https://greensock.com/) | GreenSock | Standard |
| [VanillaTilt.js](https://micku7zu.github.io/vanilla-tilt.js/) | Șandor Sergiu | MIT |
| [Inter Font](https://rsms.me/inter/) | Rasmus Andersson | OFL |

---

## 📮 联系方式

如有问题或建议，欢迎通过以下方式联系：

- 📧 Email: [你的邮箱]
- 🐙 GitHub: [你的 GitHub 主页]
- 💬 Issues: [提交 Issue](https://github.com/zgy123454zgy-afk/arti-guide-showcase/issues)

---

<div align="center">

### 如果这个项目对你有帮助，请给一个 ⭐ Star 支持一下！

<br>

![Star History](https://api.star-history.com/svg?repos=zgy123454zgy-afk/arti-guide-showcase&type=Date)

<br>

**Made with ❤️ by [Your Name](https://github.com/你的用户名)**

</div>
