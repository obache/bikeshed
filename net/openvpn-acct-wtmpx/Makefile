# $NetBSD: Makefile,v 1.10 2020/01/26 17:31:53 rillig Exp $

.include "../../net/openvpn/Makefile.common"

DISTNAME=	openvpn-acct-wtmpx-20130210
DISTFILES=	${DISTNAME}${EXTRACT_SUFX} ${OPENVPN_DISTFILE}
CATEGORIES=	net
MASTER_SITES=	http://ftp.espci.fr/pub/openvpn-acct-wtmpx/
EXTRACT_SUFX=	.tgz

MAINTAINER=	manu@NetBSD.org
HOMEPAGE=	https://ftp.espci.fr/pub/openvpn-acct-wtmpx/
COMMENT=	Log OpenVPN logins and logouts to wtmpx
LICENSE=	2-clause-bsd

USE_LIBTOOL=	yes
USE_TOOLS+=	install

MAKE_ENV+=	OPENVPN_PLUGINSDIR=${PREFIX}/${OPENVPN_PLUGINSDIR}
MAKE_ENV+=	OPENVPN_DISTNAME=${OPENVPN_DISTNAME}

PLIST_SUBST+=	OPENVPN_PLUGINSDIR=${OPENVPN_PLUGINSDIR}
MESSAGE_SUBST+=	OPENVPN_PLUGINSDIR=${PREFIX}/${OPENVPN_PLUGINSDIR}

SPECIAL_PERMS+=	bin/logwtmpx ${SETUID_ROOT_PERMS}

DEPENDS+=	openvpn>=2.4.2:../../net/openvpn

.include "../../mk/bsd.pkg.mk"
