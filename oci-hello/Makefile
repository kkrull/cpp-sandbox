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
	$(docker) run -it --rm -vsrc:/src kkrull/gcc:latest bash

.PHONY: docker-run
docker-run:
	$(docker) run --rm -vsrc:/src kkrull/gcc:latest
