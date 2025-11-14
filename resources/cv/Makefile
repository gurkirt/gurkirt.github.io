all: pdf

foo=cv_gurkirt_singh

pdf: *.tex
	pdflatex $(foo).tex
	open $(foo).pdf &

bib: *.tex
	pdflatex $(foo)
	bibtex $(foo) 
	pdflatex $(foo)
	pdflatex $(foo)
	evince $(foo).pdf &

clean:
	rm -rf *.aux *.bbl *.blg *.log *.brf *.fdb_latexmk *.out *.fls *.gz

cleanbeamer:
	rm -rf *.nav *.snm *.toc *.bak

cleanpdf:
	rm  -rf *.pdf

