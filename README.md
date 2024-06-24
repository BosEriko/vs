# Bos Eriko's VSCodium Config

## List all extensions
List all VSCodium extensions
```sh
    codium --list-extensions | xargs -L 1 echo codium --install-extension | pbcopy
    rm -rf ~/config/vs/extensions.sh
    pbpaste > ~/config/vs/extensions.sh
```
