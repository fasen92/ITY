SHELL = /usr/bin/env bash
NAME:=proj4

all:
	latex $(NAME)
	bibtex $(NAME)
	latex $(NAME)
	latex $(NAME)
	dvips -t a4 $(NAME).dvi
	ps2pdf -sPAPERSIZE=a4 $(NAME).ps

clean:
	rm -f $(NAME).{aux,dvi,log,pdf,ps}

zip: clean
	zip xmahut01 $(NAME).tex $(NAME).bib czechiso.bst Makefile

