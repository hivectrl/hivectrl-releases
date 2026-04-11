# HiveCtrl Releases

HiveCtrl 桌面客户端的安装包在 **GitHub Releases** 中发布，请在下述页面选择对应平台与架构的文件下载。

## 下载

- **最新版本**：[Releases · Latest](https://github.com/hivectrl/hivectrl-releases/releases/latest)
- **历史版本**：[Releases 列表](https://github.com/hivectrl/hivectrl-releases/releases)

## 如何选择安装包

| 系统 | 常见安装包类型 |
|------|----------------|
| macOS | `.dmg`（请按页面上的文件名或说明选择适合你 Mac 的版本，例如 Apple Silicon 与 Intel 可能分别提供） |
| Linux | `.deb`、`.AppImage` 等（以 Release 页面实际提供的文件名为准） |

## 校验（可选）

若 Release 说明中提供了 SHA256，可在下载后与本地文件比对。

**macOS：**

```bash
shasum -a 256 ./你下载的文件名.dmg
```

**Linux：**

```bash
sha256sum ./你下载的文件名.deb
```

请将命令中的文件名换成你在 Releases 里实际下载的文件名。

## 许可证

见仓库根目录 [LICENSE](./LICENSE)（MIT）。
