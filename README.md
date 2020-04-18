# hello-rust
* [Installation](https://www.rust-lang.org/tools/install)
* [hello-world](https://doc.rust-lang.org/stable/rust-by-example/hello.html)

## 1. First app:
```bash
$ source $HOME/.cargo/env
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

$ mkdir -p target/temp
$ cd target/temp/
$ cp ../../src/main.rs ./hello.rs
$ vi hello.rs 
$ rustc hello.rs 
$ ll
total 544
drwxr-xr-x  4 Ryan  staff   128B Apr 18 09:37 .
drwxr-xr-x  5 Ryan  staff   160B Apr 18 09:36 ..
-rwxr-xr-x  1 Ryan  staff   265K Apr 18 09:37 hello
-rw-r--r--  1 Ryan  staff    45B Apr 18 09:37 hello.rs
$ ./hello 
Hello, world!

```

## Installation
```bash
$ curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
info: downloading installer

Welcome to Rust!

This will download and install the official compiler for the Rust
programming language, and its package manager, Cargo.

It will add the cargo, rustc, rustup and other commands to
Cargo's bin directory, located at:

  /Users/Ryan/.cargo/bin

This can be modified with the CARGO_HOME environment variable.

Rustup metadata and toolchains will be installed into the Rustup
home directory, located at:

  /Users/Ryan/.rustup

This can be modified with the RUSTUP_HOME environment variable.

This path will then be added to your PATH environment variable by
modifying the profile files located at:

  /Users/Ryan/.profile
/Users/Ryan/.bash_profile

You can uninstall at any time with rustup self uninstall and
these changes will be reverted.

Current installation options:


   default host triple: x86_64-apple-darwin
     default toolchain: stable
               profile: default
  modify PATH variable: yes

1) Proceed with installation (default)
2) Customize installation
3) Cancel installation
>1

$ source $HOME/.cargo/env
$ cargo help
$ cargo --version
```

