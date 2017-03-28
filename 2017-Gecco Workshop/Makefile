
all: paper-front.pdf

paper-front.tex: paper-body.tex
	touch $@

%.pdf: %.tex
	pdflatex $<
	bibtex $(basename $<)
	pdflatex $<
	pdflatex $<

