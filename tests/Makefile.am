AM_CPPFLAGS = \
	-I$(top_srcdir)/include \
	-I$(top_srcdir)/common \
	@LIBCERROR_CPPFLAGS@ \
	@LIBCTHREADS_CPPFLAGS@ \
	@LIBCDATA_CPPFLAGS@ \
	@LIBCLOCALE_CPPFLAGS@ \
	@LIBCNOTIFY_CPPFLAGS@ \
	@LIBCSPLIT_CPPFLAGS@ \
	@LIBUNA_CPPFLAGS@ \
	@LIBCFILE_CPPFLAGS@ \
	@LIBCPATH_CPPFLAGS@ \
	@LIBBFIO_CPPFLAGS@ \
	@LIBCSYSTEM_CPPFLAGS@ \
	@PTHREAD_CPPFLAGS@ \
	@LIBHIBR_DLL_IMPORT@

TESTS = \
	test_api_functions.sh \
	test_api_types.sh \
	test_hibrinfo.sh

check_SCRIPTS = \
	test_api_functions.sh \
	test_api_types.sh \
	test_hibrinfo.sh \
	test_runner.sh

EXTRA_DIST = \
	$(check_SCRIPTS)

check_PROGRAMS = \
	hibr_test_error \
	hibr_test_file \
	hibr_test_notify \
	hibr_test_support

hibr_test_error_SOURCES = \
	hibr_test_error.c \
	hibr_test_libhibr.h \
	hibr_test_macros.h \
	hibr_test_unused.h

hibr_test_error_LDADD = \
	../libhibr/libhibr.la

hibr_test_file_SOURCES = \
	hibr_test_file.c \
	hibr_test_libcerror.h \
	hibr_test_libclocale.h \
	hibr_test_libcsystem.h \
	hibr_test_libhibr.h \
	hibr_test_libuna.h \
	hibr_test_macros.h \
	hibr_test_memory.c hibr_test_memory.h

hibr_test_file_LDADD = \
	@LIBCSYSTEM_LIBADD@ \
	@LIBUNA_LIBADD@ \
	@LIBCNOTIFY_LIBADD@ \
	@LIBCLOCALE_LIBADD@ \
	@LIBCDATA_LIBADD@ \
	../libhibr/libhibr.la \
	@LIBCTHREADS_LIBADD@ \
	@LIBCERROR_LIBADD@ \
	@PTHREAD_LIBADD@

hibr_test_notify_SOURCES = \
	hibr_test_libhibr.h \
	hibr_test_macros.h \
	hibr_test_notify.c \
	hibr_test_unused.h

hibr_test_notify_LDADD = \
	../libhibr/libhibr.la

hibr_test_support_SOURCES = \
	hibr_test_libcerror.h \
	hibr_test_libclocale.h \
	hibr_test_libcsystem.h \
	hibr_test_libhibr.h \
	hibr_test_libuna.h \
	hibr_test_macros.h \
	hibr_test_support.c \
	hibr_test_unused.h

hibr_test_support_LDADD = \
	@LIBCSYSTEM_LIBADD@ \
	@LIBUNA_LIBADD@ \
	@LIBCNOTIFY_LIBADD@ \
	@LIBCLOCALE_LIBADD@ \
	@LIBCDATA_LIBADD@ \
	../libhibr/libhibr.la \
	@LIBCERROR_LIBADD@

MAINTAINERCLEANFILES = \
	Makefile.in

distclean: clean
	/bin/rm -f Makefile

