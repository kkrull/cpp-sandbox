#Configuration for MacOS with XCode tools installed
CXX=clang++
CXXFLAGS=-std=c++11 -stdlib=libc++

objects = helloworld.o
output_dir = $(CURDIR)/bin
executable = $(output_dir)/helloworld

$(executable): $(objects)
	@mkdir -p $(output_dir)
	$(CXX) $(CXXFLAGS) -o $(executable) $(objects)
	@echo "Created: $(executable)"

.PHONY: clean
clean:
	rm -Rf $(executable) $(objects)
