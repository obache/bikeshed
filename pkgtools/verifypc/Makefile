# $NetBSD: Makefile,v 1.17 2019/05/23 19:23:13 rillig Exp $
#

PKGNAME=	verifypc-1.7
CATEGORIES=	pkgtools

MAINTAINER=	jmmv@NetBSD.org
COMMENT=	Sanity check package dependencies according to pkg-config
LICENSE=	modified-bsd

NO_BUILD=		YES
WRKSRC=			${WRKDIR}

SUBST_CLASSES+=		vars
SUBST_STAGE.vars=	do-configure
SUBST_MESSAGE.vars=	Configuring sources.
SUBST_FILES.vars=	*
SUBST_VARS.vars=	MAKE
SUBST_VARS.vars+=	SH

INSTALLATION_DIRS=	${PKGMANDIR}/man1 bin

do-extract:
	${CP} ${FILESDIR}/verifypc.sh ${WRKSRC}
	${CP} ${FILESDIR}/verifypc.1 ${WRKSRC}

do-install:
	${INSTALL_SCRIPT} ${WRKSRC}/verifypc.sh \
		${DESTDIR}${PREFIX}/bin/verifypc
	${INSTALL_MAN} ${WRKSRC}/verifypc.1 ${DESTDIR}${PREFIX}/${PKGMANDIR}/man1/

.include "../../mk/bsd.pkg.mk"
