# Rust Embedded Template
generic rust embedded project template

[中文](README.md)

## Usage
* create project
    ```
    cargo generate --git https://github.com/Liangdi/rust-rv-embedded-template.git  -n your-project

    ```
* debug
  
  install Embedded-Debug extension in vscode , and press `F5` to start debug
* build firmware
  
  run vscode (shortcut `Ctrl + Alt + T`) task `Build firmware`

## Dev tools

* cargo-generate
  
  gen cargo project template tool
  ```
  cargo install cargo-generate
  
  # usage
  cargo generate --git https://github.com/Liangdi/rust-rv-embedded-template.git

  ```
* cargo-edit

  cargo dependences tool
  ```
  cargo install cargo-edit

  # usage
  cargo add riscv
  cargo add riscv-rt
  ```
* cargo-binutils

  binutils for cargo
  ```
  cargo install cargo-binutils

  # usage
  cargo size
  cargo objcopy -- -O binary firmware.bin
  ```

## Source Struct
* .cargo
* .vscode
* build/debug
  
  debug firmware output folder
* build/release
  
  release firmware outout folder
* openocd
  
  openocd config file folder
* ld-script

  linker scripts