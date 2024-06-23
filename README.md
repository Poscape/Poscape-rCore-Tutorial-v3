# Poscape-rCore-Tutorial-v3
## Install
> macOS 14.5 (Apple M1)
### rust & vscode & homebrew
### riscv toolchain
- `brew tap riscv/riscv`
- `brew install riscv-tools`
### riscv gdb
- download and unzip: https://static.dev.sifive.com/dev-tools/riscv64-unknown-elf-gcc-8.3.0-2020.04.1-x86_64-apple-darwin.tar.gz
- .zshrc: `export PATH="$PATH:/Users/<username>/riscv64-unknown-elf-gcc-8.3.0-2020.04.1-x86_64-apple-darwin/bin"`
> then can command `riscv64-unknown-elf-gdb`
### qemu
- `brew install qemu`
## Run
### debug server
- cd `./os` & command: `make gdbserver`
- use os in this terminal
### debug client
- (default) cd `./os` & command: `make gdbclient`
- (recommand) set `.vscode/launch.json` and run vscode debug