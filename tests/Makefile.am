if ENABLE_TESTS

@CODE_COVERAGE_RULES@
TESTS = check_base64 check_base32 check_base16
check_PROGRAMS = check_base64 check_base32 check_base16

check_base64_SOURCES = check_base64.c
check_base64_CFLAGS = @CHECK_CFLAGS@
check_base64_LDADD = $(top_builddir)/src/libbase64.a @CHECK_LIBS@

check_base32_SOURCES = check_base32.c
check_base32_CFLAGS = @CHECK_CFLAGS@
check_base32_LDADD = $(top_builddir)/src/libbase32.a @CHECK_LIBS@

check_base16_SOURCES = check_base16.c
check_base16_CFLAGS = @CHECK_CFLAGS@
check_base16_LDADD = $(top_builddir)/src/libbase16.a @CHECK_LIBS@

else

check:
	echo "Testing not enabled (run ./configure --enable-tests)"; false

endif
