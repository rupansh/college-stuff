format:
	clang-format -i stack-linked-list.cpp conio.h

%.out: %.cpp
	clang++ -Wall -Werror $< -o $@

build:	$(addsuffix .out, $(basename $(wildcard *.cpp)))

clean:
	rm -f *.out

.DEFAULT_GOAL := build
