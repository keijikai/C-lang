CC	= cc
CFLAGS	= -g -Wall
OBJ	= aurevoir.o
OBJS	= au.o revoir.o
LIBS	= libaurevoir.so
LDLIBS	= -L./ -laurevoir
PRGRM	= aurevoir

all: $(OBJS) $(LIBS) $(PRGRM)

aurevoir.o: aurevoir.c
	$(CC) $(CFLAGS) -fPIC -o aurevoir.o -c aurevoir.c

au.o: au.c
	$(CC) $(CFLAGS) -fPIC -o au.o -c au.c

revoir.o: revoir.c
	$(CC) $(CFLAGS) -fPIC -o revoir.o -c revoir.c

libaurevoir.so: $(OBJS)
	 $(CC) -shared $(OBJS) -o libaurevoir.so

aurevoir: $(OBJ)
	$(CC) $(CFLAGS) $(OBJ) $(LDLIBS) -o $(PRGRM)

clean:
	rm -fr $(OBJ) $(OBJS) $(LIBS) $(PRGRM)
