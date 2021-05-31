# brainfuck on shuorv

构建命令

```
mkdir build
cd build
export CC=${RISCV_GCC_PATH}/riscv-none-embed-gcc
cmake ..
make
```

human read dump 命令

```
./${RISCV_GCC_PATH}/riscv-none-embed-objdump -d -z -M numeric,no-aliases libbrainfuck.a > lib.dump
```

本项目使用了[brainfuck in C](https://github.com/fabianishere/brainfuck)以及[XPACK GNU CC](https://github.com/xpack-dev-tools/riscv-none-embed-gcc-xpack)
