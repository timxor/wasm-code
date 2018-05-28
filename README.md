# wasm-code
Wasm code templates and examples


## make sure you have emscripten installed
``` 
git submodule update --init
cd emsdk
git pull
./emsdk install latest
./emsdk activate latest
source ./emsdk_env.sh
emcc -v
```

###You should get something like this:
``` 
[~/Documents/Projects/wasm-code/c-fibonacci]$emcc -v
emcc (Emscripten gcc/clang-like replacement + linker emulating GNU ld) 1.38.3
clang version 6.0.1  (emscripten 1.38.3 : 1.38.3)
Target: x86_64-apple-darwin17.5.0
Thread model: posix
InstalledDir: /Users/tim.siwula/Documents/Projects/wasm-code/emsdk/clang/e1.38.3_64bit
INFO:root:(Emscripten: Running sanity checks)
```

###If not then see the docs on your platform dependencies:
``` 
https://kripken.github.io/emscripten-site/docs/getting_started/downloads.html#platform-notes-installation-instructions-sdk
```
