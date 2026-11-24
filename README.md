# Pebrel Winc 插件社区 / Plugin Community

在 **Pebrel Winc → 设置 → 插件 → 插件社区** 浏览插件。选择「审阅并安装」后，Pebrel Winc 会显示插件请求的权限，由你确认安装。

Browse in **Pebrel Winc → Settings → Plugins → Plugin Community**. Choose **Review and install** to see the permissions before approving installation.

| 插件 / Plugin | 功能 / Features |
| --- | --- |
| [Winc](plugins/local.winc-directory) | 在 Winc 或资源管理器打开当前目录。提供本机 `winc.exe` 路径，支持 Windows 和 WSL 窗格。 / Open the focused Windows or WSL directory in Winc or File Explorer. Select your local `winc.exe` during setup. |
| [临时终端 / Scratch Terminal](plugins/local.scratch-terminal) | 给当前标签加可隐藏、停靠或浮动的临时命令行。 / Add a hideable, docked or floating shell to the current terminal tab. |

## Contributing / 提交插件

Open a pull request with a manifest and usage instructions under `plugins/<id>/`. The catalog currently accepts standalone manifests. Explain what the plugin does, which platforms it supports and which permissions users will review. After the package commit lands, a separate catalog change can point `catalog.json` at its full commit SHA. Keep the plugin ID, English name and version consistent with the manifest. Increase the plugin version when changing its package.

提交 PR 时，在 `plugins/<id>/` 中放入插件清单和使用说明。社区目录目前收录只需要清单的插件。请说明功能、支持平台和用户需要审阅的权限。插件源码合入后，再把 `catalog.json` 指向该提交的完整 SHA。插件 ID、英文名称和版本须与清单一致，修改插件内容时请更新版本。

Host / 宿主项目 · [Pebrel Winc](https://github.com/suzikuo/pebrel-winc)

License / 许可 · [GPL-3.0](LICENSE)
