new_contents = "Hello:\n\techo \$$(cooly)"

all:
	mkdir -p subdir
	printf $(new_contents) | sed -e 's/^ //' > subdir/Makefile
	@echo "---MAKEFILE CONTENTS---"
	@cd subdir && cat Makefile
	@echo "---END MAKEFILE CONTENTS---"
	cd subdir && $(MAKE)

export cooly = "the subdir can see me!"

one = "this is locally"
export two = "this is in all command"

exp:
	@echo $(one)
	@echo $$one
	@echo $(two)
	@echo $$two

three = one ${later}
four := two ${later}
five = hello
five := ${five} there

later = l_a_t_e_r

vars:
	echo $(three)
	echo $(four)
	echo $(five)

six = hi
six ?= will not be adjusted
seven ?= will be adjusted
not_def:
	echo $(six)
	echo $(seven)

with_spaces = hello      # ttt
after = $(with_spaces)there
nullstring =
space = $(nullstring) #single
foo := start
foo +=end

spaces:
	echo $(xz)
	echo "$(after)"
	echo start"$(space)"end
	echo $(foo)

clean:
	rm -rf subdir

