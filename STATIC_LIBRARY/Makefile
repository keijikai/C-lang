CC	= cc
CFLAGS	= -g -Wall
OBJ	= aurevoir.o
OBJS	= au.o revoir.o
LIBS	= libaurevoir.a
LDLIBS	= -L./ -laurevoir
PRGRM	= aurevoir

all: $(OBJS) $(LIBS) $(PRGRM)

aurevoir.o: aurevoir.c
	$(CC) $(CFLAGS) -o aurevoir.o -c aurevoir.c

au.o: au.c
	$(CC) $(CFLAGS) -o au.o -c au.c

revoir.o: revoir.c
	$(CC) $(CFLAGS) -o revoir.o -c revoir.c

libaurevoir.a: au.o revoir.o
	ar rcs $(LIBS) $(OBJS)

aurevoir: $(OBJ)
	$(CC) $(CFLAGS) $(OBJ) $(LDLIBS) -o $(PRGRM)

clean:
	rm -fr $(OBJ) $(OBJS) $(LIBS) $(PRGRM)
