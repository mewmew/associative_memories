all: report.pdf clean_aux

%.pdf: %.tex
	pdflatex report.tex
	bibtex report
	pdflatex report.tex
	pdflatex report.tex

.PHONY: clean_aux

clean_aux:
	rm -f *.aux *.log *.out *.toc *.bbl *.blg *.dvi *.rtf *.bcf *-blx.bib *.run.xml sections/*.aux
