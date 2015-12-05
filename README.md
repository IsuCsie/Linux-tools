Linux 裝B 小工具
===

這是一份整理Linux小工具的文件。

本文內容僅提供安裝方式，詳細特效與範例請參照來源使用。

- Linux 裝B 小工具
  - [推薦必裝軟體](#推薦必裝軟體)
  - [Zsh](#zsh)
  - [fish](#fish)
  - [Antigen](#antigen)
  - [Oh my zsh](#oh-my-zsh)
  - [The Fuck](#the-fuck)
  - [Ranger](#ranger)
  - [vim](#vim)
    - [Vundle](#vundle)

## 推薦必裝軟體
原本在Linux就廣為人知且必裝之好用工具

- wget, curl
  - 終端機用下載工具
- git
  - 版本控制工具
- vim
  - 終端機用文字編輯器
- tmux
  - 終端機多工軟體
- htop, nmon
  - 終端機的系統監控
- aptitude
  - Ubuntu用安裝套件工具
- yaourt
  - AUR工具
- packer
  - Archlinux上比yaourt還好用的AUR工具

```
//Ubuntu
sudo apt-get update && sudo apt-get install -y wget git vim tmux htop nmon aptitude
```

```
//Archlinux
sudo pacman -Syu wget curl git vim tmux htop yaourt
sudo yaourt -S packer
```

### Zsh
來源：[Zsh](http://www.zsh.org/)

```
//Ubuntu
sudo apt-get update && sudo apt-get install -y zsh
```

```
//Archlinux
sudo pacman -Syu zsh
```

- 切換預設Shell為Zsh

```
chsh -s /bin/zsh
```


### fish
來源：[fish shell](http://fishshell.com/)
很厲害的 shell

```
//Ubuntu
sudo apt-get update && sudo apt-get install -y fish
```

```
//Archlinux
sudo pacman -Syu fish
```


### Antigen
來源：[zsh-users/antigen](https://github.com/zsh-users/antigen)

```
//Install
curl -L https://raw.githubusercontent.com/zsh-users/antigen/master/antigen.zsh > antigen.zsh
source antigen.zsh
```

裝好之後就可以裝zsh的plugin
#### Oh my zsh
來源: [robbyrussell/oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)

很多好用東西的Zsh擴充

```
//oh-my-zsh
antigen bundle robbyrussell/oh-my-zsh
```

安裝完Oh-my-Zsh後修改`~/.zshrc`
```
ZSH_THEME=robbyrussell
```
將robbyrussell修改成想要的名稱，[主題一覽](https://github.com/robbyrussell/oh-my-zsh/wiki/themes)

### The Fuck
來源: [nvbn/thefuck](https://github.com/nvbn/thefuck)

一個可以校正指令的好用工具
[安裝來源參考](https://github.com/nvbn/thefuck/wiki/Installation)

```
//Ubuntu
sudo apt-get update && sudo apt-get install -y python-pip python-dev
sudo pip install thefuck
```

```
//Archlinux
sudo pacman -Syu thefuck
```
### Ranger
來源: [hut/ranger](https://github.com/hut/ranger)

vi風格的檔案瀏覽器
```
//Ubuntu
sudo apt-get update && sudo apt-get install -y ranger
```

```
//Archlinux
sudo pacman -Syu ranger
```

###vim
Linux 上超級好用的編輯器被稱為***編輯器之神***
常被拿來與 Emacs (神的編輯器) 做比較。


###Vundle
來源：[gmarik/Vundle.vim](https://github.com/gmarik/Vundle.vim)

一款好用的 vim 套件管理工具，讓你可以輕易的將自己的 vim 提升到另一個層次。

如果你有在寫 python 就可以嘗試一下 [fisa-vim-config](https://github.com/fisadev/fisa-vim-config)
