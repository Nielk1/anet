dnl $Id: $
dnl
AC_INIT(anet,0.11)
AC_PREREQ(2.54)

AC_CONFIG_AUX_DIR(macros)
AC_CONFIG_MACRO_DIR([macros])
AC_CANONICAL_HOST
AC_CANONICAL_TARGET

AM_INIT_AUTOMAKE([subdir-objects foreign])
AM_CONFIG_HEADER(h/anet_config.h)
AM_MAINTAINER_MODE
AC_PROG_MAKE_SET

AC_PROG_CC(cl gcc cc KCC CC egcs)
AC_PROG_LIBTOOL
AC_LANG(C)
AC_PATH_PROG(UNZIP,unzip,no)
if test "x$UNZIP" == "xno"
then
   AC_MSG_ERROR([

        unzip could not be found!

	Make sure unzip is in your path.

   ])
fi
AC_SUBST(UNZIP)

AC_LIBANET_INTERNAL

AC_OUTPUT([
   GNUmakefile
   demo/GNUmakefile
   demo/gtest/GNUmakefile
   src/GNUmakefile
   src/3rdparty/GNUmakefile
   src/linux/GNUmakefile
   src/linux/dp/GNUmakefile
   src/test/GNUmakefile
])

