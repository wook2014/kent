kentSrc = ../../..
include ../../../inc/common.mk


L += $(MYSQLLIBS) -lm
MYLIBDIR = ../../../lib/$(MACHTYPE)
MYLIBS =  $(MYLIBDIR)/jkhgap.a $(MYLIBDIR)/jkweb.a

O = cmpMap.o 

cmpMap: $O $(MYLIBS)
	${CC} ${COPT} ${CFLAGS} -o ${BINDIR}/cmpMap $O $(MYLIBS) $L

lib:
	cd ../../lib && ${MAKE}
	cd ../../../lib && ${MAKE}

clean::
	rm -f ${O}
