<p align="center">
  <img src="images/app-icon.svg" width="128" height="128" alt="" />
</p>

<h1 align="center">Windows 11 Context Menu</h1>

<p align="center"><strong>Take back control of the Windows 11 right-click menu.</strong></p>

<p align="center">
  <a href="https://github.com/Xavinooo/Windows11ContextMenu.Releases/releases/latest"><img alt="Latest version" src="https://img.shields.io/github/v/release/Xavinooo/Windows11ContextMenu.Releases?display_name=tag" /></a>
  <a href="https://github.com/Xavinooo/Windows11ContextMenu.Releases/releases"><img alt="Downloads" src="https://img.shields.io/github/downloads/Xavinooo/Windows11ContextMenu.Releases/total.svg" /></a>
  <img alt="Windows 11" src="https://img.shields.io/badge/Windows-11-0078D4?logo=windows11&logoColor=white" />
  <a href="LICENSE"><img alt="License: free, proprietary" src="https://img.shields.io/badge/license-free%2C%20proprietary-555" /></a>
  <a href="https://www.paypal.me/xaviergehl"><img alt="Donate with PayPal" src="https://img.shields.io/badge/Donate-PayPal-00457C?logo=paypal&logoColor=white" /></a>
</p>

<p align="center">
  <a href="https://github.com/Xavinooo/Windows11ContextMenu.Releases/releases/latest"><strong>⬇ Download</strong></a>
</p>

<p align="center">
  <img src="images/custom-menu.png" alt="The custom menu: quick action bar, colour icons and an open “Tools” group" />
</p>

## Why?

The Windows 11 right-click menu looks better, but it is less handy:

- **Two menus instead of one.** 7-Zip, Notepad++, “Send to”… are hidden behind “Show more options”.
- **Nothing to adjust.** You cannot remove an entry, add one or change their order without editing the registry.
- **The old menu looks out of place.** Bringing it back takes a little-known registry key, and it has neither icons nor a dark theme.
- **It gets cluttered** as you install more software.

Windows 11 Context Menu fixes all this without modifying Windows: one switch brings back the original menu.

## What it does

| | |
| --- | --- |
| 🙈 **Hide** | The entries of Windows and of your apps that you never use, even those Windows will not let you remove (Open with, Send to…). |
| ➕ **Add** | Your own commands or sub-menus (a 7-Zip template is provided). |
| 🎨 **One menu** | Everything in a single menu, without “Show more options”, redrawn like Windows 11: icons, light or dark theme, adjustable transparent background, action bar. Each entry can be hidden, grouped or moved. |
| ⌨️ **Shortcuts** | Shift + right-click for Windows' classic menu, Ctrl + right-click for your menu with the extended commands (Ctrl + Shift: the extended classic menu), Ctrl + Shift on an entry to run it as administrator. |
| ↩️ **Go back** | One switch restores the original menu, without losing your settings. |
| 💾 **Back up** | Export your settings to a file and import them back, on this PC or another one. |
| 🌍 **Six languages** | English, French, German, Spanish, Italian and Portuguese, following Windows. |
| 🔄 **Updates** | The app lets you know and updates in one click. |

<p align="center">
  <img src="images/menu-entries-page.png" alt="The “Menu entries” page: hide, group and place each entry" width="820" />
</p>

> [!IMPORTANT]
> **Closely tied to how Windows works.** To change the menu, the app relies on how File Explorer builds its right-click menu, which Microsoft does not document and can change at any time. A simple Windows update, Insider builds first, can break it. If that happens, one switch brings the original menu back while a fix is on its way: please report it in an [Issue](https://github.com/Xavinooo/Windows11ContextMenu.Releases/issues/new/choose) with your Windows version.

> [!NOTE]
> **Windows 11 26H2 and its new menu.** Newer Windows 11 builds have a new right-click menu and no longer open the classic one on their own. So that your menu still opens on a plain right-click there, the app runs a small program that starts with your Windows session. You can turn it off in Settings, under **Replace Windows' new context menu** — Windows' new menu then shows instead. It only runs on PCs that have the new menu, and leaves nothing behind once turned off or uninstalled.

## Installation

Windows 11 (25H2 or later), x64. Download the latest version from the [**Releases**](https://github.com/Xavinooo/Windows11ContextMenu.Releases/releases/latest) page.

| File | For whom |
| --- | --- |
| **Setup-selfcontained** ⭐ | The full installer, everything included. No administrator rights needed. |
| **Setup-light** | The same, smaller, if you already have the [.NET 11 Desktop Runtime](https://dotnet.microsoft.com/download/dotnet/11.0) and the [Windows App SDK runtime](https://learn.microsoft.com/windows/apps/windows-app-sdk/downloads) (the release notes give its version). |
| **selfcontained** (zip) | The full version, without installation. |
| **light** (zip) | The light version, without installation. |

Zip version: extract it where you want to keep it, then run `ContextMenu.App.exe`. It must stay in that folder.

<details>
<summary><strong>“Windows protected your PC”</strong></summary>

<br>

The app is not signed by a recognised authority. Click **More info**, then **Run anyway**.

</details>

## Getting started

1. Launch the app, then click **Restart File Explorer**: the new menu replaces the Windows 11 one.
2. Right-click a few times, on a file, a folder and a folder background: the **Menu entries** page fills up with what you have seen.
3. Tick “Hide” on the entries you no longer want, group them or set their order: the change shows at the next right-click.
4. In **My entries**, add your own commands.

## Updates

At startup, at most once a day, the app checks whether a new version exists. **Update** downloads it, checks its fingerprint and restarts the app; if anything goes wrong, the previous version is kept.

## Uninstalling

<details>
<summary>See the two ways</summary>

<br>

- **From the app**: **Settings > Uninstall completely** restores the original menu, removes the extension and deletes your settings. For a zip version, then delete its folder.
- **Installed version**: Settings > Apps > Windows 11 Context Menu > Uninstall. The original menu comes back; the uninstaller asks whether to delete your settings.

</details>

## Known limitations

<details>
<summary>See the list</summary>

<br>

- Turning the menu on or off requires restarting File Explorer (a button does it).
- An entry appears in “Menu entries” only after it has been seen once in a real menu.
- Screen readers do not read the names of the redrawn entries.

</details>

## A problem, an idea?

- 🐞 A bug or an idea: open an [**Issue**](https://github.com/Xavinooo/Windows11ContextMenu.Releases/issues/new/choose). Give the app version (**About** page) and your Windows version and, if you can, turn on **Settings > Diagnostic log**, reproduce the problem and attach `%LocalAppData%\Windows11ContextMenu\shell.log`.
- 💬 A question, some feedback: use the [**Discussions**](https://github.com/Xavinooo/Windows11ContextMenu.Releases/discussions).

## Support the project

The app is free. If it helps you, you can support its development:

<p align="center">
  <a href="https://www.paypal.me/xaviergehl"><img alt="Donate with PayPal" src="https://img.shields.io/badge/Donate-PayPal-00457C?style=for-the-badge&logo=paypal&logoColor=white" /></a>
</p>

## License

Free, for personal or professional use. The source code is not published. See [LICENSE](LICENSE).
