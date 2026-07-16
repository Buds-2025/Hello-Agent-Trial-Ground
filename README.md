# Hello Agent-Trial Ground

我把 datawhalechina/hello-agents 的 16 章内容做成了一款 Windows 桌面互动游戏。你可以跟着地图逐章学习，在剧情中完成选择、排序与代码诊断；通关后还能打开 CG、OST 与媒体中心，并配有开场 CG、片尾曲和 4K 级 CG 资源。

## 1. 硬件要求

- 操作系统：Windows 10 / Windows 11 64-bit
- 处理器：Intel Core i5 第 8 代 / 同等性能或以上
- 内存：8 GB RAM 及以上
- 硬盘：≥ 2 GB 可用空间（解压后目录约 1.7 GB）
- 显卡：支持硬件解码 H.264 视频；4K 输出建议独立显卡或集显 UHD 620 以上
- 显示器：1080P 起步；4K 全分辨率渲染需 4K 显示器
- 网络：首次启动无需联网，所有资源离线运行

## 2. 游玩方式

1. 前往 [Releases](../../releases) 页面，下载最新版本的 `Hello-Agent-Trial-Ground-v1.0.0-windows-x64.zip`
2. **完整解压**到任意目录（路径建议不含中文以避免部分 Windows 环境下的兼容性问题）
3. 进入解压后的文件夹，双击运行 `Hello Agent-Trial Ground.exe`
4. exe 默认以**无边框全屏**模式启动；可用 F11 切换窗口模式，Esc 仅返回上一级
5. 首次启动：
   - 选择 **NEW GAME · 新游戏** 开始；通关后可使用 **CONTINUE · 继续游戏** 从存档加载
   - 完成全部 16 章后，title 屏的 **CG · 媒体中心** 自动解锁

存档位置：`文档\Hello Agent-Trial Ground\save\save.json`，桌面版稳定运行后会自动创建。

发行包内附带全通关测试存档，方便快速预览全部内容。

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

4K 母版在制作端经 Seedance 2.0 生成并由 Topaz Video AI 超分处理；1080P 为独立渲染档位，源 4K 与 1080P 各自保留，运行时不重编码、不重打包。全部 CG 视频通过 `game/assets/movies/` 暴露。

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
