# clox

This is the C implementation of lox in http://www.craftinginterpreters.com/
book.

This repository most definitely contains code not found in the original book,
checking out the original repo is recommended if you've landed here not
knowing what this is.

## How to build

You can use `clang` or `gcc` for compiling the main file.
`cd` into the root of this repo.

### Make the target directory (optional)
You can optionally create a directory named `target`:

```bash
mkdir target
```

**Note:** you only need to run this once.

### Compile the code
To compile the code into an binary inside `target`:

```bash
clang main.c debug.c chunk.c memory.c value.c vm.c compiler.c scanner.c -o target\clox.exe
```

**Note:** You can optionally pass any other target path in the `-o` flag.

### Execute

Now you can run the code by `cd`ing into whatever target directory you passed
in the step above.

E.g.:
```bash
.\target\clox.exe
```

## Other implementations

- My `jlox` implementation - [abhinavgunwant/jlox](https://github.com/abhinavgunwant/jlox)
- Original implementation(s) from [book's](http://www.craftinginterpreters.com/) author - [munificent/craftinginterpreters](https://github.com/munificent/craftinginterpreters).

