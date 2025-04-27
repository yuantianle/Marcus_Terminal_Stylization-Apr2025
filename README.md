# Marcus_Terminal_Stylization-Apr2025

| Quick guidance to install Marcus shell style on terminal (MacOS/GitBash)

# 1. Install git
type `git` to install git

# 2. Install Oh-my-zsh
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

# 3. Install [powerlevel10k](https://github.com/romkatv/powerlevel10k)

## pull powerlevel10k
```
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ~/powerlevel10k
echo 'source ~/powerlevel10k/powerlevel10k.zsh-theme' >>! ~/.zshrc
```
## install Font & Icons
Font: You need a Nerd Font (with Powerline symbols, icons).
Install one like MesloLGS NF → it's recommended by Powerlevel10k.

👉 You can download it here:
https://github.com/ryanoasis/nerd-fonts/releases (search Meslo)

Or just install by Homebrew if you are on Mac:

```
brew tap homebrew/cask-fonts
brew install --cask font-meslo-lg-nerd-font
```

## start powerlevel10k setup app
source ~/.zshrc

## reset through powerlevel10k app: 
p10k configure


# Reference
https://www.google.com/search?sca_esv=e5eeec09d3fdc8a2&rlz=1C5CHFA_enUS1159US1159&sxsrf=AHTn8zoodR8pspjLyOKecFV85uxJBcjkRQ:1745796969139&q=Powerlevel10k+install+macos&udm=7&fbs=ABzOT_CWdhQLP1FcmU5B0fn3xuWp6IcynRBrzjy_vjxR0KoDMnbkfvm4jW0eza52i_Pv0GHXGdsPP4OV948uPyYLz4MWe-1RHr9g-cqNjTKbzsDkKzimGRQLXU4ygZh-gEK7vv9l7T8SL4JLiKSgQkjh2BcZZkYPaOoO1ZLaCbMq4aVDf-ytObY6llLKXzdpvClqxzKO3NDYtaVD-lBUS77P6uIC0ZwC9g&sa=X&ved=2ahUKEwiE-sfBsPmMAxWpJzQIHYBED-gQtKgLegQIGBAB&biw=852&bih=858&dpr=2#fpstate=ive&vld=cid:a3ead2bb,vid:eh7lM3Yvf94,st:0
