bar := ${subst not, "totally", "I am not a machine not ttttt"}
comma := ,
empty:=
space := $(empty) $(empty)
var1 := a b c
var2 := $(subst $(space), $(comma)   , $(var1))

subst:
	@echo $(bar)
	@echo $(var2)


foo := a.o b.o l.a c.o
one := $(patsubst %.o,%.c,$(foo))
# This is a shorthand for the above
two := $(foo:%.o=%.c)
# This is the suffix-only shorthand, and is also equivalent to the above.
three := $(foo:.o=.c)

patsubst:
	@echo $(one)
	@echo $(two)
	@echo $(three)

str1 := who are,you.rrrr
str2 := $(foreach wrd, $(str1), $(wrd)++++++!)

foreach:
	@echo $(str2)

str3 := $(if this-is-not-empty, tra-ta-ta, truuuuu)
empty :=
str4 := $(if $(empty),yet++,not!!!)

iff:
	@echo $(str3)
	@echo $(str4)

new_fn = Variable name: $(0) fi: $(1), sec $(2), empty $(3)
call:
	@echo $(call new_fn, ttt, zxxzz)

shell:
	@echo $(shell ls -la)

obj_files = test.c test.o var.o b.o
filter_files = $(filter %.o, $(obj_files))
filter_out_obj = $(filter %.c, $(obj_files))

filter:
	@echo $(filter_files)
	@echo $(filter_out_obj)

