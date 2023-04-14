FROM gcc:12.2
RUN apt-get update && apt-get install -y \
  cmake=3.18.4-2+deb11u1

#TODO KDK: Consider using entrypoint: make, cmd: --help if it's always going to use make
#TODO KDK: Consider no entrypoint or cmd, if it should run c++ dev tools in general
#cmake, make, and compiler should be on same image so the makefile and compiler are configured the
#same
WORKDIR /src
CMD ["make"]
