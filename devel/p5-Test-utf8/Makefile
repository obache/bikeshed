# $NetBSD: Makefile,v 1.10 2021/05/24 19:51:52 wiz Exp $
#

DISTNAME=		Test-utf8-1.02
PKGNAME=		p5-${DISTNAME}
PKGREVISION=		2
CATEGORIES=		devel perl5
MASTER_SITES=		${MASTER_SITE_PERL_CPAN:=Test/}

MAINTAINER=		pkgsrc-users@NetBSD.org
HOMEPAGE=		https://metacpan.org/release/Test-utf8
COMMENT=		Handy UTF-8 tests
LICENSE=		${PERL5_LICENSE}

PERL5_PACKLIST=		auto/Test/utf8/.packlist

.include "../../lang/perl5/module.mk"
.include "../../mk/bsd.pkg.mk"
