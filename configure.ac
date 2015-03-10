AC_INIT([network-stack], [1.0], [jasonchin221@163.com])
AM_INIT_AUTOMAKE([-Wall -Werror])
AC_PROG_CXX
AC_PROG_LIBTOOL
AC_CONFIG_MACRO_DIR([m4])
AC_CONFIG_HEADERS([config.h])

CPPFLAGS="${CPPFLAGS} -I/usr/local/include"
LIBS="${LIBS} -L/usr/local/lib"

LPTHREAD=""
AC_CHECK_LIB([pthread], [pthread_create], , LPTHREAD="no")

if test "$LPTHREAD" = "no"; then
    echo
    echo "   ERROR!  pthread library not found, go get it from"
    echo "   or use the --with-pthread-* options, if you have it installed"
    echo "   in unusual place"
    exit
fi

AC_CONFIG_FILES([
				 Makefile
				 src/Makefile
				 src/net/Makefile
				 src/app/Makefile
				 ])

AC_OUTPUT
