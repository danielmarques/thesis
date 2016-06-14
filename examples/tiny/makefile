# LaTeX Makefile

FILE=tiny

all: $(FILE).pdf

.PHONY: clean

clean:
	rm -f *.aux *.blg *.out *.bbl *.log *.dvi *.pdf *.lof *.lot *.toc

$(FILE).pdf: $(FILE).tex
	pdflatex $(FILE)
	bibtex $(FILE)
	pdflatex $(FILE)
	pdflatex $(FILE)