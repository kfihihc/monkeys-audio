AUTOMAKE_OPTIONS = gnu

SUBDIRS = Assembly

lib_LTLIBRARIES = libmac.la

shared_ldadd = $(top_builddir)/src/Shared/libmacshared.la
asm_ldadd = $(top_builddir)/src/MACLib/Assembly/libmacasm.la

libmac_la_CPPFLAGS = -I$(top_srcdir)/src/Shared
libmac_la_LIBADD = $(shared_ldadd) $(asm_ldadd)
libmac_la_LDFLAGS = \
	-export-dynamic \
	-version-info 2:0:0

libmac_la_SOURCES = \
	APECompress.cpp \
	APECompressCore.cpp \
	APECompressCreate.cpp \
	APEDecompress.cpp \
	APEHeader.cpp \
	APEInfo.cpp \
	APELink.cpp \
	APESimple.cpp \
	APETag.cpp \
	BitArray.cpp \
	BitArray.h \
	MACLib.cpp \
	MACProgressHelper.cpp \
	MD5.cpp \
	MD5.h \
	MultichannelNNFilter.h \
	NNFilter.cpp \
	NNFilter.h \
	NewPredictor.cpp \
	NewPredictor.h \
	Predictor.h \
	Prepare.cpp \
	Prepare.h \
	ScaledFirstOrderFilter.h \
	StartFilter.h \
	UnBitArray.cpp \
	UnBitArray.h \
	UnBitArrayBase.cpp \
	UnBitArrayBase.h \
	WAVInputSource.cpp \
	WAVInputSource.h 

pkginclude_HEADERS = \
	APECompress.h \
	APECompressCore.h \
	APECompressCreate.h \
	APEDecompress.h \
	APEHeader.h \
	APEInfo.h \
	APELink.h \
	APETag.h \
	MACLib.h \
	MACProgressHelper.h

