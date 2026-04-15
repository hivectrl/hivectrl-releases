# HiveCtrl Releases

**HiveCtrl** 是面向多台 Android 真机的桌面管控与镜像客户端，适合开发调试、测试与需要同时操作多台设备的场景。本仓库用于发布安装包；
**程序本体与更新说明见 [GitHub Releases](https://github.com/hivectrl/hivectrl-releases/releases/latest)**。

## HiveCtrl 能做什么

- **设备发现与连接**：支持通过 **USB** 与 **局域网（Wi‑Fi）** 发现设备，并建立连接，便于在桌面端统一管理多台手机或平板。
- **屏幕镜像与操控**：基于 **scrcpy**，在电脑上实时查看设备画面，并进行触控、按键等操作；可同时镜像多台设备，方便对照与并行操作。
- **批量与规模化操作**：面向多设备场景提供批量类能力（具体以各版本 Release 说明与应用内功能为准），减少逐台重复操作。
- **桌面端体验**：在 macOS / Linux 上以原生应用形式运行，与常见开发、测试环境结合使用。


## 下载

- **最新版本**：[Releases · Latest](https://github.com/hivectrl/hivectrl-releases/releases/latest)
- **历史版本**：[Releases 列表](https://github.com/hivectrl/hivectrl-releases/releases)

## v0.1.0 安装包

本版本提供 **Apple Silicon macOS** 与 **Debian 系 Linux（x86_64）** 安装包。
文件名以 Release 页面附件为准；下表为 **v0.1.0** 当前命名：

| 平台                               | 文件                         |
| ---------------------------------- | ---------------------------- |
| macOS（Apple Silicon，aarch64）    | `HiveCtrl_0.1.0_aarch64.dmg` |
| Linux（x86_64 / amd64，Debian 系） | `HiveCtrl_0.1.0_amd64.deb`   |

其他版本的文件名与校验和请以对应 Release 说明为准。

## 安装

- **macOS**  
  打开 `HiveCtrl_0.1.0_aarch64.dmg`，将 **HiveCtrl** 拖入 **应用程序**。  
  若出现「未验证开发者」等提示，可在 **系统设置 → 隐私与安全性** 中按需放行。

- **Linux**（示例，请按发行版调整）

```bash
sudo apt install ./HiveCtrl_0.1.0_amd64.deb
```

或：

```bash
sudo dpkg -i HiveCtrl_0.1.0_amd64.deb
```

## 校验（推荐）

下载后请将本地文件的 SHA‑256 与下表比对。**以下校验和仅对 v0.1.0 且与本仓库 Release 附件中完全一致的文件有效**（重新构建安装包会改变哈希）。

| 文件                         | SHA‑256                                                            |
| ---------------------------- | ------------------------------------------------------------------ |
| `HiveCtrl_0.1.0_aarch64.dmg` | `dd89d4e323823fefc981cb67e18fcf5c00dd5a1763e409d1e0f1c6a7537c4473` |
| `HiveCtrl_0.1.0_amd64.deb`   | `93e933d3a20a093f181a21a2919af7dae22258a9045c2e969613efbd1283f15c` |

**macOS：**

```bash
shasum -a 256 ./HiveCtrl_0.1.0_aarch64.dmg
```

**Linux：**

```bash
sha256sum ./HiveCtrl_0.1.0_amd64.deb
```

命令输出应与上表一致。

## 许可证

安装包及 HiveCtrl 应用程序按 **MIT License** 分发，见[LICENSE](https://github.com/hivectrl/hivectrl-releases/blob/master/LICENSE)。
