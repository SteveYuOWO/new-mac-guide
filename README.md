# New mac guide 💻

最近换了新的电脑，记录一下我的新电脑的软件安装过程。节省下一次换电脑的配置时间。由于我换电脑的时候不太喜欢迁移文件（使用 Mac 的 TimeMachine，重要文件我都存储在 icloud 里面），所以仅记录我的配置过程。

1. 切换输入法为微软双拼，并添加简体和繁体中文。
2. 安装 VPN，机场✈️✈️✈️的选择使用 [次元链接](https://cylink.app/) ，VPN 选择使用 [ClashX](https://download.ovor.cc/cx) 客户端。（机场要选择好，否则以下步骤都会比较麻烦）
3. 安装 1Password（助记词在 icloud），安装 chrome 并登陆同步。
4. 配置 1Password 和 chrome 后，下载 [brew](https://brew.sh/) 包管理工具。🍺🍺🍺
5. 安装 xcode-select

```bash
xcode-select --install
```

6. 使用 brew 安装 git

```bash
# git installation
brew install git

# config personal info
git config --global user.name "Steve Yu"
git config --global user.email steveyuowo@gmail.com

# config ssh 
ssh-keygen
# trigger enter 🧐
# donot forgot setting for git after generate new ssh keygen
```

7. 安装 [nodejs](https://nodejs.org/en/)，官网安装一个稳定版，之后用 n 切换。

```bash
# if error, please append `sudo` prefix
npm install -g yarn
npm install -g n
n stable
```

8. 安装工具

```bash
brew install typora # 写作工具
brew install python@3.8 # 之后 vim-plus 需要
brew install visual-studio-code # 代码编辑工具
```

9. Terminal

```bash
# Install Oh my zsh
# https://github.com/ohmyzsh/ohmyzsh
# Change the theme from '~/.zshrc'

# follow the official guide
ZSH_THEME="takashiyoshida"

git clone git://github.com/zsh-users/zsh-autosuggestions ~/.oh-my-zsh/plugins/zsh-autosuggestions

# Install vim-plus
# https://github.com/chxuan/vimplus
# follow the official guide
cd .vim/plugged
rm -rf LeaderF
rm -rf YouCompleteMe # 不想安装，mac下有些补齐比较难安装
```

