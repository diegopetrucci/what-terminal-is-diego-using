# What terminal is Diego using

![How my terminal looks](assets/terminal.png)

I use [iTerm](https://iterm2.com/) as a replacement for the default Mac terminal, and install it via homebrew `brew install --cask iterm2`. I configure it as such:

* [Solarised dark theme, patched](https://raw.githubusercontent.com/mbadolato/iTerm2-Color-Schemes/master/schemes/Solarized%20Dark%20-%20Patched.itermcolors). Double click on the downloaded file, and then iTerm > Preferences > Profiles > Colors > Load presets > select the theme
* Natural syntax selection: the default way terminals treat word selection doesn't sit well with my habits, so I enable the "natural" one: iTerm > Preferences > Profiles > Keys > Key mappings > Presets... > Natural Text Editing > Apply (and replace) 
* [Oh my zsh](https://github.com/ohmyzsh/ohmyzsh), for configuring zsh: `sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`
* [PowerLevel10k](https://github.com/romkatv/powerlevel10k?tab=readme-ov-file#oh-my-zsh) as a prompt theme: `git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k`. After installing it, I swap the theme in `~/.zshrc` with `ZSH_THEME="powerlevel10k/powerlevel10k"`. When opening a new iTerm window the configuration wizard will start, but if it doesn't it can be triggered by `p10k configure`. I mostly use the standard/recommended config
* I use a few zsh plugins (add them as a new line in `~/.zshrc` > `plugins=()`). Here's my current ones: `git`, `zsh-syntax-highlighting`, `zsh-autosuggestions`, `zsh-history-substring-search`, `z`, `sudo`, `macos`, `you-should-use`
