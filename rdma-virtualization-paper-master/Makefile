


PAPER=URN-paper

default: paper

paper: 
	pdflatex -synctex=1 -interaction=nonstopmode $(PAPER).tex
	bibtex $(PAPER)
	pdflatex -synctex=1 -interaction=nonstopmode $(PAPER).tex
	pdflatex -synctex=1 -interaction=nonstopmode $(PAPER).tex
	pdflatex -synctex=1 -interaction=nonstopmode $(PAPER).tex

tidy:
	rm -f $(PAPER).aux $(PAPER).bbl $(PAPER).bib $(PAPER).blg $(PAPER).log $(PAPER).out $(PAPER).synctex.gz

clean: tidy
	rm -f $(PAPER).pdf