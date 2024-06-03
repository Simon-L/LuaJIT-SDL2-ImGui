`apt install cmake build-essential git libgl-dev libxext-dev`
`cmake -Bbuild -DLUAJIT_BIN=build/install && cmake --build build --parallel 16 --verbose && cmake --install build --prefix build/install`