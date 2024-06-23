SHELL = /bin/bash

all: blah


make_var = I am a make var

blah::
	echo "test1"
	sh_var='shell var'; echo $$sh_var
	echo $(make_var)

blah::
	echo "test2"
	cd ..
	echo `pwd`
	cd ..; echo `pwd`
	cd ..; \
		echo `pwd`


data = "hello:\n\ttouch new.file"
req:
	mkdir -p subdir
	printf $(data) | sed -e 's/^ //' > subdir/Makefile
	cd subdir && $(MAKE)

shell:
	echo $$env_var
	echo $(env_var)

shell_env_var=Sh1 in make
export shell_env_var
var:
	echo $(shell_env_var)
	echo $$shell_env_var

clean:
	-rm -rf subdir

