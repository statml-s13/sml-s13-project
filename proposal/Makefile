SHELL = /bin/bash

proposal.pdf: proposal.tex proposal.bib
	pdflatex $<
	bibtex proposal
	pdflatex $<
	pdflatex $<

midterm.pdf: midterm.tex proposal.bib
	pdflatex $<
	bibtex $(basename $<)
	pdflatex $<
	pdflatex $<

clean:
	rm -f proposal.{aux,log,blg,bbl}
	rm -f midterm.{aux,log,blg,bbl}

spotless: clean
	rm -f proposal.pdf
	rm -f midterm.pdf

.PHONY: clean spotless
