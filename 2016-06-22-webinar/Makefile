
RMD := $(shell ls *.Rmd)
HTML := $(patsubst %.Rmd, %.html, $(RMD))

all: $(HTML)

%.html: %.Rmd style.css
	R -e 'rmarkdown::render("$<")'
