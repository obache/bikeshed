# $NetBSD: Makefile,v 1.3 2019/12/06 19:30:10 markd Exp $

DISTNAME=	lcyw
PKGNAME=	tex-${DISTNAME}-1.1
TEXLIVE_REV=	15878

MAINTAINER=	minskim@NetBSD.org
COMMENT=	Make Classic Cyrillic CM fonts accessible in LaTeX
LICENSE=	lppl-1.3c

DEPENDS+=	tex-latex-bin-[0-9]*:../../print/tex-latex-bin
DEPENDS+=	tex-oberdiek-[0-9]*:../../print/tex-oberdiek

TEXLIVE_UNVERSIONED=	yes
.include "../../print/texlive/package.mk"
.include "../../mk/bsd.pkg.mk"
