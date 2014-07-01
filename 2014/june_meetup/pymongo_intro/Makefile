NOTEBOOK = gpug_mongo_talk.ipynb
REVEAL_TPL= res/slides_reveal.tpl

ifdef REVEAL_TPL
REVEAL_TPL := --SlidesExporter.template_file=$(REVEAL_TPL)
endif

all: slides

slides:
	ipython nbconvert $(NOTEBOOK) --to slides --reveal-prefix=res/reveal.js $(REVEAL_TPL)

serve:
	python -m SimpleHTTPServer
