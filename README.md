# wasm-micropython
MicroPython transmuted into Javascript (WASM) by Emscripten.

Official Repo [https://github.com/micropython/micropython/tree/master/ports/javascript](https://github.com/micropython/micropython/tree/master/ports/javascript)

Running MicroPython on Webpack is a little bit tricky. It expects the firmware.wasm file at /static/js/firmware.wasm. So a simple solution is to make static and js folder on webpack's public directory and put firmware.wasm on it. (PR is accepted for a better solution)

```
mkdir -p public/static/js
cp node_modules/micropython/lib/firmware.wasm public/static/js
```
