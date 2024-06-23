
all: f1.o f2.o

f1.o f2.o:
	echo $@

print: $(wildcard *.c)
	echo $?
	ls -la $?

printno: $(*.c)
	echo $?
	ls -la $?

wrong := *.c
ok := $(wildcard *.c)

target: one two three four

one: $(wrong)
	echo $?

two: *.c
	echo $?

three: $(ok)
	echo $?

four: $(wildcard *.c)
	echo $?


