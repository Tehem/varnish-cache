#

AM_CPPFLAGS = \
	-I$(top_srcdir)/include \
	-I$(top_builddir)/include

AM_LDFLAGS  = $(AM_LT_LDFLAGS)

pkglib_LTLIBRARIES = libvarnishcompat.la

libvarnishcompat_la_CFLAGS = \
	@SAN_CFLAGS@

libvarnishcompat_la_LDFLAGS = $(AM_LDFLAGS) -avoid-version \
	@SAN_LDFLAGS@

libvarnishcompat_la_SOURCES = \
	daemon.c \
	execinfo.c
