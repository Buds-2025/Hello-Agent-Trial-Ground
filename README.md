# Hello Agent-Trial Ground

我把 datawhalechina/hello-agents 的 16 章内容做成了一款 Windows 桌面互动游戏。你可以跟着地图逐章学习，在剧情中完成选择、排序与代码诊断；通关后还能打开 CG、OST 与媒体中心，并配有开场 CG、片尾曲和 4K 级 CG 资源。

## 1. 硬件要求

能满足日常办公的主流配置即可畅玩本游戏。

## 2. 游玩方式

1. 前往 Releases 页面，下载最新版本的游戏包。
2. 完整解压到任意目录（路径建议不含中文以避免部分 Windows 环境下的兼容性问题）
进入解压后的文件夹，双击运行 Hello Agent-Trial Ground.exe
exe 默认以无边框全屏模式启动；可用 F11 切换窗口模式，Esc 仅返回上一级
3. 发行包内附带全通关测试存档，方便快速预览全部内容。存档位置：文档\Hello Agent-Trial Ground\save\save.json，桌面版稳定运行后会自动创建。

## 3. 技术路径

| 项目 | 采用方案 |
| --- | --- |
| 游戏各章节 BGM | MiniMax M3 |
| 游戏 title 页 BGM、片尾曲 | Suno |
| 游戏外观（主要 UI） | MiniMax M3 |
| 人设图（4K） | GPT Image 2 生图模型 API 调用 |
| CG 写真（4K） | GPT Image 2 生图模型 API 调用 |
| CG 视频（开场 + 媒体中心 ending） | Seedance 2.0 + Topaz Video AI 超分 |
| 游戏关卡 / 正文内容 / 工程实现 | MiniMax M3 in Claude Code + Codex |

详细说明见桌面包内 `TECH_CREDITS.md`。

## 4. 即将到来的更新

开场 CG 优化
更多写真图片
立绘动态效果
剧情内容打磨优化
各章节 BGM 可能优化
几个 DLC（长期项目，不会很快）

## 5. 致谢

本项目灵感来自 [datawhalechina/hello-agents](https://github.com/datawhalechina/hello-agents)，游戏内相关文案取材于该项目教材。
