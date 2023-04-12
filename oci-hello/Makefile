#TODO KDK: How to detect WSL, or that docker and podman are aliases?
docker := podman.exe

.PHONY: docker-build
docker-build:
	$(docker) build -t kkrull/gcc:latest .

.PHONY: docker-interactive
docker-interactive:
	$(docker) run -it --rm -vsrc:/src kkrull/gcc:latest bash

.PHONY: docker-run
docker-run:
	$(docker) run --rm -vsrc:/src kkrull/gcc:latest
