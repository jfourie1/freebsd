# $FreeBSD$

PACKAGE=runtime
PROG=	nvmecontrol
SRCS=	comnd.c nvmecontrol.c
SRCS+=	devlist.c firmware.c format.c identify.c logpage.c ns.c perftest.c power.c reset.c
#SRCS+=	passthru.c
SRCS+=	identify_ext.c nvme_util.c nc_util.c
MAN=	nvmecontrol.8
LDFLAGS+= -rdynamic
LIBADD+= util
SUBDIR=	modules

.PATH:	${SRCTOP}/sys/dev/nvme

.include <bsd.prog.mk>
.include <bsd.subdir.mk>
