# PPT 图片配置说明

## 使用方法

1. 将你的 PPT / 演示文稿导出为图片格式（PNG 或 JPG）
2. 将所有图片放入此文件夹 (`./ppt/`)
3. 图片按顺序命名为：
   - `1.png`, `2.png`, `3.png` ...
   - 或者使用自定义名称

4. 打开 `perform.html`，找到以下配置区域并修改：

```javascript
// ========== PPT 配置区域 ==========
const PPT_TOTAL = 0;  // ← 修改为你的PPT图片总数
const PPT_PATH = './ppt/';  // ← PPT图片存放路径
const PPT_IMAGES = [];  // ← 可选：自定义图片文件名数组
// ========== 配置区域结束 ==========
```

## 示例

如果你有 10 张 PPT 图片，命名为 `slide1.png` 到 `slide10.png`：

```javascript
const PPT_TOTAL = 10;
const PPT_PATH = './ppt/';
const PPT_IMAGES = ['slide1.png', 'slide2.png', 'slide3.png', 'slide4.png', 'slide5.png',
                    'slide6.png', 'slide7.png', 'slide8.png', 'slide9.png', 'slide10.png'];
```

或者使用默认命名 `1.png` ~ `10.png`：

```javascript
const PPT_TOTAL = 10;
const PPT_PATH = './ppt/';
const PPT_IMAGES = [];  // 留空则自动使用 1.png ~ 10.png
```

## 图片建议

- 推荐使用 PNG 格式以保持最佳画质
- 推荐 16:9 比例（如 1920x1080）
- 文件大小建议控制在 2MB 以内以保证加载速度
