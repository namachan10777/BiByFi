SOURCES=$(wildcard *.saty)
TARGETS=$(patsubst %.saty,%.pdf,$(SOURCES))

SATYSFI_OPTS+=-b

ifdef SATYSFI_RUNTIME
	SATYSFI_OPTS+=-C "$(SATYSFI_RUNTIME)"
endif

.PHONY: all

all: $(TARGETS)

%.pdf: %.saty
	satysfi $(SATYSFI_OPTS) $< -o $@

.PHONY: clean

clean:
	rm *.pdf
	rm *.satysfi-aux
