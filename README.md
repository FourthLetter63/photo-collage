# 3:4 Photo Collage

一个用于制作 **3:4 竖版拼图** 的轻量网页工具，适合在 Mac、iPhone 和 iPad 上使用。支持图片与文字混排，所有照片处理和导出都在浏览器本地完成。

## 功能

- 固定 3:4 画布，导出尺寸为 **1800 × 2400 px**
- 2–9 个框的预设布局，包括：
  - 2：上下 / 左右
  - 3：上 1 + 下 2 / 左 1 + 右 2 / 三行
  - 4：2 × 2 / 上 1 + 下 3
  - 5：上 1 + 下 2 × 2 / 上 2 + 下 3
  - 6：2 × 3
  - 9：3 × 3
- 每个框可独立设置为 **图片** 或 **文字**
- 图片可独立移动、缩放和重置构图
- 规则网格可单独调整每行高度和每列宽度
- 可调整外边距、框间距、圆角和背景色
- 文字支持字号、颜色、字重、字体选择和位置调整
- 支持批量选择图片
- 支持导出 PNG / JPG，并使用日期和时间作为文件名

## 字体

项目内置：

- **Cormorant**：英文默认字体
- **ChillHuoFangKai_F（寒蝉活仿楷）**：中文默认字体

字体文件位于 `fonts/`，对应许可证位于 `licenses/`。

当前使用的字体文件：

```text
fonts/Cormorant[wght].ttf
fonts/ChillHuoFangKai_F_Regular.otf
```

Cormorant 和寒蝉活仿楷均按各自的 **SIL Open Font License 1.1** 许可证随项目分发。请保留 `licenses/` 中的许可证文本。

## 隐私

选择的照片不会上传到服务器。

网页只读取用户在浏览器中主动选择或拖入的本地图片，并使用浏览器的 Canvas 在设备本地完成裁切、排版和导出。当前页面没有照片上传接口，也没有远程图片处理服务。

## 使用

### Mac

1. 打开网页。
2. 点击“选择图片”，或直接从 Finder 把图片拖到目标框。
3. 用鼠标在预览中移动照片；使用缩放滑块调整大小。
4. 根据需要调整布局、行列比例、间距、圆角、颜色或文字。
5. 点击“保存 PNG”或“保存 JPG”。

### iPhone / iPad

1. 使用 Safari 打开网页。
2. 选择单张图片，或使用“批量选择图片”。
3. 平时单指滑动用于滚动页面。
4. 需要重新构图时，在对应框点“调整构图”；进入调整模式后：
   - 单指移动图片
   - 双指缩放图片
   - 完成后点预览下方的“完成调整”
5. 文字位置同样通过“调整位置”进入调整模式。
6. 导出时使用系统分享菜单保存到“照片”或“文件”。

大尺寸手机或相机照片在首次载入时会先缩放到适合画布处理的尺寸，因此可能短暂停顿；之后的编辑会更流畅。

## GitHub Pages

这个项目是纯静态网页，可以直接通过 GitHub Pages 部署。

仓库根目录至少需要：

```text
index.html
fonts/
licenses/
```

GitHub Pages 可设置为：

```text
Settings → Pages → Deploy from a branch → main → / (root)
```

发布后，通过生成的 GitHub Pages 地址访问即可。

## 项目结构

```text
photo-collage/
├── index.html
├── fonts/
│   ├── Cormorant[wght].ttf
│   └── ChillHuoFangKai_F_Regular.otf
├── licenses/
│   ├── Cormorant-OFL.txt
│   └── ChillMovableType-OFL.txt
└── README.md
```

## Notes

- 其他字体选项依赖当前设备是否安装对应字体。
- 寒蝉活仿楷当前内置的是 Regular；Medium / Semibold / Bold 可能由浏览器合成。
- 当前版本没有服务器端组件、账号系统或云端存储。
