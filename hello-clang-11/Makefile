#Configuration for MacOS with XCode tools installed
#TODO Conditional for platform-specific settings?
CXX := clang++
CXXFLAGS := -std=c++11 -stdlib=libc++

sources := $(wildcard *.cpp)
objects := $(patsubst %.cpp,%.o,$(sources))
output_dir := bin
executable := $(output_dir)/helloworld

$(executable): $(objects)
	@mkdir -p $(output_dir)
	$(CXX) $(CXXFLAGS) -o $(executable) $(objects)
	@echo "Created: $(executable)"

.PHONY: clean
clean:
	rm -Rf $(executable) $(objects)

run: $(executable)
	@$(executable)
