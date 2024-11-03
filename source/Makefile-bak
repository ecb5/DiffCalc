all: jing web pdf view

jing: *.ptx 
	jing /home/ecb5/.ptx/schema/pretext.rng main.ptx

latex: *.ptx Makefile 
	pretext build latex

pdf: *.ptx Makefile 
	/home/ecb5/.local/bin/pretext build print

viewpdf: *.ptx Makefile 
	/home/ecb5/.local/bin/pretext view print

web: Makefile 
	/home/ecb5/.local/bin/pretext build web

view:
	/home/ecb5/.local/bin/pretext view web;

deploy:
	/home/ecb5/.local/bin/pretext deploy -u
