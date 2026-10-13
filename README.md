# Momikk Dalamud Plugins

Momikk 的 Dalamud 插件统一发布清单。这个仓库只维护统一安装入口；各插件的源码、图标和安装包由各自项目维护。

## 库链

在 Dalamud 设置的第三方插件仓库中添加：

```text
https://raw.githubusercontent.com/Momikk/DalamudPlugins/main/pluginmaster.json
```

新入口上线后，移除原先的 GlamourKing/pluginmaster.json 或 GlamourKing/repo.json 来源，避免重复配置。

## 当前插件

| 插件 | 版本 | API | 项目 |
| --- | --- | --- | --- |
| 幻化之王 GlamourKing | 0.1.0.2 | 15 | [GlamourKing](https://github.com/Momikk/GlamourKing) |
| 亚拉戈市场 AllaganMarket | 1.4.0.3 | 15 | [AllaganMarket](https://github.com/Momikk/AllaganMarket) |

AllaganMarket 安装包已发布，构建、包内容与公开下载地址已验证；游戏内加载及国服功能兼容性仍需实际验收。

## 维护

更新插件时，从其发布产物取得 manifest，在 pluginmaster.json 数组中更新对应的 InternalName 条目；维护 AssemblyVersion、DalamudApiLevel、IconUrl、DownloadLinkInstall、DownloadLinkUpdate 和 LastUpdate。保留原作者与插件项目链接。

提交前核对清单是合法 JSON 数组、InternalName 不重复、版本和 API 与实际 ZIP 内 manifest 一致，并确认图标与下载链接可访问。新增插件追加对应条目即可，统一库链保持不变。
