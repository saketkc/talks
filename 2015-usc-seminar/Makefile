SRC = buettner_et_al.tex
PDF = buettner_et_al.pdf
AUX = buetnner_et_al.aux
TEXC := xelatex
TEXC_OPTS += -shell-escape

.PHONY: clean

all: $(PDF)

$(AUX):
	$(TEXC) $(TEXC_OPTS) $(SRC)

$(PDF): beamerthemem.sty $(AUX) $(SRC)
	$(TEXC) $(TEXC_OPTS) $(SRC)

clean:
	@rm -f $(PDF)
	@git clean -xf
