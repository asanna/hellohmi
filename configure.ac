# Autoconf -*-
# Process this file with autoconf to produce a configure script.
 
AC_PREREQ(2.61)
AC_INIT(hellohmi,0.1,andrea.sanna@mmarelli-se.com)

AM_INIT_AUTOMAKE
AC_CONFIG_HEADER([src/config.h])
# Old configure
AC_PREFIX_DEFAULT(/usr/)
if test "$prefix" = "NONE"; then
prefix="/usr/"
fi

CFLAGS="-O0"
CXXFLAGS="-O0"

# Checks for programs.
AC_PROG_CXX
AC_PROG_CC

# Checks for header files.
AC_HEADER_STDC
AC_CHECK_HEADERS([stdlib.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_HEADER_STDBOOL
AC_C_CONST

# Checks for library functions.


PKG_CHECK_MODULES(GTK,gtk+-2.0)
AC_SUBST(GTK_CFLAGS)
AC_SUBST(GTK_LIBS)

# List of all you Makefile.am are placed
AC_CONFIG_FILES([Makefile
                 src/Makefile
                 ])
AC_OUTPUT
