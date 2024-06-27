bar := ${subst not, "totally", "I am not a machine not ttttt"}
comma := ,
empty:=
space := $(empty) $(empty)
var1 := a b c
var2 := $(subst $(space), $(comma)   , $(var1))

subst:
	@echo $(bar)
	@echo $(var2)


