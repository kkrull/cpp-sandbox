# OCI Hello World

Use an OCI (a.k.a Docker, podman) container to build C++ for Linux with
[GCC](https://hub.docker.com/_/gcc).

## What compiler?

Ok so I was a little lost since last using g++ about 20 years ago, and I couldn't remember if that
was still a thing.  Apparently it is - it's the C++ front-end for the GNU Compiler Collection (GCC).
This post describes the diffeerence between `gcc` and `g++`:
<https://stackoverflow.com/a/173007/112682>

## Usage

Who has time to remember how to run Docker?  Just use the `Makefile`!

```shell
make docker-build #Build the dev image
make docker-run #Runs `make` in the container, working at src/
make docker-interactive #Start an interactive session in the container
```

When finished, the contents of `src/` are updated with whatever that `Makefile`
produces (e.g. a compiled program).
