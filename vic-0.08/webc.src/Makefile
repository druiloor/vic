#
#       Makefile
#
#       Makefile for documentation directory
#
#       The major make commands the user uses are:
#           make        Make the static web pages
#           clean       Remove things which can be recreated
#

.SUFFIXES: .wc .html

.wc.html:
	../SupportBin/webc $*.wc
	cp -f $*.html ..
	chmod ug+rw,a+r $*.html ../$*.html

all:
	chmod a+r *.wc *.wh
	make `ls *.wc | sed "s/\.wc/.html/"`

clean:
	rm -f `find . -name "*.wc" -a -print | sed "s/\.wc/.html/"`
	rm -f version.wh

install: all
