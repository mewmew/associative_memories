all: report.pdf

%.pdf: %.tex
	latexmk -pdf $<
	latexmk -c -bibtex $<

.PHONY: clean

clean:
	rm -f *.aux *.log *.out *.toc *.bbl *.blg *.dvi *.rtf *.bcf *-blx.bib *.run.xml sections/*.aux
