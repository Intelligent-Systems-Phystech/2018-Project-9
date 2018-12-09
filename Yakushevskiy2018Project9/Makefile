article="main"

all: build clean view

clean:
	@rm -rf                \
	${article}.aux         \
	${article}.bbl         \
	${article}.blg         \
	${article}.fdb_latexmk \
	${article}.fls         \
	${article}.log         \
	${article}.synctex.gz

build:
	@latexmk ${article}.tex -pdf \
	1>/dev/null                  \
	2>/dev/null

view:
	@evince ${article}.pdf \
	1>/dev/null            \
	2>/dev/null

help:
	@echo "make        - alias for build -> clean -> view"
	@echo "make build  - to compile .tex file and convert to .pdf file"
	@echo "make view   - to view article as .pdf file."
	@echo "make clean  - to clean from excessive files"