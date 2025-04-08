SRC=\
	2025-01-21.qmd \
	2025-01-23.qmd \
	2025-01-28.qmd \
	2025-01-30.qmd \
	2025-02-04.qmd \
	2025-02-11.qmd \
	2025-02-13.qmd \
	2025-02-20.qmd \
	2025-03-04.qmd \
	2025-03-06.qmd \
	2025-03-11.qmd \
	2025-03-18.qmd \
	2025-03-20.qmd \
	2025-03-25.qmd \
	2025-03-27.qmd \
	2025-04-08.qmd \
	2025-04-10.qmd 

.PHONY: all web

all: ${SRC:.qmd=.pdf}

web: all
	cp *.html ../web/lec
	cp *.pdf  ../web/lec

%.html %.pdf: %.qmd
	quarto render $<
