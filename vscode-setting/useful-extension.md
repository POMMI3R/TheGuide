---
description: 이 섹션은 건너뛸 수 있습니다.
---

# 유용한 확장

## Bracket Pair Colorizer 2

짝별로 괄호의 색을 다르게 만들어 괄호 짝을 쉽게 찾을 수 있도록 도와줍니다. 좌측에 괄호 영역을 표시하는 법은 다음과 같습니다.

1. settings.json에 들어갑니다.
2. 전체 중괄호 안에 다음 내용을 추가해 줍니다.

```text
    "bracket-pair-colorizer-2.showBracketsInGutter": true
```

## Better Align

`=`, `:` 등에 맞춰 줄을 정렬하도록 도와줍니다. 단축키를 설정하는 법은 다음과 같습니다.

1. 플러그인 설치 후, `Ctrl + Shift + p를 눌러 기본 설정: 바로 가기 키 열기(JSON)`를 누릅니다.
2. 전체 대괄호 안에 다음 내용을 추가합니다.

```text
    {
        "key"    : "ctrl+y",
        "command": "wwm.aligncode",
        "when"   : "editorTextFocus && !editorReadonly"
    }
```

 이제 코드를 드래그한 후 `Ctrl` + `y` 키를 눌러 줄을 정렬할 수 있습니다.

## vscode-pdf

vscode에서 pdf 파일을 열 수 있게 해줍니다.

## Markdown All in One, Markdown Preview Enhanced

마크다운 작성을 도와줍니다.

## Tabnine Autocomplete AI

자동완성 기능을 강력하게 해줍니다.

