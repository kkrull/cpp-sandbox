#Configuration for MacOS with XCode tools installed
CXX=clang++
CXXFLAGS=-std=c++11 -stdlib=libc++

bin/helloworld: helloworld.cpp
	@mkdir -p bin
	$(CXX) $(CXXFLAGS) helloworld.cpp -o bin/helloworld

.PHONY: clean
clean:
	rm -Rf bin/
