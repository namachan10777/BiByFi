SOURCES=$(wildcard *.saty)
TARGETS=$(patsubst %.saty,%.pdf,$(SOURCES))

.PHONY: all

all: $(TARGETS)

%.pdf: %.saty
	satysfi -b $< -o $@

.PHONY: clean

clean:
	rm *.pdf
	rm *.satysfi-aux
