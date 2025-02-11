SRC=\
	2025-02-11.qmd

.PHONY: all web

all: ${SRC:.qmd=.pdf}

web: all
	cp * ../web/lec

%.html %.pdf: %.qmd
	quarto render $<
