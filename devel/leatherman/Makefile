# $FreeBSD$

PORTNAME=	leatherman
PORTVERSION=	0.10.1
PORTREVISION=	1
CATEGORIES=	devel

MAINTAINER=	jslagle@gmail.com
COMMENT=	Leatherman C++ Tool library

LICENSE=	APACHE20

LIB_DEPENDS=	libboost_system.so:devel/boost-libs \
		libcurl.so:ftp/curl

USE_GITHUB=	yes
GH_ACCOUNT=	puppetlabs

USES=		cmake
USE_RUBY=	yes
CMAKE_ARGS=	-DLEATHERMAN_SHARED:BOOL=ON
USE_LDCONFIG=	yes

PLIST_SUB=	PORTVERSION=${PORTVERSION}

.include <bsd.port.mk>
