# $NetBSD: Makefile,v 1.6 2021/05/24 19:52:23 wiz Exp $

DISTNAME=	lxqt-themes-0.17.0
PKGREVISION=	1
CATEGORIES=	graphics
MASTER_SITES=	${MASTER_SITE_GITHUB:=lxqt/}
GITHUB_RELEASE=	${PKGVERSION_NOREV}
EXTRACT_SUFX=	.tar.xz

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	https://github.com/lxqt/lxqt-themes/
COMMENT=	Themes, graphics and icons for LXQt
LICENSE=	gnu-lgpl-v2.1

USE_CMAKE=	yes
USE_TOOLS+=	pkg-config perl
USE_LANGUAGES=	c c++

CONFIGURE_DIRS=	build
CMAKE_ARG_PATH=	..

pre-configure:
	${MKDIR} -p ${WRKSRC}/build

TOOL_DEPENDS+=	lxqt-build-tools>=0.9:../../devel/lxqt-build-tools

.include "../../graphics/hicolor-icon-theme/buildlink3.mk"
.include "../../mk/bsd.pkg.mk"
