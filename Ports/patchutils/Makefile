include ../../Library/GNU.mk

Title=		Patch utilities
Name=		patchutils
Version=	0.3.3
Revision=	1
Site=		http://cyberelk.net/tim/software/patchutils/
Source=		http://cyberelk.net/tim/data/patchutils/stable//$(Name)-$(Version).tar.xz
License=	GPL


define test_inner_hook
$(BinDir)/combinediff --version | grep $(Version)
endef
