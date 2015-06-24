Linux 裝B 小工具
===

這是一份整理Linux小工具的套件。

## 預裝軟體:tmux, git, zsh, curl, vim, ranger

ranger來源: [hut/ranger](https://github.com/hut/ranger)

```bash
//Ubuntu
sudo apt-get install -y tmux git zsh curl vim ranger
```

```bash
//Archlinux
sudo pacman -Sy tmux git zsh curl vim ranger
```


## Start fucking 擴充功能
### Antigen
來源：[zsh-users/antigen](https://github.com/zsh-users/antigen)

```bash
//Install
curl -L https://raw.githubusercontent.com/zsh-users/antigen/master/antigen.zsh > antigen.zsh
source antigen.zsh
```

裝好之後就可以裝zsh的plugin
#### Oh my zsh
來源: [robbyrussell/oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)

很多好用東西的Zsh擴充

```bash
//oh-my-zsh
antigen bundle robbyrussell/oh-my-zsh
```

安裝完Oh-my-Zsh後修改`~/.zshrc`
```bash
ZSH_THEME=robbyrussell
```
將robbyrussell修改成想要的名稱，[主題一覽](https://github.com/robbyrussell/oh-my-zsh/wiki/themes)
