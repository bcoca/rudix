include ../../Library/GNU.mk

Title=		Pkg-Config
Name=		pkg-config
Version=	0.28
Revision=	1
Site=		http://www.freedesktop.org/wiki/Software/pkg-config
Source=		http://pkgconfig.freedesktop.org/releases/$(Name)-$(Version).tar.gz
Checksum=	71853779b12f958777bffcb8ca6d849b4d3bed46
License=	GPL

GnuConfigureExtra += --with-internal-glib
GnuConfigureExtra += --disable-host-tool

define test_inner_hook
$(BinDir)/pkg-config --version | grep $(Version)
endef
