.DEFAULT_GOAL := bin/helloworld

bin/helloworld: helloworld.cpp
	mkdir -p bin
	clang++ helloworld.cpp -o bin/helloworld

.PHONY: clean
clean:
	rm -Rf bin/
