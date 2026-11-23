# Jebba ACC Operations — Windows installer build

This repository builds the offline Jebba ACC desktop application on a hosted Windows runner. The installation computer does not need Node.js, npm, or a terminal.

The workflow reconstructs the compressed source package from `build-package/part*.b64`, installs dependencies on GitHub's Windows runner, runs the Electron NSIS packaging step, and uploads `Jebba-ACC-Windows-Installer`.

Open the **Actions** tab and select **Build Jebba ACC Windows Installer**. The finished `.exe` is available as an artifact after a successful run.

Important: this is an MVP build. The weekly TCN Word report export and final operational field validation are not yet complete. The installer is unsigned; follow TCN IT security approval requirements before installing on an operational control-room PC.
