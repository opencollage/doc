LATEXTOPDF=xelatex
PROGRAM=OpenCollage-Agent-Orchestrator
MV=mv

all: $(PROGRAM).pdf

$(PROGRAM).pdf:
	$(LATEXTOPDF) 000-opencollage.tex
	$(LATEXTOPDF) 000-opencollage.tex
	$(MV) 000-opencollage.pdf $(PROGRAM).pdf
clean:
	rm -frv *.aux *.nav *.out *.toc *.log *.snm *.vrb *.xdv *~
clobber:
	rm -frv *.aux *.nav *.out *.toc *.pdf *.log *.snm *.vrb *.xdv *~
test:
	$(LATEXTOPDF) -no-pdf 000-opencollage.tex

.PHONY: all $(PROGRAM).pdf clean clobber test
