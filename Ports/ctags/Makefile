include ../../Library/GNU.mk
OptFlags=-O1 # https://trac.macports.org/changeset/93604

Title=		Exuberant Ctags
Name=		ctags
Version=	5.8
Revision=	8
Site=		http://ctags.sourceforge.net/
Source=		http://downloads.sourceforge.net/ctags/$(Name)-$(Version).tar.gz
License=	GPL

GnuConfigureExtra = --enable-etags
MakeInstallExtra += prefix=$(PortDir)/$(InstallDir)/$(Prefix)
MakeInstallExtra += mandir=$(PortDir)/$(InstallDir)/$(ManDir)

define install_post_hook
install	-m 644 $(SourceDir)/{FAQ,*.html} $(InstallDir)/$(DocDir)/$(Name)
cd $(InstallDir)/$(BinDir) ; ln -sf ctags exuberant-ctags ; ln -sf etags exuberant-etags
cd $(InstallDir)/$(ManDir)/man1 ; ln -sf ctags.1 exuberant-ctags.1 ; ln -sf etags.1 exuberant-etags.1
endef

define test_inner_hook
$(BinDir)/ctags --version | grep $(Version)
endef
