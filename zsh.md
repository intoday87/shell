# .zshrc

- [theme agnoster](https://github.com/ohmyzsh/ohmyzsh/wiki/Themes#agnoster)
- [powerline font](https://github.com/powerline/fonts)
  - [`install.sh`](https://github.com/powerline/fonts#installation) 사용
  - 메뉴 -> Preferences -> Profiles ->  Font에서 `Anonymice Pro for powerline` 사용

```.zshrc
# theme
ZSH_THEME="agnoster"

# plugins
plugins=(git docker kubectl helm npx zsh-vi-mode)

# 이전 이후 히스토리
bindkey '^P' up-line-or-search
bindkey '^N' down-line-or-search
# set -o vi로 설정하게 되면 zsh의 키 바인딩이 전체적으로 바뀌게 되어서 기존 `^X^V`외에 별도로 바인딩
bindkey '^V' vi-cmd-mode

# vi 환경으로 cli 사용
set -o vi

# kubectl 자동 완성
# mini kube가 설치되어 있어야
# @see https://kubernetes.io/ko/docs/tutorials/hello-minikube/
source < (kubectl completion zsh)
```
## item2
- Preferences -> Profile -> Color Presets... -> `Solarized Dark` 

## plugins
- [zsh-vi-mode](https://github.com/jeffreytse/zsh-vi-mode#as-an-oh-my-zsh-custom-plugin)
  - 플러그인 추가하고 `.zshrc` 다시 읽으면 vi 모드
