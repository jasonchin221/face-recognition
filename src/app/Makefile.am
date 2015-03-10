bin_PROGRAMS = ns_app ns_test
ns_app_SOURCES = ns_app.cpp
ns_app_LDADD = $(srcdir)/../net/libnetwork_stack.la
ns_test_SOURCES = ns_test.cpp
ns_test_LDADD = $(srcdir)/../net/libnetwork_stack.la

AM_CPPFLAGS = -I$(srcdir)/../include
AM_CFLAGS = -Wall -Werror
