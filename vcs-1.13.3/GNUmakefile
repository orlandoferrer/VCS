#
# $Id: GNUmakefile 562 2013-03-08 16:07:17Z toni $
# Makefile for GNU-make
#

VERSION:=$(shell sed -n '/VERSION=/s/.*"\([^"]*\)".*/\1/p' vcs | head -n1)
PACKAGER:=$(shell finger -lp `echo $USER` 2>/dev/null | head -n1 | cut -d: -f3)
ifeq ($(PACKAGER),)
  PACKAGER:=$(shell getent passwd "`id -un`" | cut -d: -f5 | cut -d, -f1)
endif

GMAKE?=make

include common.mk

