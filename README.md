<div align="center">

# 文物智鉴 · ArtiGuide

**中华文物多模态检索与数字人讲解系统展示页**

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![License](https://img.shields.io/badge/License-MIT-blue.svg)

**中文** | [English](./README_EN.md)

</div>

---

## 项目简介

`ArtiGuide` 是一个用于毕业设计答辩、项目路演和产品演示的深色科技风静态展示页。页面围绕“文物智鉴”系统展开，展示多模态文物数据集、CLIP + FAISS 检索管线、Live2D 数字人讲解、语音合成与数据可视化等核心模块。

项目无需构建工具，直接打开 [perform.html](./perform.html) 或通过本地静态服务器访问即可运行。

## 效果预览

![首页预览](./screenshots/hero.png)
![卡片效果](./screenshots/cards.png)

## 核心亮点

- **沉浸式首页**：粒子背景、鼠标光晕、标题入场动画和关键数据计数。
- **双标签内容区**：数据集来源与技术特色分栏展示，支持分类筛选。
- **交互卡片**：3D 倾斜、聚光跟随、涟漪反馈和滚动触发动画。
- **PPT 全屏播放器**：将答辩 PPT 导出为图片后即可在页面内播放。
- **静态部署友好**：单 HTML 架构，适合 GitHub Pages、Netlify、Vercel 等平台。

## 技术栈

| 技术 | 用途 |
| --- | --- |
| HTML / CSS / JavaScript | 页面结构、样式与交互逻辑 |
| tsparticles | 粒子背景 |
| GSAP + ScrollTrigger | 入场动画与滚动动画 |
| VanillaTilt | 卡片 3D 倾斜 |
| GitHub Pages | 静态页面部署 |

## 快速开始

```bash
git clone https://github.com/zgy123454zgy-afk/arti-guide-showcase.git
cd arti-guide-showcase
python -m http.server 8080
```

然后访问：

```text
http://localhost:8080/perform.html
```

也可以直接用浏览器打开 `perform.html`。如果希望 CDN 动画依赖稳定加载，推荐使用本地服务器方式访问。

## 配置 PPT

1. 将答辩 PPT 导出为 PNG 或 JPG 图片。
2. 将图片放入 `./ppt/` 目录。
3. 在 `perform.html` 中修改配置：

```javascript
const PPT_TOTAL = 10;
const PPT_PATH = './ppt/';
const PPT_IMAGES = [];
```

默认会按 `1.png`、`2.png`、`3.png` 的顺序读取。若使用自定义文件名，可填写：

```javascript
const PPT_IMAGES = ['cover.png', 'method.png', 'demo.png'];
```

更多说明见 [ppt/README.md](./ppt/README.md)。

## 自定义内容

- 页面文案与卡片：修改 `perform.html` 中的 `dataSources` 和 `features` 数组。
- 主题配色：修改 `:root` 下的 CSS 变量，例如 `--accent-glow` 与 `--accent-purple`。
- 预览截图：替换 `screenshots/hero.png`、`screenshots/cards.png`；也可以按需补充 `screenshots/ppt.png`。
- PPT 图片：按上方说明放入 `ppt/` 并更新配置。

## 目录结构

```text
.
├── perform.html          # 主展示页面
├── README.md             # 中文说明
├── README_EN.md          # 英文说明
├── ppt/                  # PPT 图片目录
│   └── README.md
├── screenshots/          # README 预览图目录
│   ├── hero.png
│   ├── cards.png
│   ├── ppt.png             # 可选：PPT 弹窗截图
│   └── README.md
└── LICENSE
```

## 部署

GitHub Pages 推荐设置：

1. 打开仓库 `Settings`。
2. 进入 `Pages`。
3. Source 选择 `Deploy from a branch`。
4. Branch 选择 `main`，目录选择 `/(root)`。
5. 保存后访问生成的 Pages 地址，并打开 `/perform.html`。

## 说明

当前仓库主要是展示页框架，不包含完整后端、模型权重或真实数据库。页面中的技术说明用于展示毕业设计系统的能力边界与实现思路。

## 开源协议

[MIT License](./LICENSE)
