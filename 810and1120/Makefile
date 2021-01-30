# Makefile of printer driver
# Belfaux, July-August 2004 -- Nicolas Boichat
# Adapted from Samsung ML-85P driver by Rildo Pragana

CC=gcc
CFLAGS=-O2 -g

RELEASE=0.1

all: capt

capt: capt.c capt.h Makefile
	${CC} ${INCLUDE} ${CFLAGS} capt.c -o capt

install: all
	install -s -m a=rx capt /usr/bin
	install -m a=rx capt-print /usr/bin
	install -m a=r ppd/Canon-LBP-810-capt.ppd /usr/share/cups/model

clean:
	rm -f capt

package: clean
	rm -f *~ ppd/*~
	cp -a ../code ../capt-${RELEASE}
	tar cvfz ../capt-${RELEASE}.tar.gz ../capt-${RELEASE}
