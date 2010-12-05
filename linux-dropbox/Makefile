# New ports collection makefile for:   nautilus-dropbox
# Date created:        4 December 2010
# Whom:                Vassilis Laganakos <vassilis.laganakos@yahoo.com>
#
# $FreeBSD$
#

PORTNAME=		linux-dropbox
PORTVERSION=	0.7.110
CATEGORIES=		net
MASTER_SITES=	http://www.dropbox.com/download/?plat=lnx.x86
DIST_SUBDIR=	gnome2

MAINTAINER=		vassilis.laganakos@yahoo.com
COMMENT=		A cross-computer file sharing/syncing service

BUILD_DEPENDS=	pydoc:${PORTSDIR}/textproc/py-docutils

do-fetch:
.if !exists(${DISTDIR}/${DIST_SUBDIR}/${PORTNAME}-${PORTVERSION}.tar.gz)
	${FETCH} -pRo ${DISTDIR}/${DIST_SUBDIR}/${PORTNAME}-${PORTVERSION}.tar.gz "${MASTER_SITES}"
.endif

FETCH?=			fetch
USE_GZIP=		yes
USE_LINUX=		yes
NO_BUILD=		yes
EXTRACT_AFTER_ARGS=	| tar --strip-components=1 -xf -

WRKSRC=			${WRKDIR}

LICENSE=		GPLv2

.include <bsd.port.mk>
