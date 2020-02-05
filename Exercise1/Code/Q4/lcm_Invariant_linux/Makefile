INCLUDE_DIRS = 
LIB_DIRS = 
CC=gcc

CDEFS=
CFLAGS= -O3 $(INCLUDE_DIRS) $(CDEFS)
LIBS= 

HFILES= 
CFILES= rtesCode.c

SRCS= ${HFILES} ${CFILES}
OBJS= ${CFILES:.c=.o}

all:	rtesCode

clean:
	-rm -f *.o *.d
	-rm -f perfmon rtesCode

distclean:
	-rm -f *.o *.d
	-rm -f rtesCode

rtesCode: rtesCode.o
	$(CC) $(LDFLAGS) $(CFLAGS) -o $@ $@.o -lpthread

depend:

.c.o:
	$(CC) $(CFLAGS) -c $<
