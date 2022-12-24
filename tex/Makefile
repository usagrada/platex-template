all:
	mkdir -p out
	platex -output-directory=out main.tex
	bibtex out/main
	platex -output-directory=out main.tex
	platex -output-directory=out main.tex
	dvipdfmx out/main
	rm -f *.aux *.dvi
clean:
	rm -f *.aux *.dvi *.log *.pdf
