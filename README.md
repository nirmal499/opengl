## How to Use

```bash
git clone --recursive-modules https://github.com/nirmal499/opengl.git

cd opengl

mkdir build

cmake -B build -S .

cmake --build build

./build/main
```

##### IMPORTANT : Make sure to change the macro SHADER_PATH defined in main.cpp with the absolute path to your assets directory