# Created by: gahr
# $FreeBSD$

PORTNAME=	tcloo
PORTVERSION=	1.0.4
CATEGORIES=	devel
MASTER_SITES=	http://core.tcl.tk/tcloo/tarball/
DISTNAME=	TclOO+Package-${FOSSIL_CHECKIN}

MAINTAINER=	tcltk@FreeBSD.org
COMMENT=	Implementation of TclOO for Tcl 8.5

BROKEN=		unfetchable
DEPRECATED=	Broken for more than 6 months
EXPIRATION_DATE=	2020-05-05

LICENSE=	TclTk
LICENSE_NAME=	Tcl/Tk License
LICENSE_FILE=	${WRKSRC}/license.terms
LICENSE_PERMS=	dist-mirror dist-sell pkg-mirror pkg-sell auto-accept

FOSSIL_CHECKIN=	0a6e9f1ea3
WRKSRC=		${WRKDIR}/${DISTNAME:S/+/_/}
USE_LDCONFIG=	yes
USES+=		tcl:85,tea
TCL_PKG=	TclOO${PORTVERSION}

TEST_TARGET=	test

.include <bsd.port.mk>
