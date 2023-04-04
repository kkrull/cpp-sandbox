#Configuration for MacOS with XCode tools installed
CXX=clang++
CXXFLAGS=-std=c++11 -stdlib=libc++

objects = helloworld.o

bin/helloworld: $(objects)
	@mkdir -p bin
	$(CXX) $(CXXFLAGS) -o bin/helloworld $(objects)
	@echo "Created: bin/helloworld"

helloworld.o: helloworld.cpp
	$(CXX) $(CXXFLAGS) -c helloworld.cpp

.PHONY: clean
clean:
	rm -Rf bin/ *.o
