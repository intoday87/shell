# .zshrc

```.zshrc
# plugins
plugins=(git docker kubectl helm npx)

# 이전 이후 히스토리
bindkey '^P' up-line-or-search
bindkey '^N' down-line-or-search
# set -o vi로 설정하게 되면 zsh의 키 바인딩이 전체적으로 바뀌게 되어서 기존 `^X^V`외에 별도로 바인딩
bindkey '^V' vi-cmd-mode

# vi 환경으로 cli 사용
set -o vi

#kubectl 자동 완성
source < (kubectl completion zsh)
```
