include $(top_srcdir)/config/Rules.am

# Unconditionally enable debugging for zdbm
AM_CPPFLAGS += -DDEBUG -UNDEBUG

DEFAULT_INCLUDES += \
	-I$(top_srcdir)/include \
	-I$(top_srcdir)/lib/libspl/include

sbin_PROGRAMS = zdbm

zdbm_SOURCES = \
	zdbm.c \
	zdbm_il.c \
	zdbm.h

zdbm_LDADD = \
	$(top_builddir)/lib/libnvpair/libnvpair.la \
	$(top_builddir)/lib/libzpool/libzpool.la
