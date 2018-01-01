# Process this file with autoconf to produce a configure script.

AC_PREREQ([2.67])
AC_INIT([gerb2tiff], [1.2], [a_seychell@yahoo.com.au])
AC_CONFIG_AUX_DIR(build-aux)
AC_CONFIG_SRCDIR(src/main.cpp)
AC_CONFIG_HEADERS([src/config.h])

AM_INIT_AUTOMAKE()

# Checks for programs.
AC_PROG_YACC
AC_PROG_CXX
AC_PROG_CC
AC_PROG_CPP
AC_PROG_LEX
AC_PROG_INSTALL

# Checks for libraries.
AC_CHECK_LIB([tiff], [TIFFOpen], [], [], [-lz])

# Checks for header files.
AC_FUNC_ALLOCA
AC_CHECK_HEADERS([inttypes.h libintl.h limits.h malloc.h stddef.h stdlib.h string.h unistd.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_HEADER_STDBOOL
AC_C_INLINE
AC_TYPE_INT16_T
AC_TYPE_INT32_T
AC_TYPE_INT8_T
AC_C_RESTRICT
AC_TYPE_SIZE_T
AC_TYPE_UINT16_T
AC_TYPE_UINT32_T
AC_TYPE_UINT8_T

# Checks for library functions.
AC_FUNC_ERROR_AT_LINE
AC_FUNC_MALLOC
AC_FUNC_REALLOC
AC_FUNC_STRTOD
AC_CHECK_FUNCS([memset pow sqrt strchr strrchr strstr])

AC_CONFIG_FILES([Makefile
		 src/Makefile])

AC_OUTPUT

echo
echo "Now type \"make\""
echo "then \"sudo make install\""

