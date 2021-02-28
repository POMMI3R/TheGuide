---
description: 이 섹션은 건너뛸 수 있습니다.
---

# zsh 설치하기

## 소개

많은 Linux 배포판에서 기본 셸로 bash를 사용합니다. 우리는 기본 셸을 zsh로 교체하여 다양한 플러그인\(테마, 자동완성 등\)을 설치할 것입니다.

## 설치

yay를 사용해 `zsh` 패키지를 설치합니다.

```text
yay -S zsh
```

## 기본 셸 변경

터미널에 다음의 내용을 입력해 zsh를 기본 셸로 설정합니다.

```text
chsh -s $(which zsh)
```

## Oh My Zsh 설치

터미널에 다음의 내용을 입력해 Oh My Zsh를 설치합니다.

```text
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

## 주요 플러그인 설치

터미널에 다음의 내용을 차례로 입력해 하이라이팅과 자동완성 플그인을 설치합니다.

```text
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

## zsh 설정

터미널에 다음의 내용을 입력해 `.zshrc` 설정파일을 엽니다.

```text
code ~/.zshrc
```

`plugins=(git)`이라고 되어있는 부분을 다음과 같이 수정 후 저장합니다.

```text
plugins=(
    git
    zsh-autosuggestions
    zsh-syntax-highlighting
)
```

터미널에 다음의 내용을 입력해 적용합니다.

```text
source ~/.zshrc
```

## Powerline 설치

1. yay를 사용해 `powerline`과 `powerline-fonts-git` 패키지를 설치합니다.
2. 터미널에 다음의 내용을 차례로 입력해 Powerlevel10k 플러그인을 설치합니다.

```text
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ~/powerlevel10k
echo 'source ~/powerlevel10k/powerlevel10k.zsh-theme' >>~/.zshrc
```

## Powerlevel10k 설정

터미널을 재시작하면 Powerlevel10k 설정 마법사가 자동으로 실행됩니다. 자신이 원하는 대로 적절히 설정합니다. `p10k configure` 명령을 통해 언제 다시 설정할 수 있습니다.

