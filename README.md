# AI Effect Video

[한국어](README.ko.md)

**AI Effect Video** is a video editor for Windows. It copies parts of an effect video (fire, explosions, light and so on) onto your original video, frame by frame and without resizing, adds text, mosaics and pictures, and exports the result as a new video.

This repository is where the program is **downloaded**. The program's source code is not published here.

## Download

Get the latest version from the **[Releases page](https://github.com/NexCreDesign/AIEffectVideo_release/releases/latest)**.

| File | What it is |
|---|---|
| `EffectVideo-<version>.zip` | **The program.** This is the only file you need. |
| `EffectVideo-<version>-ffmpeg-source.zip` | Source code of the FFmpeg parts inside the program, provided for license reasons ([details](FFMPEG_SOURCE.md)). You don't need it to use the program. |

## Requirements

- Windows 11 (64-bit). Windows 10 may work, but is not tested.
- A graphics card that supports DirectX 11 is recommended. Without one, the program still works but is slower.
- Videos up to 3840×2160.

## How to run

1. Download `EffectVideo-<version>.zip`.
2. Unzip it to a folder you will keep, for example `C:\Tools`. The zip already contains a folder named `EffectVideo-<version>`, so you get `C:\Tools\EffectVideo-<version>`. There is nothing to install.
   - In the Windows **Extract All** window, enter only `C:\Tools` as the destination. If the destination ends with `EffectVideo-<version>`, you get that folder twice, one inside the other.
3. Double-click `effect_video.exe` in that folder.
   - If a blue **"Windows protected your PC"** window appears, click **More info**, then **Run anyway**. It appears because the program is not code-signed yet.
4. Press **F1** in the program to open the user guide.

To remove the program, delete the folder. Settings and logs are kept in `%APPDATA%\EffectVideo` and `%LOCALAPPDATA%\EffectVideo`; delete those folders too if you want to remove everything.

## Free edition

The free edition has every feature. Exported videos, and the work viewer in the program, show a small **"AI Effect Video Free"** mark in the bottom right corner.

## Edit with AI (optional)

You can connect an AI app such as Claude Desktop and edit by chatting. Changes appear in the editor right away and can be undone with Ctrl+Z. The AI app is installed separately; the editor does not contain an AI model.
How to connect: **[ai-effect-video-mcp](https://github.com/NexCreDesign/ai-effect-video-mcp)**

## Checking the download (optional)

Each release lists the SHA-256 checksum of its files. To check yours, run this in PowerShell and compare the result with the release page:

```powershell
Get-FileHash .\EffectVideo-1.0.0.zip -Algorithm SHA256
```

## Questions and bug reports

Email **nexcredesign@protonmail.com**, or use **Help › Contact Support** in the program. It helps to include:

- The version: **Help › About AI Effect Video…**
- What you did and what happened
- The log file: save it with **Help › Save Log…**

Questions about the AI connection can also go to [ai-effect-video-mcp Issues](https://github.com/NexCreDesign/ai-effect-video-mcp/issues).

## License and privacy

- [License terms](LICENSE.md): free to use; the program may not be redistributed. Open source components keep their own licenses.
- [Privacy policy](PRIVACY.md): the program collects no personal data.
- Open source notices: `THIRD_PARTY_NOTICES.html` and the `licenses` folder inside the zip, also shown in **Help › About AI Effect Video…**
- [Changelog](CHANGELOG.md)
