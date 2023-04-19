PODMAN := $(shell command -v podman.exe 2> /dev/null)
ifdef PODMAN
	#Podman on WSL: Use short form to avoid whitespace in Program Files/
	docker := podman.exe
else
	#Native docker installed
	docker := docker
endif

.PHONY: docker-build
docker-build:
	$(docker) build -t kkrull/gcc:latest .

.PHONY: docker-clean
docker-clean:
	-$(docker) rmi kkrull/gcc:latest

.PHONY: docker-interactive
docker-interactive:
	$(docker) run -it --rm -v$(pwd)/src:/src kkrull/gcc:latest bash

.PHONY: docker-run
docker-run:
	#TODO KDK: Use an absolute path for local src, then it works
	$(docker) run --rm -vsrc:/src kkrull/gcc:latest

.PHONY: test
test:
	echo "Makefile: $MAKEFILE"
