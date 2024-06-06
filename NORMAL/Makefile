CC = cc
CFLAGS = -g -Wall
OBJS = aurevoir.o au.o revoir.o
TARGET = aurevoir

ALL: $(OBJS)
	$(CC) $(CFLAGS) -o $(TARGET) $(OBJS)

aurevoir.o: aurevoir.c
	$(CC) $(CFLAGS) -o aurevoir.o -c aurevoir.c

au.o: au.c
	$(CC) $(CFLAGS) -o au.o -c au.c

revoir.o: revoir.c
	$(CC) $(CFLAGS) -o revoir.o -c revoir.c

clean:
	rm -fr $(OBJS)
