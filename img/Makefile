# Makefile

SOURCES := $(wildcard *.gv)
OBJECTS := $(SOURCES:.gv=.png)

all: $(OBJECTS)

%.png: %.gv
	dot $< -T png:cairo -o $@ -v

clean:
	rm -f $(OBJECTS)

.PHONY: all clean
