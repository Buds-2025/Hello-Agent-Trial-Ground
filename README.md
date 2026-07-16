# Hello Agent-Trial Ground

当前最新版本为v1.0.1，适用于Windows x64。

## 下载与运行

请前往[GitHub Releases](https://github.com/Buds-2025/Hello-Agent-Trial-Ground/releases/latest)下载`Hello-Agent-Trial-Ground-v1.0.1-windows-x64.zip`，完整解压后运行`Hello Agent-Trial Ground.exe`。

游戏默认无边框全屏启动。按F11或左Alt+Enter切换全屏。标题页5秒内连续按3次Esc可打开退出确认；设置面板底部也提供保存并退出按钮。

该版本未使用受信任的Windows Authenticode证书签名，Windows可能显示“未知发布者”或SmartScreen提示。

## 全流程通过存档

仓库中的[`全流程通过存档/save.json`](./全流程通过存档/save.json)已完成全部16章和127个场景，可解锁CG、写真与OST。

使用前先关闭游戏，将该文件复制到：

```text
文档\Hello Agent-Trial Ground\save\save.json
```

如果目标位置已有存档，请先备份。不要在游戏运行期间替换存档。

## v1.0.1修复内容

- 完成设置面板保存并退出按钮。
- 重做标题页三击Esc退出确认交互。
- 修复BGM播放断续和媒体资源分段读取。
- 修复CG全屏退出后错误跳回媒体中心。
- 加固桌面存档、运行时隔离和release完整性检查。

GitHub Release只提供游戏ZIP。README和全流程通过存档保留在本仓库，不放入游戏ZIP。
