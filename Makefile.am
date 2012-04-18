AUTOMAKE_OPTIONS = 1.4 foreign
MAINTAINERCLEANFILES = Makefile.in aclocal.m4 config.h.in configure depcomp install-sh missing

INCLUDES = -I$(top_srcdir)

bin_PROGRAMS = elm_hello

elm_hello_SOURCES = main.c
elm_hello_LDADD = @ELEMENTARY_LIBS@ @EVAS_LIBS@
elm_hello_CFLAGS = @ELEMENTARY_CFLAGS@ @EVAS_CFLAGS@

filesdir = $(datadir)/elementary/themes
files_DATA = modest.edj

modest.edj: modest.edc
	edje_cc modest.edc modest.edj
