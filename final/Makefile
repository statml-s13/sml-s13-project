SHELL = /bin/bash

MAINDOC = main
TEXFILES = main.tex

main.pdf: $(TEXFILES)
	pdflatex $<
	bibtex $(MAINDOC)
	pdflatex $<
	pdflatex $<


clean:
	rm -f $(MAINDOC).{aux,bbl,blg,log}

spotless: clean
	rm -f $(MAINDOC).pdf

.PHONY: clean spotless
