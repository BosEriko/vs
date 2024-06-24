# Bos Eriko's Visual Studio Code Config

## List all extensions
List all Visual Studio Code extensions
```sh
    code --list-extensions | xargs -L 1 echo code --install-extension | pbcopy
    rm -rf ~/config/vs/extensions.sh
    pbpaste > ~/config/vs/extensions.sh
```
