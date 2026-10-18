# 封面排版 / Cover Layout

一个用于制作 **小红书 3:4 图文封面** 的本地网页工具。当前主要面向 macOS 和 iPhone / iPad 使用。

照片的读取、编辑和导出都在当前设备上完成。

## Features

- 固定 **3:4** 画布，导出尺寸为 **1800 × 2400 px**
- 提供 **1–6 格及 9 格**的多种预设布局
- 通过 **格数 + 构图缩略图**选择布局
- 每个框可独立使用图片或文字
- 图片支持移动、缩放、重置构图和中心吸附
- 可调整布局比例、外边距、框间距、圆角和背景色
- 支持批量导入图片和框内容重排
- 支持多条叠加文字，并可调整位置、字号、颜色、字体、字重和阴影
- 框内文字和叠加文字都可使用内置字体或本机字体
- 分别导出 **PNG** / **JPG**

## Usage

1. 选择格数和构图。
2. 批量导入图片，或在各个框中分别添加图片 / 文字。
3. 在预览中调整图片、框内文字和排列顺序。
4. 按需添加叠加文字。
5. 使用“保存 PNG”或“保存 JPG”导出成品。

Mac 上可从 Finder 直接拖入图片；支持时会使用系统保存对话框。iPhone / iPad 上可通过触控手势调整图片，并优先使用系统分享菜单导出。

## Privacy

选择的照片只会在当前设备上读取和处理。

本项目没有照片上传功能、服务器端图片处理、账号系统或云端照片存储。

## Fonts & Licenses

内置字体包括：

- Cormorant
- Corben
- Oleo Script
- Sacramento
- WindSong
- 寒蝉活仿楷
- 寒蝉活仿楷・窄体
- LXGW Bright
- 萌神拼音体
- 芝士奶盖乌龙宋
- 匯文明朝體 v1.00

界面中文使用 **匯文明朝體 v1.00**，英文使用 **Cormorant**。

字体文件位于 `fonts/`，对应许可或授权说明位于 `licenses/`。其中大部分字体按各自的 **SIL Open Font License 1.1** 分发；匯文明朝體 v1.00 使用作者发布的单独授权声明，详见 `licenses/Huiwen-Mincho-License.txt`。

## Limitations

- 当前不保存可继续编辑的工程；刷新或关闭页面会清空当前编辑状态。
- “自定义设备字体”的可用性取决于浏览器和系统。
- 当前版本主要在 macOS 和 iOS 上使用与调试。

## Development

本项目采用 **vibe coding** 方式开发，代码由 **ChatGPT** 根据维护者的需求生成并迭代。

## Structure

```text
photo-collage/
├── index.html
├── fonts/
├── licenses/
├── wrangler.jsonc
├── .assetsignore
└── README.md
```
