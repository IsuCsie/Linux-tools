Linux 裝B 小工具
===

- [推薦預裝軟體](#)
	- [Zsh](#)
	- [Antigen](#)
		- [Oh my zsh](#)
	- [The Fuck](#)
	- [Ranger](#)
	- [Vundle](#)

這是一份整理Linux小工具的文件。

本文內容僅提供安裝方式，詳細特效與範例請參照來源使用。

## 推薦預裝軟體
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
- packer
  - Archlinux上比yaourt還好用的AUR工具

```
//Ubuntu
sudo apt-get install -y wget git vim tmux htop nmon aptitude
```

```
//Archlinux
sudo pacman -Sy wget curl git vim tmux htop packer
```

### Zsh

```bash
//Ubuntu
sudo apt-get install -y zsh
```

```bash
//Archlinux
sudo pacman -Sy zsh
```

- 切換預設Shell為Zsh

```bash
chsh -s /bin/zsh
```


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

### The Fuck
來源: [nvbn/thefuck](https://github.com/nvbn/thefuck)

一個可以校正指令的好用工具
[安裝來源參考](https://github.com/nvbn/thefuck/wiki/Installation)

```bash
//Ubuntu
sudo apt-get install -y python-pip python-dev
sudo pip install thefuck
```

```bash
//Archlinux
sudo pacman -Sy thefuck
```
### Ranger
來源: [hut/ranger](https://github.com/hut/ranger)

vi風格的檔案瀏覽器
```bash
//Ubuntu
sudo apt-get install -y ranger
```

```bash
//Archlinux
sudo pacman -Sy ranger
```
