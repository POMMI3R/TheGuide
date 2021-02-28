---
description: 이 섹션은 건너뛸 수 있습니다.
---

# Arch 계열 Linux에서 프로그램 설치하기

## 소개

Arch 계열 Linux에서는 공식 패키지 매니저로 `pacman`을 사용합니다. 그러나 공식 저장소의 패키지뿐만 아니라 유저들이 등록한 패키지도 관리하기 위해 우리는 `yay` 패키지 매니저를 사용할 것입니다.

## 설치

다음의 명령어를 입력해 `yay`를 설치합니다.

```text
sudo pacman -S yay
```

## 사용법

다음은 yay의 주요 명령어입니다.

* 패키지 설치

```text
yay -S <name1> <name2> ...
```

* 모든 패키지 업데이트

```text
yay -Syu
```

* 패키지 제거

```text
yay -Rns <name1> <name2> ...
```

* 패키지 관리자 캐시 제거

```text
yay -Scc
```

