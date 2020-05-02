ACLOCAL_AMFLAGS = -I m4

lib_LTLIBRARIES = libpcsclitebcas.la

libpcsclitebcas_la_SOURCES = Crypto.cpp Decoder-ECM.cpp Keys.cpp Keyset.cpp winscard.cpp

libpcsclitebcas_la_LIBADD = $(AM_LIBS) $(pcsclite_LIBS) $(PCSC_LIBS)

libpcsclitebcas_la_CXXFLAGS = -g -fPIC -O2 -I /usr/include/PCSC 

libpcsclitebcas_la_LDFLAGS =  -g -fPIC -shared

pkginclude_HEADERS = Crypto.h Decoder.h Global.h Keys.h Keyset.h

pkgconfigdir = $(libdir)/pkgconfig

pkgconfig_DATA = libpcsclite-bcas.pc

dist_doc_DATA = README.md
