#Configuration for MacOS with XCode tools installed
CXX=clang++
CXXFLAGS=-std=c++11 -stdlib=libc++

bin/helloworld: helloworld.o
	@mkdir -p bin
	$(CXX) $(CXXFLAGS) -o bin/helloworld helloworld.o
	@echo "Created: bin/helloworld"

helloworld.o: helloworld.cpp
	$(CXX) $(CXXFLAGS) -c helloworld.cpp

.PHONY: clean
clean:
	rm -Rf bin/ *.o
