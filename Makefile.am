AUTOMAKE_OPTIONS = foreign
bin_PROGRAMS = myprogram
myprogram_SOURCES = main.c func.c
include_HEADERS = header.h

install-exec-hook:
    $(INSTALL) -d $(DESTDIR)/usr/local/bin
    $(INSTALL) -m 755 myprogram $(DESTDIR)/usr/local/bin/

install-data-hook:
    $(INSTALL) -d $(DESTDIR)/usr/local/include
    $(INSTALL) -m 644 header.h $(DESTDIR)/usr/local/include/

clean-local:
    rm -f myprogram

clean-all:
    rm -rf autom4te.cache config.log config.status Makefile
    rm -f /usr/local/bin/myprogram /usr/local/include/header.h
