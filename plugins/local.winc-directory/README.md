# Winc

For Pebrel Winc on Windows. In **Settings → Plugins → Plugin Community**, select **Winc**, choose the `winc.exe` already installed on your computer, then review and approve the two directory actions. The **Winc** button opens the focused Windows or WSL pane’s directory in Winc. The **文件夹** button opens that directory in Windows File Explorer. An accessible WSL network share is required for Explorer to show a guest path.

For manual installation, copy `plugin.toml` to a local folder, replace `executable = "{select-executable}"` with the absolute path to your `winc.exe` (use a TOML literal string in single quotes), then select the folder under **Settings → Plugins → Install from folder**. The host must support the `windows-explorer` directory action. Winc itself is installed separately.

## 中文

适用于 Windows 上的 Pebrel Winc。打开 **设置 → 插件 → 插件社区**，选择 **Winc**，再选择电脑上已经安装的 `winc.exe`，审阅并批准两项目录操作。顶栏 **Winc** 用 Winc 打开当前 Windows 或 WSL 窗格的目录，**文件夹** 用 Windows 文件资源管理器打开。资源管理器需要能访问 WSL 的网络共享。

手动安装时，把 `plugin.toml` 复制到本地文件夹，将 `executable = "{select-executable}"` 改为本机 `winc.exe` 的绝对路径（建议用 TOML 单引号字符串），再通过 **设置 → 插件 → 从文件夹安装** 选择该文件夹。宿主需要支持 `windows-explorer` 目录操作。Winc 程序需自行安装。
