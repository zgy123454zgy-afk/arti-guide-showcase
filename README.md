# 文物智鉴 · ArtiGuide - 展示页面框架

一个精美的深色主题展示页面框架，适用于项目答辩、产品展示、技术演示等场景。具有粒子背景、卡片动画、Tab切换、PPT幻灯片展示等功能。

## 预览特点

- 深色科技风格设计
- 粒子动画背景 (tsparticles)
- 鼠标跟踪光晕效果
- 卡片 3D 倾斜动画 (vanilla-tilt)
- 平滑滚动与视差效果 (GSAP + ScrollTrigger)
- Tab 标签页切换动画
- PPT 幻灯片全屏展示
- 响应式布局，支持移动端

## 快速开始

1. 克隆或下载本仓库
2. 直接用浏览器打开 `perform.html` 即可预览
3. 根据需要修改内容和样式

## 自定义 PPT 展示

本项目支持嵌入 PPT 幻灯片展示功能，用户可按需放入自己的 PPT 图片：

1. 将 PPT 导出为图片（PNG/JPG 格式）
2. 将图片放入 `./ppt/` 文件夹
3. 修改 `perform.html` 中的配置：

```javascript
// ========== PPT 配置区域 ==========
const PPT_TOTAL = 0;  // ← 修改为你的PPT图片总数
const PPT_PATH = './ppt/';  // ← PPT图片存放路径
const PPT_IMAGES = [];  // ← 可选：自定义图片文件名数组
// ========== 配置区域结束 ==========
```

详细说明请查看 `ppt/README.md`

## 页面结构

```
├── perform.html          # 主页面（包含 HTML + CSS + JS）
├── ppt/                  # PPT 图片存放目录
│   └── README.md         # PPT 配置说明
├── .gitignore
├── LICENSE               # MIT 开源协议
└── README.md             # 本文件
```

## 技术栈

- HTML5 + CSS3 + JavaScript
- [tsparticles](https://particles.js.org/) - 粒子动画
- [VanillaTilt](https://micku7zu.github.io/vanilla-tilt.js/) - 卡片倾斜效果
- [GSAP](https://greensock.com/gsap/) - 动画引擎
- [ScrollTrigger](https://greensock.com/scrolltrigger/) - 滚动触发动画

## 自定义指南

### 修改颜色主题

在 `perform.html` 的 `:root` CSS 变量中修改：

```css
:root {
    --bg-dark: #030307;           /* 背景色 */
    --accent-glow: #d4a843;       /* 主强调色（金色） */
    --accent-purple: #2e8b57;     /* 次强调色（绿色） */
    --accent-jade: #3aaf7c;       /* 辅助色 */
}
```

### 修改内容

- **标题和描述**：修改 Hero 区域的 HTML
- **数据卡片**：修改 JavaScript 中的 `dataSources` 和 `features` 数组
- **统计数据**：修改 `.hero-stat` 元素的 `data-target` 属性

## 浏览器兼容性

- Chrome 80+
- Firefox 75+
- Safari 13+
- Edge 80+

## 开源协议

MIT License - 详见 [LICENSE](LICENSE) 文件
