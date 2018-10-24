pkgconfigdir = $(libdir)/pkgconfig
nodist_pkgconfig_DATA = libenet.pc

enetincludedir=$(includedir)/enet
enetinclude_HEADERS = \
	enet/callbacks.h \
	enet/enet.h \
	enet/list.h \
	enet/protocol.h \
	enet/time.h \
	enet/types.h \
	enet/unix.h \
	enet/utility.h \
	enet/win32.h \
	common.h

lib_LTLIBRARIES = libenet.la
libenet_la_SOURCES = callbacks.c compress.c host.c list.c packet.c peer.c protocol.c unix.c win32.c
# see info '(libtool) Updating version info' before making a release
libenet_la_LDFLAGS = $(AM_LDFLAGS) -version-info 7:1:0
AM_CPPFLAGS = -I$(top_srcdir)/include

ACLOCAL_AMFLAGS = -Im4
