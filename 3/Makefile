SHELL = /usr/bin/env bash
NAME:=proj3

all:
	latex $(NAME).tex
	latex $(NAME).tex
	dvips $(NAME).dvi
	ps2pdf -sPAPERSIZE=a4 $(NAME).ps

clean:
	rm -f $(NAME).{aux,dvi,log,pdf,ps}

zip: clean
	zip xmahut01 $(NAME).tex {oniisan,oniisan2,etiopan}.eps algorithm2e.sty Makefile

