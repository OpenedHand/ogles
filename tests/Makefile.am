noinst_PROGRAMS = test

INCLUDES = -I$(top_srcdir)/include

test_SOURCES = test.c
test_CFLAGS = $(VINCENT_CFLAGS)
test_LDFLAGS = \
    $(VINCENT_LIBS) \
    $(top_builddir)/src/libvincent.la 
