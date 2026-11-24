# Scratch Terminal

Install **Scratch Terminal** from **Settings → Plugins → Plugin Community** and approve workspace access. For manual installation, download this folder and select it under **Settings → Plugins → Install from folder**. With a Pebrel Winc build that supports Scratch Terminal, you can also run the following command from this repository’s root.

```powershell
pebrel plugin install plugins/local.scratch-terminal --grant workspace-ui
```

In a local terminal tab, click the terminal icon in the title bar or press **Ctrl+Alt+J**. The same action hides the panel and returns focus to your pane. Click **＋** to start another scratch shell in the current tab, then click a shell’s label to switch. Every shell keeps running while hidden or unselected. Use **×** to end the selected shell, or type `exit`. When the tab has several scratch shells, the circled **×** closes all of them. If any has a running job, Pebrel asks before closing the group. Each tab has its own set of shells within the window.

Under **Settings → Plugins → Scratch terminal** you can choose a dock below the pane, a floating panel below or on the right, a size from 25%, 35%, 50%, and 65%, whether to inherit the focused pane’s directory, and whether Esc hides the panel while it has focus. A WSL pane opens a shell under the same distribution and user. Directory inheritance applies when a shell is created. Layout changes also apply to existing shells. Set the scratch terminal font size on the same page, or use **Ctrl+scroll** inside a scratch shell. All scratch shells share this size, independently of the regular terminals. The reset button restores the base font size.

In either floating layout, drag the grip at the left of the panel header to move it. Drag any edge or corner to resize. Double-click the grip to restore the default placement and size. Each tab remembers its floating geometry while the tab stays in the window, including when you hide the panel.

Each shell lasts for the lifetime of its tab in the current window. Scratch shells are not restored after restart. Disabling the plugin hides its panels and preserves running shells for the rest of that lifetime. Re-enable the plugin to reopen them. The plugin uses a declarative manifest and ships no scripts.
