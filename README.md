# Marcus_Terminal_Stylization-Apr2025

| Quick guidance to install Marcus shell style on terminal (MacOS/GitBash)

# 1. Install git
type `git` to install git

# 2. Install Oh-my-zsh
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

# 3. Install [powerlevel10k](https://github.com/romkatv/powerlevel10k)

## install homebrew for later font and icons feature
`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

### homebrew ==> Next steps:
- Run these commands in your terminal to add Homebrew to your PATH:
    `echo >> /Users/marcus/.zprofile`
    `echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> /Users/marcus/.zprofile`
    `eval "$(/opt/homebrew/bin/brew shellenv)"`
- Run `brew help` to get started
- Further documentation:
    https://docs.brew.sh

## pull powerlevel10k
```
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ~/powerlevel10k
```

## change .zshrc file
Under `/Users/marcus/.zshrc`, update from `ZSH_THEME="robbyrussell"` to `ZSH_THEME="powerlevel10k/powerlevel10k"`

## install Font & Icons
Font: You need a Nerd Font (with Powerline symbols, icons).
Install one like MesloLGS NF → it's recommended by Powerlevel10k.

👉 You can download it here:
https://github.com/ryanoasis/nerd-fonts/releases (search Meslo)

Or just install by Homebrew if you are on Mac:

```
brew install alfred
brew install --cask font-meslo-lg-nerd-font
```

## setting up terminal
- open "Terminal → Preferences → Profiles → Text"
- find "Font", click "Change" or "Edit"
- set up font："MesloLGS NF"

<img width="835" alt="SCR-20250427-ozjn" src="https://github.com/user-attachments/assets/42c05bb2-e3ce-414f-8142-d3022166a7be" />


## start powerlevel10k setup app
source ~/.zshrc

## reset through powerlevel10k app: 
p10k configure

## NOTICE: 
You should choose Unicode for the advanced features:
![SCR-20250427-petl](https://github.com/user-attachments/assets/61bb698c-b034-4b7a-a7d2-f6e6059a5663)

# 4. Result
![SCR-20250427-pftz](https://github.com/user-attachments/assets/372b5eaf-3885-4197-90dc-9442228e2a44)


# Reference
[How To Make Your Boring Mac Terminal So Much Better](https://www.youtube.com/watch?v=CF1tMjvHDRA&t=6s)

[How to install oh-my-zsh and Powerlevel10k theme](https://www.google.com/search?sca_esv=e5eeec09d3fdc8a2&rlz=1C5CHFA_enUS1159US1159&sxsrf=AHTn8zoodR8pspjLyOKecFV85uxJBcjkRQ:1745796969139&q=Powerlevel10k+install+macos&udm=7&fbs=ABzOT_CWdhQLP1FcmU5B0fn3xuWp6IcynRBrzjy_vjxR0KoDMnbkfvm4jW0eza52i_Pv0GHXGdsPP4OV948uPyYLz4MWe-1RHr9g-cqNjTKbzsDkKzimGRQLXU4ygZh-gEK7vv9l7T8SL4JLiKSgQkjh2BcZZkYPaOoO1ZLaCbMq4aVDf-ytObY6llLKXzdpvClqxzKO3NDYtaVD-lBUS77P6uIC0ZwC9g&sa=X&ved=2ahUKEwiE-sfBsPmMAxWpJzQIHYBED-gQtKgLegQIGBAB&biw=852&bih=858&dpr=2#fpstate=ive&vld=cid:a3ead2bb,vid:eh7lM3Yvf94,st:0)
