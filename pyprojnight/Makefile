all: p.pdf

p.pdf: p.tex
	pdflatex p.tex

.PHONY: clean
clean:
	rm -f p.{aux,bbl,blg,lof,log,lot,nav,out,pdf,snm,toc}

.PHONY: sync
sync: p.pdf
	scp p.pdf scooby-doo.csail.mit.edu:~/public_html/wip/sf-pyprojnight-aug14.pdf
