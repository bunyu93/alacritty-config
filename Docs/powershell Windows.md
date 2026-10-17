# powershell Windows

PSReadLine

oh-my-posh

DockerCompletion

posh-git

eza-community.eza



```powershell
# Enable PSReadLine prediction and history options - Install-Module PSReadLine
Import-Module PSReadLine
Set-PSReadLineOption -PredictionSource History
Set-PSReadLineOption -PredictionViewStyle Listview

# Git - Install-Module posh-git
Import-Module posh-git

# Docker completion - Install-Module DockerCompletion
Import-Module DockerCompletion

# Oh My Posh - winget install --id JanDeDobbeleer.OhMyPosh -e
oh-my-posh init pwsh | Invoke-Expression

# eza-community.eza - winget install eza-community.eza
function ls {
    eza --icons=auto --group-directories-first @args
}

function l {
    eza --git-ignore --icons=auto --group-directories-first @args
}

function ll {
    eza --all --header --long --git --icons=auto --group-directories-first @args
}

function llm {
    eza --all --header --long --sort=modified --icons=auto --group-directories-first @args
}

function la {
    eza -lbhHigUmuSa --icons=auto --group-directories-first @args
}

function lx {
    eza -lbhHigUmuSa@ --icons=auto --group-directories-first @args
}

function lt {
    eza --tree --icons=auto --group-directories-first @args
}

function tree {
    eza --tree --icons=auto --group-directories-first @args
}
```
