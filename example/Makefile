#
#
#
LATEX = pdflatex
SOURCE = sheldon-cooper.cv
#OUTPUT = $(SOURCE)

all: fr en

pdf:
	$(LATEX) $(SOURCE)

fr:
	sed -i -e '/^\\usepackage/s/\[.*\]{eccehomo-cv}/\[fr\]{eccehomo-cv}/g' $(SOURCE).tex
	$(LATEX) -jobname $(SOURCE).fr $(SOURCE)

en:
	sed -i -e '/^\\usepackage/s/\[.*\]{eccehomo-cv}/\[en\]{eccehomo-cv}/g' $(SOURCE).tex
	$(LATEX) -jobname $(SOURCE).en $(SOURCE)

clean:
	rm -f $(SOURCE).en.log $(SOURCE).fr.log

mrproper: clean
	rm -f $(SOURCE).en.pdf $(SOURCE).fr.pdf
