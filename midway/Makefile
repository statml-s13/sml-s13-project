main.pdf: main.tex main.bib
	pdflatex $<
	bibtex main
	pdflatex $<
	pdflatex $<

clean:
	rm -f main.aux
	rm -f main.log
	rm -f main.blg
	rm -f main.bbl

spotless: clean
	rm -f main.pdf

.PHONY: clean spotless
