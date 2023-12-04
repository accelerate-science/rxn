ADOC=/usr/bin/asciidoctor
ifneq ("$(wildcard $(/home/rlopez/.rvm/gems/ruby-3.0.0/bin/asciidoctor))","")
	ADOC=/home/rlopez/.rvm/gems/ruby-3.0.0/bin/asciidoctor
endif
AFLAGS=-D ./build -a stylesheet=./clean.css
ASOURCES=index.adoc quick_start.adoc predict_retrosynthesis.adoc predict_product.adoc predict_reagents.adoc plan_synthesis.adoc

html: $(ASOURCES)
	$(ADOC) $(AFLAGS) $(ASOURCES)
