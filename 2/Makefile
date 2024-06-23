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
	-rm sf
	-rm blah*

files = file1 file2
sf2: $(files)
	echo "look at this var: " $(files)
	touch sf2

file1:
	touch file1
file2:
	touch file2
cleansf2:
	-rm $(files) sf2


