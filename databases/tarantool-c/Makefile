# $FreeBSD$

PORTNAME=	tarantool-c
PORTVERSION=	1.0.0
PORTREVISION=	1
CATEGORIES=	databases

MAINTAINER=	vg@FreeBSD.org
COMMENT=	C client for Tarantool 1.6+

LIB_DEPENDS=	libmsgpuck.so:devel/msgpuck

USE_GITHUB=	yes
GH_ACCOUNT=	tarantool
GH_TAGNAME=	a251965

USES=		cmake
CMAKE_ARGS=	-DENABLE_BUNDLED_MSGPUCK=false

BROKEN_aarch64=		Fails to compile: clang compiler does not support -march=native
BROKEN_mips64=		Fails to compile: clang compiler does not support -march=native
BROKEN_powerpc64=	Fails to compile: clang compiler does not support -march=native
BROKEN_sparc64=		Fails to compile: clang compiler does not support -march=native

.include <bsd.port.mk>
