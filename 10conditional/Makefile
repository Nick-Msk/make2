SHELL=/bin/bash
foo = 11

all:
	ifeq($(foo), 11)
	echo "foo equal 11"
	else
	echo "not equal"
	endif

nullstring = 
str1 = $(nullstring) # 1

checknull:
	ifeq($(strip $(str1)), )
		echo "str1 is empty after strip"
	endif
	ifeq($(nullstring))
		echo "nullstring have no any space"
	endif

var2 =
var1 = $(var2)

checkdef:
ifdef var1
	echo "var1 is defined"
endif
ifndef var2
	echo "var2 is not"
endif

find:
	ifneq(,$(findstring i, $(MAKEFLAGS)))
	echo "-i was passed to MAKEFLAGS"
	endif


