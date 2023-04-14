# Compiler settings

uname := $(shell uname)
ifeq ($(uname), Darwin)
	CXX := clang++
	CXXFLAGS := -std=c++11 -stdlib=libc++
endif

# Project settings

sources := $(wildcard *.cpp)
objects := $(patsubst %.cpp,%.o,$(sources))
output_dir := bin
executable := $(output_dir)/helloworld

# Recipes

.PHONY: build
build: $(executable)

$(executable): $(objects)
	@mkdir -p $(output_dir)
	$(CXX) $(CXXFLAGS) -o $(executable) $(objects)
	@echo "Created: $(executable)"

.PHONY: clean
clean:
	rm -Rf $(executable) $(objects)

run: $(executable)
	@$(executable)
