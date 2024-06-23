CC = gcc
CFALGS = -g

all: one two
	# all
	echo $@
	# prereqs nevew target
	echo $?
	#all prereqs
	echo $^
	#firest prereqs
	echo $<
	touch all

one:
	touch one
two:
	touch two

blah: blah.o

blah.c:
	echo "int main(void) { return 0; }" > blah.c

clean:
	-rm all one two
	-rm blah*

