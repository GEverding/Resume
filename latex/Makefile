

all: latex pdf
	
latex:
	@latex resume.tex

pdf: latex
	@pdflatex resume.tex

production: all
	@cp resume.pdf GarrettEverding_Resume.pdf

.PHONY: all latex pdf production
