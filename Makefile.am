ACLOCAL_AMFLAGS = -I m4
SUBDIRS = data screenshots overview
dist_doc_DATA = COPYING README.md

if WITH_MARKDOWN
doc_DATA = index.html
index.html: $(top_srcdir)/README.md
	$(AM_V_GEN)$(MARKDOWN) $(top_srcdir)/README.md > $@
CLEANFILES = index.html
endif

DISTCHECK_CONFIGURE_FLAGS = --with-geany-libdir='$${libdir}/geany'
