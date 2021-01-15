# llvm-10-notes
Installation notes, updates, scripts, etc

- Install LLVM 10

`$ sudo vim /etc/apt/sources.list`

`$ deb http://apt.llvm.org/bionic/ llvm-toolchain-bionic-10 main`

`$ deb-src http://apt.llvm.org/bionic/ llvm-toolchain-bionic-10 main`

`$ wget -O - https://apt.llvm.org/llvm-snapshot.gpg.key |sudo apt-key add - `


` $ sudo apt-get update `


# LLVM
` sudo apt-get install libllvm-10-ocaml-dev libllvm10 llvm-10 llvm-10-dev llvm-10-doc llvm-10-examples llvm-10-runtime `

# Clang and co
` sudo apt-get install clang-10 clang-tools-10 clang-10-doc libclang-common-10-dev libclang-10-dev libclang1-10 clang-format-10 clangd-10 `

# libfuzzer
` sudo apt-get install libfuzzer-10-dev `

# lldb
` sudo apt-get install lldb-10 `

# lld (linker)
` sudo apt-get install lld-10 `

# libc++
` sudo apt-get install libc++-10-dev libc++abi-10-dev `

# OpenMP
` sudo apt-get install libomp-10-dev `

# clang-tidy
` sudo apt-get install clang-tidy-10 `


- Update and replace new version in the bin

` $sudo ln -s /usr/bin/clang-10 /usr/bin/clang `

` $sudo ln -s /usr/bin/clang++-10 /usr/bin/clang++ `

` $sudo ln -s /usr/bin/llvm-ar-10 /usr/bin/llvm-ar `

` $sudo ln -s /usr/bin/llvm-as-10 /usr/bin/llvm-as `

` $sudo ln -s /usr/bin/clangd-10 /usr/bin/clangd `

` $sudo ln -s /usr/bin/clang-tidy-10 /usr/bin/clang-tidy `