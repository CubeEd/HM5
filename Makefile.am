bin_PROGRAMS = HelloWorld
HelloWorld_SOURCES = main.c src/func.c
AUTOMAKE_OPTIONS = subdir-objects
AM_CPPFLAGS = -I$(srcdir)/headers
pkginclude_HEADERS = headers/header.h

clean-local:
	rm -f $(bin_PROGRAMS)
	rm -f COPYING compile depcomp install-sh missing INSTALL
	rm -f config.h* configure

clean-all: clean-local
	rm -f /usr/local/bin/hm5
	rm -f /usr/local/include/header.h

clean: clean-local clean-all 
	find . -type f ! -name '*.c' ! -name '*.h' ! -name '*.am' ! -name '*.ac' -exec rm -f {} +
	rm -rf autom4te.cache/