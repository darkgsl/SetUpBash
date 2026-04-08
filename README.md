# SetUpBash
alias, competition и другие настройки
## alias
делаем два варинат
1) setup_aliases.sh
curl -sL https://your-server/setup_aliases.sh | bash
2) прямо вставить в терминал (~/.bash_aliases)

cat >> ~/.bash_aliases << 'EOF'
# Git aliases
alias gs='git status'
alias ga='git add'
alias gc='git commit -m'
alias gac='git add . && git commit -m'
alias gp='git push'
alias gl='git log --oneline --graph --all'
alias gd='git diff'
# Docker
alias d=docker
alias di="docker images"
alias dps="docker ps"
# k8s
alias k='kubectl'
alias kgp='kubectl get pods'
EOF
source ~/.bash_aliases
