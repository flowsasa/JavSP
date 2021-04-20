![JavSP](https://github.com/Yuukiy/JavSP/blob/master/image/javsp_logo.png?raw=true)

# Jav Scraper Package

**汇总多站点数据的AV元数据刮削器**

提取影片文件名中的番号信息，自动抓取并汇总多个站点数据的 AV 元数据，按照指定的规则分类整理影片文件，并创建供 Emby、Jellyfin、Kodi 等软件使用的元数据文件

![License](https://img.shields.io/github/license/Yuukiy/JavSP)
![Python 3.8](https://img.shields.io/badge/python-3.8-green.svg)
![Latest release](https://img.shields.io/github/v/release/Yuukiy/JavSP)

## 功能特点

下面这些是一开始就决定要做的主要功能，在逐渐实现和完善，如果想到新的功能点也会加进来。

- [x] 自动识别影片番号
- [x] 支持处理影片分片
- [x] 汇总多个站点的数据生成NFO数据文件
- [x] 多线程并行抓取
- [x] 下载高清封面
- [x] 自动检查新版本
- [x] 翻译标题和剧情简介
- [ ] 匹配本地字幕
- [ ] 使用小缩略图创建文件夹封面
- [ ] 保持不同站点间 genre 分类的统一
- [ ] 不同的运行模式（抓取数据+整理，仅抓取数据）
- [ ] 可选：所有站点均抓取失败时由人工介入

目前软件还处于比较初期的阶段，部分功能还没有完成。如果你愿意试一下，可以参照下面的说明。如果使用的时候遇到什么问题也欢迎给我反馈😊

## 安装

- 想要快速上手？

	前往[软件发布页](https://github.com/Yuukiy/JavSP/releases/latest)下载最新版本的软件，无需安装额外工具，开箱即用

- 更喜欢源代码？

	请确保已安装 Python （此项目以 Python 3.8 开发）
	```
	git clone https://github.com/Yuukiy/JavSP.git
	cd JavSP
	pip install -r requirements.txt
	```

## 使用

软件开箱即用，首次运行时会在软件目录下生成默认的配置文件 ```config.ini```。如果想让软件更符合你的使用需求，也许你需要更改配置文件:

> 以任意文本编辑器打开 ```config.ini```，根据各个配置项的说明选择你需要的配置即可。

此外软件也支持从命令行指定运行参数（命令行参数的优先级高于配置文件）。运行 ```JavSP -h``` 查看支持的命令列表

更详细的使用说明请前往 [JavSP Wiki](https://github.com/Yuukiy/JavSP/wiki) 查看


## 问题反馈

如果使用中遇到了 Bug，请[前往 Issue 区反馈](https://github.com/Yuukiy/JavSP/issues)（提问前请先搜索是否已有类似问题）


## 参与贡献

此项目不需要捐赠。如果你想要帮助改进这个项目，欢迎通过以下方式参与进来（并不仅局限于代码）：

- 帮助撰写和改进Wiki

- 帮助完善单元测试数据

- 帮助翻译 genre

- Bugfix / 新功能？欢迎发 Pull Request

- 要不考虑点个 Star ?


## 许可

此项目以 GPL-3.0 License 发布。此外，如果你使用此项目，表明你还额外接受以下条款：

- 本软件仅供学习 Python 和技术交流使用

- 请勿在微博、微信等面向大众的公共社交平台上宣传此项目

- 用户在使用本软件时，请遵守当地法律法规

- 禁止将本软件用于商业用途
