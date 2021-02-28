# WSL 연결

## Remote Development 설치

![](../.gitbook/assets/vscode%20%281%29.png)

1. 빨간색 버튼을 클릭해 확장 탭을 엽니다.
2. Remote Development 확장을 검색해 설치합니다.

## 여기서 Manjaro vscode 열기

1. `Win` + `s` 키를 눌러 `레지스트리 편집`를 입력해 엽니다. 
2.  `컴퓨터\HKEY_CLASSES_ROOT\Directory\Background\shell` 폴더를 우클릭합니다.
3. `새로 만들기` &gt; `키`를 선택합니다.
4. 이름에 `ManjaroCode`를 입력합니다.
5. `(기본값)`을 더블클릭합니다.
6. 값 데이터에 `여기서 Manjaro vscode 열기`를 입력합니다.
7. `컴퓨터\HKEY_CLASSES_ROOT\Directory\Background\shell\ManjaroCode` 폴더를 우클릭합니다.
8. `새로 만들기` &gt; `키`를 선택합니다.
9. 이름에 `command`를 입력합니다.
10. `(기본값)`을 더블클릭합니다.
11. 값 데이터에 `<directory> run code .`를 입력합니다. `<directory>`는 Manjaro.exe의 위치\(예: `C:\Users\Administrator\Desktop\Manjaro\Manjaro.exe`\)로 변경하면 됩니다.

이제 아무 폴더나 들어가 우클릭을 하면 `여기서 Manjaro vscode 열기` 메뉴가 있는 것을 확인할 수 있습니다. 앞으로 우리는 그 방법으로 vscode를 열 것입니다.

## 

