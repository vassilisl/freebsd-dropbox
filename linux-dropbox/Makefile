# New ports collection makefile for:   linux-dropbox
# Date created:        4 December 2010
# Whom:                Vassilis Laganakos <vassilis.laganakos@yahoo.com>
#
# $FreeBSD$
#

PORTNAME=		dropbox
PORTVERSION=	0.7.110
DISTVERSIONPREFIX=	lnx.x86-
CATEGORIES=		net
MASTER_SITES=	http://dl-web.dropbox.com/u/17/
PKGNAMEPREFIX=	linux-
DIST_SUBDIR=	gnome2

MAINTAINER=		vassilis.laganakos@yahoo.com
COMMENT=		A cross-computer file sharing/syncing service - Linux prebuilt bins

BUILD_DEPENDS=	pydoc:${PORTSDIR}/textproc/py-docutils

USE_GZIP=		yes
USE_LINUX=		yes
NO_BUILD=		yes
EXTRACT_AFTER_ARGS=	| tar --strip-components=1 -xf -

WRKSRC=			${WRKDIR}

LICENSE=		GPLv2

.include <bsd.port.mk>
