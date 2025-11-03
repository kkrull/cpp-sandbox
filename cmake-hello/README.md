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
...
```

Or build with a specific generator:

```shell
build/ $ cmake .. -G <generator>
```

### Run build files

```shell
build/ $ make
...
```
