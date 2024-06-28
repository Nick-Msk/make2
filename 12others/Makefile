multiline = abcde\
	         bla bal bla

mult:
	@echo $(multiline)

.DELETE_ON_ERROR:
dd: del del2
del:
	touch one.h
	false

del2:
	touch two.h
	false

