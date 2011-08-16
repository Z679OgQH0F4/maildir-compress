# $URL: https://svn.mediatemple.net/dev/apps/maildir-compress/Makefile.am $
# $Id: Makefile.am 121217 2011-07-26 14:55:50Z gene $

dist_bin_SCRIPTS = maildir-compress

rpm: package

package: dist
	make check
	make dist
	mkdir -p rpm/{SOURCES,BUILD,RPMS}
	mv mt-maildir-compress-@PACKAGE_VERSION@*.gz rpm/SOURCES
	rpmbuild -bb REDHAT.spec
