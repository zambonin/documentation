LATEX = latexmk
LATEX_FLAGS = -shell-escape -e "\$$pdflatex=q/pdflatex -synctex=1 -interaction=nonstopmode/" -pdf

all: main.tex
	pdflatex -interaction=nonstopmode main.tex ; \
	biber main; \
	pdflatex -interaction=nonstopmode main.tex ;\
	pdflatex -interaction=nonstopmode main.tex; \
	mv main.pdf the-nanvix-kernel.pdf

clean:
	rm -f             \
		*.aux         \
		*.bbl         \
		*.bcf         \
		*.blg         \
		*.fls         \
		*.log         \
		*.out         \
		*.xml         \
		*.toc         \
		*.fdb_latexmk \
		the-nanvix-kernel.pdf         \
		*.gz          \
		*.glo         \
		*.ist         \
		*.acn
