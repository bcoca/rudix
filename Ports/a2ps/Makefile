# Contributor: Qichang Liang <kcleung@cs.otago.ac.nz>

include ../../Library/GNU.mk

Title=		GNU a2ps
Name=		a2ps
Version=	4.14
Revision=	1
Site=		http://www.gnu.org/software/a2ps/
Source=		http://ftp.gnu.org/gnu/a2ps//$(Name)-$(Version).tar.gz
License=	GPL

define install_post_hook
mv $(InstallDir)/$(SysConfDir)/a2ps.cfg \
	$(InstallDir)/$(SysConfDir)/a2ps.cfg.default
mv $(InstallDir)/$(SysConfDir)/a2ps-site.cfg \
	$(InstallDir)/$(SysConfDir)/a2ps-site.cfg.default
endef

define test_inner_hook
$(BinDir)/a2ps --version | grep $(Version)
endef
