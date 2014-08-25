build: out lint
	pdflatex --output-directory out/ Report.tex
	bibtex out/Report.aux
	pdflatex --output-directory out/ Report.tex
	pdflatex --output-directory out/ Report.tex
out:
	@mkdir -p out

clean:
	@rm -fR out

open: build
	@open out/Report.pdf

lint:
	@chktex Report.tex


.PHONY: clean out lint