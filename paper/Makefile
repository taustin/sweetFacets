FILENAME=sweetjsIFC
TEXBIN=/usr/texbin
${FILENAME}.pdf: ${FILENAME}.tex biblio.bib
	${TEXBIN}/latex ${FILENAME}.tex
	#${TEXBIN}/bibtex ${FILENAME}
	#${TEXBIN}/latex ${FILENAME}.tex
	#${TEXBIN}/latex ${FILENAME}.tex
	${TEXBIN}/dvips ${FILENAME}.dvi
	ps2pdf ${FILENAME}.ps # on path
	open ${FILENAME}.pdf

clean:
	-rm ${FILENAME}.dvi
	-rm ${FILENAME}.bbl
	-rm ${FILENAME}.blg
	-rm ${FILENAME}.ps
	-rm ${FILENAME}.log
	-rm ${FILENAME}.aux
	-rm ${FILENAME}.ps.plog
	-rm ${FILENAME}.ps

spotless: clean
	-rm ${FILENAME}.pdf

