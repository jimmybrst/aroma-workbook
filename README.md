# 香气练习册

![香气练习册截图](screenshot.png)

一个 macOS 桌面程序，把 SCA 咖啡价值评估（CVA）描述表的官方嗅觉范例库整理成中文，方便日常做香气训练。

## 功能
- 收录官方全部 10 个大类、21 个描述词，共 171 个参照物
- 每个参照物都有中文的准备方法和推荐品牌，可以切换显示英文原文
- 左侧大类可以折叠，点一下展开；支持中英文搜索
- 不联网也能用

大类顺序：青绿、花香、果香、酸/发酵、香料、甜、坚果、可可、烘焙、其他

## 安装
1. 打开 [Releases 页面](https://github.com/jimmybrst/aroma-workbook/releases/latest)，下载最新版本里的 `aroma-workbook-macos.zip`（[直接下载](https://github.com/jimmybrst/aroma-workbook/releases/latest/download/aroma-workbook-macos.zip)），双击解压，会得到 `香气练习册.app`
2. 把 `香气练习册.app` 拖到「应用程序」或桌面
3. 程序没有签名，第一次打开要右键点它，选「打开」，再点「打开」
4. 如果还是打不开，在终端运行一次：
   ```
   xattr -dr com.apple.quarantine /Applications/香气练习册.app
   ```

### 不想装程序？用浏览器打开
1. 打开仓库里的 [index.html](https://github.com/jimmybrst/aroma-workbook/blob/main/index.html)，点右上角的下载按钮（Download raw file）把它存到电脑上；或者点仓库首页绿色的「Code」按钮，选「Download ZIP」（[直接下载](https://github.com/jimmybrst/aroma-workbook/archive/refs/heads/main.zip)），解压后找到里面的 index.html
2. 双击 `index.html`，会用默认浏览器（Safari、Chrome 等）打开
3. 数据都在这一个文件里，不用联网，Windows 电脑也能用

## 参照物怎么选
- 同一个描述词下面会列出多个参照物，选一个就能练，不用全部准备
- 不带品牌名的参照物用超市食材就能自己做，比如欧芹水、白葡萄汁
- 带编号的是商用闻香瓶套装，例如 Le Nez du Café、Scentone、The Coffee Sensorium、FlavorActiV，有哪套就用哪套

## 关于翻译
原料中文名都逐一核对过，官方简体版的错误已经改正，比如柠檬和莱姆糖浆写反、黑莓被写成覆盆莓、Revelation 第 22 号和第 23 号写反。拿不准的译名在旁边保留了英文原文。

## 数据来源
[SCA Olfactory Examples](https://sca.coffee/value-assessment/olfactory-examples)。内容归 Specialty Coffee Association 所有，本项目只是整理和翻译，方便大家学习交流。

## 文件
- `index.html`：程序界面，数据已经内置
- `data_en.json` / `data_zh.json`：英文原始数据和中文数据
- `screenshot.png` / `icon_preview.png`：截图和图标预览
- `aroma-workbook-macos.zip`：macOS 程序（解压得到 `香气练习册.app`），不在仓库里，请到 [Releases 页面](https://github.com/jimmybrst/aroma-workbook/releases/latest) 下载
