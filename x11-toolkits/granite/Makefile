# Created by: Olivier Duchateau
# $FreeBSD$
#

PORTNAME=	granite
PORTVERSION=	0.4.0.1
CATEGORIES=	x11-toolkits
MASTER_SITES=	https://launchpadlibrarian.net/277504431/ \
	https://launchpad.net/${PORTNAME}/0.4/loki-beta2/+download/

MAINTAINER=	ports@FreeBSD.org
COMMENT=	Extensions of GTK+3 toolkit

LICENSE=	LGPL3
LICENSE_FILE=	${WRKSRC}/COPYING

BUILD_DEPENDS=	valac:lang/vala
LIB_DEPENDS=	libgee-0.8.so:devel/libgee
RUN_DEPENDS=	contractor:sysutils/contractor

USES=	cmake gettext pkgconfig tar:xz
USE_GNOME=	glib20 gtk30 cairo introspection:build
INSTALLS_ICONS=	yes
USE_LDCONFIG=	yes

CFLAGS+=	-Wno-return-type

post-patch:
	${REINPLACE_CMD} -e 's|FFREE_|FREE_|' ${WRKSRC}/CMakeLists.txt

.include <bsd.port.mk>
