# Hello World with CMake

First time trying out CMake.

Source: <https://cmake.org/cmake/help/latest/>

## Run

### Clear cache

```shell
git clean -fdx
```

### Generate build files

Build with whatever the default generator is, for your platform:

```shell
build/ $ cmake ..
Hello from CMake
-- Configuring done (0.1s)
-- Generating done (0.0s)
-- Build files have been written to: .../cmake-hello/build
```

Or build with a specific generator:

```shell
build/ $ cmake -G 'Unix Makefiles'
```

List available generators:

```shell
cmake -G
```

### Run build files

```shell
build/ $ make
...
```
