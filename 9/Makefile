override option_one = did_over
option_two = not_over

over:
	echo $(option_one)
	echo $(option_two)

one = export blah="I set"; echo $$blah

define two
export blah="WAs"
echo $$blah
echo "haha"
endef

def:
	@echo "Prints..."
	@$(one)
	@echo "not Print.."
	@$(two)

t1: per = zzz

t1:
	echo def var $(per)

t2:
	echo not def var $(per)

%.c: winc = ty

blah.c:
	@echo "def $(winc)"

blah.h:
	@echo "not def $(winc)..."

