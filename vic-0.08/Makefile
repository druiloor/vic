#
#	Simple makefile for this package
#

include mkrules

MAJPROG = vic
PROGS	= vic show.locks
SRCDIRS	= webc.src

all::	version.wh

#
#       Create the distribution tar file once we have removed
#       any extraneous files.
#
dist:	clean tar all

install::
	install -m a=rx $(PROGS) $(BINDIR)
