# zsh OSX/Linux

zsh-autocomplete

oh my posh

zsh-syntax-highlighting

eza

```shellscript
# zsh-autocomplete - brew install zsh-autocomplete
source /opt/homebrew/share/zsh-autocomplete/zsh-autocomplete.plugin.zsh

# Oh my Posh - brew install oh-my-posh
eval "$(oh-my-posh init zsh)"

# zsh-syntax-highlighting - brew install zsh-syntax-highlighting
source /opt/homebrew/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh

# Eza defaults - brew install eza
_zsh_eza_params=(
  --icons=auto
  --group-directories-first
)

# Eza aliases
alias ls='eza ${(@)_zsh_eza_params}'
alias l='eza --git-ignore ${(@)_zsh_eza_params}'
alias ll='eza --all --header --long ${(@)_zsh_eza_params}'
alias llm='eza --all --header --long --sort=modified ${(@)_zsh_eza_params}'
alias la='eza -lbhHigUmuSa ${(@)_zsh_eza_params}'
alias lx='eza -lbhHigUmuSa@ ${(@)_zsh_eza_params}'
alias lt='eza --tree ${(@)_zsh_eza_params}'
alias tree='eza --tree ${(@)_zsh_eza_params}'
```

