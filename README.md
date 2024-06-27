# Visual Studio Code (Editor & Terminal)
Download [Scoop](https://github.com/BosEriko/scoop) as your package manager then install [Visual Studio Code](https://scoop.sh/#/apps?q=vscode).

## Install Visual Studio Code
```sh
scoop bucket add extras
scoop install extras/vscode
```

## Update Configuration
1. [Install your extensions](extensions.sh)
2. [Update your settings.json](settings.json)
3. [Update your keybindings.json](keybindings.json)

## Update Default Profile
If you have a [Virtual Machine](https://github.com/BosEriko/wsl) set up, update your default terminal profile by pressing `Ctrl`+`Shift`+`P` to `Show All Commands`. Then on the list select `Terminal: Select Default Profile` and choose the [Distro](https://github.com/BosEriko/nix) of your choice.

## List all extensions
List all Visual Studio Code extensions. Make sure to use the proper `copy` and `paste` commands.
```sh
code --list-extensions | xargs -L 1 echo code --install-extension | copy
rm -rf ~/config/vs/extensions.sh
paste > ~/config/vs/extensions.sh
```