DVI=/usr/share/texmf/bin/latex
PS=/usr/share/texmf/bin/dvips
PDF=/usr/share/texmf/bin/pdflatex

SRC=TrabRedesOSI.tex

DVI_DOC=TrabRedesOSI.dvi
PS_DOC=TrabRedesOSI.ps
PDF_DOC=TrabRedesOSI.pdf

dvi: ${SRC}
	${DVI} -interaction=nonstopmode ${SRC}

ps: ${DVI_DOC}
	${PS} -o ${PS_DOC} ${DVI_DOC}

pdf: ${SRC}
	${PDF} -interaction=nonstopmode ${SRC}

.PHONY: clean clean_all

clean:
	rm *.aux *.log *~

clean_all:
	rm *.aux *.log *~ ${DVI_DOC} ${PS_DOC} ${PDF_DOC}

