# $NetBSD: Makefile,v 1.5 2017/07/30 22:32:24 wiz Exp $

DISTNAME=	feed-normalizer-1.5.2
PKGREVISION=	1
CATEGORIES=	textproc

MAINTAINER=	minskim@NetBSD.org
HOMEPAGE=	https://github.com/aasmith/feed-normalizer
COMMENT=	Extensible Ruby wrapper for Atom and RSS parsers
LICENSE=	modified-bsd

DEPENDS+=	${RUBY_PKGPREFIX}-simple-rss>=1.1:../../textproc/ruby-simple-rss
DEPENDS+=	${RUBY_PKGPREFIX}-hpricot>=0.6:../../textproc/ruby-hpricot

.include "../../lang/ruby/gem.mk"
.include "../../mk/bsd.pkg.mk"
