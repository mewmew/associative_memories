all: project_proposal.pdf clean_aux

%.pdf: %.tex
	pdflatex project_proposal.tex
	bibtex project_proposal
	pdflatex project_proposal.tex
	pdflatex project_proposal.tex

.PHONY: clean_aux

clean_aux:
	rm -f *.aux *.log *.out *.toc *.bbl *.blg *.dvi *.rtf *.bcf *-blx.bib *.run.xml sections/*.aux
