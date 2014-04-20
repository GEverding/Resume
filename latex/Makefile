

all: latex pdf
	
resume: 
	@latex resume.tex

coverletter:
	@latex cover_letter.tex

latex: resume coverletter

pdf: latex
	@pdflatex resume.tex
	@pdflatex cover_letter.tex

prod: all
	@cp resume.pdf Garrett_Everding_Resume.pdf

full: all
	@pdftk cover_letter.pdf resume.pdf output Garrett_Everding_CV.pdf

.PHONY: all latex pdf production
