# $FreeBSD: head/print/indexinfo/Makefile 424688 2016-10-26 11:06:02Z bapt $

PORTNAME=	indexinfo
PORTVERSION=	0.2.6
CATEGORIES=	print ports-mgmt

MAINTAINER=	bapt@FreeBSD.org
COMMENT=	Utility to regenerate the GNU info page index

LICENSE=	BSD2CLAUSE
LICENSE_FILE=	${WRKSRC}/COPYING

USE_GITHUB=	yes
GH_ACCOUNT=	bapt
INSTALL_TARGET=	install-strip
PLIST_FILES=	bin/indexinfo

.if exists(/usr/include/sys/capsicum.h)
CFLAGS+=	-DHAVE_CAPSICUM
.endif

.include <bsd.port.mk>
