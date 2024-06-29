# Visual Studio Code (Editor & Terminal)
Download [Scoop](https://github.com/BosEriko/scoop) as your package manager then install [Visual Studio Code](https://scoop.sh/#/apps?q=vscode).

## Install Visual Studio Code
```sh
scoop bucket add extras
scoop install extras/vscode
```

## Sync your settings
Go to the folder where the current `settings.json` and `keybindings.json` are located and run the following script.
```sh
curl -fsSL https://raw.githubusercontent.com/BosEriko/vs/HEAD/install.sh | sh
```

_Note: If you're having a hard time locating the folder you can easily get it by pressing `Ctrl`+`Shift`+`P` to `Show All Commands`. Then on the list select `Preferences: Open User Settings (JSON)` then `File: Copy Relative Path of Active File`._

## Install Extensions
Run the command below on PowerShell to install the extensions.
```sh
irm https://raw.githubusercontent.com/BosEriko/vs/HEAD/extensions.sh | iex
```

## Update Default Profile
If you have a [Virtual Machine](https://github.com/BosEriko/wsl) set up, update your default terminal profile by pressing `Ctrl`+`Shift`+`P` to `Show All Commands`. Then on the list select `Terminal: Select Default Profile` and choose the [Distro](https://github.com/BosEriko/ubuntu) of your choice.

## List all extensions
List all Visual Studio Code extensions. Make sure to use the proper `copy` and `paste` commands.
```sh
code --list-extensions | xargs -L 1 echo code --install-extension | copy
rm -rf ~/config/vs/extensions.sh
paste > ~/config/vs/extensions.sh
```