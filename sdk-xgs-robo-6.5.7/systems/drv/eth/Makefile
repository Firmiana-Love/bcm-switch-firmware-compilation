# $Id: Makefile,v 1.3 Broadcom SDK $
# $Copyright: (c) 2016 Broadcom.
# Broadcom Proprietary and Confidential. All rights reserved.$
#
# Makefile for eth driver
#

LOCALDIR = systems/drv/eth

include ${SDK}/make/Make.config

ifeq (${targetbase},posix)
CFLAGS += -DLINUX
endif

ifeq (${targetbase},unix)
CFLAGS += -DLINUX
endif

ifeq (${targetbase},linux)
CFLAGS += -DLINUX -DKERNEL
endif

ifeq (${targetbase},vxworks)
CFLAGS += -DVXWORKS
endif

lib = libeth
include ${SDK}/make/Make.lib

include ${SDK}/make/Make.depend
