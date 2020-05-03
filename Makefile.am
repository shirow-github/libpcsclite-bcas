ACLOCAL_AMFLAGS = -I m4

lib_LTLIBRARIES = libpcsclitebcas.la

libpcsclitebcas_la_SOURCES = src/Crypto.cpp src/Decoder-ECM.cpp src/Keys.cpp src/Keyset.cpp src/winscard.cpp

libpcsclitebcas_la_LIBADD = $(AM_LIBS) $(pcsclite_LIBS) $(PCSC_LIBS)

libpcsclitebcas_la_CXXFLAGS = -g -fPIC -O2 -I /usr/include/PCSC 

libpcsclitebcas_la_LDFLAGS =  -g -fPIC -shared

pkginclude_HEADERS = src/Crypto.h src/Decoder.h src/Global.h src/Keys.h src/Keyset.h

pkgconfigdir = $(libdir)/pkgconfig

pkgconfig_DATA = src/libpcsclite-bcas.pc

dist_doc_DATA = README.md
