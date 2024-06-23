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


