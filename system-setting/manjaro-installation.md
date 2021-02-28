# Manjaro 설치

## 설치

1. [링크](https://github.com/sileshn/ManjaroWSL/releases)에서 최신 버전의 `Manjaro.zip`을 다운로드합니다.
2. 적절한 폴더에 압축을 풀고, `Manjaro.exe`를 실행해 배포판을 등록합니다.

## 사용자 등록

1. `Manjaro.exe`를 실행합니다.
2. 다음의 내용을 한 줄씩 입력해 사용자와 비밀번호를 등록합니다. `<username>`은 자신이 원하는 것으로 변경하면 됩니다.

```text
passwd
useradd -m -G wheel -s /bin/bash <username>
passwd <username>
exit
```

{% hint style="info" %}
비밀번호를 입력할 때는 입력한 내용이 보이지 않습니다.
{% endhint %}

## 기본 사용자 설정

1. `Win` + `s` 키를 눌러 `cmd`를 입력하고 `명령 프롬프트`를 누릅니다.
2. 다음의 내용을 한 줄씩 입력해 기본 사용자를 설정합니다. `<username>`은 아까 자신이 설정한 사용자 이름으로, `<directory>`는 Manjaro.exe가 있는 위치\(예: `C:\Users\Administrator\Desktop\Manjaro`\)로 변경하면 됩니다.

```text
cd <directory>
Manjaro.exe config --default-user <username>
```

