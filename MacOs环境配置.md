## 安装iTerm
* download iTerm2: [https://www.iterm2.com/](https://www.iterm2.com/)
* download Homebrew: [https://brew.sh/](https://brew.sh/)
* install wget: `brew install wget`
* download Oh My Zsh: [https://ohmyz.sh/](https://ohmyz.sh/)
* install atuojump: `brew install autojump`，并添加`[[ -sbrew --prefix/etc/autojump.sh ]] && .brew --prefix/etc/autojump.sh`到`.zshrc`

## Git
* 记住用户名和密码：`git config credential.helper store`

## node
* download node:
```
curl "https://nodejs.org/dist/latest/node-${VERSION:-$(wget -qO- https://nodejs.org/dist/latest/ | sed -nE 's|.*>node-(.*)\.pkg</a>.*|\1|p')}.pkg" > "$HOME/Downloads/node-latest.pkg" && sudo installer -store -pkg "$HOME/Downloads/node-latest.pkg" -target "/"
```

* download nvm: [https://github.com/creationix/nvm](https://github.com/creationix/nvm)
