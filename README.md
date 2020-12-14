# Rust Embedded Template
generic rust embedded project template

[English](README.en-us.md)


## 使用的开发工具
* vscode `Embedded-Debug` 调试工具

* `cargo-generate`
  
  使用模板创建 cargo 项目工具
  ```
  cargo install cargo-generate
  
  # usage
  cargo generate https://github.com/Liangdi/rust-rv-embedded-template.git

  ```
* cargo-edit

  `cargo` 依赖管理工具
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
## 项目木板使用方法
* 创建项目
    ```
    cargo generate https://github.com/Liangdi/rust-rv-embedded-template.git your-project

    ```
* 调试
  
  vscode 中安装了 Embedded-Debug 插件后, 按 `F5` 便可启动调试
* 生成固件和烧录
  
  执行 vscode 的任务 `Build firmware` 生成 bin 文件, 保存路径为 `build/release/firmware.bin`

## Source Struct
* .cargo

  `cargo` 配置目录
* .vscode
  
  `vscode` 配置目录, 配置了调试以及可执行任务
* build/debug
  
  调试程序输出目录
* build/release
  
  固件输出目录
* openocd
  
  `openocd` 配置文件目录
* ld-script

  链接文件目录