# $NetBSD: Makefile,v 1.35 2018/07/31 12:34:55 fhajny Exp $

DISTNAME=	consul-1.2.2
CATEGORIES=	sysutils
MASTER_SITES=	${MASTER_SITE_GITHUB:=hashicorp/}

MAINTAINER=	filip@joyent.com
HOMEPAGE=	https://www.consul.io/
COMMENT=	Tool for service discovery, monitoring and configuration
LICENSE=	mpl-2.0

EXTRACT_USING=	bsdtar

GITHUB_TAG=	v${PKGVERSION_NOREV}

GO_DIST_BASE=	${DISTNAME}
GO_SRCPATH=	github.com/hashicorp/consul

USE_LANGUAGES=		c c99
USE_TOOLS+=		bash gmake

INSTALLATION_DIRS+=	bin

do-install:
	${INSTALL_PROGRAM} ${WRKDIR}/bin/consul ${DESTDIR}${PREFIX}/bin

.include "../../lang/go/go-package.mk"
.include "../../mk/bsd.pkg.mk"
