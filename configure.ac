#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_INIT([mt-maildir-compress], [0.14], [Media Temple <dev@mediatemple.net>])
AM_INIT_AUTOMAKE([foreign])
AC_CONFIG_SRCDIR([maildir-compress])

AC_PREFIX_DEFAULT([/opt/mt])

AC_PATH_PROG(PERL, perl, no)
AC_SUBST(PERL)

m4_include([ax_prog_perl_modules.m4])

AC_PROG_PERL_MODULES(Readonly IO::Compress::Bzip2 Log::Log4perl, , AC_MSG_ERROR(Need Readonly, Bzip2 and Log4perl Perl modules))

AC_CONFIG_FILES([
 Makefile
 REDHAT.spec
])

AC_OUTPUT
