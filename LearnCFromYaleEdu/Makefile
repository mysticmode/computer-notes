CC=gcc
CFLAGS=-g3 -Wall

all: hello-world

hello-world: hello-world.o hello-library.o
	$(CC) $(CFLAGS) -o $@ $^
	echo "I just built hello-world! Hooray!"

hello-world.o: hello-world.c hello-library.h
hello-library.o: hello-library.c hello-library.h

test: hello-world
	./hello-world

clean:
	$(RM) hello-world *.o
