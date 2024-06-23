blah: blah.o
	gcc blah.o -o blah

blah.o: blah.c
	gcc -c blah.c -o blah.o

blah.c:
	echo "int main(void) { return 0; }" > blah.c


sf: of
	@echo "Always run, second!"
	@touch sf

of:
	@echo "Always run, first!"

clean:
	rm sf

