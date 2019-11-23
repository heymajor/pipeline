m4_define([p_version],
          m4_esyscmd_s([echo `git rev-parse --abbrev-ref HEAD`-`git describe --always --dirty`])))

AC_INIT([pipeline], [p_version], [https://github.com/codekitchen/pipeline/issues], [pipeline], [https://github.com/codekitchen/pipeline])
AM_INIT_AUTOMAKE([-Wall -Werror subdir-objects foreign])
AC_PROG_CC
AC_SEARCH_LIBS(readline, readline)
AC_SEARCH_LIBS(setupterm, ncurses)
AC_CONFIG_HEADERS([config.h])
AC_CHECK_HEADERS([stdlib.h unistd.h])
# Checks for typedefs, structures, and compiler characteristics.
AC_TYPE_SIZE_T
AC_TYPE_SSIZE_T
# Checks for library functions.
AC_FUNC_FORK
AC_CONFIG_FILES([
 Makefile
])
AC_OUTPUT