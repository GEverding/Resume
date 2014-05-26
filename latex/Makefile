

all: resume coverletter

resume: 
	@latex resume.tex
	@pdflatex resume.tex

coverletter:
	@cat cover_letter.tex | sed -e "s/;\<company\>;/$(company)/g;s/;\<address\>;/$(address)/g;s/;\<country\>;/$(country)/g" > out.tex && latex out.tex && pdflatex out.tex && cp out.pdf cover_letter.pdf && rm -fr out.*

prod: all
	@cp resume.pdf Garrett_Everding_CV.pdf

full: all
	@pdftk cover_letter.pdf resume.pdf output Garrett_Everding_CV_and_CoverLetter.pdf

clean:
	@rm -f *.pdf
	@rm -f *.aux *.log *.dvi

.PHONY: all latex pdf production coverletter resume
