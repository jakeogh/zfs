include $(top_srcdir)/config/Rules.am

# Unconditionally enable debugging for zdbm
AM_CPPFLAGS += -DDEBUG -UNDEBUG

sbin_PROGRAMS = zdbm

zdb_SOURCES = \
	zdbm.c \
	zdbm_il.c \
	zdbm.h

zdb_LDADD = \
	$(top_builddir)/lib/libnvpair/libnvpair.la \
	$(top_builddir)/lib/libzpool/libzpool.la
