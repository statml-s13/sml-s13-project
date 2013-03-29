proposal.pdf: proposal.tex proposal.bib
	pdflatex $<
	bibtex proposal
	pdflatex $<
	pdflatex $<

clean:
	rm -f proposal.aux
	rm -f proposal.log
	rm -f proposal.blg
	rm -f proposal.bbl

spotless: clean
	rm -f proposal.pdf

.PHONY: clean spotless
