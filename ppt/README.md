# PPT 图片配置说明

这个目录用于存放答辩 PPT 导出的图片。页面会读取这里的图片，并在 `perform.html` 的全屏 PPT 弹窗中播放。

## 推荐流程

1. 在 PowerPoint、WPS 或 Keynote 中将演示文稿导出为图片。
2. 推荐格式：`PNG`，比例：`16:9`，尺寸：`1920x1080`。
3. 将导出的图片放入当前目录。
4. 在 `perform.html` 中修改 PPT 配置。

## 默认命名方式

如果图片命名为：

```text
1.png
2.png
3.png
...
```

只需要设置图片总数：

```javascript
const PPT_TOTAL = 10;
const PPT_PATH = './ppt/';
const PPT_IMAGES = [];
```

## 自定义命名方式

如果你希望使用自定义文件名，例如：

```text
cover.png
dataset.png
retrieval.png
demo.png
```

可以这样配置：

```javascript
const PPT_TOTAL = 4;
const PPT_PATH = './ppt/';
const PPT_IMAGES = ['cover.png', 'dataset.png', 'retrieval.png', 'demo.png'];
```

## 注意事项

- `PPT_TOTAL` 必须和实际展示的图片数量一致。
- 图片过大可能影响加载速度，建议单张控制在 2MB 以内。
- 如果暂时不放 PPT 图片，保持 `PPT_TOTAL = 0`，页面会展示未配置提示，不会报错。
