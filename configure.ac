m4_define(vincent_version_major, 0)
m4_define(vincent_version_minor, 0)
m4_define(vincent_version_micro, 1)

AC_INIT([vincent], 
       vincent_version_major.vincent_version_minor.vincent_version_micro, 
        [foo])
AC_CONFIG_SRCDIR([src/linux-x11/egl.cpp])
AM_CONFIG_HEADER([linux-config.h])

AM_INIT_AUTOMAKE([1.7])

VINCENT_MAJORMINOR=vincent_version_major.vincent_version_minor
AC_SUBST(VINCENT_MAJORMINOR)

# CURRENT, REVISION, AGE
# - library source changed -> increment REVISION
# - interfaces added/removed/changed -> increment CURRENT, REVISION = 0
# - interfaces added -> increment AGE
# - interfaces removed -> AGE = 0
VINCENT_LT_CURRENT=1
VINCENT_LT_REV=0
VINCENT_LT_AGE=1
VINCENT_LT_VERSION="$VINCENT_LT_CURRENT:$VINCENT_LT_REV:$VINCENT_LT_AGE"
VINCENT_LT_LDFLAGS="-version-info $VINCENT_LT_VERSION"

AC_SUBST(VINCENT_LT_VERSION)
AC_SUBST(VINCENT_LT_LDFLAGS)

AC_PROG_CC
AC_PROG_CPP
AC_PROG_LIBTOOL

#Check pthreads
AC_MSG_CHECKING([for pthread options])
AC_CHECK_LIB(pthread, pthread_join, PTHREAD_LIBS="-lpthread",
     AC_MSG_ERROR([Could not find pthread_join in -lpthread.]))
AC_CHECK_HEADERS([pthread.h])

PKG_CHECK_MODULES(X11, x11)

if test "x$GCC" = "xyes"; then
        GCC_FLAGS="-g -Wall"
fi

VINCENT_CFLAGS="$X11_FLAGS $PTHREAD_CFLAGS"
VINCENT_LIBS="$X11_LIBS $PTHREAD_LIBS"

AC_SUBST(VINCENT_CFLAGS)
AC_SUBST(VINCENT_LIBS)
AC_SUBST(GCC_FLAGS)

AC_OUTPUT(Makefile              \
          src/Makefile          \
	  include/Makefile      \
	  tests/Makefile      \
          libvincent.pc )
