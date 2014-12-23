engine="xelatex -interactive=nonstopmode --shell-escape %O %S"

all: lysa.pdf

lysa.pdf: lysa.ltx
	latexmk -pdf -pdflatex=${engine} $<

clean:
	latexmk -C lysa.ltx
	$(RM) *run.xml *blx.bib *.bbl


.PHONY: lysa.pdf all clean
