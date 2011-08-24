dist_bin_SCRIPTS = maildir-compress

rpm: package

package: dist
	make check
	make dist
	mkdir -p rpm/{SOURCES,BUILD,RPMS}
	mv mt-maildir-compress-@PACKAGE_VERSION@*.gz rpm/SOURCES
	rpmbuild -bb REDHAT.spec
