# Makefile for ...su/graphics/cplot

include $(CWPROOT)/src/Makefile.config

LFLAGS= -L$L -lsu -lvplotcwp -lvplot -lpar -lcwp -lm


PROGS  = $B/suwig 

INSTALL	: $(PROGS)
	touch $@


$(PROGS):$$(@F).c
	$(CC) $(CFLAGS) $? $(LFLAGS) -o $@
	@$(MCHMODLINE)
	@echo $(@F) installed in $B

remake	:
	-touch *.c
	$(MAKE)

clean:
	rm -f a.out junk* JUNK* core
