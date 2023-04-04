.DEFAULT_GOAL := bin/helloworld

bin/helloworld: helloworld.cpp
	mkdir -p bin
	clang++ -std=c++11 -stdlib=libc++ helloworld.cpp -o bin/helloworld

.PHONY: clean
clean:
	rm -Rf bin/
