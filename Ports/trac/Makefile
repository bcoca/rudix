Requires += org.rudix.pkg.genshi,genshi,genshiinstall.pkg

include ../../Library/Python.mk

Title=		Trac
Name=		trac
Version=	1.0.1
Revision=	0
Site=		http://trac.edgewall.org
Source=		http://download.edgewall.org/trac//Trac-$(Version).tar.gz
License=	BSD

define test_inner_hook
$(BinDir)/trac-admin --version
endef
