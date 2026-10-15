# 香气练习册

![香气练习册截图](screenshot.png)

把 SCA 咖啡价值评估（CVA）描述性表单的嗅觉参照物库整理成中文，方便日常做香气训练。可以作为 macOS 程序使用，也可以在任何电脑的浏览器里直接打开（包括 Windows）。

## 功能
- 收录 SCA 官网英文和简体中文页面的全部样品：10 个大类、21 个描述词，共 171 个参照物（其中 17 个只出现在简体中文页面）
- 每个参照物都有中文的准备方法和推荐品牌，可以切换显示英文原文
- 左侧大类可以折叠，点一下展开；支持中英文搜索
- 不联网也能用

大类顺序：青绿、花香、果香、酸/发酵、香料、甜、坚果、可可、烘焙、其他

## 安装（Mac）
1. 打开 [Releases 页面](https://github.com/jimmybrst/aroma-workbook/releases/latest)，下载 `aroma-workbook-macos.zip`（[直接下载](https://github.com/jimmybrst/aroma-workbook/releases/latest/download/aroma-workbook-macos.zip)）
2. 双击解压，得到 `香气练习册.app`
3. 把 `香气练习册.app` 拖到「应用程序」文件夹

### 第一次打开
程序没有经过 Apple 签名，所以第一次打开时 macOS 会拦截。代码全部公开在本仓库，可以自行查看。按你的系统版本操作：

**macOS 14 及更早**
1. 在「应用程序」里右键点 `香气练习册.app`（或按住 Control 键点按）
2. 选「打开」
3. 在弹出的提示里再点「打开」

**macOS 15 Sequoia 及以后**
1. 先双击 `香气练习册.app`，会提示无法打开，点「完成」关掉提示
2. 打开「系统设置 → 隐私与安全性」
3. 滚到下方，找到关于「香气练习册」的提示，点「仍要打开」
4. 输入电脑密码确认

**备用方法（终端）**

如果上面的方法都不行，打开「终端」，粘贴下面这行并按回车：
```
xattr -cr /Applications/香气练习册.app
```
然后双击 `香气练习册.app` 即可。

只有第一次需要这样做，以后直接双击就能打开。

## Windows 电脑（或不想装程序的 Mac）
1. 点这个链接下载：[aroma-workbook-web.html](https://github.com/jimmybrst/aroma-workbook/releases/latest/download/aroma-workbook-web.html)
2. 如果 Edge 或 Chrome 提示「保留 / 放弃」，选「保留」
3. 在「下载」文件夹里双击这个文件（图标是浏览器图标），会用 Edge、Chrome 或 Firefox 打开
4. 不需要安装，也不用联网；设置（比如是否显示英文）保存在浏览器里

**另一种方法：下载整个项目**

点 [下载整个项目 ZIP](https://github.com/jimmybrst/aroma-workbook/archive/refs/heads/main.zip)，右键「全部解压缩」，打开解压出的 `aroma-workbook-main` 文件夹，双击里面的 `index.html`。Windows 默认隐藏扩展名，这个文件可能只显示为 `index`，图标是浏览器图标的那个就是。

## 系统要求
- macOS 10.13 及以上（10.15 及以上显示效果最好），Intel 和 Apple 芯片都支持
- Windows：Edge、Chrome 或 Firefox

## 参照物怎么选
- 同一个描述词下面会列出多个参照物，选一个就能练，不用全部准备
- 不带品牌名的参照物用超市食材就能自己做，比如欧芹水、白葡萄汁
- 带编号的是商用闻香瓶套装，例如 Le Nez du Café、Scentone、The Coffee Sensorium、FlavorActiV，有哪套就用哪套

## 关于翻译
原料中文名都逐一核对过，官方简体版的错误已经改正，比如柠檬和青柠（莱姆）糖浆写反、黑莓被写成覆盆莓、Revelation 第 22 号和第 23 号写反。拿不准的译名在旁边保留了英文原文。

Le Nez du Café 2.0 的「焦油」（Tar）官网标为 29 号，与百里香重复；按套装顺序应为 39 号。程序里保留官网编号，并加了说明。

## 数据来源与许可
- 样品数据来自 [SCA 官网 Olfactory Examples](https://sca.coffee/value-assessment/olfactory-examples)（页面内嵌的英文和简体中文 Airtable 列表），版权归 Specialty Coffee Association 所有。本项目是个人整理和翻译，仅供学习交流。
- 数据抓取日期：2026-10-14
- 代码采用 [MIT 许可证](LICENSE)；许可证只适用于代码，不包括样品数据。

## 文件
- `index.html`：程序界面，数据已经内置
- `data_en.json` / `data_zh.json`：英文原始数据和中文数据
- `screenshot.png` / `screenshot_windows.png` / `icon_preview.png`：界面截图、Windows 字体效果截图和图标预览
- `aroma-workbook-macos.zip`：macOS 程序（解压得到 `香气练习册.app`）；`aroma-workbook-web.html`：浏览器版（和 `index.html` 相同）。这两个文件不在仓库里，请到 [Releases 页面](https://github.com/jimmybrst/aroma-workbook/releases/latest) 下载
- `LICENSE`：代码的 MIT 许可证
