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

## List all extensions
List all Visual Studio Code extensions
```sh
code --list-extensions | xargs -L 1 echo code --install-extension | pbcopy
rm -rf ~/config/vs/extensions.sh
pbpaste > ~/config/vs/extensions.sh
```