## Build from source code

For now you need to build Amun from source code, it's simple to do that in small steps

## Requirements

To build Amun source code you need to have some program installed

- C++ Compiler (GCC or Clang) that supports C++20
- LLVM 14 or 15
- Cmake 3.16.0 or more
- Python (Optional only for development)
- Clang Format (Optional only for development)
- Clangd (Optional only for development)
- Ninja (Optional only for development)
- CCashe (Optional only for development)

## Clone the repository

```
git clone https://github.com/amrdeveloper/amun.git
```

## Build the project

```
cd amun
mkdir build
cd build
cmake ..
make
```

## Formating source code
For development you can format the source code easily using python3 script

```
python scripts/format_code.py
```

## Validate all samples
For development you can check and validate all samples options using python3 script

```
python scripts/check_samples.py
```

## Compling all samples to executables
For development you can compile all samples options using python3 script

```
python scripts/compile_samples.py
```

## Compling all samples to LLVM IR
For development you can compile all samples options using python3 script

```
python scripts/compile_samples_ir.py
```