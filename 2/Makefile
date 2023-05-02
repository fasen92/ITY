SHELL = /usr/bin/env bash
NAME:=proj2

all:
	latex $(NAME).tex
	latex $(NAME).tex
	dvips -t a4 $(NAME).dvi
	ps2pdf $(NAME).ps

clean:
	rm -f $(NAME).{aux,dvi,log,pdf,ps}