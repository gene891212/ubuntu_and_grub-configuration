# Zsh

## Install Z Shell

```bash
sudo apt-get install zsh
```

## Install oh-my-zsh

```bash
# You can use "cat /etc/shells" to check ZSH was installed.
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

Change default terminal to ZSH

```bash
chsh -s /bin/zsh
```

## Install Plugins

- [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions)

```bash
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

- [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)

```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

- [zsh-you-should-use](https://github.com/MichaelAquilina/zsh-you-should-use)

> Reminds you to use your aliases for a command you typed

```bash
git clone https://github.com/MichaelAquilina/zsh-you-should-use.git $ZSH_CUSTOM/plugins/you-should-use
```

Activate the plugin in ~/.zshrc

```bash
nano ~/.zshrc
```

Edit the line `plugins=(.....)` to

```bash
plugins=(git zsh-syntax-highlighting zsh-autosuggestions you-should-use)
```

## Install Theme

- [Powerlevel10k Github](https://github.com/romkatv/powerlevel10k#meslo-nerd-font-patched-for-powerlevel10k)

```bash
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
```

You can use the command to change your style

```bash
p10k configure
```

## Reference 

- [oh-my-zsh Github](https://github.com/ohmyzsh/ohmyzsh)
