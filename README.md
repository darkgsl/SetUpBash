# SetUpBash
alias, competition и другие настройки
## alias
делаем два варинат
1) install_aliases.sh
curl -sL https://raw.githubusercontent.com/darkgsl/SetUpBash/main/install_aliases.sh | bash && source ~/.bashrc
2) прямо вставить в терминал (~/.bash_aliases) скрипт из install_aliases.sh

Пример. Последняя версия в install_aliases.sh
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
