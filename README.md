# configs

Configure tmux : 
```
1) git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
2) copy tmux.conf from repo
3) prefix + shift i
```

Configure zsh:
```
1) apt install zsh -y
2) sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
3) git clone https://github.com/zsh-users/zsh-syntax-highlighting.git .oh-my-zsh/plugins/zsh-syntax-highlighting
4) apt install fzf
5) git clone --depth=1 https://github.com/romkatv/powerlevel10k.git $HOME/.oh-my-zsh/themes/powerlevel10k
6) git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
7) copy conf .zshrc from repo
```

For OpenStack :
```
1) git clone https://github.com/t0mk/oh-my-zsh-openstack
2) for d in $(find `pwd`/oh-my-zsh-openstack -mindepth 1 -maxdepth 1 -type d -not -iwholename '*.git'); do echo `basename $d`; ln -s $d .oh-my-zsh/custom/plugins/`basename $d`; done
```
