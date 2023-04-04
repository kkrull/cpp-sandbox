CXX=clang++
CXXFLAGS=-std=c++11 -stdlib=libc++
.DEFAULT_GOAL := bin/helloworld

bin/helloworld: helloworld.cpp
	mkdir -p bin
	$(CXX) $(CXXFLAGS) helloworld.cpp -o bin/helloworld

.PHONY: clean
clean:
	rm -Rf bin/
