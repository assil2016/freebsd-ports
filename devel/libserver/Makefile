# Created by: James Bailie <jimmy@mammothcheese.ca>
# $FreeBSD$

PORTNAME=	libserver
PORTVERSION=	3.17
CATEGORIES=	devel
MASTER_SITES=	http://www.mammothcheese.ca/

MAINTAINER=	jimmy@mammothcheese.ca
COMMENT=	Generic TCP server in a library

BROKEN=		unfetchable
DEPRECATED=	Broken for more than 6 months
EXPIRATION_DATE=	2020-05-05

LICENSE=	BSD3CLAUSE
LICENSE_FILE=	${WRKSRC}/LICENSE

USE_LDCONFIG=	yes

MAKE_ENV+=	STAGEDIR=${STAGEDIR}
PLIST_SUB+=	PORTVERSION=${PORTVERSION}

.include <bsd.port.mk>
