# HiveCtrl Releases

本仓库用于 **公开发布 HiveCtrl 桌面端安装包**。源代码为私有仓库，此处仅提供构建产物与版本说明。

## 下载

- **最新版本**：[Releases · Latest](https://github.com/hivectrl/hivectrl-releases/releases/latest)
- 所有历史版本见 [Releases 列表](https://github.com/hivectrl/hivectrl-releases/releases)。

安装包通过 **GitHub Release 附件** 分发，**不会**以超大文件形式提交到本仓库的 Git 历史中。

## 文件说明（发版时建议在 Release 中附带）

| 平台 | 常见产物 |
|------|----------|
| macOS | `.dmg`（Apple Silicon / Intel 请在 Release 标题或说明中标注） |
| Linux | `.deb` / `.AppImage` 等 |

建议在每次 Release 的说明中写明：**版本号、最低系统版本、架构、已知问题**；可选附带 **`SHA256SUMS`** 或单文件校验值，便于用户校验。

## 校验示例

```bash
shasum -a 256 HiveCtrl_xxx.dmg
# 与 Release 说明中的 SHA256 比对
```

## 许可证

见仓库根目录 [LICENSE](./LICENSE)（MIT）。
