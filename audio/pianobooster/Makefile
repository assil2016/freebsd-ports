# $FreeBSD$

PORTNAME=	pianobooster
DISTVERSIONPREFIX=	v
DISTVERSION=	0.7.2b
CATEGORIES=	audio

MAINTAINER=	yuri@FreeBSD.org
COMMENT=	MIDI file player that teaches how to play the piano

LICENSE=	GPLv3
LICENSE_FILE=	${WRKSRC}/gplv3.txt

LIB_DEPENDS=	libftgl.so:graphics/ftgl \
		libjack.so:audio/jack \
		librtmidi.so:audio/rtmidi

USES=		cmake desktop-file-utils gl pkgconfig qt:5
USE_GITHUB=	yes
GH_ACCOUNT=	captnfab
GH_PROJECT=	PianoBooster
USE_QT=		core gui opengl widgets xml buildtools_build linguisttools_build qmake_build
USE_GL=		gl glu

CMAKE_ON=	USE_SYSTEM_RTMIDI USE_JACK
CMAKE_ARGS=	-DDATA_DIR:STRING=share/${PORTNAME}

OPTIONS_DEFINE=		FLUIDSYNTH
OPTIONS_DEFAULT=	FLUIDSYNTH

FLUIDSYNTH_CMAKE_BOOL=	EXPERIMENTAL_USE_FLUIDSYNTH
FLUIDSYNTH_LIB_DEPENDS=	libfluidsynth.so:audio/fluidsynth

post-stage:
	@${RM} -r ${STAGEDIR}${DOCSDIR}

.include <bsd.port.mk>
