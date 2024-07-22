# .zshrc

- [theme agnoster](https://github.com/ohmyzsh/ohmyzsh/wiki/Themes#agnoster)
- [powerline font](https://github.com/powerline/fonts)
  - [`install.sh`](https://github.com/powerline/fonts#installation) 사용
  - 메뉴 -> Preferences -> Profiles ->  Font에서 `Anonymice Pro for powerline` 사용

```.zshrc
# theme
ZSH_THEME="agnoster"

# plugins
plugins=(git docker kubectl helm zsh-vi-mode)

# kubectl 자동 완성
# https://kubernetes.io/ko/docs/tasks/tools/included/optional-kubectl-configs-zsh/
source < (kubectl completion zsh)
```
## item2
- Preferences -> Profile -> Color Presets... -> `Solarized Dark` 

## plugins
- [zsh-vi-mode](https://github.com/jeffreytse/zsh-vi-mode#as-an-oh-my-zsh-custom-plugin)
  - 플러그인 추가하고 `.zshrc` 다시 읽으면 vi 모드
