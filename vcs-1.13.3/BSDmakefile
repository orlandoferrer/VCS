#
# $Id: BSDmakefile 562 2013-03-08 16:07:17Z toni $
# Makefile for BSD-make
#

VERSION!=sed -n '/VERSION=/s/.*"\([^"]*\)".*/\1/p' vcs | head -n1
PACKAGER!=finger -lp `echo $USER` 2>/dev/null | head -n1 | cut -d: -f3
.if empty($(PACKAGER))
PACKAGER!=getent passwd "`id -un`" | cut -d: -f5 | cut -d, -f1
.endif

GMAKE?=gmake
RM?=rm -f

include common.mk

