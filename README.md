# Visual Studio Code (Editor & Terminal)
Download [Scoop](https://github.com/BosEriko/scoop) as your package manager then install [Visual Studio Code](https://scoop.sh/#/apps?q=vscode).

## Install Visual Studio Code
```sh
scoop bucket add extras
scoop install extras/vscode
```

## Install Font
```sh
scoop bucket add nerd-fonts
scoop install nerd-fonts/JetBrainsMono-NF-Mono
```

_Note: If the font doesn't show, please restart your pc._

## Sync your settings
Go to the folder where the current `settings.json` and `keybindings.json` are located and run the following script.
```sh
curl -fsSL https://raw.githubusercontent.com/BosEriko/vs/HEAD/install.sh | sh
```

_Note: If you're having a hard time locating the folder you can easily get it by pressing `Ctrl`+`Shift`+`P` to `Show All Commands`. Then on the list select `Preferences: Open User Settings (JSON)` then `File: Copy Relative Path of Active File`._

## Sync Your CSS
Add the proper path of the CSS on `settings.json` for the parameter `vscode_custom_css.imports`.

## Install Extensions
Run the command below on PowerShell to install the extensions.
```sh
irm https://raw.githubusercontent.com/BosEriko/vs/HEAD/extensions.sh | iex
```

## Update Default Profile
If you have a [Virtual Machine](https://github.com/BosEriko/wsl) set up, update your default terminal profile by pressing `Ctrl`+`Shift`+`P` to `Show All Commands`. Then on the list select `Terminal: Select Default Profile` and choose the Distro of your choice.