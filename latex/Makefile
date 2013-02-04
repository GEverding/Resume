

all: pdf
	
latex:
	echo "Running Latex..\n"
	latex resume.tex
	echo "Completed Latex\n"

pdf: latex
	echo "Running pdflatex...\n"
	pdflatex resume.tex
	echo "Completed pdflatex\n"

production: all
	cp resume.pdf GarrettEverding_Resume.pdf

.PHONY: all latex pdf production
