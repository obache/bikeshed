# $NetBSD: Makefile,v 1.1 2020/05/25 14:30:15 taca Exp $

DISTNAME=	rbpdf-1.20.1
CATEGORIES=	print

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	https://github.com/naitoh/rbpdf/
COMMENT=	Ruby on Rails TCPDF plugin
LICENSE=	gnu-lgpl-v2.1

DEPENDS+=	${RUBY_PKGPREFIX}-htmlentities>=4.3.4:../../textproc/ruby-htmlentities
DEPENDS+=	${RUBY_PKGPREFIX}-rbpdf-font>=1.19.0<1.20:../../print/ruby-rbpdf-font

USE_LANGUAGES=	# none

.include "../../lang/ruby/gem.mk"
.include "../../mk/bsd.pkg.mk"
