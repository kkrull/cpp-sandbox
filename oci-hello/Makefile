
.PHONY: docker-build
docker-build:
	docker build -t kkrull/gcc:latest .

.PHONY: docker-run
docker-run:
	docker run --rm kkrull/gcc:latest

.PHONY: docker-interactive
docker-interactive:
	echo "TODO KDK: Add volume mount to eventually use for sources and Makefile"
	docker run -it --rm kkrull/gcc:latest bash
