Assignment1.pdf: Assignment1.tex
	xelatex $<

Assign1source.pdf: Assign1sourc.tex sources.bib
	xelatex $<
	biber Assign1sourc
	xelatex $<



.PHONY: clean clean_pdfs

tex_files := $(wildcard *.tex) 
pdf_files := $(tex_files:tex=pdf)


clean: 
	rm -f *.aux *.log
	rm -f *.out 
	rm -f *.bbl *.bcf *.blg *.run.xml
	rm -f *.fdb_latexmk *.fls 


clean_pdfs:
	rm -f $(pdf_files)