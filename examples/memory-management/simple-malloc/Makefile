
CC=gcc
CFLAGS=-g  -MMD -Wall
LIBS=

PROGS=simple-malloc-random-test simple-malloc-test

all: $(PROGS)

simple-malloc-test: simple-malloc-test.o simple-malloc.o
	$(CC) $(CFLAGS) -o $@  $^ $(LIBS)

simple-malloc-random-test: simple-malloc-random-test.o simple-malloc.o
	$(CC) $(CFLAGS) -o $@  $^ $(LIBS)

-include: *.d

clean:
	/bin/rm -f *.o *.d a.out  $(PROGS)
