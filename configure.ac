#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ([2.69])
AC_INIT([libpcsclite-bcas], [0.9.0], [shirowxxx@gmail.com])
AM_INIT_AUTOMAKE([foreign subdir-objects])
AC_CONFIG_MACRO_DIR([m4])
AC_CONFIG_SRCDIR([Decoder-ECM.cpp])
AC_CONFIG_HEADERS([config.h])

# Checks for programs.
AC_USE_SYSTEM_EXTENSIONS

AC_PROG_CXX
AC_PROG_CC
AC_PROG_CC_STDC
AC_PROG_INSTALL
AC_PROG_LN_S
AC_PROG_MAKE_SET
LT_INIT

# Checks for libraries.
PKG_CHECK_MODULES(pcsclite, "libpcsclite", [
    AC_DEFINE(HAVE_PCSC, 1, "have libpcsclite")
    AC_SUBST(PC_REQUIRE, "libpcsclite")
    AC_SUBST(PC_LIBS, "-lpcsclite")
  ], [AC_MSG_ERROR([${pcsclite_PKG_ERRORS}.])])
# Checks for header files.
AC_CHECK_HEADERS([string.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_CHECK_HEADER_STDBOOL

# Checks for library functions.
AC_CHECK_FUNCS([memset])

#AC_CONFIG_HEADERS([/usr/include/PCSC/pcsclite.h])
AC_CONFIG_FILES([Makefile libpcsclite-bcas.pc])
AC_OUTPUT
