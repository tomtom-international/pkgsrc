# $NetBSD: Makefile,v 1.10 2018/08/22 09:44:55 wiz Exp $
#

DISTNAME=	accessors-fast-0.03
PKGNAME=	p5-${DISTNAME}
PKGREVISION=	6
CATEGORIES=	devel
MASTER_SITES=	${MASTER_SITE_PERL_CPAN:=../../authors/id/M/MO/MONS/}

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	http://search.cpan.org/dist/accessors-fast/
COMMENT=	Compiletime accessors using Class::Accessor::Fast
LICENSE=	${PERL5_LICENSE}

DEPENDS+=	p5-Class-Accessor-[0-9]*:../../devel/p5-Class-Accessor
DEPENDS+=	p5-Class-C3-[0-9]*:../../devel/p5-Class-C3
BUILD_DEPENDS+=	p5-Test-NoWarnings-[0-9]*:../../devel/p5-Test-NoWarnings
#BUILD_DEPENDS+=	{perl>=5.6.2,p5-Test-Simple-[0-9]*}:../../devel/p5-Test-Simple
DEPENDS+=	p5-constant-def>=0.01:../../devel/p5-constant-def
BUILD_DEPENDS+=	p5-lib-abs>=0.90:../../devel/p5-lib-abs

REPLACE_PERL+=	cpants.pl

MAKE_ENV+=	PERL_USE_UNSAFE_INC=1

.include "../../lang/perl5/module.mk"
.include "../../mk/bsd.pkg.mk"
