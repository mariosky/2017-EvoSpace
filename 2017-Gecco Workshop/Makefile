
all: paper-front.pdf

paper-front.tex: paper-body.tex ../bib/biblio.bib
	touch $@

%.pdf: %.tex
	pdflatex $<
	bibtex $(basename $<)
	pdflatex $<
	pdflatex $<

