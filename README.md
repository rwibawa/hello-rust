# hello-rust
* [Installation](https://www.rust-lang.org/tools/install)
* [hello-world](https://doc.rust-lang.org/stable/rust-by-example/hello.html)

## 1. Installation
```bash
$ curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
$ source $HOME/.cargo/env
$ cargo help
$ cargo --version
```

## 2. First app:
```bash
$ mkdir -p ~/Documents/workspace_rust
$ cd ~/Documents/workspace_rust

$ cargo new hello-rust
$ tree ./hello-rust/
./hello-rust/
├── Cargo.lock
├── Cargo.toml
├── README.md
├── src
│   └── main.rs
└── target
    └── debug
        ├── build

$ cd hello-rust/
$ cargo run
$ vi Cargo.toml 
$ cargo build
$ vi src/main.rs 
$ cargo run
```
