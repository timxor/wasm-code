# c-fibonacci


## confirm you have emscripten installed
``` 
emcc --version
```

## compile fib.c
``` 
emcc -s WASM=1 -o fib.js fib.c -s EXPORTED_FUNCTIONS='["_fib"]' -s EXTRA_EXPORTED_RUNTIME_METHODS='["ccall", "cwrap"]'
```

## open up your browser to index.html
``` 
http://localhost:63342/wasm-code/c-fibonacci/index.html
```
You should get an alert that of the computation of fib(12).

Boom! That was your first c-to-easw program transpiled from c and executed in the browser.





