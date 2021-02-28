# 필수 확장

## Korean Language Pack for Visual Studio Code

vscode를 위한 한국어 팩입니다.

## Code Runner

간편하게 터미널로 특정 명령을 수행할 수 있도록 도와줍니다. 언어별 명령을 설정하는 법은 다음과 같습니다.

1. `settings.json`에 들어갑니다.
2. 전체 중괄호 안에 다음 내용을 추가합니다.

```text
    "code-runner.saveFileBeforeRun"  : true,
    "code-runner.clearPreviousOutput": true,
    "code-runner.runInTerminal"      : true,
    "code-runner.ignoreSelection"    : true,
    "code-runner.executorMap"        : {
        "python": "cd $dir && python $fileName",
        "c"     : "cd $dir && gcc $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt",
        "cpp"   : "cd $dir && g++ $fileName -o $fileNameWithoutExt && $dir$fileNameWithoutExt",
        "rust"  : "cargo run"
    }
```

