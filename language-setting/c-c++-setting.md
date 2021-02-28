# C / C++ 설정

## GCC 설치

yay를 사용해 `gcc`패키지를 설치합니다.

```text
yay -S gcc
```

## vscode 설정

1. `C/C++`, `Better C++ Syntax` 확장을 검색해 설치합니다.
2. `c` 혹은 `cpp` 확장자 파일을 엽니다.
3. `Ctrl` + `Alt` + `n`으로 파일을 실행합니다. 다음의 C / C++ 예제를 통해 확인하십시오.

### C

```c
#include <stdio.h>

int main() {
    printf("Hello, world!\n");
    return 0;
}
```

### C++

```cpp
#include <iostream>

auto main() -> int {
    std::cout << "Hello, world\n";
    return 0;
}
```

