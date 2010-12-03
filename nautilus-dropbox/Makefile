# New ports collection makefile for:   nautilus-dropbox
# Date created:        1 December 2010
# Whom:                Vassilis Laganakos <vassilis.laganakos@yahoo.com>
#
# $FreeBSD$
#

PORTNAME=		nautilus-dropbox
PORTVERSION=	0.6.7
CATEGORIES=		net
MASTER_SITES=	http://www.dropbox.com/download?dl=packages/
DIST_SUBDIR=	gnome2

MAINTAINER=		vassilis.laganakos@yahoo.com
COMMENT=		A cross-computer file sharing/syncing plugin for nautilus

BUILD_DEPENDS=	nautilus:${PORTSDIR}/x11-fm/nautilus \
			pydoc:${PORTSDIR}/textproc/py-docutils

do-fetch:
.if !exists(${DISTDIR}/${DIST_SUBDIR}/${PORTNAME}-${PORTVERSION}.tar.bz2)
	${FETCH} -pRro ${DISTDIR}/${DIST_SUBDIR} "${MASTER_SITES}${PORTNAME}-${PORTVERSION}.tar.bz2"
.endif

FETCH?=			fetch
USE_BZIP2=		yes
USE_GMAKE=		yes
GNU_CONFIGURE=	yes
INSTALLS_ICONS=	yes

WRKSRC=			${WRKDIR}/${PORTNAME}-${PORTVERSION}

MAN1=			dropbox.1
LICENSE=		GPLv2

.include <bsd.port.mk>
