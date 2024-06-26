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


clean:
	rm -rf subdir

