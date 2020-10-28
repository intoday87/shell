# .zshrc

```.zshrc
# 이전 이후 히스토리
bindkey '^P' up-line-or-search
bindkey '^N' down-line-or-search

# vi 환경으로 cli 사용
set -o vi
```
## kubectl 자동 완성
```zsh
$ kubectl completion zsh > kubectl-completion-zsh.sh
$ chmod +x kubectl-completion-zsh.sh
$ source kubectl-completion-zsh.sh # .zshrc에 추가
```
