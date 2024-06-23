CC = gcc

objects = foo.o bar.o all.o ttt.o eee.o ddd.o

all: $(objects)
	$(CC) $^ -o $@

$(object): %.o: %.c:
	$(CC) -c $^ -o $@

#foo.o: foo.c
#	$(CC) -c $^ -o $@

#bar.o: bar.c
#	$(CC) -c $^ -o $@

#all.o: all.c
#	$(CC) -c $^ -o $@

all.c:
	echo "int main(void) { return 0; } " > all.c

%.c:
	touch $@

clean:
	-rm *.c *.o all
