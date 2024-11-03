all: jing latex pdf web view 

web: *.ptx  Makefile 
	pretext build web

deploy: *.ptx  Makefile
	pretext deploy -u

jing: *.ptx 
	jing /home/ecb5/.ptx/2.8.0/core/schema/pretext.rng main.ptx
#	jing /home/ecb5/.ptx/2.6.2/core/schema/pretext.rng main.ptx


latex: *.ptx Makefile 
	pretext build latex

pdf: *.ptx Makefile 
	pretext build print

epub: *.ptx Makefile
	pretext build epub

view: Makefile
	pretext view

viewpdf: 
#	pretext view print
	evince /home/ecb5/Dropbox/CalcText/Boman/IntCalc/output/print/main.pdf

debug:
	pretext -v debug build web

support:
	pretext support

