# Rust 설정

## rustup 설치

터미널에 다음의 내용을 한 줄씩 입력해 rustup을 설치합니다.

```text
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
1
source $HOME/.cargo/env
```

## Rust 프로젝트 만들기

Manjaro에서 원하는 폴더에 들어가 다음의 내용을 입력합니다. `<name>`은 자신이 원하는 이름으로 변경하면 됩니다. 이후의 내용은 해당 프로젝트 폴더에서 우클릭해 vscode를 열고 실행합니다.

```text
cargo new --bin <name>
```

## vscode 설정

1. `rust-analyzer`와 `Better TOML`과 `crates` 확장을 검색해 설치합니다.
2. 우측 하단의 경고창을 통해 Language Server를 설치합니다.
3. `src/main.rs`에서 `Ctrl` + `Alt` + `n`으로 프로젝트를 실행합니다. 다음의 Rust 예제를 통해 확인하십시오.

```rust
fn main() {
    println!("Hello, world!");
}
```

