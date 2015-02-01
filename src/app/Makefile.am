bin_PROGRAMS = fr_app fr_test
fr_app_SOURCES = fr_app.c
fr_app_LDADD = $(srcdir)/../opencv/libopencv_can.la $(srcdir)/../core/libface_recognize.la
fr_test_SOURCES = fr_test.c
fr_test_LDADD = $(srcdir)/../opencv/libopencv_can.la $(srcdir)/../core/libface_recognize.la

AM_CPPFLAGS = -I$(srcdir)/../include
AM_CFLAGS = -Wall -Werror
